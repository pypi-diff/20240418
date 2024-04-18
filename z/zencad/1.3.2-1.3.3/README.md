# Comparing `tmp/zencad-1.3.2.tar.gz` & `tmp/zencad-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zencad-1.3.2.tar", last modified: Wed Apr 17 09:10:41 2024, max compression
+gzip compressed data, was "zencad-1.3.3.tar", last modified: Thu Apr 18 13:34:16 2024, max compression
```

## Comparing `zencad-1.3.2.tar` & `zencad-1.3.3.tar`

### file list

```diff
@@ -1,189 +1,189 @@
-drwxrwxr-x   0 mirmik    (1000) mirmik    (1000)        0 2024-04-17 09:10:41.852691 zencad-1.3.2/
--rw-rw-r--   0 mirmik    (1000) mirmik    (1000)     1067 2023-06-20 06:58:00.000000 zencad-1.3.2/LICENSE.txt
--rw-rw-r--   0 mirmik    (1000) mirmik    (1000)      245 2023-06-20 06:58:00.000000 zencad-1.3.2/MANIFEST.in
--rw-rw-r--   0 mirmik    (1000) mirmik    (1000)     2612 2024-04-17 09:10:41.852691 zencad-1.3.2/PKG-INFO
--rw-rw-r--   0 mirmik    (1000) mirmik    (1000)     2253 2023-06-20 06:58:00.000000 zencad-1.3.2/README.md
--rw-rw-r--   0 mirmik    (1000) mirmik    (1000)       38 2024-04-17 09:10:41.852691 zencad-1.3.2/setup.cfg
--rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)     1630 2024-04-17 09:06:21.000000 zencad-1.3.2/setup.py
-drwxrwxr-x   0 mirmik    (1000) mirmik    (1000)        0 2024-04-17 09:10:41.824691 zencad-1.3.2/zencad/
--rw-rw-r--   0 mirmik    (1000) mirmik    (1000)     3459 2023-08-16 06:34:27.000000 zencad-1.3.2/zencad/__init__.py
--rw-rw-r--   0 mirmik    (1000) mirmik    (1000)     4558 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/__main__.py
--rw-rw-r--   0 mirmik    (1000) mirmik    (1000)     3086 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/animate.py
--rw-rw-r--   0 mirmik    (1000) mirmik    (1000)       42 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/assemble.py
--rw-rw-r--   0 mirmik    (1000) mirmik    (1000)      491 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/axis.py
--rw-rw-r--   0 mirmik    (1000) mirmik    (1000)     1968 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/bbox.py
--rw-rw-r--   0 mirmik    (1000) mirmik    (1000)     2851 2023-08-16 06:34:27.000000 zencad-1.3.2/zencad/color.py
-drwxrwxr-x   0 mirmik    (1000) mirmik    (1000)        0 2024-04-17 09:10:41.824691 zencad-1.3.2/zencad/convert/
--rw-rw-r--   0 mirmik    (1000) mirmik    (1000)     3287 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/convert/api.py
--rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)    10948 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/convert/svg.py
--rw-rw-r--   0 mirmik    (1000) mirmik    (1000)      677 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/convert/test.svg
--rw-rw-r--   0 mirmik    (1000) mirmik    (1000)      149 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/curve.py
-drwxrwxr-x   0 mirmik    (1000) mirmik    (1000)        0 2024-04-17 09:10:41.816691 zencad-1.3.2/zencad/examples/
-drwxrwxr-x   0 mirmik    (1000) mirmik    (1000)        0 2024-04-17 09:10:41.824691 zencad-1.3.2/zencad/examples/0.Base/
--rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)      243 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/examples/0.Base/csg.py
--rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)      194 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/examples/0.Base/helloworld.py
-drwxrwxr-x   0 mirmik    (1000) mirmik    (1000)        0 2024-04-17 09:10:41.816691 zencad-1.3.2/zencad/examples/1.GeomPrim/
-drwxrwxr-x   0 mirmik    (1000) mirmik    (1000)        0 2024-04-17 09:10:41.828691 zencad-1.3.2/zencad/examples/1.GeomPrim/1.prim3d/
--rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)     1118 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/examples/1.GeomPrim/1.prim3d/box.py
--rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)      514 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/examples/1.GeomPrim/1.prim3d/cone.py
--rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)      688 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/examples/1.GeomPrim/1.prim3d/cylinder.py
--rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)     1110 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/examples/1.GeomPrim/1.prim3d/halfspace.py
--rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)      284 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/examples/1.GeomPrim/1.prim3d/platonic.py
--rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)      630 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/examples/1.GeomPrim/1.prim3d/sphere.py
--rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)      471 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/examples/1.GeomPrim/1.prim3d/torus.py
-drwxrwxr-x   0 mirmik    (1000) mirmik    (1000)        0 2024-04-17 09:10:41.828691 zencad-1.3.2/zencad/examples/1.GeomPrim/2.prim2d/
--rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)      734 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/examples/1.GeomPrim/2.prim2d/circle.py
--rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)      928 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/examples/1.GeomPrim/2.prim2d/ellipse.py
--rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)     1152 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/examples/1.GeomPrim/2.prim2d/fillet_ngon.py
--rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)      350 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/examples/1.GeomPrim/2.prim2d/interpolate2.py
--rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)      425 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/examples/1.GeomPrim/2.prim2d/ngon.py
--rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)      140 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/examples/1.GeomPrim/2.prim2d/polygon.py
--rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)      386 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/examples/1.GeomPrim/2.prim2d/rectangle.py
--rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)     1067 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/examples/1.GeomPrim/2.prim2d/textshape.py
--rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)      312 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/examples/1.GeomPrim/2.prim2d/widewire.py
-drwxrwxr-x   0 mirmik    (1000) mirmik    (1000)        0 2024-04-17 09:10:41.828691 zencad-1.3.2/zencad/examples/1.GeomPrim/3.prim1d/
--rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)      315 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/examples/1.GeomPrim/3.prim1d/bezier.py
--rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)      889 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/examples/1.GeomPrim/3.prim1d/bspline.py
--rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)      324 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/examples/1.GeomPrim/3.prim1d/helix.py
--rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)      200 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/examples/1.GeomPrim/3.prim1d/interpolate.py
--rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)      463 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/examples/1.GeomPrim/3.prim1d/polysegment.py
--rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)      579 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/examples/1.GeomPrim/3.prim1d/rounded_polysegment.py
--rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)      143 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/examples/1.GeomPrim/3.prim1d/segment.py
-drwxrwxr-x   0 mirmik    (1000) mirmik    (1000)        0 2024-04-17 09:10:41.832691 zencad-1.3.2/zencad/examples/2.Operations/
-drwxrwxr-x   0 mirmik    (1000) mirmik    (1000)        0 2024-04-17 09:10:41.832691 zencad-1.3.2/zencad/examples/2.Operations/1.AphineTrans/
--rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)     1033 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/examples/2.Operations/1.AphineTrans/rotate_array.py
--rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)      299 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/examples/2.Operations/1.AphineTrans/scale.py
--rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)     1934 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/examples/2.Operations/1.AphineTrans/short_rotate.py
-drwxrwxr-x   0 mirmik    (1000) mirmik    (1000)        0 2024-04-17 09:10:41.832691 zencad-1.3.2/zencad/examples/2.Operations/2.Operations/
--rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)      542 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/examples/2.Operations/2.Operations/loft.py
--rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)      122 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/examples/2.Operations/2.Operations/offset.py
--rw-rw-r--   0 mirmik    (1000) mirmik    (1000)      162 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/examples/2.Operations/2.Operations/thicksolid.py
-drwxrwxr-x   0 mirmik    (1000) mirmik    (1000)        0 2024-04-17 09:10:41.832691 zencad-1.3.2/zencad/examples/2.Operations/3.Sweep/
--rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)      234 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/examples/2.Operations/3.Sweep/extrude.py
--rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)      816 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/examples/2.Operations/3.Sweep/pipe_shell.py
--rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)      446 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/examples/2.Operations/3.Sweep/pipe_shell_frenet.py
--rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)     1016 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/examples/2.Operations/3.Sweep/revol.py
--rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)      686 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/examples/2.Operations/3.Sweep/revol2.py
--rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)     1662 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/examples/2.Operations/3.Sweep/tube.py
--rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)      620 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/examples/2.Operations/3.Sweep/tube_by_points.py
-drwxrwxr-x   0 mirmik    (1000) mirmik    (1000)        0 2024-04-17 09:10:41.832691 zencad-1.3.2/zencad/examples/2.Operations/4.Mesh/
--rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)     1234 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/examples/2.Operations/4.Mesh/triangulate.py
--rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)     1489 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/examples/2.Operations/boolean.py
--rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)      265 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/examples/2.Operations/unify.py
-drwxrwxr-x   0 mirmik    (1000) mirmik    (1000)        0 2024-04-17 09:10:41.832691 zencad-1.3.2/zencad/examples/3.Animation/
--rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)      276 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/examples/3.Animation/base.py
--rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)      272 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/examples/3.Animation/camera.py
--rw-rw-r--   0 mirmik    (1000) mirmik    (1000)      598 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/examples/3.Animation/change_color.py
--rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)      598 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/examples/3.Animation/color.py
--rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)     2013 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/examples/3.Animation/pacman.py
-drwxrwxr-x   0 mirmik    (1000) mirmik    (1000)        0 2024-04-17 09:10:41.836691 zencad-1.3.2/zencad/examples/4.Assemble/
--rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)      923 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/examples/4.Assemble/EulerAngles.py
--rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)     2837 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/examples/4.Assemble/manual-control-2.py
--rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)     1783 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/examples/4.Assemble/manual-control.py
--rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)     6504 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/examples/4.Assemble/robot.py
-drwxrwxr-x   0 mirmik    (1000) mirmik    (1000)        0 2024-04-17 09:10:41.836691 zencad-1.3.2/zencad/examples/Integration/
-drwxrwxr-x   0 mirmik    (1000) mirmik    (1000)        0 2024-04-17 09:10:41.836691 zencad-1.3.2/zencad/examples/Integration/pillow/
--rw-rw-r--   0 mirmik    (1000) mirmik    (1000)    24512 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/examples/Integration/pillow/senku.png
--rw-rw-r--   0 mirmik    (1000) mirmik    (1000)    12025 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/examples/Integration/pillow/smile.png
--rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)      490 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/examples/Integration/pillow/smile.py
-drwxrwxr-x   0 mirmik    (1000) mirmik    (1000)        0 2024-04-17 09:10:41.836691 zencad-1.3.2/zencad/examples/Integration/skimage-mechanicus/
--rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)     1144 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/examples/Integration/skimage-mechanicus/cube.py
--rw-rw-r--   0 mirmik    (1000) mirmik    (1000)   203132 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/examples/Integration/skimage-mechanicus/image.png
--rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)     2697 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/examples/Integration/skimage-mechanicus/mech.py
--rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)      714 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/examples/Integration/svg.py
-drwxrwxr-x   0 mirmik    (1000) mirmik    (1000)        0 2024-04-17 09:10:41.836691 zencad-1.3.2/zencad/examples/Integration/trimesh/
--rw-rw-r--   0 mirmik    (1000) mirmik    (1000)       60 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/examples/Integration/trimesh/README.md
--rw-rw-r--   0 mirmik    (1000) mirmik    (1000)    17484 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/examples/Integration/trimesh/bulbasaur.STL
--rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)      453 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/examples/Integration/trimesh/bulbasaur.py
-drwxrwxr-x   0 mirmik    (1000) mirmik    (1000)        0 2024-04-17 09:10:41.836691 zencad-1.3.2/zencad/examples/MiniGames/
--rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)     3384 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/examples/MiniGames/tennis.py
--rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)     5924 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/examples/MiniGames/tetris.py
-drwxrwxr-x   0 mirmik    (1000) mirmik    (1000)        0 2024-04-17 09:10:41.836691 zencad-1.3.2/zencad/examples/Models/
--rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)     1848 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/examples/Models/bottle.py
--rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)      770 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/examples/Models/cup.py
--rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)     1604 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/examples/Models/logo.py
--rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)     1177 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/examples/Models/nut.py
-drwxrwxr-x   0 mirmik    (1000) mirmik    (1000)        0 2024-04-17 09:10:41.836691 zencad-1.3.2/zencad/examples/Models/organizer/
--rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)      443 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/examples/Models/organizer/assembly.py
--rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)      650 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/examples/Models/organizer/case.py
--rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)     1004 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/examples/Models/organizer/organizer.py
-drwxrwxr-x   0 mirmik    (1000) mirmik    (1000)        0 2024-04-17 09:10:41.840691 zencad-1.3.2/zencad/examples/OpenscadLike/
--rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)      243 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/examples/OpenscadLike/csg.py
--rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)      358 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/examples/OpenscadLike/logo.py
-drwxrwxr-x   0 mirmik    (1000) mirmik    (1000)        0 2024-04-17 09:10:41.840691 zencad-1.3.2/zencad/examples/fonts/
--rw-rw-r--   0 mirmik    (1000) mirmik    (1000)    85884 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/examples/fonts/mandarinc.ttf
--rw-rw-r--   0 mirmik    (1000) mirmik    (1000)   205748 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/examples/fonts/testfont.ttf
-drwxrwxr-x   0 mirmik    (1000) mirmik    (1000)        0 2024-04-17 09:10:41.844691 zencad-1.3.2/zencad/geom/
--rw-rw-r--   0 mirmik    (1000) mirmik    (1000)     2895 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/geom/boolops.py
--rw-rw-r--   0 mirmik    (1000) mirmik    (1000)      667 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/geom/boolops_base.py
--rw-rw-r--   0 mirmik    (1000) mirmik    (1000)     4305 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/geom/curve.py
--rw-rw-r--   0 mirmik    (1000) mirmik    (1000)     1836 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/geom/curve2.py
--rw-rw-r--   0 mirmik    (1000) mirmik    (1000)     3767 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/geom/curve_algo.py
--rw-rw-r--   0 mirmik    (1000) mirmik    (1000)     2818 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/geom/exttrans.py
--rw-rw-r--   0 mirmik    (1000) mirmik    (1000)     9128 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/geom/face.py
--rw-rw-r--   0 mirmik    (1000) mirmik    (1000)     1630 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/geom/general_transformation.py
--rw-rw-r--   0 mirmik    (1000) mirmik    (1000)     2152 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/geom/near.py
--rw-rw-r--   0 mirmik    (1000) mirmik    (1000)     1194 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/geom/offset.py
--rw-rw-r--   0 mirmik    (1000) mirmik    (1000)     5046 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/geom/operations.py
--rw-rw-r--   0 mirmik    (1000) mirmik    (1000)     6973 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/geom/platonic.py
--rw-rw-r--   0 mirmik    (1000) mirmik    (1000)      309 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/geom/project.py
--rw-rw-r--   0 mirmik    (1000) mirmik    (1000)     1069 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/geom/reflect_helpers.py
--rw-rw-r--   0 mirmik    (1000) mirmik    (1000)     2712 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/geom/sew.py
--rw-rw-r--   0 mirmik    (1000) mirmik    (1000)    15185 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/geom/shape.py
--rw-rw-r--   0 mirmik    (1000) mirmik    (1000)     2397 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/geom/shell.py
--rw-rw-r--   0 mirmik    (1000) mirmik    (1000)     5883 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/geom/solid.py
--rw-rw-r--   0 mirmik    (1000) mirmik    (1000)     2200 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/geom/surface.py
--rw-rw-r--   0 mirmik    (1000) mirmik    (1000)     8419 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/geom/sweep.py
--rw-rw-r--   0 mirmik    (1000) mirmik    (1000)     1219 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/geom/sweep_law.py
--rw-rw-r--   0 mirmik    (1000) mirmik    (1000)     3696 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/geom/trans.py
--rw-rw-r--   0 mirmik    (1000) mirmik    (1000)     2563 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/geom/transformable.py
--rw-rw-r--   0 mirmik    (1000) mirmik    (1000)     4084 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/geom/unify.py
--rw-rw-r--   0 mirmik    (1000) mirmik    (1000)     4084 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/geom/unify_ops.py
--rw-rw-r--   0 mirmik    (1000) mirmik    (1000)     8648 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/geom/wire.py
--rw-rw-r--   0 mirmik    (1000) mirmik    (1000)     9556 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/geom/wire_builder.py
--rw-rw-r--   0 mirmik    (1000) mirmik    (1000)     6291 2023-06-21 08:27:57.000000 zencad-1.3.2/zencad/geombase.py
--rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)    14896 2024-04-17 09:05:09.000000 zencad-1.3.2/zencad/geometry_core_installer.py
-drwxrwxr-x   0 mirmik    (1000) mirmik    (1000)        0 2024-04-17 09:10:41.848691 zencad-1.3.2/zencad/gui/
--rw-rw-r--   0 mirmik    (1000) mirmik    (1000)    13641 2023-08-16 06:34:27.000000 zencad-1.3.2/zencad/gui/actions.py
--rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)    27047 2023-08-16 06:34:27.000000 zencad-1.3.2/zencad/gui/display.py
--rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)     1046 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/gui/display_only.py
--rw-rw-r--   0 mirmik    (1000) mirmik    (1000)      394 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/gui/display_unbounded.py
--rw-rw-r--   0 mirmik    (1000) mirmik    (1000)     3370 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/gui/info_widget.py
--rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)     6999 2023-06-20 07:20:16.000000 zencad-1.3.2/zencad/gui/libinstaller.py
--rw-rw-r--   0 mirmik    (1000) mirmik    (1000)     3436 2023-06-20 07:20:16.000000 zencad-1.3.2/zencad/gui/mainwindow.py
--rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)     5143 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/gui/settingswdg.py
--rw-rw-r--   0 mirmik    (1000) mirmik    (1000)     1328 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/gui/util.py
--rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)     3340 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/gutil.py
--rw-rw-r--   0 mirmik    (1000) mirmik    (1000)     3395 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/industrial-robot.svg
-drwxrwxr-x   0 mirmik    (1000) mirmik    (1000)        0 2024-04-17 09:10:41.848691 zencad-1.3.2/zencad/interactive/
--rw-rw-r--   0 mirmik    (1000) mirmik    (1000)     1480 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/interactive/__init__.py
--rw-rw-r--   0 mirmik    (1000) mirmik    (1000)    12178 2023-08-16 06:34:27.000000 zencad-1.3.2/zencad/interactive/assemble.py
--rw-rw-r--   0 mirmik    (1000) mirmik    (1000)      284 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/interactive/axis.py
--rw-rw-r--   0 mirmik    (1000) mirmik    (1000)       91 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/interactive/displayable.py
--rw-rw-r--   0 mirmik    (1000) mirmik    (1000)     4002 2023-08-16 06:34:27.000000 zencad-1.3.2/zencad/interactive/interactive_object.py
--rw-rw-r--   0 mirmik    (1000) mirmik    (1000)     1942 2023-06-21 11:51:36.000000 zencad-1.3.2/zencad/interactive/line.py
--rw-rw-r--   0 mirmik    (1000) mirmik    (1000)      585 2023-06-21 08:27:57.000000 zencad-1.3.2/zencad/interactive/point.py
--rw-rw-r--   0 mirmik    (1000) mirmik    (1000)      627 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/interactive/shape.py
-drwxrwxr-x   0 mirmik    (1000) mirmik    (1000)        0 2024-04-17 09:10:41.852691 zencad-1.3.2/zencad/internal_models/
--rw-rw-r--   0 mirmik    (1000) mirmik    (1000)       37 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/internal_models/__init__.py
--rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)     2442 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/internal_models/knight.py
--rw-rw-r--   0 mirmik    (1000) mirmik    (1000)     2139 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/lazifier.py
-drwxrwxr-x   0 mirmik    (1000) mirmik    (1000)        0 2024-04-17 09:10:41.852691 zencad-1.3.2/zencad/libs/
--rw-rw-r--   0 mirmik    (1000) mirmik    (1000)     6781 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/libs/kinematic.py
--rw-rw-r--   0 mirmik    (1000) mirmik    (1000)     6570 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/libs/malgo.py
--rw-rw-r--   0 mirmik    (1000) mirmik    (1000)     4030 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/libs/screw.py
--rw-rw-r--   0 mirmik    (1000) mirmik    (1000)     1307 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/opencascade_types.py
--rw-rw-r--   0 mirmik    (1000) mirmik    (1000)     1961 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/scene.py
--rw-rw-r--   0 mirmik    (1000) mirmik    (1000)     1077 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/settings.py
--rw-rw-r--   0 mirmik    (1000) mirmik    (1000)     3362 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/showapi.py
--rw-rw-r--   0 mirmik    (1000) mirmik    (1000)    97883 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/techpriest.jpg
--rw-rw-r--   0 mirmik    (1000) mirmik    (1000)     1713 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/util.py
--rw-rw-r--   0 mirmik    (1000) mirmik    (1000)      319 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/version.py
--rw-rw-r--   0 mirmik    (1000) mirmik    (1000)   173855 2023-06-20 06:58:00.000000 zencad-1.3.2/zencad/zencad_logo.png
-drwxrwxr-x   0 mirmik    (1000) mirmik    (1000)        0 2024-04-17 09:10:41.824691 zencad-1.3.2/zencad.egg-info/
--rw-rw-r--   0 mirmik    (1000) mirmik    (1000)     2612 2024-04-17 09:10:40.000000 zencad-1.3.2/zencad.egg-info/PKG-INFO
--rw-rw-r--   0 mirmik    (1000) mirmik    (1000)     5247 2024-04-17 09:10:40.000000 zencad-1.3.2/zencad.egg-info/SOURCES.txt
--rw-rw-r--   0 mirmik    (1000) mirmik    (1000)        1 2024-04-17 09:10:40.000000 zencad-1.3.2/zencad.egg-info/dependency_links.txt
--rw-rw-r--   0 mirmik    (1000) mirmik    (1000)       49 2024-04-17 09:10:40.000000 zencad-1.3.2/zencad.egg-info/entry_points.txt
--rw-rw-r--   0 mirmik    (1000) mirmik    (1000)       92 2024-04-17 09:10:40.000000 zencad-1.3.2/zencad.egg-info/requires.txt
--rw-rw-r--   0 mirmik    (1000) mirmik    (1000)        7 2024-04-17 09:10:40.000000 zencad-1.3.2/zencad.egg-info/top_level.txt
+drwxrwxr-x   0 mirmik    (1000) mirmik    (1000)        0 2024-04-18 13:34:16.041184 zencad-1.3.3/
+-rw-rw-r--   0 mirmik    (1000) mirmik    (1000)     1067 2023-06-20 06:58:00.000000 zencad-1.3.3/LICENSE.txt
+-rw-rw-r--   0 mirmik    (1000) mirmik    (1000)      245 2023-06-20 06:58:00.000000 zencad-1.3.3/MANIFEST.in
+-rw-rw-r--   0 mirmik    (1000) mirmik    (1000)     2612 2024-04-18 13:34:16.041184 zencad-1.3.3/PKG-INFO
+-rw-rw-r--   0 mirmik    (1000) mirmik    (1000)     2253 2023-06-20 06:58:00.000000 zencad-1.3.3/README.md
+-rw-rw-r--   0 mirmik    (1000) mirmik    (1000)       38 2024-04-18 13:34:16.041184 zencad-1.3.3/setup.cfg
+-rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)     1630 2024-04-18 13:31:51.000000 zencad-1.3.3/setup.py
+drwxrwxr-x   0 mirmik    (1000) mirmik    (1000)        0 2024-04-18 13:34:16.005183 zencad-1.3.3/zencad/
+-rw-rw-r--   0 mirmik    (1000) mirmik    (1000)     3459 2023-08-16 06:34:27.000000 zencad-1.3.3/zencad/__init__.py
+-rw-rw-r--   0 mirmik    (1000) mirmik    (1000)     4558 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/__main__.py
+-rw-rw-r--   0 mirmik    (1000) mirmik    (1000)     3086 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/animate.py
+-rw-rw-r--   0 mirmik    (1000) mirmik    (1000)       42 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/assemble.py
+-rw-rw-r--   0 mirmik    (1000) mirmik    (1000)      491 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/axis.py
+-rw-rw-r--   0 mirmik    (1000) mirmik    (1000)     1968 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/bbox.py
+-rw-rw-r--   0 mirmik    (1000) mirmik    (1000)     2851 2023-08-16 06:34:27.000000 zencad-1.3.3/zencad/color.py
+drwxrwxr-x   0 mirmik    (1000) mirmik    (1000)        0 2024-04-18 13:34:16.005183 zencad-1.3.3/zencad/convert/
+-rw-rw-r--   0 mirmik    (1000) mirmik    (1000)     3287 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/convert/api.py
+-rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)    10948 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/convert/svg.py
+-rw-rw-r--   0 mirmik    (1000) mirmik    (1000)      677 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/convert/test.svg
+-rw-rw-r--   0 mirmik    (1000) mirmik    (1000)      149 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/curve.py
+drwxrwxr-x   0 mirmik    (1000) mirmik    (1000)        0 2024-04-18 13:34:15.997183 zencad-1.3.3/zencad/examples/
+drwxrwxr-x   0 mirmik    (1000) mirmik    (1000)        0 2024-04-18 13:34:16.005183 zencad-1.3.3/zencad/examples/0.Base/
+-rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)      243 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/examples/0.Base/csg.py
+-rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)      194 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/examples/0.Base/helloworld.py
+drwxrwxr-x   0 mirmik    (1000) mirmik    (1000)        0 2024-04-18 13:34:15.993183 zencad-1.3.3/zencad/examples/1.GeomPrim/
+drwxrwxr-x   0 mirmik    (1000) mirmik    (1000)        0 2024-04-18 13:34:16.009183 zencad-1.3.3/zencad/examples/1.GeomPrim/1.prim3d/
+-rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)     1118 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/examples/1.GeomPrim/1.prim3d/box.py
+-rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)      514 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/examples/1.GeomPrim/1.prim3d/cone.py
+-rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)      688 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/examples/1.GeomPrim/1.prim3d/cylinder.py
+-rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)     1110 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/examples/1.GeomPrim/1.prim3d/halfspace.py
+-rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)      284 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/examples/1.GeomPrim/1.prim3d/platonic.py
+-rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)      630 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/examples/1.GeomPrim/1.prim3d/sphere.py
+-rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)      471 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/examples/1.GeomPrim/1.prim3d/torus.py
+drwxrwxr-x   0 mirmik    (1000) mirmik    (1000)        0 2024-04-18 13:34:16.009183 zencad-1.3.3/zencad/examples/1.GeomPrim/2.prim2d/
+-rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)      734 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/examples/1.GeomPrim/2.prim2d/circle.py
+-rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)      928 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/examples/1.GeomPrim/2.prim2d/ellipse.py
+-rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)     1152 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/examples/1.GeomPrim/2.prim2d/fillet_ngon.py
+-rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)      350 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/examples/1.GeomPrim/2.prim2d/interpolate2.py
+-rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)      425 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/examples/1.GeomPrim/2.prim2d/ngon.py
+-rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)      140 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/examples/1.GeomPrim/2.prim2d/polygon.py
+-rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)      386 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/examples/1.GeomPrim/2.prim2d/rectangle.py
+-rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)     1067 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/examples/1.GeomPrim/2.prim2d/textshape.py
+-rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)      312 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/examples/1.GeomPrim/2.prim2d/widewire.py
+drwxrwxr-x   0 mirmik    (1000) mirmik    (1000)        0 2024-04-18 13:34:16.013183 zencad-1.3.3/zencad/examples/1.GeomPrim/3.prim1d/
+-rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)      315 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/examples/1.GeomPrim/3.prim1d/bezier.py
+-rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)      889 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/examples/1.GeomPrim/3.prim1d/bspline.py
+-rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)      324 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/examples/1.GeomPrim/3.prim1d/helix.py
+-rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)      200 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/examples/1.GeomPrim/3.prim1d/interpolate.py
+-rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)      463 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/examples/1.GeomPrim/3.prim1d/polysegment.py
+-rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)      579 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/examples/1.GeomPrim/3.prim1d/rounded_polysegment.py
+-rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)      143 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/examples/1.GeomPrim/3.prim1d/segment.py
+drwxrwxr-x   0 mirmik    (1000) mirmik    (1000)        0 2024-04-18 13:34:16.013183 zencad-1.3.3/zencad/examples/2.Operations/
+drwxrwxr-x   0 mirmik    (1000) mirmik    (1000)        0 2024-04-18 13:34:16.013183 zencad-1.3.3/zencad/examples/2.Operations/1.AphineTrans/
+-rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)     1033 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/examples/2.Operations/1.AphineTrans/rotate_array.py
+-rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)      299 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/examples/2.Operations/1.AphineTrans/scale.py
+-rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)     1934 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/examples/2.Operations/1.AphineTrans/short_rotate.py
+drwxrwxr-x   0 mirmik    (1000) mirmik    (1000)        0 2024-04-18 13:34:16.013183 zencad-1.3.3/zencad/examples/2.Operations/2.Operations/
+-rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)      542 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/examples/2.Operations/2.Operations/loft.py
+-rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)      122 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/examples/2.Operations/2.Operations/offset.py
+-rw-rw-r--   0 mirmik    (1000) mirmik    (1000)      162 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/examples/2.Operations/2.Operations/thicksolid.py
+drwxrwxr-x   0 mirmik    (1000) mirmik    (1000)        0 2024-04-18 13:34:16.017183 zencad-1.3.3/zencad/examples/2.Operations/3.Sweep/
+-rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)      234 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/examples/2.Operations/3.Sweep/extrude.py
+-rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)      816 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/examples/2.Operations/3.Sweep/pipe_shell.py
+-rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)      446 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/examples/2.Operations/3.Sweep/pipe_shell_frenet.py
+-rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)     1016 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/examples/2.Operations/3.Sweep/revol.py
+-rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)      686 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/examples/2.Operations/3.Sweep/revol2.py
+-rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)     1662 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/examples/2.Operations/3.Sweep/tube.py
+-rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)      620 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/examples/2.Operations/3.Sweep/tube_by_points.py
+drwxrwxr-x   0 mirmik    (1000) mirmik    (1000)        0 2024-04-18 13:34:16.017183 zencad-1.3.3/zencad/examples/2.Operations/4.Mesh/
+-rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)     1234 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/examples/2.Operations/4.Mesh/triangulate.py
+-rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)     1489 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/examples/2.Operations/boolean.py
+-rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)      265 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/examples/2.Operations/unify.py
+drwxrwxr-x   0 mirmik    (1000) mirmik    (1000)        0 2024-04-18 13:34:16.017183 zencad-1.3.3/zencad/examples/3.Animation/
+-rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)      276 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/examples/3.Animation/base.py
+-rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)      272 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/examples/3.Animation/camera.py
+-rw-rw-r--   0 mirmik    (1000) mirmik    (1000)      598 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/examples/3.Animation/change_color.py
+-rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)      598 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/examples/3.Animation/color.py
+-rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)     2013 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/examples/3.Animation/pacman.py
+drwxrwxr-x   0 mirmik    (1000) mirmik    (1000)        0 2024-04-18 13:34:16.017183 zencad-1.3.3/zencad/examples/4.Assemble/
+-rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)      923 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/examples/4.Assemble/EulerAngles.py
+-rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)     2837 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/examples/4.Assemble/manual-control-2.py
+-rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)     1783 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/examples/4.Assemble/manual-control.py
+-rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)     6504 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/examples/4.Assemble/robot.py
+drwxrwxr-x   0 mirmik    (1000) mirmik    (1000)        0 2024-04-18 13:34:16.017183 zencad-1.3.3/zencad/examples/Integration/
+drwxrwxr-x   0 mirmik    (1000) mirmik    (1000)        0 2024-04-18 13:34:16.021183 zencad-1.3.3/zencad/examples/Integration/pillow/
+-rw-rw-r--   0 mirmik    (1000) mirmik    (1000)    24512 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/examples/Integration/pillow/senku.png
+-rw-rw-r--   0 mirmik    (1000) mirmik    (1000)    12025 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/examples/Integration/pillow/smile.png
+-rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)      490 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/examples/Integration/pillow/smile.py
+drwxrwxr-x   0 mirmik    (1000) mirmik    (1000)        0 2024-04-18 13:34:16.021183 zencad-1.3.3/zencad/examples/Integration/skimage-mechanicus/
+-rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)     1144 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/examples/Integration/skimage-mechanicus/cube.py
+-rw-rw-r--   0 mirmik    (1000) mirmik    (1000)   203132 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/examples/Integration/skimage-mechanicus/image.png
+-rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)     2697 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/examples/Integration/skimage-mechanicus/mech.py
+-rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)      714 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/examples/Integration/svg.py
+drwxrwxr-x   0 mirmik    (1000) mirmik    (1000)        0 2024-04-18 13:34:16.021183 zencad-1.3.3/zencad/examples/Integration/trimesh/
+-rw-rw-r--   0 mirmik    (1000) mirmik    (1000)       60 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/examples/Integration/trimesh/README.md
+-rw-rw-r--   0 mirmik    (1000) mirmik    (1000)    17484 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/examples/Integration/trimesh/bulbasaur.STL
+-rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)      453 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/examples/Integration/trimesh/bulbasaur.py
+drwxrwxr-x   0 mirmik    (1000) mirmik    (1000)        0 2024-04-18 13:34:16.021183 zencad-1.3.3/zencad/examples/MiniGames/
+-rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)     3384 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/examples/MiniGames/tennis.py
+-rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)     5924 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/examples/MiniGames/tetris.py
+drwxrwxr-x   0 mirmik    (1000) mirmik    (1000)        0 2024-04-18 13:34:16.021183 zencad-1.3.3/zencad/examples/Models/
+-rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)     1848 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/examples/Models/bottle.py
+-rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)      770 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/examples/Models/cup.py
+-rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)     1604 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/examples/Models/logo.py
+-rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)     1177 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/examples/Models/nut.py
+drwxrwxr-x   0 mirmik    (1000) mirmik    (1000)        0 2024-04-18 13:34:16.025184 zencad-1.3.3/zencad/examples/Models/organizer/
+-rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)      443 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/examples/Models/organizer/assembly.py
+-rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)      650 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/examples/Models/organizer/case.py
+-rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)     1004 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/examples/Models/organizer/organizer.py
+drwxrwxr-x   0 mirmik    (1000) mirmik    (1000)        0 2024-04-18 13:34:16.025184 zencad-1.3.3/zencad/examples/OpenscadLike/
+-rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)      243 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/examples/OpenscadLike/csg.py
+-rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)      358 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/examples/OpenscadLike/logo.py
+drwxrwxr-x   0 mirmik    (1000) mirmik    (1000)        0 2024-04-18 13:34:16.025184 zencad-1.3.3/zencad/examples/fonts/
+-rw-rw-r--   0 mirmik    (1000) mirmik    (1000)    85884 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/examples/fonts/mandarinc.ttf
+-rw-rw-r--   0 mirmik    (1000) mirmik    (1000)   205748 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/examples/fonts/testfont.ttf
+drwxrwxr-x   0 mirmik    (1000) mirmik    (1000)        0 2024-04-18 13:34:16.033184 zencad-1.3.3/zencad/geom/
+-rw-rw-r--   0 mirmik    (1000) mirmik    (1000)     2895 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/geom/boolops.py
+-rw-rw-r--   0 mirmik    (1000) mirmik    (1000)      667 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/geom/boolops_base.py
+-rw-rw-r--   0 mirmik    (1000) mirmik    (1000)     4305 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/geom/curve.py
+-rw-rw-r--   0 mirmik    (1000) mirmik    (1000)     1836 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/geom/curve2.py
+-rw-rw-r--   0 mirmik    (1000) mirmik    (1000)     3767 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/geom/curve_algo.py
+-rw-rw-r--   0 mirmik    (1000) mirmik    (1000)     2818 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/geom/exttrans.py
+-rw-rw-r--   0 mirmik    (1000) mirmik    (1000)     9128 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/geom/face.py
+-rw-rw-r--   0 mirmik    (1000) mirmik    (1000)     1630 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/geom/general_transformation.py
+-rw-rw-r--   0 mirmik    (1000) mirmik    (1000)     2152 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/geom/near.py
+-rw-rw-r--   0 mirmik    (1000) mirmik    (1000)     1194 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/geom/offset.py
+-rw-rw-r--   0 mirmik    (1000) mirmik    (1000)     5046 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/geom/operations.py
+-rw-rw-r--   0 mirmik    (1000) mirmik    (1000)     6973 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/geom/platonic.py
+-rw-rw-r--   0 mirmik    (1000) mirmik    (1000)      309 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/geom/project.py
+-rw-rw-r--   0 mirmik    (1000) mirmik    (1000)     1069 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/geom/reflect_helpers.py
+-rw-rw-r--   0 mirmik    (1000) mirmik    (1000)     2712 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/geom/sew.py
+-rw-rw-r--   0 mirmik    (1000) mirmik    (1000)    15185 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/geom/shape.py
+-rw-rw-r--   0 mirmik    (1000) mirmik    (1000)     2397 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/geom/shell.py
+-rw-rw-r--   0 mirmik    (1000) mirmik    (1000)     5883 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/geom/solid.py
+-rw-rw-r--   0 mirmik    (1000) mirmik    (1000)     2200 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/geom/surface.py
+-rw-rw-r--   0 mirmik    (1000) mirmik    (1000)     8419 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/geom/sweep.py
+-rw-rw-r--   0 mirmik    (1000) mirmik    (1000)     1219 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/geom/sweep_law.py
+-rw-rw-r--   0 mirmik    (1000) mirmik    (1000)     3696 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/geom/trans.py
+-rw-rw-r--   0 mirmik    (1000) mirmik    (1000)     2563 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/geom/transformable.py
+-rw-rw-r--   0 mirmik    (1000) mirmik    (1000)     4084 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/geom/unify.py
+-rw-rw-r--   0 mirmik    (1000) mirmik    (1000)     4084 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/geom/unify_ops.py
+-rw-rw-r--   0 mirmik    (1000) mirmik    (1000)     8648 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/geom/wire.py
+-rw-rw-r--   0 mirmik    (1000) mirmik    (1000)     9556 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/geom/wire_builder.py
+-rw-rw-r--   0 mirmik    (1000) mirmik    (1000)     6291 2023-06-21 08:27:57.000000 zencad-1.3.3/zencad/geombase.py
+-rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)    14896 2024-04-17 09:05:09.000000 zencad-1.3.3/zencad/geometry_core_installer.py
+drwxrwxr-x   0 mirmik    (1000) mirmik    (1000)        0 2024-04-18 13:34:16.037184 zencad-1.3.3/zencad/gui/
+-rw-rw-r--   0 mirmik    (1000) mirmik    (1000)    13641 2023-08-16 06:34:27.000000 zencad-1.3.3/zencad/gui/actions.py
+-rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)    27047 2023-08-16 06:34:27.000000 zencad-1.3.3/zencad/gui/display.py
+-rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)     1046 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/gui/display_only.py
+-rw-rw-r--   0 mirmik    (1000) mirmik    (1000)      394 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/gui/display_unbounded.py
+-rw-rw-r--   0 mirmik    (1000) mirmik    (1000)     3370 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/gui/info_widget.py
+-rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)     6999 2023-06-20 07:20:16.000000 zencad-1.3.3/zencad/gui/libinstaller.py
+-rw-rw-r--   0 mirmik    (1000) mirmik    (1000)     3436 2023-06-20 07:20:16.000000 zencad-1.3.3/zencad/gui/mainwindow.py
+-rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)     5143 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/gui/settingswdg.py
+-rw-rw-r--   0 mirmik    (1000) mirmik    (1000)     1328 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/gui/util.py
+-rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)     3340 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/gutil.py
+-rw-rw-r--   0 mirmik    (1000) mirmik    (1000)     3395 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/industrial-robot.svg
+drwxrwxr-x   0 mirmik    (1000) mirmik    (1000)        0 2024-04-18 13:34:16.041184 zencad-1.3.3/zencad/interactive/
+-rw-rw-r--   0 mirmik    (1000) mirmik    (1000)     1480 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/interactive/__init__.py
+-rw-rw-r--   0 mirmik    (1000) mirmik    (1000)    12178 2023-08-16 06:34:27.000000 zencad-1.3.3/zencad/interactive/assemble.py
+-rw-rw-r--   0 mirmik    (1000) mirmik    (1000)      284 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/interactive/axis.py
+-rw-rw-r--   0 mirmik    (1000) mirmik    (1000)       91 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/interactive/displayable.py
+-rw-rw-r--   0 mirmik    (1000) mirmik    (1000)     4002 2023-08-16 06:34:27.000000 zencad-1.3.3/zencad/interactive/interactive_object.py
+-rw-rw-r--   0 mirmik    (1000) mirmik    (1000)     1942 2023-06-21 11:51:36.000000 zencad-1.3.3/zencad/interactive/line.py
+-rw-rw-r--   0 mirmik    (1000) mirmik    (1000)      585 2023-06-21 08:27:57.000000 zencad-1.3.3/zencad/interactive/point.py
+-rw-rw-r--   0 mirmik    (1000) mirmik    (1000)      627 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/interactive/shape.py
+drwxrwxr-x   0 mirmik    (1000) mirmik    (1000)        0 2024-04-18 13:34:16.041184 zencad-1.3.3/zencad/internal_models/
+-rw-rw-r--   0 mirmik    (1000) mirmik    (1000)       37 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/internal_models/__init__.py
+-rwxrwxr-x   0 mirmik    (1000) mirmik    (1000)     2442 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/internal_models/knight.py
+-rw-rw-r--   0 mirmik    (1000) mirmik    (1000)     2139 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/lazifier.py
+drwxrwxr-x   0 mirmik    (1000) mirmik    (1000)        0 2024-04-18 13:34:16.041184 zencad-1.3.3/zencad/libs/
+-rw-rw-r--   0 mirmik    (1000) mirmik    (1000)     6781 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/libs/kinematic.py
+-rw-rw-r--   0 mirmik    (1000) mirmik    (1000)     6570 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/libs/malgo.py
+-rw-rw-r--   0 mirmik    (1000) mirmik    (1000)     4030 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/libs/screw.py
+-rw-rw-r--   0 mirmik    (1000) mirmik    (1000)     1307 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/opencascade_types.py
+-rw-rw-r--   0 mirmik    (1000) mirmik    (1000)     1961 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/scene.py
+-rw-rw-r--   0 mirmik    (1000) mirmik    (1000)     1077 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/settings.py
+-rw-rw-r--   0 mirmik    (1000) mirmik    (1000)     3362 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/showapi.py
+-rw-rw-r--   0 mirmik    (1000) mirmik    (1000)    97883 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/techpriest.jpg
+-rw-rw-r--   0 mirmik    (1000) mirmik    (1000)     1713 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/util.py
+-rw-rw-r--   0 mirmik    (1000) mirmik    (1000)      319 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/version.py
+-rw-rw-r--   0 mirmik    (1000) mirmik    (1000)   173855 2023-06-20 06:58:00.000000 zencad-1.3.3/zencad/zencad_logo.png
+drwxrwxr-x   0 mirmik    (1000) mirmik    (1000)        0 2024-04-18 13:34:16.005183 zencad-1.3.3/zencad.egg-info/
+-rw-rw-r--   0 mirmik    (1000) mirmik    (1000)     2612 2024-04-18 13:34:15.000000 zencad-1.3.3/zencad.egg-info/PKG-INFO
+-rw-rw-r--   0 mirmik    (1000) mirmik    (1000)     5247 2024-04-18 13:34:15.000000 zencad-1.3.3/zencad.egg-info/SOURCES.txt
+-rw-rw-r--   0 mirmik    (1000) mirmik    (1000)        1 2024-04-18 13:34:15.000000 zencad-1.3.3/zencad.egg-info/dependency_links.txt
+-rw-rw-r--   0 mirmik    (1000) mirmik    (1000)       49 2024-04-18 13:34:15.000000 zencad-1.3.3/zencad.egg-info/entry_points.txt
+-rw-rw-r--   0 mirmik    (1000) mirmik    (1000)       92 2024-04-18 13:34:15.000000 zencad-1.3.3/zencad.egg-info/requires.txt
+-rw-rw-r--   0 mirmik    (1000) mirmik    (1000)        7 2024-04-18 13:34:15.000000 zencad-1.3.3/zencad.egg-info/top_level.txt
```

### Comparing `zencad-1.3.2/LICENSE.txt` & `zencad-1.3.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zencad-1.3.2/PKG-INFO` & `zencad-1.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: zencad
-Version: 1.3.2
+Version: 1.3.3
 Summary: CAD system for righteous zen programmers 
 Home-page: https://github.com/mirmik/zencad
 Author: mirmik
 Author-email: mirmikns@yandex.ru
 License: MIT
 Keywords: testing,cad
 Platform: UNKNOWN
