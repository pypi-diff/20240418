# Comparing `tmp/btrview-0.5.0.tar.gz` & `tmp/btrview-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "btrview-0.5.0.tar", last modified: Wed Apr 10 20:48:29 2024, max compression
+gzip compressed data, was "btrview-0.6.0.tar", last modified: Thu Apr 18 04:05:24 2024, max compression
```

## Comparing `btrview-0.5.0.tar` & `btrview-0.6.0.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2024-04-10 20:48:29.356026 btrview-0.5.0/
--rw-r--r--   0 chris     (1000) chris     (1000)     1069 2023-05-17 21:10:51.000000 btrview-0.5.0/LICENSE.md
--rw-r--r--   0 chris     (1000) chris     (1000)     5948 2024-04-10 20:48:29.356026 btrview-0.5.0/PKG-INFO
--rw-r--r--   0 chris     (1000) chris     (1000)     4067 2024-04-10 20:27:39.000000 btrview-0.5.0/README.md
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2024-04-10 20:48:29.356026 btrview-0.5.0/btrview/
--rw-r--r--   0 chris     (1000) chris     (1000)       77 2024-04-10 20:36:39.000000 btrview-0.5.0/btrview/__init__.py
--rwxr-xr-x   0 chris     (1000) chris     (1000)     1843 2024-04-10 20:33:52.000000 btrview-0.5.0/btrview/__main__.py
--rw-r--r--   0 chris     (1000) chris     (1000)     6935 2024-04-10 16:19:25.000000 btrview-0.5.0/btrview/btrfs.py
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2024-04-10 20:48:29.356026 btrview-0.5.0/btrview/scripts/
--rwxr-xr-x   0 chris     (1000) chris     (1000)     1660 2024-04-10 13:31:52.000000 btrview-0.5.0/btrview/scripts/btrsend.py
--rwxr-xr-x   0 chris     (1000) chris     (1000)     1843 2024-04-10 20:33:52.000000 btrview-0.5.0/btrview/scripts/btrview.py
--rw-r--r--   0 chris     (1000) chris     (1000)     7642 2024-04-10 20:22:21.000000 btrview-0.5.0/btrview/subvolume.py
--rw-r--r--   0 chris     (1000) chris     (1000)     1254 2024-04-10 13:31:52.000000 btrview-0.5.0/btrview/utils.py
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2024-04-10 20:48:29.356026 btrview-0.5.0/btrview.egg-info/
--rw-r--r--   0 chris     (1000) chris     (1000)     5948 2024-04-10 20:48:29.000000 btrview-0.5.0/btrview.egg-info/PKG-INFO
--rw-r--r--   0 chris     (1000) chris     (1000)      372 2024-04-10 20:48:29.000000 btrview-0.5.0/btrview.egg-info/SOURCES.txt
--rw-r--r--   0 chris     (1000) chris     (1000)        1 2024-04-10 20:48:29.000000 btrview-0.5.0/btrview.egg-info/dependency_links.txt
--rw-r--r--   0 chris     (1000) chris     (1000)       57 2024-04-10 20:48:29.000000 btrview-0.5.0/btrview.egg-info/entry_points.txt
--rw-r--r--   0 chris     (1000) chris     (1000)       64 2024-04-10 20:48:29.000000 btrview-0.5.0/btrview.egg-info/requires.txt
--rw-r--r--   0 chris     (1000) chris     (1000)        8 2024-04-10 20:48:29.000000 btrview-0.5.0/btrview.egg-info/top_level.txt
--rw-r--r--   0 chris     (1000) chris     (1000)     1072 2024-04-10 20:48:24.000000 btrview-0.5.0/pyproject.toml
--rw-r--r--   0 chris     (1000) chris     (1000)       38 2024-04-10 20:48:29.356026 btrview-0.5.0/setup.cfg
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2024-04-18 04:05:24.693535 btrview-0.6.0/
+-rw-r--r--   0 chris     (1000) chris     (1000)     1069 2023-05-17 21:10:51.000000 btrview-0.6.0/LICENSE.md
+-rw-r--r--   0 chris     (1000) chris     (1000)     5948 2024-04-18 04:05:24.693535 btrview-0.6.0/PKG-INFO
+-rw-r--r--   0 chris     (1000) chris     (1000)     4067 2024-04-10 22:20:31.000000 btrview-0.6.0/README.md
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2024-04-18 04:05:24.693535 btrview-0.6.0/btrview/
+-rw-r--r--   0 chris     (1000) chris     (1000)       86 2024-04-18 04:05:12.000000 btrview-0.6.0/btrview/__init__.py
+-rwxr-xr-x   0 chris     (1000) chris     (1000)     2172 2024-04-18 03:01:25.000000 btrview-0.6.0/btrview/__main__.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     3665 2024-04-18 01:10:40.000000 btrview-0.6.0/btrview/btr_dict.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     7362 2024-04-18 03:01:25.000000 btrview-0.6.0/btrview/btrfs.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     6934 2024-04-18 03:01:25.000000 btrview-0.6.0/btrview/rich_output.py
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2024-04-18 04:05:24.693535 btrview-0.6.0/btrview/scripts/
+-rwxr-xr-x   0 chris     (1000) chris     (1000)     2172 2024-04-18 03:01:25.000000 btrview-0.6.0/btrview/scripts/btrview.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     5914 2024-04-18 01:10:40.000000 btrview-0.6.0/btrview/subvolume.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     1254 2024-04-10 13:31:52.000000 btrview-0.6.0/btrview/utils.py
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2024-04-18 04:05:24.693535 btrview-0.6.0/btrview.egg-info/
+-rw-r--r--   0 chris     (1000) chris     (1000)     5948 2024-04-18 04:05:24.000000 btrview-0.6.0/btrview.egg-info/PKG-INFO
+-rw-r--r--   0 chris     (1000) chris     (1000)      388 2024-04-18 04:05:24.000000 btrview-0.6.0/btrview.egg-info/SOURCES.txt
+-rw-r--r--   0 chris     (1000) chris     (1000)        1 2024-04-18 04:05:24.000000 btrview-0.6.0/btrview.egg-info/dependency_links.txt
+-rw-r--r--   0 chris     (1000) chris     (1000)       57 2024-04-18 04:05:24.000000 btrview-0.6.0/btrview.egg-info/entry_points.txt
+-rw-r--r--   0 chris     (1000) chris     (1000)       64 2024-04-18 04:05:24.000000 btrview-0.6.0/btrview.egg-info/requires.txt
+-rw-r--r--   0 chris     (1000) chris     (1000)        8 2024-04-18 04:05:24.000000 btrview-0.6.0/btrview.egg-info/top_level.txt
+-rw-r--r--   0 chris     (1000) chris     (1000)     1070 2024-04-18 04:05:12.000000 btrview-0.6.0/pyproject.toml
+-rw-r--r--   0 chris     (1000) chris     (1000)       38 2024-04-18 04:05:24.693535 btrview-0.6.0/setup.cfg
```

### Comparing `btrview-0.5.0/LICENSE.md` & `btrview-0.6.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `btrview-0.5.0/PKG-INFO` & `btrview-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: btrview
-Version: 0.5.0
+Version: 0.6.0
 Summary: View btrfs snapshot trees
 Author: Chris Copley
 License: MIT License
         
         Copyright (c) 2022 Chris Copley
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `btrview-0.5.0/README.md` & `btrview-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `btrview-0.5.0/btrview/__main__.py` & `btrview-0.6.0/btrview/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,49 @@
 #!/usr/bin/env python
 import argparse
 
 import btrview
 from btrview.utils import check_root
-from btrview.rich_output import logic
+from btrview.rich_output import logic,SORT_FUNCS
+from btrview.btrfs import SubvolumeSieve
 
 def parser() -> argparse.ArgumentParser:
     """Returns the argument parser for the command line arguments"""
     arg_parser = argparse.ArgumentParser(
             description = "Better way to view btrfs filesystems.",
             epilog = f"btrview version {btrview.__version__}, created by Chris Copley")
 
     arg_parser.add_argument(
             "--labels",
             help="The label of the filesystem(s) to view",
             nargs="+",)
 
     arg_parser.add_argument(
-            "--include",
-            help = "Types of subvolumes to include in the tree. Default are root and unreachable.",
+            "--exclude",
+            help = "Types of subvolumes to exclude in the tree. Default is deleted. Pass the flag with no arguments to exclude no subvolumes.",
             nargs = "*",
-            choices = ("root","deleted","unreachable"),
-            default = ("root","unreachable"))
+            choices = SubvolumeSieve.SIEVES.keys(),
+            default = ("deleted",))
 
     arg_parser.add_argument(
             "--property",
             help = "The subvolume property to print out in the tree. These are the keys from the `btrfs subvolume show` command.",)
 
     arg_parser.add_argument(
+            "--sort",
+            help = "How to sort subvolumes.",
+            choices = SORT_FUNCS.keys(),
+            default = "size")
+
+    arg_parser.add_argument(
+            "--ascending",
+            help = "Sort ascending instead of descending",
+            action = "store_true")
+
+    arg_parser.add_argument(
             "--fold",
             help = "Fold child output greater than N lines.",
             metavar = "N",
             type = int)
 
     arg_parser.add_argument(
             "--export",
@@ -39,15 +51,13 @@
             help = "Export the specifed type instead of a rich table. Using this flag will still write to stdout. If you wish to save to a file use shell redirection.",)
 
     return arg_parser
 
 def main():
     check_root()
     args = parser().parse_args()
-    root = "root" in args.include
-    deleted = "deleted" in args.include
-    unreachable = "unreachable" in args.include
-    output = logic(args.labels, root, deleted, unreachable, args.property, args.fold, args.export)
+    output = logic(args.labels, args.exclude, args.property, 
+                   args.fold, args.export, SORT_FUNCS[args.sort], not args.ascending)
     print(output)
  
 if __name__ == "__main__":
     main()
```