-Requires-Python: >3.8.0
+Requires-Python: >3.6.0
 Description-Content-Type: text/markdown
 Provides-Extra: gui
 License-File: LICENSE.txt
 
 ZenCad
 ======
 CAD system for righteous zen programmers
```

### Comparing `zencad-1.3.2/README.md` & `zencad-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `zencad-1.3.2/setup.py` & `zencad-1.3.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 
 directory = os.path.dirname(os.path.realpath(__file__))
 
 
 setup(
     name="zencad",
     packages=["zencad"],
-    python_requires='>3.8.0',
-    version="1.3.2",
+    python_requires='>3.6.0',
+    version="1.3.3",
     license="MIT",
     description="CAD system for righteous zen programmers ",
     author="mirmik",
     author_email="mirmikns@yandex.ru",
     url="https://github.com/mirmik/zencad",
     long_description=open(os.path.join(
         directory, "README.md"), "r", encoding="utf8").read(),
```

### Comparing `zencad-1.3.2/zencad/__init__.py` & `zencad-1.3.3/zencad/__init__.py`

 * *Files identical despite different names*

### Comparing `zencad-1.3.2/zencad/__main__.py` & `zencad-1.3.3/zencad/__main__.py`

 * *Files identical despite different names*

### Comparing `zencad-1.3.2/zencad/animate.py` & `zencad-1.3.3/zencad/animate.py`

 * *Files identical despite different names*

### Comparing `zencad-1.3.2/zencad/bbox.py` & `zencad-1.3.3/zencad/bbox.py`

 * *Files identical despite different names*

### Comparing `zencad-1.3.2/zencad/color.py` & `zencad-1.3.3/zencad/color.py`

 * *Files identical despite different names*

### Comparing `zencad-1.3.2/zencad/convert/api.py` & `zencad-1.3.3/zencad/convert/api.py`

 * *Files identical despite different names*

### Comparing `zencad-1.3.2/zencad/convert/svg.py` & `zencad-1.3.3/zencad/convert/svg.py`

 * *Files identical despite different names*

### Comparing `zencad-1.3.2/zencad/convert/test.svg` & `zencad-1.3.3/zencad/convert/test.svg`

 * *Files identical despite different names*

### Comparing `zencad-1.3.2/zencad/examples/1.GeomPrim/1.prim3d/box.py` & `zencad-1.3.3/zencad/examples/1.GeomPrim/1.prim3d/box.py`

 * *Files identical despite different names*

### Comparing `zencad-1.3.2/zencad/examples/1.GeomPrim/1.prim3d/cone.py` & `zencad-1.3.3/zencad/examples/1.GeomPrim/1.prim3d/cone.py`

 * *Files identical despite different names*

### Comparing `zencad-1.3.2/zencad/examples/1.GeomPrim/1.prim3d/cylinder.py` & `zencad-1.3.3/zencad/examples/1.GeomPrim/1.prim3d/cylinder.py`

 * *Files identical despite different names*