### Comparing `btrview-0.5.0/btrview/btrfs.py` & `btrview-0.6.0/btrview/btrfs.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,53 @@
 """Classes and functions to interact with a btrfs filesystem."""
 import json
-import re
 from collections import defaultdict
 from pathlib import Path, PurePath
-from typing import Self
+from typing import Self, Callable, TypeAlias, Iterable
 
 from treelib import Tree
 
 from btrview.utils import run
 from btrview.subvolume import Subvolume, Mount
 
+Sieve: TypeAlias = Callable[[Subvolume], bool]
+
+class SubvolumeSieve:
+    """A class for sieving subvolumes"""
+    SIEVES: dict[str, Sieve] = {
+            "deleted": lambda s: s.deleted,
+            "root": lambda s: s.root_subvolume,
+            "snapshot": lambda s: s.snapshot and not s.root_subvolume,
+            "unreachable": lambda s: not (s.mounted or s.deleted),
+            "non-mounts": lambda s: not s.mount_points
+            }
+
+    def __init__(self, subvolumes: list[Subvolume]) -> None:
+        self.subvolumes = subvolumes
+
+    def sieve_str(self, string_sieves: Iterable[str]):
+        """Removes subvolumes from a list based on string"""
+        sieves = [self.SIEVES[s] for s in string_sieves]
+        return self.sieve(sieves)
+
+    def sieve(self, remove_funcs: Iterable[Sieve]) -> list[Subvolume]:
+        """Remove subvolumes from a list determined by an iterable of sieve functions"""
+        to_remove = []
+        for subvol in self.subvolumes:
+            #if any of them evaluate True, then remove
+            bools = [f(subvol) for f in remove_funcs]
+            remove = any(bools)
+            if remove:
+                #don't want to remove in place while iterating
+                to_remove.append(subvol)
+        copy = self.subvolumes.copy()
+        for subvol in to_remove:
+            copy.remove(subvol)
+        return copy
+    
 class Btrfs:
     """A class representing a btrfs filesystem"""
     _UUIDs:  dict[str,str] = dict()
     _all_mounts: defaultdict[str,set[Mount]] = defaultdict(set)
 
     def __init__(self, uuid: str, label: str|None = None) -> None:
         """Initialist with the filesystem uuid, and label if it exists."""