### Comparing `zencad-1.3.2/zencad/examples/1.GeomPrim/1.prim3d/halfspace.py` & `zencad-1.3.3/zencad/examples/1.GeomPrim/1.prim3d/halfspace.py`

 * *Files identical despite different names*

### Comparing `zencad-1.3.2/zencad/examples/1.GeomPrim/1.prim3d/sphere.py` & `zencad-1.3.3/zencad/examples/1.GeomPrim/1.prim3d/sphere.py`

 * *Files identical despite different names*

### Comparing `zencad-1.3.2/zencad/examples/1.GeomPrim/2.prim2d/circle.py` & `zencad-1.3.3/zencad/examples/1.GeomPrim/2.prim2d/circle.py`

 * *Files identical despite different names*

### Comparing `zencad-1.3.2/zencad/examples/1.GeomPrim/2.prim2d/ellipse.py` & `zencad-1.3.3/zencad/examples/1.GeomPrim/2.prim2d/ellipse.py`

 * *Files identical despite different names*

### Comparing `zencad-1.3.2/zencad/examples/1.GeomPrim/2.prim2d/fillet_ngon.py` & `zencad-1.3.3/zencad/examples/1.GeomPrim/2.prim2d/fillet_ngon.py`

 * *Files identical despite different names*

### Comparing `zencad-1.3.2/zencad/examples/1.GeomPrim/2.prim2d/textshape.py` & `zencad-1.3.3/zencad/examples/1.GeomPrim/2.prim2d/textshape.py`

 * *Files identical despite different names*

### Comparing `zencad-1.3.2/zencad/examples/1.GeomPrim/3.prim1d/bspline.py` & `zencad-1.3.3/zencad/examples/1.GeomPrim/3.prim1d/bspline.py`

 * *Files identical despite different names*

### Comparing `zencad-1.3.2/zencad/examples/1.GeomPrim/3.prim1d/rounded_polysegment.py` & `zencad-1.3.3/zencad/examples/1.GeomPrim/3.prim1d/rounded_polysegment.py`

 * *Files identical despite different names*

### Comparing `zencad-1.3.2/zencad/examples/2.Operations/1.AphineTrans/rotate_array.py` & `zencad-1.3.3/zencad/examples/2.Operations/1.AphineTrans/rotate_array.py`

 * *Files identical despite different names*

### Comparing `zencad-1.3.2/zencad/examples/2.Operations/1.AphineTrans/short_rotate.py` & `zencad-1.3.3/zencad/examples/2.Operations/1.AphineTrans/short_rotate.py`

 * *Files identical despite different names*

### Comparing `zencad-1.3.2/zencad/examples/2.Operations/2.Operations/loft.py` & `zencad-1.3.3/zencad/examples/2.Operations/2.Operations/loft.py`

 * *Files identical despite different names*

### Comparing `zencad-1.3.2/zencad/examples/2.Operations/3.Sweep/pipe_shell.py` & `zencad-1.3.3/zencad/examples/2.Operations/3.Sweep/pipe_shell.py`

 * *Files identical despite different names*