@@ -41,14 +75,22 @@
     @property
     def mounts(self) -> tuple[Mount,...]:
         """Returns the mounts for a certain filesystem as a tuple."""
         #cast to tuple makes for easier referencing, also has the benefit of
         #preventing direct access to the set object
         return tuple(self._all_mounts[self.uuid])
 
+    @property
+    def default_subvolume(self) -> str:
+        """Return the default subvolume for the filesystem"""
+        mount = self.mounts[0]
+        out = run(f"btrfs subvolume get-default {mount.target}")
+        subvol_id = out.stdout.split()[1]
+        return subvol_id
+
     @classmethod
     def get_filesystems(cls, labels:list[str] | None = None) -> list[Self]:
         """Returns a list of each filesystem on the system."""
         #had to be here in case nothing gets initialized
         if not cls._UUIDs:
             cls._get_mounts() 
         filesystems = []
@@ -57,68 +99,41 @@
                 fs = cls(uuid,label)
                 filesystems.append(fs)
         return filesystems
 
     @classmethod
     def _get_deleted_subvols(cls, subvols: list[Subvolume]) -> list[Subvolume]:
         """Returns a list of deleted subvolumes"""
-        uuids = {s.id("snap") for s in subvols}
-        puuids = set()
-        deleted_subvols = []
-        for subvol in subvols:
-            puuid = subvol.parent("snap")
-            if puuid and (puuid not in uuids) and (puuid not in puuids):
-                puuids.add(puuid)
-                deleted_dict = {"UUID":puuid,"Subvolume ID":puuid, "Name":puuid}
-                deleted_subvols.append(Subvolume(deleted_dict,tuple(),deleted=True))
+        uuids: set[str] = {s.id("snap") for s in subvols}
+        puuids: set[str] = {s.parent("snap") for s in subvols if s.parent("snap")}
+        deleted_puuids = puuids - uuids
+        deleted_subvols = [Subvolume.from_deleted(puuid) for puuid in deleted_puuids]
         return deleted_subvols