### Comparing `zencad-1.3.2/zencad/examples/2.Operations/3.Sweep/revol.py` & `zencad-1.3.3/zencad/examples/2.Operations/3.Sweep/revol.py`

 * *Files identical despite different names*

### Comparing `zencad-1.3.2/zencad/examples/2.Operations/3.Sweep/revol2.py` & `zencad-1.3.3/zencad/examples/2.Operations/3.Sweep/revol2.py`

 * *Files identical despite different names*

### Comparing `zencad-1.3.2/zencad/examples/2.Operations/3.Sweep/tube.py` & `zencad-1.3.3/zencad/examples/2.Operations/3.Sweep/tube.py`

 * *Files identical despite different names*

### Comparing `zencad-1.3.2/zencad/examples/2.Operations/3.Sweep/tube_by_points.py` & `zencad-1.3.3/zencad/examples/2.Operations/3.Sweep/tube_by_points.py`

 * *Files identical despite different names*

### Comparing `zencad-1.3.2/zencad/examples/2.Operations/4.Mesh/triangulate.py` & `zencad-1.3.3/zencad/examples/2.Operations/4.Mesh/triangulate.py`

 * *Files identical despite different names*

### Comparing `zencad-1.3.2/zencad/examples/2.Operations/boolean.py` & `zencad-1.3.3/zencad/examples/2.Operations/boolean.py`

 * *Files identical despite different names*

### Comparing `zencad-1.3.2/zencad/examples/3.Animation/change_color.py` & `zencad-1.3.3/zencad/examples/3.Animation/change_color.py`

 * *Files identical despite different names*

### Comparing `zencad-1.3.2/zencad/examples/3.Animation/color.py` & `zencad-1.3.3/zencad/examples/3.Animation/color.py`

 * *Files identical despite different names*

### Comparing `zencad-1.3.2/zencad/examples/3.Animation/pacman.py` & `zencad-1.3.3/zencad/examples/3.Animation/pacman.py`

 * *Files identical despite different names*

### Comparing `zencad-1.3.2/zencad/examples/4.Assemble/EulerAngles.py` & `zencad-1.3.3/zencad/examples/4.Assemble/EulerAngles.py`

 * *Files identical despite different names*

### Comparing `zencad-1.3.2/zencad/examples/4.Assemble/manual-control-2.py` & `zencad-1.3.3/zencad/examples/4.Assemble/manual-control-2.py`

 * *Files identical despite different names*

### Comparing `zencad-1.3.2/zencad/examples/4.Assemble/manual-control.py` & `zencad-1.3.3/zencad/examples/4.Assemble/manual-control.py`

 * *Files identical despite different names*

### Comparing `zencad-1.3.2/zencad/examples/4.Assemble/robot.py` & `zencad-1.3.3/zencad/examples/4.Assemble/robot.py`

 * *Files identical despite different names*

### Comparing `zencad-1.3.2/zencad/examples/Integration/pillow/senku.png` & `zencad-1.3.3/zencad/examples/Integration/pillow/senku.png`

 * *Files identical despite different names*

### Comparing `zencad-1.3.2/zencad/examples/Integration/pillow/smile.png` & `zencad-1.3.3/zencad/examples/Integration/pillow/smile.png`

 * *Files identical despite different names*

### Comparing `zencad-1.3.2/zencad/examples/Integration/skimage-mechanicus/cube.py` & `zencad-1.3.3/zencad/examples/Integration/skimage-mechanicus/cube.py`

 * *Files identical despite different names*

### Comparing `zencad-1.3.2/zencad/examples/Integration/skimage-mechanicus/image.png` & `zencad-1.3.3/zencad/examples/Integration/skimage-mechanicus/image.png`

 * *Files identical despite different names*

### Comparing `zencad-1.3.2/zencad/examples/Integration/skimage-mechanicus/mech.py` & `zencad-1.3.3/zencad/examples/Integration/skimage-mechanicus/mech.py`

 * *Files identical despite different names*

### Comparing `zencad-1.3.2/zencad/examples/Integration/svg.py` & `zencad-1.3.3/zencad/examples/Integration/svg.py`

 * *Files identical despite different names*

### Comparing `zencad-1.3.2/zencad/examples/Integration/trimesh/bulbasaur.STL` & `zencad-1.3.3/zencad/examples/Integration/trimesh/bulbasaur.STL`

 * *Files identical despite different names*

### Comparing `zencad-1.3.2/zencad/examples/MiniGames/tennis.py` & `zencad-1.3.3/zencad/examples/MiniGames/tennis.py`

 * *Files identical despite different names*

### Comparing `zencad-1.3.2/zencad/examples/MiniGames/tetris.py` & `zencad-1.3.3/zencad/examples/MiniGames/tetris.py`

 * *Files identical despite different names*

### Comparing `zencad-1.3.2/zencad/examples/Models/bottle.py` & `zencad-1.3.3/zencad/examples/Models/bottle.py`

 * *Files identical despite different names*

### Comparing `zencad-1.3.2/zencad/examples/Models/cup.py` & `zencad-1.3.3/zencad/examples/Models/cup.py`

 * *Files identical despite different names*

### Comparing `zencad-1.3.2/zencad/examples/Models/logo.py` & `zencad-1.3.3/zencad/examples/Models/logo.py`

 * *Files identical despite different names*

### Comparing `zencad-1.3.2/zencad/examples/Models/nut.py` & `zencad-1.3.3/zencad/examples/Models/nut.py`

 * *Files identical despite different names*

### Comparing `zencad-1.3.2/zencad/examples/Models/organizer/case.py` & `zencad-1.3.3/zencad/examples/Models/organizer/case.py`

 * *Files identical despite different names*

### Comparing `zencad-1.3.2/zencad/examples/Models/organizer/organizer.py` & `zencad-1.3.3/zencad/examples/Models/organizer/organizer.py`

 * *Files identical despite different names*

### Comparing `zencad-1.3.2/zencad/examples/fonts/mandarinc.ttf` & `zencad-1.3.3/zencad/examples/fonts/mandarinc.ttf`

 * *Files identical despite different names*

### Comparing `zencad-1.3.2/zencad/examples/fonts/testfont.ttf` & `zencad-1.3.3/zencad/examples/fonts/testfont.ttf`

 * *Files identical despite different names*

### Comparing `zencad-1.3.2/zencad/geom/boolops.py` & `zencad-1.3.3/zencad/geom/boolops.py`

 * *Files identical despite different names*

### Comparing `zencad-1.3.2/zencad/geom/boolops_base.py` & `zencad-1.3.3/zencad/geom/boolops_base.py`

 * *Files identical despite different names*

### Comparing `zencad-1.3.2/zencad/geom/curve.py` & `zencad-1.3.3/zencad/geom/curve.py`

 * *Files identical despite different names*

### Comparing `zencad-1.3.2/zencad/geom/curve2.py` & `zencad-1.3.3/zencad/geom/curve2.py`

 * *Files identical despite different names*

### Comparing `zencad-1.3.2/zencad/geom/curve_algo.py` & `zencad-1.3.3/zencad/geom/curve_algo.py`

 * *Files identical despite different names*

### Comparing `zencad-1.3.2/zencad/geom/exttrans.py` & `zencad-1.3.3/zencad/geom/exttrans.py`

 * *Files identical despite different names*

### Comparing `zencad-1.3.2/zencad/geom/face.py` & `zencad-1.3.3/zencad/geom/face.py`

 * *Files identical despite different names*

### Comparing `zencad-1.3.2/zencad/geom/general_transformation.py` & `zencad-1.3.3/zencad/geom/general_transformation.py`

 * *Files identical despite different names*

### Comparing `zencad-1.3.2/zencad/geom/near.py` & `zencad-1.3.3/zencad/geom/near.py`

 * *Files identical despite different names*

### Comparing `zencad-1.3.2/zencad/geom/offset.py` & `zencad-1.3.3/zencad/geom/offset.py`

 * *Files identical despite different names*