-            
-    def subvolumes(self, root: bool, deleted: bool, unreachable: bool,) -> list[Subvolume]:
+
+    def _parse_subvol_list(self, list_str: str) -> list[Subvolume]:
+        """Turns output from `btrfs subvolume list` command into a list of subvolumes"""
+        list_lines = list_str.splitlines()
+        return [Subvolume.from_list(line, self.mounts) for line in list_lines]
+
+    def subvolumes(self, remove: tuple[str, ...]) -> list[Subvolume]:
         """Return a list of subvolumes on the file system"""
         mount_point = self.mounts[0].target 
+        subvols = [] if "root" in remove else [Subvolume.from_ID("5",mount_point, self.mounts)]
         out = run(f"sudo btrfs subvolume list -apcguqR {mount_point}")
+        subvols.extend(self._parse_subvol_list(out.stdout))
+        subvols.extend(self._get_deleted_subvols(subvols))
+        sieve = SubvolumeSieve(subvols)
 
-        subvols = []
-        keys = "ID,gen,cgen,parent,parent_uuid,received_uuid,uuid".split(",")
-        vals = "Subvolume ID,Generation,Gen at creation,Parent ID,Parent UUID,Received UUID,UUID".split(",")
-        key_dict = {key:val for key,val in zip(keys,vals)}
-        for line in out.stdout.splitlines():
-            match_dict = {}
-            for key,val in key_dict.items():
-                match = re.search(f"\\b{key}\\s+(\\S+)",line)
-                if match and match.group(1) == "-":
-                    match_dict[val] = None
-                elif match :
-                    match_dict[val] = match.group(1)
-            path_match = re.search(r"path\s*(.*)",line).group(1).removeprefix("<FS_TREE>/")
-            match_dict["btrfs Path"] = Path(f"/{path_match}")
-            match_dict["Name"] = match_dict["btrfs Path"].name
-            subvols.append(Subvolume(match_dict,self.mounts))
-        if not unreachable:
-            to_remove = []
-            for subvol in subvols:
-                if not subvol.mounted:
-                    to_remove.append(subvol)
-            for subvol in to_remove:
-                subvols.remove(subvol)
-        #order matters here, root should override unreachable
-        if root:
-            root_subvol = Subvolume.from_ID("5", mount_point, self.mounts)
-            subvols.append(root_subvol)
-        #but also deleted needs to go after root
-        #this is kinda fragile, plan to fix it soon™
-        if deleted:
-            subvols.extend(self._get_deleted_subvols(subvols))
-        return subvols
+        return sieve.sieve_str(remove)
 
-    def forest(self, snapshots = False, root = True, deleted = False, unreachable = True,) -> list[Tree]:
+    def forest(self, snapshots: bool, remove: tuple[str, ...]) -> list[Tree]:
         """Returns a forest of subvolumes with parent/child relationships
         being based on subvolume layout or snapshots."""
         kind = "snap" if snapshots else "subvol"