### Comparing `zencad-1.3.2/zencad/geom/operations.py` & `zencad-1.3.3/zencad/geom/operations.py`

 * *Files identical despite different names*

### Comparing `zencad-1.3.2/zencad/geom/platonic.py` & `zencad-1.3.3/zencad/geom/platonic.py`

 * *Files identical despite different names*

### Comparing `zencad-1.3.2/zencad/geom/reflect_helpers.py` & `zencad-1.3.3/zencad/geom/reflect_helpers.py`

 * *Files identical despite different names*

### Comparing `zencad-1.3.2/zencad/geom/sew.py` & `zencad-1.3.3/zencad/geom/sew.py`

 * *Files identical despite different names*

### Comparing `zencad-1.3.2/zencad/geom/shape.py` & `zencad-1.3.3/zencad/geom/shape.py`

 * *Files identical despite different names*

### Comparing `zencad-1.3.2/zencad/geom/shell.py` & `zencad-1.3.3/zencad/geom/shell.py`

 * *Files identical despite different names*

### Comparing `zencad-1.3.2/zencad/geom/solid.py` & `zencad-1.3.3/zencad/geom/solid.py`

 * *Files identical despite different names*

### Comparing `zencad-1.3.2/zencad/geom/surface.py` & `zencad-1.3.3/zencad/geom/surface.py`

 * *Files identical despite different names*

### Comparing `zencad-1.3.2/zencad/geom/sweep.py` & `zencad-1.3.3/zencad/geom/sweep.py`

 * *Files identical despite different names*

### Comparing `zencad-1.3.2/zencad/geom/sweep_law.py` & `zencad-1.3.3/zencad/geom/sweep_law.py`

 * *Files identical despite different names*

### Comparing `zencad-1.3.2/zencad/geom/trans.py` & `zencad-1.3.3/zencad/geom/trans.py`

 * *Files identical despite different names*

### Comparing `zencad-1.3.2/zencad/geom/transformable.py` & `zencad-1.3.3/zencad/geom/transformable.py`

 * *Files identical despite different names*

### Comparing `zencad-1.3.2/zencad/geom/unify.py` & `zencad-1.3.3/zencad/geom/unify.py`

 * *Files identical despite different names*

### Comparing `zencad-1.3.2/zencad/geom/unify_ops.py` & `zencad-1.3.3/zencad/geom/unify_ops.py`

 * *Files identical despite different names*

### Comparing `zencad-1.3.2/zencad/geom/wire.py` & `zencad-1.3.3/zencad/geom/wire.py`

 * *Files identical despite different names*

### Comparing `zencad-1.3.2/zencad/geom/wire_builder.py` & `zencad-1.3.3/zencad/geom/wire_builder.py`

 * *Files identical despite different names*

### Comparing `zencad-1.3.2/zencad/geombase.py` & `zencad-1.3.3/zencad/geombase.py`

 * *Files identical despite different names*

### Comparing `zencad-1.3.2/zencad/geometry_core_installer.py` & `zencad-1.3.3/zencad/geometry_core_installer.py`

 * *Files identical despite different names*

### Comparing `zencad-1.3.2/zencad/gui/actions.py` & `zencad-1.3.3/zencad/gui/actions.py`

 * *Files identical despite different names*

### Comparing `zencad-1.3.2/zencad/gui/display.py` & `zencad-1.3.3/zencad/gui/display.py`

 * *Files identical despite different names*

### Comparing `zencad-1.3.2/zencad/gui/display_only.py` & `zencad-1.3.3/zencad/gui/display_only.py`

 * *Files identical despite different names*

### Comparing `zencad-1.3.2/zencad/gui/info_widget.py` & `zencad-1.3.3/zencad/gui/info_widget.py`

 * *Files identical despite different names*

### Comparing `zencad-1.3.2/zencad/gui/libinstaller.py` & `zencad-1.3.3/zencad/gui/libinstaller.py`

 * *Files identical despite different names*

### Comparing `zencad-1.3.2/zencad/gui/mainwindow.py` & `zencad-1.3.3/zencad/gui/mainwindow.py`

 * *Files identical despite different names*

### Comparing `zencad-1.3.2/zencad/gui/settingswdg.py` & `zencad-1.3.3/zencad/gui/settingswdg.py`

 * *Files identical despite different names*

### Comparing `zencad-1.3.2/zencad/gui/util.py` & `zencad-1.3.3/zencad/gui/util.py`

 * *Files identical despite different names*

### Comparing `zencad-1.3.2/zencad/gutil.py` & `zencad-1.3.3/zencad/gutil.py`

 * *Files identical despite different names*

### Comparing `zencad-1.3.2/zencad/industrial-robot.svg` & `zencad-1.3.3/zencad/industrial-robot.svg`

 * *Files identical despite different names*

### Comparing `zencad-1.3.2/zencad/interactive/__init__.py` & `zencad-1.3.3/zencad/interactive/__init__.py`

 * *Files identical despite different names*

### Comparing `zencad-1.3.2/zencad/interactive/assemble.py` & `zencad-1.3.3/zencad/interactive/assemble.py`

 * *Files identical despite different names*

### Comparing `zencad-1.3.2/zencad/interactive/interactive_object.py` & `zencad-1.3.3/zencad/interactive/interactive_object.py`

 * *Files identical despite different names*

### Comparing `zencad-1.3.2/zencad/interactive/line.py` & `zencad-1.3.3/zencad/interactive/line.py`

 * *Files identical despite different names*

### Comparing `zencad-1.3.2/zencad/interactive/point.py` & `zencad-1.3.3/zencad/interactive/point.py`

 * *Files identical despite different names*

### Comparing `zencad-1.3.2/zencad/interactive/shape.py` & `zencad-1.3.3/zencad/interactive/shape.py`

 * *Files identical despite different names*

### Comparing `zencad-1.3.2/zencad/internal_models/knight.py` & `zencad-1.3.3/zencad/internal_models/knight.py`

 * *Files identical despite different names*

### Comparing `zencad-1.3.2/zencad/lazifier.py` & `zencad-1.3.3/zencad/lazifier.py`

 * *Files identical despite different names*

### Comparing `zencad-1.3.2/zencad/libs/kinematic.py` & `zencad-1.3.3/zencad/libs/kinematic.py`

 * *Files identical despite different names*

### Comparing `zencad-1.3.2/zencad/libs/malgo.py` & `zencad-1.3.3/zencad/libs/malgo.py`

 * *Files identical despite different names*

### Comparing `zencad-1.3.2/zencad/libs/screw.py` & `zencad-1.3.3/zencad/libs/screw.py`

 * *Files identical despite different names*

### Comparing `zencad-1.3.2/zencad/opencascade_types.py` & `zencad-1.3.3/zencad/opencascade_types.py`

 * *Files identical despite different names*

### Comparing `zencad-1.3.2/zencad/scene.py` & `zencad-1.3.3/zencad/scene.py`

 * *Files identical despite different names*

### Comparing `zencad-1.3.2/zencad/settings.py` & `zencad-1.3.3/zencad/settings.py`

 * *Files identical despite different names*

### Comparing `zencad-1.3.2/zencad/showapi.py` & `zencad-1.3.3/zencad/showapi.py`

 * *Files identical despite different names*

### Comparing `zencad-1.3.2/zencad/techpriest.jpg` & `zencad-1.3.3/zencad/techpriest.jpg`

 * *Files identical despite different names*

### Comparing `zencad-1.3.2/zencad/util.py` & `zencad-1.3.3/zencad/util.py`

 * *Files identical despite different names*

### Comparing `zencad-1.3.2/zencad/zencad_logo.png` & `zencad-1.3.3/zencad/zencad_logo.png`

 * *Files identical despite different names*

### Comparing `zencad-1.3.2/zencad.egg-info/PKG-INFO` & `zencad-1.3.3/zencad.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: zencad
-Version: 1.3.2
+Version: 1.3.3
 Summary: CAD system for righteous zen programmers 
 Home-page: https://github.com/mirmik/zencad
 Author: mirmik
 Author-email: mirmikns@yandex.ru
 License: MIT
 Keywords: testing,cad
 Platform: UNKNOWN
-Requires-Python: >3.8.0
+Requires-Python: >3.6.0
 Description-Content-Type: text/markdown
 Provides-Extra: gui
 License-File: LICENSE.txt
 
 ZenCad
 ======
 CAD system for righteous zen programmers
```

### Comparing `zencad-1.3.2/zencad.egg-info/SOURCES.txt` & `zencad-1.3.3/zencad.egg-info/SOURCES.txt`

 * *Files identical despite different names*