-        return get_forest(self.subvolumes(root, deleted, unreachable), kind)
+        return get_forest(self.subvolumes(remove), kind)
         
     def __str__(self) -> str:
         return f"{self.label or self.uuid}"
 
 def subvol_in_list(ID: str, subvolumes: list[Subvolume], kind = "subvol") -> Subvolume | None:
     """Returns a subvolume from a list if there, else returns None."""
     for subvolume in subvolumes:
@@ -155,7 +170,8 @@
     """Turns a flat list of subvolumes into a forest of trees."""
     trees: list[Tree] = []
     subvolumes = subvolumes.copy()
     while subvolumes:
         subvol = subvolumes[0]
         get_tree(subvol, subvolumes, trees, kind)
     return trees
+
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `btrview-0.5.0/btrview/scripts/btrview.py` & `btrview-0.6.0/btrview/scripts/btrview.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,49 @@
 #!/usr/bin/env python
 import argparse
 
 import btrview
 from btrview.utils import check_root
-from btrview.rich_output import logic
+from btrview.rich_output import logic,SORT_FUNCS
+from btrview.btrfs import SubvolumeSieve
 
 def parser() -> argparse.ArgumentParser:
     """Returns the argument parser for the command line arguments"""
     arg_parser = argparse.ArgumentParser(
             description = "Better way to view btrfs filesystems.",
             epilog = f"btrview version {btrview.__version__}, created by Chris Copley")
 
     arg_parser.add_argument(
             "--labels",
             help="The label of the filesystem(s) to view",
             nargs="+",)
 
     arg_parser.add_argument(
-            "--include",
-            help = "Types of subvolumes to include in the tree. Default are root and unreachable.",
+            "--exclude",
+            help = "Types of subvolumes to exclude in the tree. Default is deleted. Pass the flag with no arguments to exclude no subvolumes.",
             nargs = "*",
-            choices = ("root","deleted","unreachable"),
-            default = ("root","unreachable"))
+            choices = SubvolumeSieve.SIEVES.keys(),
+            default = ("deleted",))
 
     arg_parser.add_argument(
             "--property",
             help = "The subvolume property to print out in the tree. These are the keys from the `btrfs subvolume show` command.",)
 
     arg_parser.add_argument(
+            "--sort",
+            help = "How to sort subvolumes.",
+            choices = SORT_FUNCS.keys(),
+            default = "size")
+
+    arg_parser.add_argument(
+            "--ascending",
+            help = "Sort ascending instead of descending",
+            action = "store_true")
+
+    arg_parser.add_argument(
             "--fold",
             help = "Fold child output greater than N lines.",
             metavar = "N",
             type = int)
 
     arg_parser.add_argument(
             "--export",
@@ -39,15 +51,13 @@
             help = "Export the specifed type instead of a rich table. Using this flag will still write to stdout. If you wish to save to a file use shell redirection.",)
 
     return arg_parser
 
 def main():
     check_root()
     args = parser().parse_args()
-    root = "root" in args.include
-    deleted = "deleted" in args.include
-    unreachable = "unreachable" in args.include
-    output = logic(args.labels, root, deleted, unreachable, args.property, args.fold, args.export)
+    output = logic(args.labels, args.exclude, args.property, 
+                   args.fold, args.export, SORT_FUNCS[args.sort], not args.ascending)
     print(output)
  
 if __name__ == "__main__":
     main()
```

### Comparing `btrview-0.5.0/btrview/subvolume.py` & `btrview-0.6.0/btrview/subvolume.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,87 +1,97 @@
 """Subvolume Classes and errors."""
-import subprocess
-import re
 from pathlib import Path, PurePath
-from datetime import datetime
 from typing import Self
 from dataclasses import dataclass
 
-from btrview.utils import get_UUIDs, run
+from btrview.utils import run
+from btrview.btr_dict import BtrDict, BtrfsDict
 
 class NotASubvolumeError(NotADirectoryError):
     """Throw when a directory isn't a subvolume"""
 
 @dataclass(frozen=True)
 class Mount:
     """Basic class for working with mounted subvolumes."""
     fsroot: PurePath
     target: Path
 
-    def resolve(self, path: str) -> Path:
+    def resolve(self, path: Path) -> Path:
         """Returns the resolved path of another path"""
         fsroot_str = str(self.fsroot)
         target_str = str(self.target)
         if fsroot_str == "/":
             target_str = target_str + "/"
         path_str = str(path)
         new_path = path_str.replace(fsroot_str,target_str,1).replace("//","/",1)
         return Path(new_path)
 
     def __str__(self) -> str:
         return f"{self.fsroot} on {self.target}"
 
 class Subvolume:
     """Class representing a btrfs subvolume"""
-    def __init__(self, props: dict[str,str|None], mounts: tuple[Mount, ...],
+    def __init__(self, props: BtrDict, mounts: tuple[Mount, ...],
                  deleted: bool = False, show: bool = False) -> None:
         self.props = props
         self.mounts = mounts
         self.deleted = deleted
         self._show = show
 
     @property
     def paths(self) -> list[Path]:
-        if not self["btrfs Path"]:
+        """Returns all the reachable paths of the Subvolume"""
+        if self["btrfs Path"] is None:
             return []
         btr_path = Path(self["btrfs Path"])
         paths = [mount.resolve(btr_path) for mount in self.mounts if btr_path.is_relative_to(mount.fsroot)]
         paths = [path for path in paths if path.exists()]
         return paths
 
-
     @property
     def mounted(self) -> bool:
+        """Returns whether the subvolume is reachable via the filesystem"""
         return bool(self.paths)
 
     @property
+    def root_subvolume(self) -> bool:
+        """Returns whether the subvolume is the root_subvolume"""
+        return self["Subvolume ID"] == "5"
+
+    @property
+    def snapshot(self) -> bool:
+        """Returns whether the subvolume is a snapshot"""
+        return bool(self["Parent UUID"])
+
+    @property
     def mount_points(self) -> tuple[Path, ...]:
+        """Returns mount points of Subvolume"""
         targets = [mount.target for mount in self.mounts]
         return tuple(path for path in self.paths if path in targets)
 
     def parent(self, p_type: str) -> str | None:
         """Returns parent UUID or ID string"""
         match p_type:
             case "snap":
                 parent = self["Received UUID"] or self["Parent UUID"]
             case "subvol":
                 parent = self["Parent ID"]
             case _:
                 parent = None
         return parent
 
-    def id(self, p_type: str) -> str | None:
+    def id(self, p_type: str) -> str:
         """Returns subvolume UUID or ID string"""
         match p_type:
             case "snap":
                 ID = self["UUID"]
             case "subvol":
                 ID = self["Subvolume ID"]
             case _:
-                ID = None
+                ID = self["UUID"]
         return ID
 
     @classmethod
     def from_UUID(cls, uuid: str, path: str | Path, mounts: tuple[Mount, ...]) -> Self:
         """Creates subvolume from the subvolumes UUID and any path on the filesystem"""
         cmd = f"btrfs subvolume show -u {uuid} {path}"
         props = cls._run_cmd(cmd)
@@ -91,39 +101,34 @@
     def from_ID(cls, ID: str, path: str | Path, mounts: tuple[Mount, ...]) -> Self:
         """Creates subvolume from subvolume's ID and any path on the filesystem"""
         cmd = f"btrfs subvolume show -r {ID} {path}"
         props = cls._run_cmd(cmd)
         return cls(props, mounts, show = True)
 
     @classmethod
-    def _run_cmd(cls, cmd: str) -> dict[str, str | None]:
+    def from_list(cls, list_str: str, mounts: tuple[Mount, ...]) -> Self:
+        props = BtrfsDict.from_list(list_str).btr_dict
+        return cls(props, mounts)
+
+    @classmethod
+    def from_deleted(cls, UUID: str) -> Self:
+        """Creates subvolume from subvolume's ID and any path on the filesystem"""
+        props: BtrDict = {"UUID":UUID,"Subvolume ID":UUID, "Name":UUID}
+        return cls(props, tuple(), deleted=True)
+
+    @classmethod
+    def _run_cmd(cls, cmd: str) -> BtrDict:
         """Runs the shell command and returns the prop dictionary
         if the command doesn't error"""
         out = run(cmd)
         if out.returncode != 0:
             raise NotASubvolumeError
-        props = cls._get_props(out.stdout)
+        props = BtrfsDict.from_show(out.stdout).btr_dict
         return props
 
-    @classmethod
-    def _get_props(cls, btrfs_show_text: str) -> dict[str, str | None]:
-        """Creates btrfs prop dict based on the output of 
-        btrfs subvolume show."""
-        subvol = {}
-        lines = btrfs_show_text.splitlines()
-        subvol["btrfs Path"] = ("/" + lines[0]).replace("//","/")
-        for line in lines[1:]:
-            if re.search(r":\s+",line):
-                k,v = line.split(":",maxsplit=1)
-                k = k.strip()
-                v = v.strip()
-                v = None if v == "-" else v
-                subvol[k] = v
-        return subvol
-
     @staticmethod
     def is_btrfs(path: Path) -> bool:
         """Returns true if path is part of a btrfs filesystem."""
         response = run(f"btrfs filesystem usage '{path}'")
         return response.returncode == 0
 
     def __getitem__(self, key: str) -> str | None:
@@ -157,56 +162,7 @@
         return str(string)
 
     def __hash__(self) -> int:
         return hash(self["UUID"])
 
     def __eq__(self, other) -> bool:
         return self["UUID"] == other["UUID"]
-
-class MountedSubvolume(Subvolume):
-    """Class representing a mounted subvolume. Differs from a normal Subvolume
-    in that it can be snapshotted and sent since there's a path to it."""
-    def __init__(self, props: dict[str, str| None], path: Path) -> None:
-        self.props = props
-        self.path = path
-
-    @classmethod
-    def from_path(cls, path: str | Path) -> Self:
-        cmd = f"btrfs subvolume show {path}"
-        props = cls._run_cmd(cmd)
-        path = Path(path)
-        return cls(props, path)
-
-    def same_mount(self, path: Path) -> bool:
-        """Returns true if a subvolume is on the same filesystem as a specified path"""
-        return get_UUIDs(self.path) == get_UUIDs(path)
-
-    def snapshot(self, snap_dir: Path, format_str: str = "") -> Self:
-        """Take a snapshot of the subvolume and save it to snap_dir"""
-        if not snap_dir.is_dir():
-            raise NotADirectoryError
-        if format_str:
-            timestamp = datetime.now().astimezone().strftime(format_str)
-        else:
-            timestamp = datetime.now().astimezone().isoformat()
-        snap_file = snap_dir / timestamp
-        out = run(f"btrfs subvolume snapshot -r '{self.path}' '{snap_file}'")
-        return type(self).from_path(snap_file)
-
-    def send(self, path: Path) -> Self:
-        """Sends the subvolume to another filesystem"""
-        try:
-            #note that `shell=True` has some security implications with
-            #user input, but figuring out how to properly do this with
-            #subprocess.Popen() is not what I want to do right now.
-            subprocess.run(f"btrfs send {self} | btrfs receive {path}", shell=True, check=True)
-        except Exception as e:
-            run(f"btrfs subvolume delete '{path}'")
-            print(e)
-        return type(self).from_path(path / self.path.name)
-
-    def delete(self) -> Subvolume:
-        """Deletes the subvolume"""
-        run(f"btrfs subvolume delete '{self}'")
-        props = {"UUID":self["UUID"]}
-        return Subvolume(props, tuple(), deleted=True)
-
```

### Comparing `btrview-0.5.0/btrview/utils.py` & `btrview-0.6.0/btrview/utils.py`

 * *Files identical despite different names*

### Comparing `btrview-0.5.0/btrview.egg-info/PKG-INFO` & `btrview-0.6.0/btrview.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: btrview
-Version: 0.5.0
+Version: 0.6.0
 Summary: View btrfs snapshot trees
 Author: Chris Copley
 License: MIT License
         
         Copyright (c) 2022 Chris Copley
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `btrview-0.5.0/pyproject.toml` & `btrview-0.6.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "btrview"
-version = "0.5.0"
+version = "0.6.0"
 description = "View btrfs snapshot trees"
 readme = "README.md"
 authors = [{name = "Chris Copley"}]
 license = {file = "LICENSE.md"}
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -25,24 +25,24 @@
 btrview = "btrview.scripts.btrview:main"
 
 [build-system]
 requires      = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [tool.bumpver]
-current_version = "0.5.0"
+current_version = "0.6.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 tag_message = "{new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.setuptools]
-py-modules = ["btrview"]
+packages = ["btrview"]
 
 [tool.bumpver.file_patterns]
 "pyproject.toml" = [
     'current_version = "{version}"',
     'version = "{version}"',
 ]
 "btrview/__init__.py" = ["{version}"]
```

