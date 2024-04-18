# Comparing `tmp/autoeft-1.0.0rc0.tar.gz` & `tmp/autoeft-1.0.1.tar.gz`

## Comparing `autoeft-1.0.0rc0.tar` & `autoeft-1.0.1.tar`

### file list

```diff
@@ -1,257 +1,353 @@
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/COPYRIGHT
--rw-r--r--   0        0        0     6571 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/README.md
--rw-r--r--   0        0        0     3858 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/__init__.py
--rw-r--r--   0        0        0     8176 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/cli.py
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/exceptions.py
--rw-r--r--   0        0        0     8033 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/base/__init__.py
--rw-r--r--   0        0        0    15553 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/base/basis.py
--rw-r--r--   0        0        0     7488 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/base/classifications.py
--rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/base/groups.py
--rw-r--r--   0        0        0    14084 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/base/model.py
--rw-r--r--   0        0        0     3816 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/base/representations.py
--rw-r--r--   0        0        0    31986 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/base/tensors.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/__init__.py
--rw-r--r--   0        0        0    14113 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/generators.py
--rw-r--r--   0        0        0     6545 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/symmetric_group.py
--rw-r--r--   0        0        0     6687 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/young.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/__init__.py
--rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_2/P_1_1_cycle.npz
--rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_2/P_1_1_reflection.npz
--rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_2/P_2_cycle.npz
--rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_2/P_2_reflection.npz
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_2/__init__.py
--rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_3/P_1_1_1_cycle.npz
--rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_3/P_1_1_1_reflection.npz
--rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_3/P_2_1_cycle.npz
--rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_3/P_2_1_reflection.npz
--rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_3/P_3_cycle.npz
--rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_3/P_3_reflection.npz
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_3/__init__.py
--rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_4/P_1_1_1_1_cycle.npz
--rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_4/P_1_1_1_1_reflection.npz
--rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_4/P_2_1_1_cycle.npz
--rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_4/P_2_1_1_reflection.npz
--rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_4/P_2_2_cycle.npz
--rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_4/P_2_2_reflection.npz
--rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_4/P_3_1_cycle.npz
--rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_4/P_3_1_reflection.npz
--rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_4/P_4_cycle.npz
--rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_4/P_4_reflection.npz
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_4/__init__.py
--rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_5/P_1_1_1_1_1_cycle.npz
--rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_5/P_1_1_1_1_1_reflection.npz
--rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_5/P_2_1_1_1_cycle.npz
--rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_5/P_2_1_1_1_reflection.npz
--rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_5/P_2_2_1_cycle.npz
--rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_5/P_2_2_1_reflection.npz
--rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_5/P_3_1_1_cycle.npz
--rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_5/P_3_1_1_reflection.npz
--rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_5/P_3_2_cycle.npz
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_5/P_3_2_reflection.npz
--rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_5/P_4_1_cycle.npz
--rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_5/P_4_1_reflection.npz
--rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_5/P_5_cycle.npz
--rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_5/P_5_reflection.npz
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_5/__init__.py
--rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_6/P_1_1_1_1_1_1_cycle.npz
--rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_6/P_1_1_1_1_1_1_reflection.npz
--rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_6/P_2_1_1_1_1_cycle.npz
--rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_6/P_2_1_1_1_1_reflection.npz
--rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_6/P_2_2_1_1_cycle.npz
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_6/P_2_2_1_1_reflection.npz
--rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_6/P_2_2_2_cycle.npz
--rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_6/P_2_2_2_reflection.npz
--rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_6/P_3_1_1_1_cycle.npz
--rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_6/P_3_1_1_1_reflection.npz
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_6/P_3_2_1_cycle.npz
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_6/P_3_2_1_reflection.npz
--rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_6/P_3_3_cycle.npz
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_6/P_3_3_reflection.npz
--rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_6/P_4_1_1_cycle.npz
--rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_6/P_4_1_1_reflection.npz
--rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_6/P_4_2_cycle.npz
--rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_6/P_4_2_reflection.npz
--rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_6/P_5_1_cycle.npz
--rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_6/P_5_1_reflection.npz
--rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_6/P_6_cycle.npz
--rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_6/P_6_reflection.npz
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_6/__init__.py
--rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_7/P_1_1_1_1_1_1_1_cycle.npz
--rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_7/P_1_1_1_1_1_1_1_reflection.npz
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_7/P_2_1_1_1_1_1_cycle.npz
--rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_7/P_2_1_1_1_1_1_reflection.npz
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_7/P_2_2_1_1_1_cycle.npz
--rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_7/P_2_2_1_1_1_reflection.npz
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_7/P_2_2_2_1_cycle.npz
--rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_7/P_2_2_2_1_reflection.npz
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_7/P_3_1_1_1_1_cycle.npz
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_7/P_3_1_1_1_1_reflection.npz
--rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_7/P_3_2_1_1_cycle.npz
--rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_7/P_3_2_1_1_reflection.npz
--rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_7/P_3_2_2_cycle.npz
--rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_7/P_3_2_2_reflection.npz
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_7/P_3_3_1_cycle.npz
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_7/P_3_3_1_reflection.npz
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_7/P_4_1_1_1_cycle.npz
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_7/P_4_1_1_1_reflection.npz
--rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_7/P_4_2_1_cycle.npz
--rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_7/P_4_2_1_reflection.npz
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_7/P_4_3_cycle.npz
--rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_7/P_4_3_reflection.npz
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_7/P_5_1_1_cycle.npz
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_7/P_5_1_1_reflection.npz
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_7/P_5_2_cycle.npz
--rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_7/P_5_2_reflection.npz
--rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_7/P_6_1_cycle.npz
--rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_7/P_6_1_reflection.npz
--rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_7/P_7_cycle.npz
--rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_7/P_7_reflection.npz
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_7/__init__.py
--rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_8/P_1_1_1_1_1_1_1_1_cycle.npz
--rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_8/P_1_1_1_1_1_1_1_1_reflection.npz
--rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_8/P_2_1_1_1_1_1_1_cycle.npz
--rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_8/P_2_1_1_1_1_1_1_reflection.npz
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_8/P_2_2_1_1_1_1_cycle.npz
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_8/P_2_2_1_1_1_1_reflection.npz
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_8/P_2_2_2_1_1_cycle.npz
--rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_8/P_2_2_2_1_1_reflection.npz
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_8/P_2_2_2_2_cycle.npz
--rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_8/P_2_2_2_2_reflection.npz
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_8/P_3_1_1_1_1_1_cycle.npz
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_8/P_3_1_1_1_1_1_reflection.npz
--rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_8/P_3_2_1_1_1_cycle.npz
--rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_8/P_3_2_1_1_1_reflection.npz
--rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_8/P_3_2_2_1_cycle.npz
--rw-r--r--   0        0        0     1447 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_8/P_3_2_2_1_reflection.npz
--rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_8/P_3_3_1_1_cycle.npz
--rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_8/P_3_3_1_1_reflection.npz
--rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_8/P_3_3_2_cycle.npz
--rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_8/P_3_3_2_reflection.npz
--rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_8/P_4_1_1_1_1_cycle.npz
--rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_8/P_4_1_1_1_1_reflection.npz
--rw-r--r--   0        0        0     1846 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_8/P_4_2_1_1_cycle.npz
--rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_8/P_4_2_1_1_reflection.npz
--rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_8/P_4_2_2_cycle.npz
--rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_8/P_4_2_2_reflection.npz
--rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_8/P_4_3_1_cycle.npz
--rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_8/P_4_3_1_reflection.npz
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_8/P_4_4_cycle.npz
--rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_8/P_4_4_reflection.npz
--rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_8/P_5_1_1_1_cycle.npz
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_8/P_5_1_1_1_reflection.npz
--rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_8/P_5_2_1_cycle.npz
--rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_8/P_5_2_1_reflection.npz
--rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_8/P_5_3_cycle.npz
--rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_8/P_5_3_reflection.npz
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_8/P_6_1_1_cycle.npz
--rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_8/P_6_1_1_reflection.npz
--rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_8/P_6_2_cycle.npz
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_8/P_6_2_reflection.npz
--rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_8/P_7_1_cycle.npz
--rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_8/P_7_1_reflection.npz
--rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_8/P_8_cycle.npz
--rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_8/P_8_reflection.npz
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_8/__init__.py
--rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/P_1_1_1_1_1_1_1_1_1_cycle.npz
--rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/P_1_1_1_1_1_1_1_1_1_reflection.npz
--rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/P_2_1_1_1_1_1_1_1_cycle.npz
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/P_2_1_1_1_1_1_1_1_reflection.npz
--rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/P_2_2_1_1_1_1_1_cycle.npz
--rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/P_2_2_1_1_1_1_1_reflection.npz
--rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/P_2_2_2_1_1_1_cycle.npz
--rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/P_2_2_2_1_1_1_reflection.npz
--rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/P_2_2_2_2_1_cycle.npz
--rw-r--r--   0        0        0     1225 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/P_2_2_2_2_1_reflection.npz
--rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/P_3_1_1_1_1_1_1_cycle.npz
--rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/P_3_1_1_1_1_1_1_reflection.npz
--rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/P_3_2_1_1_1_1_cycle.npz
--rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/P_3_2_1_1_1_1_reflection.npz
--rw-r--r--   0        0        0     3214 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/P_3_2_2_1_1_cycle.npz
--rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/P_3_2_2_1_1_reflection.npz
--rw-r--r--   0        0        0     2021 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/P_3_2_2_2_cycle.npz
--rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/P_3_2_2_2_reflection.npz
--rw-r--r--   0        0        0     2441 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/P_3_3_1_1_1_cycle.npz
--rw-r--r--   0        0        0     1896 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/P_3_3_1_1_1_reflection.npz
--rw-r--r--   0        0        0     3912 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/P_3_3_2_1_cycle.npz
--rw-r--r--   0        0        0     2334 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/P_3_3_2_1_reflection.npz
--rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/P_3_3_3_cycle.npz
--rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/P_3_3_3_reflection.npz
--rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/P_4_1_1_1_1_1_cycle.npz
--rw-r--r--   0        0        0     1351 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/P_4_1_1_1_1_1_reflection.npz
--rw-r--r--   0        0        0     2945 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/P_4_2_1_1_1_cycle.npz
--rw-r--r--   0        0        0     2465 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/P_4_2_1_1_1_reflection.npz
--rw-r--r--   0        0        0     3912 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/P_4_2_2_1_cycle.npz
--rw-r--r--   0        0        0     2647 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/P_4_2_2_1_reflection.npz
--rw-r--r--   0        0        0     4031 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/P_4_3_1_1_cycle.npz
--rw-r--r--   0        0        0     2719 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/P_4_3_1_1_reflection.npz
--rw-r--r--   0        0        0     3649 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/P_4_3_2_cycle.npz
--rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/P_4_3_2_reflection.npz
--rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/P_4_4_1_cycle.npz
--rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/P_4_4_1_reflection.npz
--rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/P_5_1_1_1_1_cycle.npz
--rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/P_5_1_1_1_1_reflection.npz
--rw-r--r--   0        0        0     2907 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/P_5_2_1_1_cycle.npz
--rw-r--r--   0        0        0     2418 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/P_5_2_1_1_reflection.npz
--rw-r--r--   0        0        0     2188 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/P_5_2_2_cycle.npz
--rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/P_5_2_2_reflection.npz
--rw-r--r--   0        0        0     2970 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/P_5_3_1_cycle.npz
--rw-r--r--   0        0        0     2096 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/P_5_3_1_reflection.npz
--rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/P_5_4_cycle.npz
--rw-r--r--   0        0        0     1209 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/P_5_4_reflection.npz
--rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/P_6_1_1_1_cycle.npz
--rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/P_6_1_1_1_reflection.npz
--rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/P_6_2_1_cycle.npz
--rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/P_6_2_1_reflection.npz
--rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/P_6_3_cycle.npz
--rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/P_6_3_reflection.npz
--rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/P_7_1_1_cycle.npz
--rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/P_7_1_1_reflection.npz
--rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/P_7_2_cycle.npz
--rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/P_7_2_reflection.npz
--rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/P_8_1_cycle.npz
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/P_8_1_reflection.npz
--rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/P_9_cycle.npz
--rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/P_9_reflection.npz
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/construction/__init__.py
--rw-r--r--   0        0        0     9427 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/construction/invariants.py
--rw-r--r--   0        0        0    31847 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/construction/main.py
--rw-r--r--   0        0        0     6519 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/construction/permutation_symmetries.py
--rw-r--r--   0        0        0     4604 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/construction/symmetrizers.py
--rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/form/__init__.py
--rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/form/contract.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/io/__init__.py
--rw-r--r--   0        0        0     4892 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/io/basis.py
--rw-r--r--   0        0        0     4899 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/io/count.py
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/tex/__init__.py
--rw-r--r--   0        0        0     7110 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/autoeft/tex/main.py
--rw-r--r--   0        0        0     1287 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/models/README.md
--rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/models/all-left_sm.yml
--rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/models/bno_nf1_sm.yml
--rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/models/bno_sm.yml
--rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/models/dynkin_sm.yml
--rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/models/grsm.yml
--rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/models/mfv-sm.yml
--rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/models/nf1_sm.yml
--rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/models/sm.yml
--rw-r--r--   0        0        0     2878 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/models/bsm/README.md
--rw-r--r--   0        0        0     1424 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/models/bsm/cqs+sm.yml
--rw-r--r--   0        0        0     1421 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/models/bsm/cts+sm.yml
--rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/models/bsm/dcs+sm.yml
--rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/models/bsm/lqc1+sm.yml
--rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/models/bsm/lqc2+sm.yml
--rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/models/bsm/lqp1+sm.yml
--rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/models/bsm/lqp2+sm.yml
--rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/models/bsm/ltf+sm.yml
--rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/models/bsm/scs+sm.yml
--rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/models/bsm/u1-u1-sm.yml
--rw-r--r--   0        0        0     1970 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/models/bsm/vll+sm.yml
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/resources/LOGO
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/resources/theme.ini
--rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/resources/tex/main.tex
--rw-r--r--   0        0        0     3071 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/.gitignore
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/LICENSE
--rw-r--r--   0        0        0     5520 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/PyPI_README.md
--rw-r--r--   0        0        0     3885 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/pyproject.toml
--rw-r--r--   0        0        0     6819 2020-02-02 00:00:00.000000 autoeft-1.0.0rc0/PKG-INFO
+-rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 autoeft-1.0.1/CHANGELOG.md
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 autoeft-1.0.1/COPYRIGHT
+-rw-r--r--   0        0        0     6670 2020-02-02 00:00:00.000000 autoeft-1.0.1/README.md
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 autoeft-1.0.1/pr.yml
+-rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/__init__.py
+-rw-r--r--   0        0        0     8936 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/cli.py
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/exceptions.py
+-rw-r--r--   0        0        0     8033 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/base/__init__.py
+-rw-r--r--   0        0        0    15855 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/base/basis.py
+-rw-r--r--   0        0        0     7952 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/base/classifications.py
+-rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/base/groups.py
+-rw-r--r--   0        0        0    14309 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/base/model.py
+-rw-r--r--   0        0        0     4184 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/base/representations.py
+-rw-r--r--   0        0        0    31972 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/base/tensors.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/__init__.py
+-rw-r--r--   0        0        0    14113 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/generators.py
+-rw-r--r--   0        0        0     6545 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/symmetric_group.py
+-rw-r--r--   0        0        0     6687 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/young.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/__init__.py
+-rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_2/P_1_1_cycle.npz
+-rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_2/P_1_1_reflection.npz
+-rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_2/P_2_cycle.npz
+-rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_2/P_2_reflection.npz
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_2/__init__.py
+-rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_3/P_1_1_1_cycle.npz
+-rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_3/P_1_1_1_reflection.npz
+-rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_3/P_2_1_cycle.npz
+-rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_3/P_2_1_reflection.npz
+-rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_3/P_3_cycle.npz
+-rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_3/P_3_reflection.npz
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_3/__init__.py
+-rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_4/P_1_1_1_1_cycle.npz
+-rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_4/P_1_1_1_1_reflection.npz
+-rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_4/P_2_1_1_cycle.npz
+-rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_4/P_2_1_1_reflection.npz
+-rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_4/P_2_2_cycle.npz
+-rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_4/P_2_2_reflection.npz
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_4/P_3_1_cycle.npz
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_4/P_3_1_reflection.npz
+-rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_4/P_4_cycle.npz
+-rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_4/P_4_reflection.npz
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_4/__init__.py
+-rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_5/P_1_1_1_1_1_cycle.npz
+-rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_5/P_1_1_1_1_1_reflection.npz
+-rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_5/P_2_1_1_1_cycle.npz
+-rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_5/P_2_1_1_1_reflection.npz
+-rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_5/P_2_2_1_cycle.npz
+-rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_5/P_2_2_1_reflection.npz
+-rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_5/P_3_1_1_cycle.npz
+-rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_5/P_3_1_1_reflection.npz
+-rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_5/P_3_2_cycle.npz
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_5/P_3_2_reflection.npz
+-rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_5/P_4_1_cycle.npz
+-rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_5/P_4_1_reflection.npz
+-rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_5/P_5_cycle.npz
+-rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_5/P_5_reflection.npz
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_5/__init__.py
+-rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_6/P_1_1_1_1_1_1_cycle.npz
+-rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_6/P_1_1_1_1_1_1_reflection.npz
+-rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_6/P_2_1_1_1_1_cycle.npz
+-rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_6/P_2_1_1_1_1_reflection.npz
+-rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_6/P_2_2_1_1_cycle.npz
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_6/P_2_2_1_1_reflection.npz
+-rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_6/P_2_2_2_cycle.npz
+-rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_6/P_2_2_2_reflection.npz
+-rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_6/P_3_1_1_1_cycle.npz
+-rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_6/P_3_1_1_1_reflection.npz
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_6/P_3_2_1_cycle.npz
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_6/P_3_2_1_reflection.npz
+-rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_6/P_3_3_cycle.npz
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_6/P_3_3_reflection.npz
+-rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_6/P_4_1_1_cycle.npz
+-rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_6/P_4_1_1_reflection.npz
+-rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_6/P_4_2_cycle.npz
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_6/P_4_2_reflection.npz
+-rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_6/P_5_1_cycle.npz
+-rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_6/P_5_1_reflection.npz
+-rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_6/P_6_cycle.npz
+-rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_6/P_6_reflection.npz
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_6/__init__.py
+-rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_7/P_1_1_1_1_1_1_1_cycle.npz
+-rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_7/P_1_1_1_1_1_1_1_reflection.npz
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_7/P_2_1_1_1_1_1_cycle.npz
+-rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_7/P_2_1_1_1_1_1_reflection.npz
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_7/P_2_2_1_1_1_cycle.npz
+-rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_7/P_2_2_1_1_1_reflection.npz
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_7/P_2_2_2_1_cycle.npz
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_7/P_2_2_2_1_reflection.npz
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_7/P_3_1_1_1_1_cycle.npz
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_7/P_3_1_1_1_1_reflection.npz
+-rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_7/P_3_2_1_1_cycle.npz
+-rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_7/P_3_2_1_1_reflection.npz
+-rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_7/P_3_2_2_cycle.npz
+-rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_7/P_3_2_2_reflection.npz
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_7/P_3_3_1_cycle.npz
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_7/P_3_3_1_reflection.npz
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_7/P_4_1_1_1_cycle.npz
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_7/P_4_1_1_1_reflection.npz
+-rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_7/P_4_2_1_cycle.npz
+-rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_7/P_4_2_1_reflection.npz
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_7/P_4_3_cycle.npz
+-rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_7/P_4_3_reflection.npz
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_7/P_5_1_1_cycle.npz
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_7/P_5_1_1_reflection.npz
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_7/P_5_2_cycle.npz
+-rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_7/P_5_2_reflection.npz
+-rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_7/P_6_1_cycle.npz
+-rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_7/P_6_1_reflection.npz
+-rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_7/P_7_cycle.npz
+-rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_7/P_7_reflection.npz
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_7/__init__.py
+-rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_8/P_1_1_1_1_1_1_1_1_cycle.npz
+-rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_8/P_1_1_1_1_1_1_1_1_reflection.npz
+-rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_8/P_2_1_1_1_1_1_1_cycle.npz
+-rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_8/P_2_1_1_1_1_1_1_reflection.npz
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_8/P_2_2_1_1_1_1_cycle.npz
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_8/P_2_2_1_1_1_1_reflection.npz
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_8/P_2_2_2_1_1_cycle.npz
+-rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_8/P_2_2_2_1_1_reflection.npz
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_8/P_2_2_2_2_cycle.npz
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_8/P_2_2_2_2_reflection.npz
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_8/P_3_1_1_1_1_1_cycle.npz
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_8/P_3_1_1_1_1_1_reflection.npz
+-rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_8/P_3_2_1_1_1_cycle.npz
+-rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_8/P_3_2_1_1_1_reflection.npz
+-rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_8/P_3_2_2_1_cycle.npz
+-rw-r--r--   0        0        0     1447 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_8/P_3_2_2_1_reflection.npz
+-rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_8/P_3_3_1_1_cycle.npz
+-rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_8/P_3_3_1_1_reflection.npz
+-rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_8/P_3_3_2_cycle.npz
+-rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_8/P_3_3_2_reflection.npz
+-rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_8/P_4_1_1_1_1_cycle.npz
+-rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_8/P_4_1_1_1_1_reflection.npz
+-rw-r--r--   0        0        0     1846 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_8/P_4_2_1_1_cycle.npz
+-rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_8/P_4_2_1_1_reflection.npz
+-rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_8/P_4_2_2_cycle.npz
+-rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_8/P_4_2_2_reflection.npz
+-rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_8/P_4_3_1_cycle.npz
+-rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_8/P_4_3_1_reflection.npz
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_8/P_4_4_cycle.npz
+-rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_8/P_4_4_reflection.npz
+-rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_8/P_5_1_1_1_cycle.npz
+-rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_8/P_5_1_1_1_reflection.npz
+-rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_8/P_5_2_1_cycle.npz
+-rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_8/P_5_2_1_reflection.npz
+-rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_8/P_5_3_cycle.npz
+-rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_8/P_5_3_reflection.npz
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_8/P_6_1_1_cycle.npz
+-rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_8/P_6_1_1_reflection.npz
+-rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_8/P_6_2_cycle.npz
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_8/P_6_2_reflection.npz
+-rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_8/P_7_1_cycle.npz
+-rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_8/P_7_1_reflection.npz
+-rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_8/P_8_cycle.npz
+-rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_8/P_8_reflection.npz
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_8/__init__.py
+-rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_9/P_1_1_1_1_1_1_1_1_1_cycle.npz
+-rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_9/P_1_1_1_1_1_1_1_1_1_reflection.npz
+-rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_9/P_2_1_1_1_1_1_1_1_cycle.npz
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_9/P_2_1_1_1_1_1_1_1_reflection.npz
+-rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_9/P_2_2_1_1_1_1_1_cycle.npz
+-rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_9/P_2_2_1_1_1_1_1_reflection.npz
+-rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_9/P_2_2_2_1_1_1_cycle.npz
+-rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_9/P_2_2_2_1_1_1_reflection.npz
+-rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_9/P_2_2_2_2_1_cycle.npz
+-rw-r--r--   0        0        0     1225 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_9/P_2_2_2_2_1_reflection.npz
+-rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_9/P_3_1_1_1_1_1_1_cycle.npz
+-rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_9/P_3_1_1_1_1_1_1_reflection.npz
+-rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_9/P_3_2_1_1_1_1_cycle.npz
+-rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_9/P_3_2_1_1_1_1_reflection.npz
+-rw-r--r--   0        0        0     3214 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_9/P_3_2_2_1_1_cycle.npz
+-rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_9/P_3_2_2_1_1_reflection.npz
+-rw-r--r--   0        0        0     2021 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_9/P_3_2_2_2_cycle.npz
+-rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_9/P_3_2_2_2_reflection.npz
+-rw-r--r--   0        0        0     2441 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_9/P_3_3_1_1_1_cycle.npz
+-rw-r--r--   0        0        0     1896 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_9/P_3_3_1_1_1_reflection.npz
+-rw-r--r--   0        0        0     3912 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_9/P_3_3_2_1_cycle.npz
+-rw-r--r--   0        0        0     2334 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_9/P_3_3_2_1_reflection.npz
+-rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_9/P_3_3_3_cycle.npz
+-rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_9/P_3_3_3_reflection.npz
+-rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_9/P_4_1_1_1_1_1_cycle.npz
+-rw-r--r--   0        0        0     1351 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_9/P_4_1_1_1_1_1_reflection.npz
+-rw-r--r--   0        0        0     2945 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_9/P_4_2_1_1_1_cycle.npz
+-rw-r--r--   0        0        0     2465 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_9/P_4_2_1_1_1_reflection.npz
+-rw-r--r--   0        0        0     3912 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_9/P_4_2_2_1_cycle.npz
+-rw-r--r--   0        0        0     2647 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_9/P_4_2_2_1_reflection.npz
+-rw-r--r--   0        0        0     4031 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_9/P_4_3_1_1_cycle.npz
+-rw-r--r--   0        0        0     2719 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_9/P_4_3_1_1_reflection.npz
+-rw-r--r--   0        0        0     3649 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_9/P_4_3_2_cycle.npz
+-rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_9/P_4_3_2_reflection.npz
+-rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_9/P_4_4_1_cycle.npz
+-rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_9/P_4_4_1_reflection.npz
+-rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_9/P_5_1_1_1_1_cycle.npz
+-rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_9/P_5_1_1_1_1_reflection.npz
+-rw-r--r--   0        0        0     2907 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_9/P_5_2_1_1_cycle.npz
+-rw-r--r--   0        0        0     2418 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_9/P_5_2_1_1_reflection.npz
+-rw-r--r--   0        0        0     2188 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_9/P_5_2_2_cycle.npz
+-rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_9/P_5_2_2_reflection.npz
+-rw-r--r--   0        0        0     2970 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_9/P_5_3_1_cycle.npz
+-rw-r--r--   0        0        0     2096 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_9/P_5_3_1_reflection.npz
+-rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_9/P_5_4_cycle.npz
+-rw-r--r--   0        0        0     1209 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_9/P_5_4_reflection.npz
+-rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_9/P_6_1_1_1_cycle.npz
+-rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_9/P_6_1_1_1_reflection.npz
+-rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_9/P_6_2_1_cycle.npz
+-rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_9/P_6_2_1_reflection.npz
+-rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_9/P_6_3_cycle.npz
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_9/P_6_3_reflection.npz
+-rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_9/P_7_1_1_cycle.npz
+-rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_9/P_7_1_1_reflection.npz
+-rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_9/P_7_2_cycle.npz
+-rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_9/P_7_2_reflection.npz
+-rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_9/P_8_1_cycle.npz
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_9/P_8_1_reflection.npz
+-rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_9/P_9_cycle.npz
+-rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_9/P_9_reflection.npz
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/combinatorics/gens/S_9/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/construction/__init__.py
+-rw-r--r--   0        0        0     9873 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/construction/invariants.py
+-rw-r--r--   0        0        0    36599 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/construction/main.py
+-rw-r--r--   0        0        0     6519 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/construction/permutation_symmetries.py
+-rw-r--r--   0        0        0     4604 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/construction/symmetrizers.py
+-rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/form/__init__.py
+-rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/form/contract.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/io/__init__.py
+-rw-r--r--   0        0        0     5082 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/io/basis.py
+-rw-r--r--   0        0        0     4776 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/io/check.py
+-rw-r--r--   0        0        0     6413 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/io/count.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/io/check_basis-1_0_1/__init__.py
+-rw-r--r--   0        0        0    10113 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/io/check_basis-1_0_1/model.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/io/check_basis-1_0_1/3/__init__.py
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/io/check_basis-1_0_1/3/3FL/3GL.yml
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/io/check_basis-1_0_1/3/3FL/3WL.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/io/check_basis-1_0_1/3/3FL/__init__.py
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/io/check_basis-1_0_1/3/3FR/3GL+.yml
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/io/check_basis-1_0_1/3/3FR/3WL+.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/io/check_basis-1_0_1/3/3FR/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/io/check_basis-1_0_1/4/__init__.py
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/io/check_basis-1_0_1/4/1FL_2psiL_1phi/1BL_1LL_1eR+_1H+.yml
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/io/check_basis-1_0_1/4/1FL_2psiL_1phi/1BL_1QL_1dR+_1H+.yml
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/io/check_basis-1_0_1/4/1FL_2psiL_1phi/1BL_1QL_1uR+_1H.yml
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/io/check_basis-1_0_1/4/1FL_2psiL_1phi/1GL_1QL_1dR+_1H+.yml
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/io/check_basis-1_0_1/4/1FL_2psiL_1phi/1GL_1QL_1uR+_1H.yml
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/io/check_basis-1_0_1/4/1FL_2psiL_1phi/1WL_1LL_1eR+_1H+.yml
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/io/check_basis-1_0_1/4/1FL_2psiL_1phi/1WL_1QL_1dR+_1H+.yml
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/io/check_basis-1_0_1/4/1FL_2psiL_1phi/1WL_1QL_1uR+_1H.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/io/check_basis-1_0_1/4/1FL_2psiL_1phi/__init__.py
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/io/check_basis-1_0_1/4/1phi_2psiR_1FR/1H+_1QL+_1uR_1BL+.yml
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/io/check_basis-1_0_1/4/1phi_2psiR_1FR/1H+_1QL+_1uR_1GL+.yml
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/io/check_basis-1_0_1/4/1phi_2psiR_1FR/1H+_1QL+_1uR_1WL+.yml
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/io/check_basis-1_0_1/4/1phi_2psiR_1FR/1H_1LL+_1eR_1BL+.yml
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/io/check_basis-1_0_1/4/1phi_2psiR_1FR/1H_1LL+_1eR_1WL+.yml
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/io/check_basis-1_0_1/4/1phi_2psiR_1FR/1H_1QL+_1dR_1BL+.yml
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/io/check_basis-1_0_1/4/1phi_2psiR_1FR/1H_1QL+_1dR_1GL+.yml
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/io/check_basis-1_0_1/4/1phi_2psiR_1FR/1H_1QL+_1dR_1WL+.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/io/check_basis-1_0_1/4/1phi_2psiR_1FR/__init__.py
+-rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/io/check_basis-1_0_1/4/1psiL_2phi_1psiR_1D/1LL_1H_1H+_1LL+_1D.yml
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/io/check_basis-1_0_1/4/1psiL_2phi_1psiR_1D/1QL_1H_1H+_1QL+_1D.yml
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/io/check_basis-1_0_1/4/1psiL_2phi_1psiR_1D/1dR+_1H_1H+_1dR_1D.yml
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/io/check_basis-1_0_1/4/1psiL_2phi_1psiR_1D/1dR+_2H+_1uR_1D.yml
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/io/check_basis-1_0_1/4/1psiL_2phi_1psiR_1D/1eR+_1H_1H+_1eR_1D.yml
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/io/check_basis-1_0_1/4/1psiL_2phi_1psiR_1D/1uR+_1H_1H+_1uR_1D.yml
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/io/check_basis-1_0_1/4/1psiL_2phi_1psiR_1D/1uR+_2H_1dR_1D.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/io/check_basis-1_0_1/4/1psiL_2phi_1psiR_1D/__init__.py
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/io/check_basis-1_0_1/4/2FL_2phi/1BL_1WL_1H_1H+.yml
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/io/check_basis-1_0_1/4/2FL_2phi/2BL_1H_1H+.yml
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/io/check_basis-1_0_1/4/2FL_2phi/2GL_1H_1H+.yml
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/io/check_basis-1_0_1/4/2FL_2phi/2WL_1H_1H+.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/io/check_basis-1_0_1/4/2FL_2phi/__init__.py
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/io/check_basis-1_0_1/4/2phi_2FR/1H_1H+_1BL+_1WL+.yml
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/io/check_basis-1_0_1/4/2phi_2FR/1H_1H+_2BL+.yml
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/io/check_basis-1_0_1/4/2phi_2FR/1H_1H+_2GL+.yml
+-rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/io/check_basis-1_0_1/4/2phi_2FR/1H_1H+_2WL+.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/io/check_basis-1_0_1/4/2phi_2FR/__init__.py
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/io/check_basis-1_0_1/4/2psiL_2psiR/1LL_1QL_1LL+_1QL+.yml
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/io/check_basis-1_0_1/4/2psiL_2psiR/1LL_1QL_1dR_1uR.yml
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/io/check_basis-1_0_1/4/2psiL_2psiR/1LL_1dR+_1LL+_1dR.yml
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/io/check_basis-1_0_1/4/2psiL_2psiR/1LL_1eR+_1LL+_1eR.yml
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/io/check_basis-1_0_1/4/2psiL_2psiR/1LL_1eR+_1QL+_1dR.yml
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/io/check_basis-1_0_1/4/2psiL_2psiR/1LL_1uR+_1LL+_1uR.yml
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/io/check_basis-1_0_1/4/2psiL_2psiR/1QL_1dR+_1LL+_1eR.yml
+-rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/io/check_basis-1_0_1/4/2psiL_2psiR/1QL_1dR+_1QL+_1dR.yml
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/io/check_basis-1_0_1/4/2psiL_2psiR/1QL_1eR+_1QL+_1eR.yml
+-rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/io/check_basis-1_0_1/4/2psiL_2psiR/1QL_1uR+_1QL+_1uR.yml
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/io/check_basis-1_0_1/4/2psiL_2psiR/1dR+_1eR+_1dR_1eR.yml
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/io/check_basis-1_0_1/4/2psiL_2psiR/1dR+_1uR+_1LL+_1QL+.yml
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/io/check_basis-1_0_1/4/2psiL_2psiR/1dR+_1uR+_1dR_1uR.yml
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/io/check_basis-1_0_1/4/2psiL_2psiR/1eR+_1uR+_1eR_1uR.yml
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/io/check_basis-1_0_1/4/2psiL_2psiR/1eR+_1uR+_2QL+.yml
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/io/check_basis-1_0_1/4/2psiL_2psiR/2LL_2LL+.yml
+-rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/io/check_basis-1_0_1/4/2psiL_2psiR/2QL_1eR_1uR.yml
+-rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/io/check_basis-1_0_1/4/2psiL_2psiR/2QL_2QL+.yml
+-rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/io/check_basis-1_0_1/4/2psiL_2psiR/2dR+_2dR.yml
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/io/check_basis-1_0_1/4/2psiL_2psiR/2eR+_2eR.yml
+-rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/io/check_basis-1_0_1/4/2psiL_2psiR/2uR+_2uR.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/io/check_basis-1_0_1/4/2psiL_2psiR/__init__.py
+-rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/io/check_basis-1_0_1/4/4phi_2D/2H_2H+_2D.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/io/check_basis-1_0_1/4/4phi_2D/__init__.py
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/io/check_basis-1_0_1/4/4psiL/1LL_1QL_1eR+_1uR+.yml
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/io/check_basis-1_0_1/4/4psiL/1LL_3QL.yml
+-rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/io/check_basis-1_0_1/4/4psiL/1dR+_1eR+_2uR+.yml
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/io/check_basis-1_0_1/4/4psiL/2QL_1dR+_1uR+.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/io/check_basis-1_0_1/4/4psiL/__init__.py
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/io/check_basis-1_0_1/4/4psiR/1LL+_1QL+_1eR_1uR.yml
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/io/check_basis-1_0_1/4/4psiR/1LL+_3QL+.yml
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/io/check_basis-1_0_1/4/4psiR/1dR_1eR_2uR.yml
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/io/check_basis-1_0_1/4/4psiR/2QL+_1dR_1uR.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/io/check_basis-1_0_1/4/4psiR/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/io/check_basis-1_0_1/5/__init__.py
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/io/check_basis-1_0_1/5/2psiL_3phi/1LL_1eR+_1H_2H+.yml
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/io/check_basis-1_0_1/5/2psiL_3phi/1QL_1dR+_1H_2H+.yml
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/io/check_basis-1_0_1/5/2psiL_3phi/1QL_1uR+_2H_1H+.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/io/check_basis-1_0_1/5/2psiL_3phi/__init__.py
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/io/check_basis-1_0_1/5/3phi_2psiR/1H_2H+_1QL+_1uR.yml
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/io/check_basis-1_0_1/5/3phi_2psiR/2H_1H+_1LL+_1eR.yml
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/io/check_basis-1_0_1/5/3phi_2psiR/2H_1H+_1QL+_1dR.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/io/check_basis-1_0_1/5/3phi_2psiR/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/io/check_basis-1_0_1/6/__init__.py
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/io/check_basis-1_0_1/6/6phi/3H_3H+.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/io/check_basis-1_0_1/6/6phi/__init__.py
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/tex/__init__.py
+-rw-r--r--   0        0        0     7678 2020-02-02 00:00:00.000000 autoeft-1.0.1/autoeft/tex/main.py
+-rw-r--r--   0        0        0     1287 2020-02-02 00:00:00.000000 autoeft-1.0.1/models/README.md
+-rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 autoeft-1.0.1/models/all-left_grsm.yml
+-rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 autoeft-1.0.1/models/all-left_sm.yml
+-rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 autoeft-1.0.1/models/bno_nf1_sm.yml
+-rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 autoeft-1.0.1/models/bno_sm.yml
+-rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 autoeft-1.0.1/models/dynkin_sm.yml
+-rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 autoeft-1.0.1/models/grsm.yml
+-rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 autoeft-1.0.1/models/mfv-sm.yml
+-rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 autoeft-1.0.1/models/nf1_sm.yml
+-rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 autoeft-1.0.1/models/sm.yml
+-rw-r--r--   0        0        0     1967 2020-02-02 00:00:00.000000 autoeft-1.0.1/models/bsm/README.md
+-rw-r--r--   0        0        0     1424 2020-02-02 00:00:00.000000 autoeft-1.0.1/models/bsm/cqs+sm.yml
+-rw-r--r--   0        0        0     1421 2020-02-02 00:00:00.000000 autoeft-1.0.1/models/bsm/cts+sm.yml
+-rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 autoeft-1.0.1/models/bsm/dcs+sm.yml
+-rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 autoeft-1.0.1/models/bsm/lqc1+sm.yml
+-rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 autoeft-1.0.1/models/bsm/lqc2+sm.yml
+-rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 autoeft-1.0.1/models/bsm/lqp1+sm.yml
+-rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 autoeft-1.0.1/models/bsm/lqp2+sm.yml
+-rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 autoeft-1.0.1/models/bsm/ltf+sm.yml
+-rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 autoeft-1.0.1/models/bsm/scs+sm.yml
+-rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 autoeft-1.0.1/models/bsm/u1-u1-sm.yml
+-rw-r--r--   0        0        0     1970 2020-02-02 00:00:00.000000 autoeft-1.0.1/models/bsm/vll+sm.yml
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 autoeft-1.0.1/resources/LOGO
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 autoeft-1.0.1/resources/theme.ini
+-rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 autoeft-1.0.1/resources/tex/main.tex
+-rw-r--r--   0        0        0     3080 2020-02-02 00:00:00.000000 autoeft-1.0.1/.gitignore
+-rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 autoeft-1.0.1/LICENSE
+-rw-r--r--   0        0        0     5586 2020-02-02 00:00:00.000000 autoeft-1.0.1/PyPI_README.md
+-rw-r--r--   0        0        0     3884 2020-02-02 00:00:00.000000 autoeft-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     8130 2020-02-02 00:00:00.000000 autoeft-1.0.1/PKG-INFO
```

### Comparing `autoeft-1.0.0rc0/README.md` & `autoeft-1.0.1/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 
 Automated operator construction for effective field theories.
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
 [![Hatch project](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg)](https://github.com/pypa/hatch)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+[![PyPI - Version](https://img.shields.io/pypi/v/autoeft)](https://pypi.org/project/autoeft/)
+[![Conda (channel only)](https://img.shields.io/conda/vn/conda-forge/autoeft)](https://anaconda.org/conda-forge/autoeft)
 
 ## Table of Contents
 1. [Installation](#installation)
     1. [Requirements](#requirements)
     2. [Installing AutoEFT from PyPI](#installing-autoeft-from-pypi)
     3. [Installing AutoEFT from conda-forge](#installing-autoeft-from-conda-forge)
     4. [Building AutoEFT from Source Code](#building-autoeft-from-source-code)
@@ -20,15 +22,15 @@
     2. [Basis Construction](#basis-construction)
     3. [Loading Operators](#loading-operators)
 3. [License](#license)
 4. [Authors](#authors)
 5. [Cite](#cite)
 
 ## Installation
-AutoEFT is available on the [Python Package Index (PyPI)](https://pypi.org/) and the [conda-forge](https://conda-forge.org/) channel.
+AutoEFT is available on the [Python Package Index (PyPI)](https://pypi.org/) and the [conda-forge](https://conda-forge.org/) channel.[^installation]
 
 ### Requirements
 - [Python](https://www.python.org/) >= 3.8
 - [SageMath](https://www.sagemath.org/) >= 9.3
 - [FORM](https://www.nikhef.nl/~form/) >= 4.3
 
 #### Dependencies
@@ -44,14 +46,16 @@
 To install AutoEFT using `pip`, an already installed and running version of SageMath is required (see the [Sage Installation Guide](https://doc.sagemath.org/html/en/installation/index.html) and [Alternative Installation using PyPI](https://github.com/sagemath/sage/blob/develop/README.md#alternative-installation-using-pypi)).
 
 To install *autoeft* and its dependencies, run:[^homebrew]
 ```shell
 sage -pip install autoeft
 ```
 
+[^installation]: See also [here](https://gitlab.com/auto_eft/autoeft/-/issues?label_name=installation) for a collection of potential installation issues.
+
 [^homebrew]: On *macOS* using [Homebrew](https://brew.sh/), it may be necessary to precede this statement by `PYTHONEXECUTABLE=</path/to/sage>` with the proper path to the SageMath executable inserted.
 In addition, it may be necessary to add the path to SageMath’s executables to the `$PATH` environment variable.
 
 ### Installing AutoEFT from conda-forge
 To install *autoeft* and its dependencies, run:
 - with [conda](https://conda.io/):
 ```shell
@@ -72,14 +76,18 @@
 ```
 
 ## Usage
 Verify the installation by running:
 ```shell
 autoeft --help
 ```
+and
+```shell
+autoeft check
+```
 
 ### Model Files
 The *model file* defines the symmetry groups and field content of a low-energy theory in the [YAML](https://yaml.org/) format.
 To produce a sample *model file*, run:
 ```shell
 autoeft sample-model > sm.yml
 ```
@@ -127,22 +135,29 @@
 print(model)
 # SMEFT: Standard Model Effective Field Theory
 
 LQQQ = basis[{"LL": 1, "QL": 3}]
 print(LQQQ)
 # LL (1) QL(3)
 
-print(LQQQ.n_terms , LQQQ.n_operators , sep=" & ")
+print(LQQQ.n_terms, LQQQ.n_operators, sep=" & ")
 # 3 & 57
 ```
 
 ## License
 [MIT](LICENSE)
 
 ## Authors
-- Robert V. Harlander (RWTH Aachen University)
-- Magnus C. Schaaf (RWTH Aachen University)
+- **Robert V. Harlander** (_RWTH Aachen University_)
+- **Magnus C. Schaaf** (_RWTH Aachen University_)
 
 ## Cite
-If you use AutoEFT in your project, please refer to:
-- <!DOCTYPE html> <html> <body> <p><b> <a href="https://inspirehep.net/literature/2658915"> Standard model effective field theory up to mass dimension 12 </a> </b></p>  <p><a href="https://inspirehep.net/authors/1006678">R.V. Harlander</a> (<a href="https://inspirehep.net/institutions/910724">RWTH Aachen U.</a>), <a href="https://inspirehep.net/authors/2658916">T. Kempkens</a> (<a href="https://inspirehep.net/institutions/910724">RWTH Aachen U.</a>), <a href="https://inspirehep.net/authors/2658917">M.C. Schaaf</a> (<a href="https://inspirehep.net/institutions/910724">RWTH Aachen U.</a>)</p>  <p> e-Print: <a href="https://arxiv.org/abs/2305.06832"> 2305.06832 </a>[hep-ph]</p> <p> DOI: <a href="https://doi.org/10.1103/PhysRevD.108.055020"> 10.1103/PhysRevD.108.055020 </a>(publication) </p> <p> Published in:<span> Phys.Rev.D 108 (2023) 5, 055020</span></p> <br> </body> </html>
+- [**Standard model effective field theory up to mass dimension 12**](https://inspirehep.net/literature/2658915)  
+R.V. Harlander, T. Kempkens, M.C. Schaaf  
+[_Phys. Rev. D_ **108** (2023) 055020](https://doi.org/10.1103/PhysRevD.108.055020),
+[arXiv:2305.06832 [hep-ph]](https://arxiv.org/abs/2305.06832)
+
+- [**AutoEFT: Automated operator construction for effective field theories**](https://inspirehep.net/literature/2703514)  
+R.V. Harlander, M.C. Schaaf  
+[_Comput. Phys. Commun._ **300** (2024) 109198](https://doi.org/10.1016/j.cpc.2024.109198),
+[arXiv:2309.15783 [hep-ph]](https://arxiv.org/abs/2309.15783)
 ---
```

### Comparing `autoeft-1.0.0rc0/autoeft/__init__.py` & `autoeft-1.0.1/autoeft/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,24 +24,24 @@
     __license__ = "<license>"
     __summary__ = "<summary>"
     __webpage__ = "<url>"
 else:
     __program__ = dist.metadata["Name"]
     __version__ = dist.metadata["Version"]
     __authors__ = dist.metadata["Author"]
-    __license__ = dist.metadata["License-Expression"]
+    __license__ = dist.metadata["License"].split("\n")[0]
     __summary__ = dist.metadata["Summary"]
     __webpage__ = dist.metadata["Project-URL"]
 
 pkg_version = packaging.version.Version(__version__)
 version = semver.Version(
     *pkg_version.release,
-    prerelease=None
-    if pkg_version.pre is None
-    else "".join([str(i) for i in pkg_version.pre]),
+    prerelease=(
+        None if pkg_version.pre is None else "".join([str(i) for i in pkg_version.pre])
+    ),
     build=None if pkg_version.dev is None else f"dev{pkg_version.dev}",
 )
 
 # load resources
 try:
     if sys.version_info >= (3, 9):
         __copyright__ = (
@@ -93,15 +93,15 @@
 disclaimer.append(program, style="bold")
 disclaimer.append(" ")
 disclaimer.append(str(version), style="italic")
 disclaimer.append("\n")
 disclaimer.append(__copyright__)
 disclaimer.append("This application is licensed under the ")
 disclaimer.append(__license__, style="italic")
-disclaimer.append(" license.")
+disclaimer.append(".")
 
 conjugation_symbol = os.getenv("AUTOEFT_CS", "+")
 epsilon_dot_symbol = os.getenv("AUTOEFT_DS", "~")
 
 try:
     from sage.version import version as __sage_version__
```

### Comparing `autoeft-1.0.0rc0/autoeft/cli.py` & `autoeft-1.0.1/autoeft/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,20 +5,31 @@
 from typing import List
 from typing import Optional
 
 import autoeft
 import autoeft.base.model as model_entry
 import autoeft.combinatorics.generators as generators_entry
 import autoeft.construction.main as construction_entry
+import autoeft.io.check as check_entry
 import autoeft.io.count as count_entry
 import autoeft.tex.main as latex_entry
 
 print = autoeft.print  # noqa: A001
 
 
+def create_chk_subparser(subparsers):
+    parser = subparsers.add_parser(
+        "check",
+        add_help=False,
+        help="check functionality of this installation",
+    )
+    parser.set_defaults(main_func=check_entry.main)
+    return parser
+
+
 def create_spl_subparser(subparsers):
     parser = subparsers.add_parser(
         "sample-model",
         add_help=False,
         help="produce a sample model file",
     )
     parser.set_defaults(main_func=model_entry.main, quiet=True)
@@ -50,14 +61,20 @@
         "-t",
         "--threads",
         type=int,
         default=os.cpu_count(),
         help="set number of threads starting FORM (default: %(default)s)",
     )
     parser.add_argument(
+        "-n",
+        "--name",
+        type=str,
+        help="set the EFT name (default: <model>-eft)",
+    )
+    parser.add_argument(
         "-o",
         "--output",
         metavar="PATH",
         type=Path,
         default=Path().cwd() / "efts",
         help="set output path (default: %(default)s)",
     )
@@ -88,15 +105,20 @@
         help="set generators path (default: %(default)s)",
     )
     parser.add_argument(
         "--overwrite",
         action="store_true",
         help="overwrite existing output files",
     )
-    parser.set_defaults(main_func=construction_entry.main, no_hc=False)
+    parser.add_argument(
+        "--no_hc",
+        action="store_true",
+        help="prevent the explicit construction of conjugate operator types",
+    )
+    parser.set_defaults(main_func=construction_entry.main)
     return parser
 
 
 def create_cnt_subparser(subparsers):
     desc = (
         "Count the number of families, types, terms, and operators for a given basis."
     )
@@ -135,14 +157,19 @@
         help="do not include ignored types (default: %(default)s)",
     )
     parser.add_argument(
         "--dry-run",
         action="store_true",
         help="only list the types that match the current selection",
     )
+    parser.add_argument(
+        "--no_hc",
+        action="store_true",
+        help="prevent the implicit counting of conjugate operator types",
+    )
     parser.set_defaults(main_func=count_entry.main)
     return parser
 
 
 def create_tex_subparser(subparsers):
     desc = (
         "Generate TeX files for a given basis."
@@ -262,14 +289,15 @@
     parser.add_argument(
         "-q",
         "--quiet",
         action="store_true",
         help="suppress all output",
     )
     subparsers = parser.add_subparsers(title="commands")
+    create_chk_subparser(subparsers)
     create_spl_subparser(subparsers)
     create_con_subparser(subparsers)
     create_cnt_subparser(subparsers)
     create_tex_subparser(subparsers)
     create_gen_subparser(subparsers)
     return parser
```

### Comparing `autoeft-1.0.0rc0/autoeft/utils.py` & `autoeft-1.0.1/autoeft/utils.py`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/base/basis.py` & `autoeft-1.0.1/autoeft/base/basis.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from autoeft.combinatorics import young
 from autoeft.tex import tex
 
 
 class OperatorInfo(pydantic.BaseModel):
     model: ir_model.Model
     version: utils.Version = autoeft.version
-    type: Tuple[Counter[str], Literal["real", "complex"]]  # noqa: A003
+    type: Tuple[Counter[str], Literal["real", "complex"]]
     generations: Counter[str]
     n_terms: pydantic.PositiveInt
     n_operators: pydantic.PositiveInt
     invariants: Dict[str, List[Tuple[young.Tableau, int]]]
 
     def __str__(self):
         return str(self.op_type)
@@ -67,14 +67,23 @@
                     r"\end{description}",
                 ),
             ),
         }
         items = (rf"\item[{item}]{value}" for item, value in content.items())
         return "\n".join((r"\begin{description}", *items, r"\end{description}"))
 
+    def __eq__(self, other) -> bool:
+        if self.version.to_tuple() != other.version.to_tuple():
+            return False
+        if self.invariants != other.invariants:
+            return False
+        return self.dict(exclude={"version", "invariants"}) == other.dict(
+            exclude={"version", "invariants"},
+        )
+
     @pydantic.validator("version")
     def parse_version(cls, v):
         if not v.is_compatible(autoeft.version):
             errmsg = (
                 f"The version {v} of the operator file is not compatible with"
                 f" {autoeft.program} {autoeft.version}."
                 "\n"
@@ -122,37 +131,37 @@
         return self.op_type.family.nl
 
     @property
     def nr(self):
         return self.op_type.family.nr
 
     def is_real(self) -> bool:
-        return self.op_type.is_real(self.model)
+        return self.op_type.is_real()
 
     def is_complex(self) -> bool:
-        return self.op_type.is_complex(self.model)
+        return self.op_type.is_complex()
 
     def path(self) -> Path:
         return self.op_type.full_path()
 
     def yaml_dict(self):
         operator_data = self.dict(
             exclude={"model", "invariants", "permutation_symmetries", "expanded"},
         )
         invariants_data = defaultdict(utils.BlockMap)
         for group_name, tableaux in self.invariants.items():
             for i, (tableau, sign) in enumerate(tableaux, start=1):
                 if group_name == self.model.symmetries.lorentz_group.name:
-                    invariants_data[group_name][
-                        f"O({group_name},{i})"
-                    ] = tableau.render_tableau(self.op_type, sign)
+                    invariants_data[group_name][f"O({group_name},{i})"] = (
+                        tableau.render_tableau(self.op_type, sign)
+                    )
                 else:
-                    invariants_data[group_name][
-                        f"O({group_name},{i})"
-                    ] = tableau.render_tableau(self.op_type, group_name, sign)
+                    invariants_data[group_name][f"O({group_name},{i})"] = (
+                        tableau.render_tableau(self.op_type, group_name, sign)
+                    )
         operator_data["invariants"] = invariants_data
         return operator_data
 
     def yaml(self):
         return yaml.dump(
             self.yaml_dict(),
             Dumper=utils.YamlDumper,
```

### Comparing `autoeft-1.0.0rc0/autoeft/base/classifications.py` & `autoeft-1.0.1/autoeft/base/classifications.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import itertools
 from collections import Counter
 from math import ceil
 from math import floor
 from pathlib import Path
 from typing import Counter as Count
 from typing import Dict
 from typing import List
@@ -95,15 +96,19 @@
         return list(self.n_hel) >= list(reversed(self.n_hel))
 
     def conjugated(self) -> "Family":
         return type(self)(reversed(self.n_hel), self.nD)
 
     def field_helicities2(self) -> List[int]:
         """Return a list of the doubled field helicities."""
-        return sum(([h2] * nh for h2, nh in zip(self.hel2, self.n_hel)), start=[])
+        return list(
+            itertools.chain.from_iterable(
+                itertools.repeat(h2, nh) for h2, nh in zip(self.hel2, self.n_hel)
+            ),
+        )
 
     def primary_partition(self) -> young.Partition:
         """Return the primary partition.
 
         The primary partition is defined by the Young diagram with
         nr columns of length N - 2 and nl columns of length 2.
         """
@@ -194,36 +199,48 @@
 
     def path(self, extension: str = "yml") -> Path:
         return Path(f"{self!a}.{extension}")
 
     def full_path(self, extension: str = "yml") -> Path:
         return self.family.path() / self.path(extension)
 
-    def is_real(self, model: ir_model.Model) -> bool:
+    def is_real(self) -> bool:
         """Return true if is equal to its own conjugate."""
-        if self.family.is_real():
-            names = {f.name: m for f, m in self}
-            for f, m in self:
-                cname = f.conjugated_name()
-                if cname not in names or names[cname] != m:
-                    return False
+        return self.family.is_real() and self == self.conjugated()
+
+    def is_complex(self) -> bool:
+        """Return true if is unequal to its own conjugate."""
+        return not self.is_real()
+
+    def is_normal(self) -> bool:
+        if self.family.is_normal():
+            if self.family.is_real():
+                normal_form = tuple((f.name, m) for f, m in self)
+                cnormal_form = tuple((f.name, m) for f, m in self.conjugated())
+                return self.family.is_normal() and normal_form <= cnormal_form
             return True
         return False
 
-    def is_complex(self, model: ir_model.Model) -> bool:
-        """Return true if is unequal to its own conjugate."""
-        return not self.is_real(model)
+    def conjugated(self) -> "Type":
+        return type(self)(
+            {f.hermitian_conjugated(): m for f, m in self},
+            self.family.conjugated(),
+        )
 
     def sun_partition(self, group: symmetry_groups.SUNGroup) -> young.Partition:
         total = sum(sum(f.representations[group.name]) * m for f, m in self)
         assert total % group.N == 0
         return young.Partition([total // group.N] * group.N)
 
     def sun_content(self, group: symmetry_groups.SUNGroup) -> List[reprs.SUNRepr]:
-        return sum(([f.representations[group.name]] * m for f, m in self), start=[])
+        return list(
+            itertools.chain.from_iterable(
+                itertools.repeat(f.representations[group.name], m) for f, m in self
+            ),
+        )
 
     def field_numbers(self) -> Dict[str, List[int]]:
         field_number = 1
         return {
             f.name: list(range(field_number, field_number := field_number + m))
             for f, m in self
         }
```

### Comparing `autoeft-1.0.0rc0/autoeft/base/groups.py` & `autoeft-1.0.1/autoeft/base/groups.py`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/base/model.py` & `autoeft-1.0.1/autoeft/base/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,16 @@
 
     def __hash__(self):
         return hash(
             (self.lorentz_group, frozenset(self.sun_groups), frozenset(self.u1_groups)),
         )
 
     def __eq__(self, other):
+        if not isinstance(other, Symmetries):
+            return False
         lor = self.lorentz_group == other.lorentz_group
         sun = self.sun_groups == other.sun_groups
         u1 = self.u1_groups == other.u1_groups
         order = tuple(self.sun_groups.keys()) == tuple(other.sun_groups.keys())
         return lor and sun and u1 and order
 
     def __getitem__(self, key):
@@ -160,27 +162,34 @@
                     for name in values["symmetries"].u1_groups
                 },
             )
         return representations
 
     @pydantic.validator("conjugate", always=True)
     def parse_conjugate(cls, v, values):
+        if v is not None:
+            return v
         if {"symmetries", "representations"} <= values.keys():
             lorentz_group = values["symmetries"].lorentz_group
             sun_groups = values["symmetries"].sun_groups
             u1_groups = values["symmetries"].u1_groups
             if values["representations"][lorentz_group.name].is_complex():
-                return v if v is not None else True
+                return True
+            pseudo_reals = 0
             for group_name in sun_groups:
                 if values["representations"][group_name].is_complex():
-                    return v if v is not None else True
+                    return True
+                if values["representations"][group_name].is_pseudo_real():
+                    pseudo_reals += 1
+            if pseudo_reals % 2:
+                return True
             for group_name in u1_groups:
                 if values["representations"][group_name].is_complex():
-                    return v if v is not None else True
-            return v if v is not None else False
+                    return True
+            return False
         return v
 
     @pydantic.validator("anticommute", always=True)
     def parse_anticommute(cls, v, values):
         if {"symmetries", "representations"} <= values.keys():
             lorentz_group = values["symmetries"].lorentz_group
             helicity = values["representations"][lorentz_group.name].helicity
```

### Comparing `autoeft-1.0.0rc0/autoeft/base/representations.py` & `autoeft-1.0.1/autoeft/base/representations.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     def conjugated(self) -> "Repr":
         raise NotImplementedError
 
     def is_real(self) -> bool:
         return self == self.conjugated()
 
     def is_complex(self) -> bool:
-        return not self.is_real()
+        return self != self.conjugated()
 
     class Config:
         extra = pydantic.Extra.forbid
 
 
 class LorentzRepr(Repr):
     """A representation of the Lorentz group.
@@ -110,14 +110,25 @@
         This inverts the order of the Dynkin labels of the partition.
         """
         conj_part = young.Partition.from_dynkin(
             list(reversed(self.partition.to_dynkin(self.N))),
         )
         return self.copy(update={"N": self.N, "partition": conj_part})
 
+    def is_real(self):
+        dynkin = self.partition.to_dynkin(self.N)
+        if dynkin == list(reversed(dynkin)):
+            if (self.N + 2) % 4 == 0:
+                return dynkin[int(self.N / 2 - 1)] % 2 == 0
+            return True
+        return False
+
+    def is_pseudo_real(self) -> bool:
+        return not self.is_complex() and not self.is_real()
+
 
 class U1Repr(Repr):
     """A representation of a U(1) group.
 
     Characterized by a U(1) charge.
     """
```

### Comparing `autoeft-1.0.0rc0/autoeft/base/tensors.py` & `autoeft-1.0.1/autoeft/base/tensors.py`

 * *Files 0% similar despite different names*

```diff
@@ -838,15 +838,15 @@
         fields = "*".join(fields)
         return tensor + " * " + fields, lr_sign
 
 
 # misc
 
 
-def ibp_reduction(  # noqa: C901
+def ibp_reduction(
     lr_tableau: LRTableau,
     coeff: Optional[utils.Fraction] = None,
 ) -> Count[LRTableau]:
     if coeff is None:
         coeff = utils.Fraction(1)
     result = Counter()
     lr_tab, lr_sign = lr_tableau.normalized()
```

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/generators.py` & `autoeft-1.0.1/autoeft/combinatorics/generators.py`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/symmetric_group.py` & `autoeft-1.0.1/autoeft/combinatorics/symmetric_group.py`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/young.py` & `autoeft-1.0.1/autoeft/combinatorics/young.py`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_2/P_1_1_cycle.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_2/P_1_1_cycle.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_2/P_1_1_reflection.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_2/P_1_1_reflection.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_2/P_2_cycle.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_2/P_2_cycle.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_2/P_2_reflection.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_2/P_2_reflection.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_3/P_1_1_1_cycle.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_3/P_1_1_1_cycle.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_3/P_1_1_1_reflection.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_3/P_1_1_1_reflection.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_3/P_2_1_cycle.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_3/P_2_1_cycle.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_3/P_2_1_reflection.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_3/P_2_1_reflection.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_3/P_3_cycle.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_3/P_3_cycle.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_3/P_3_reflection.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_3/P_3_reflection.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_4/P_1_1_1_1_cycle.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_4/P_1_1_1_1_cycle.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_4/P_1_1_1_1_reflection.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_4/P_1_1_1_1_reflection.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_4/P_2_1_1_cycle.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_4/P_2_1_1_cycle.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_4/P_2_1_1_reflection.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_4/P_2_1_1_reflection.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_4/P_2_2_cycle.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_4/P_2_2_cycle.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_4/P_2_2_reflection.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_4/P_2_2_reflection.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_4/P_3_1_cycle.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_4/P_3_1_cycle.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_4/P_3_1_reflection.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_4/P_3_1_reflection.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_4/P_4_cycle.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_4/P_4_cycle.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_4/P_4_reflection.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_4/P_4_reflection.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_5/P_1_1_1_1_1_cycle.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_5/P_1_1_1_1_1_cycle.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_5/P_1_1_1_1_1_reflection.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_5/P_1_1_1_1_1_reflection.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_5/P_2_1_1_1_cycle.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_5/P_2_1_1_1_cycle.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_5/P_2_1_1_1_reflection.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_5/P_2_1_1_1_reflection.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_5/P_2_2_1_cycle.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_5/P_2_2_1_cycle.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_5/P_2_2_1_reflection.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_5/P_2_2_1_reflection.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_5/P_3_1_1_cycle.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_5/P_3_1_1_cycle.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_5/P_3_1_1_reflection.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_5/P_3_1_1_reflection.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_5/P_3_2_cycle.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_5/P_3_2_cycle.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_5/P_3_2_reflection.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_5/P_3_2_reflection.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_5/P_4_1_cycle.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_5/P_4_1_cycle.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_5/P_4_1_reflection.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_5/P_4_1_reflection.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_5/P_5_cycle.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_5/P_5_cycle.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_5/P_5_reflection.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_5/P_5_reflection.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_6/P_1_1_1_1_1_1_cycle.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_6/P_1_1_1_1_1_1_cycle.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_6/P_1_1_1_1_1_1_reflection.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_6/P_1_1_1_1_1_1_reflection.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_6/P_2_1_1_1_1_cycle.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_6/P_2_1_1_1_1_cycle.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_6/P_2_1_1_1_1_reflection.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_6/P_2_1_1_1_1_reflection.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_6/P_2_2_1_1_cycle.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_6/P_2_2_1_1_cycle.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_6/P_2_2_1_1_reflection.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_6/P_2_2_1_1_reflection.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_6/P_2_2_2_cycle.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_6/P_2_2_2_cycle.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_6/P_2_2_2_reflection.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_6/P_2_2_2_reflection.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_6/P_3_1_1_1_cycle.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_6/P_3_1_1_1_cycle.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_6/P_3_1_1_1_reflection.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_6/P_3_1_1_1_reflection.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_6/P_3_2_1_cycle.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_6/P_3_2_1_cycle.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_6/P_3_2_1_reflection.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_6/P_3_2_1_reflection.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_6/P_3_3_cycle.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_6/P_3_3_cycle.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_6/P_3_3_reflection.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_6/P_3_3_reflection.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_6/P_4_1_1_cycle.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_6/P_4_1_1_cycle.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_6/P_4_1_1_reflection.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_6/P_4_1_1_reflection.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_6/P_4_2_cycle.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_6/P_4_2_cycle.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_6/P_4_2_reflection.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_6/P_4_2_reflection.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_6/P_5_1_cycle.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_6/P_5_1_cycle.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_6/P_5_1_reflection.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_6/P_5_1_reflection.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_6/P_6_cycle.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_6/P_6_cycle.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_6/P_6_reflection.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_6/P_6_reflection.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_7/P_1_1_1_1_1_1_1_cycle.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_7/P_1_1_1_1_1_1_1_cycle.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_7/P_1_1_1_1_1_1_1_reflection.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_7/P_1_1_1_1_1_1_1_reflection.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_7/P_2_1_1_1_1_1_cycle.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_7/P_2_1_1_1_1_1_cycle.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_7/P_2_1_1_1_1_1_reflection.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_7/P_2_1_1_1_1_1_reflection.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_7/P_2_2_1_1_1_cycle.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_7/P_2_2_1_1_1_cycle.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_7/P_2_2_1_1_1_reflection.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_7/P_2_2_1_1_1_reflection.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_7/P_2_2_2_1_cycle.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_7/P_2_2_2_1_cycle.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_7/P_2_2_2_1_reflection.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_7/P_2_2_2_1_reflection.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_7/P_3_1_1_1_1_cycle.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_7/P_3_1_1_1_1_cycle.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_7/P_3_1_1_1_1_reflection.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_7/P_3_1_1_1_1_reflection.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_7/P_3_2_1_1_cycle.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_7/P_3_2_1_1_cycle.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_7/P_3_2_1_1_reflection.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_7/P_3_2_1_1_reflection.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_7/P_3_2_2_cycle.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_7/P_3_2_2_cycle.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_7/P_3_2_2_reflection.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_7/P_3_2_2_reflection.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_7/P_3_3_1_cycle.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_7/P_3_3_1_cycle.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_7/P_3_3_1_reflection.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_7/P_3_3_1_reflection.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_7/P_4_1_1_1_cycle.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_7/P_4_1_1_1_cycle.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_7/P_4_1_1_1_reflection.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_7/P_4_1_1_1_reflection.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_7/P_4_2_1_cycle.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_7/P_4_2_1_cycle.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_7/P_4_2_1_reflection.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_7/P_4_2_1_reflection.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_7/P_4_3_cycle.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_7/P_4_3_cycle.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_7/P_4_3_reflection.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_7/P_4_3_reflection.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_7/P_5_1_1_cycle.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_7/P_5_1_1_cycle.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_7/P_5_1_1_reflection.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_7/P_5_1_1_reflection.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_7/P_5_2_cycle.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_7/P_5_2_cycle.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_7/P_5_2_reflection.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_7/P_5_2_reflection.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_7/P_6_1_cycle.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_7/P_6_1_cycle.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_7/P_6_1_reflection.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_7/P_6_1_reflection.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_7/P_7_cycle.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_7/P_7_cycle.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_7/P_7_reflection.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_7/P_7_reflection.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_8/P_1_1_1_1_1_1_1_1_cycle.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_8/P_1_1_1_1_1_1_1_1_cycle.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_8/P_1_1_1_1_1_1_1_1_reflection.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_8/P_1_1_1_1_1_1_1_1_reflection.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_8/P_2_1_1_1_1_1_1_cycle.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_8/P_2_1_1_1_1_1_1_cycle.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_8/P_2_1_1_1_1_1_1_reflection.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_8/P_2_1_1_1_1_1_1_reflection.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_8/P_2_2_1_1_1_1_cycle.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_8/P_2_2_1_1_1_1_cycle.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_8/P_2_2_1_1_1_1_reflection.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_8/P_2_2_1_1_1_1_reflection.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_8/P_2_2_2_1_1_cycle.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_8/P_2_2_2_1_1_cycle.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_8/P_2_2_2_1_1_reflection.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_8/P_2_2_2_1_1_reflection.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_8/P_2_2_2_2_cycle.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_8/P_2_2_2_2_cycle.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_8/P_2_2_2_2_reflection.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_8/P_2_2_2_2_reflection.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_8/P_3_1_1_1_1_1_cycle.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_8/P_3_1_1_1_1_1_cycle.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_8/P_3_1_1_1_1_1_reflection.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_8/P_3_1_1_1_1_1_reflection.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_8/P_3_2_1_1_1_cycle.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_8/P_3_2_1_1_1_cycle.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_8/P_3_2_1_1_1_reflection.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_8/P_3_2_1_1_1_reflection.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_8/P_3_2_2_1_cycle.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_8/P_3_2_2_1_cycle.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_8/P_3_2_2_1_reflection.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_8/P_3_2_2_1_reflection.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_8/P_3_3_1_1_cycle.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_8/P_3_3_1_1_cycle.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_8/P_3_3_1_1_reflection.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_8/P_3_3_1_1_reflection.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_8/P_3_3_2_cycle.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_8/P_3_3_2_cycle.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_8/P_3_3_2_reflection.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_8/P_3_3_2_reflection.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_8/P_4_1_1_1_1_cycle.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_8/P_4_1_1_1_1_cycle.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_8/P_4_1_1_1_1_reflection.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_8/P_4_1_1_1_1_reflection.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_8/P_4_2_1_1_cycle.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_8/P_4_2_1_1_cycle.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_8/P_4_2_1_1_reflection.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_8/P_4_2_1_1_reflection.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_8/P_4_2_2_cycle.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_8/P_4_2_2_cycle.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_8/P_4_2_2_reflection.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_8/P_4_2_2_reflection.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_8/P_4_3_1_cycle.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_8/P_4_3_1_cycle.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_8/P_4_3_1_reflection.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_8/P_4_3_1_reflection.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_8/P_4_4_cycle.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_8/P_4_4_cycle.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_8/P_4_4_reflection.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_8/P_4_4_reflection.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_8/P_5_1_1_1_cycle.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_8/P_5_1_1_1_cycle.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_8/P_5_1_1_1_reflection.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_8/P_5_1_1_1_reflection.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_8/P_5_2_1_cycle.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_8/P_5_2_1_cycle.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_8/P_5_2_1_reflection.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_8/P_5_2_1_reflection.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_8/P_5_3_cycle.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_8/P_5_3_cycle.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_8/P_5_3_reflection.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_8/P_5_3_reflection.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_8/P_6_1_1_cycle.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_8/P_6_1_1_cycle.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_8/P_6_1_1_reflection.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_8/P_6_1_1_reflection.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_8/P_6_2_cycle.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_8/P_6_2_cycle.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_8/P_6_2_reflection.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_8/P_6_2_reflection.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_8/P_7_1_cycle.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_8/P_7_1_cycle.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_8/P_7_1_reflection.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_8/P_7_1_reflection.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_8/P_8_cycle.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_8/P_8_cycle.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_8/P_8_reflection.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_8/P_8_reflection.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/P_1_1_1_1_1_1_1_1_1_cycle.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_9/P_1_1_1_1_1_1_1_1_1_cycle.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/P_1_1_1_1_1_1_1_1_1_reflection.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_9/P_1_1_1_1_1_1_1_1_1_reflection.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/P_2_1_1_1_1_1_1_1_cycle.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_9/P_2_1_1_1_1_1_1_1_cycle.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/P_2_1_1_1_1_1_1_1_reflection.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_9/P_2_1_1_1_1_1_1_1_reflection.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/P_2_2_1_1_1_1_1_cycle.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_9/P_2_2_1_1_1_1_1_cycle.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/P_2_2_1_1_1_1_1_reflection.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_9/P_2_2_1_1_1_1_1_reflection.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/P_2_2_2_1_1_1_cycle.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_9/P_2_2_2_1_1_1_cycle.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/P_2_2_2_1_1_1_reflection.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_9/P_2_2_2_1_1_1_reflection.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/P_2_2_2_2_1_cycle.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_9/P_2_2_2_2_1_cycle.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/P_2_2_2_2_1_reflection.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_9/P_2_2_2_2_1_reflection.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/P_3_1_1_1_1_1_1_cycle.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_9/P_3_1_1_1_1_1_1_cycle.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/P_3_1_1_1_1_1_1_reflection.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_9/P_3_1_1_1_1_1_1_reflection.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/P_3_2_1_1_1_1_cycle.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_9/P_3_2_1_1_1_1_cycle.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/P_3_2_1_1_1_1_reflection.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_9/P_3_2_1_1_1_1_reflection.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/P_3_2_2_1_1_cycle.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_9/P_3_2_2_1_1_cycle.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/P_3_2_2_1_1_reflection.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_9/P_3_2_2_1_1_reflection.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/P_3_2_2_2_cycle.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_9/P_3_2_2_2_cycle.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/P_3_2_2_2_reflection.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_9/P_3_2_2_2_reflection.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/P_3_3_1_1_1_cycle.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_9/P_3_3_1_1_1_cycle.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/P_3_3_1_1_1_reflection.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_9/P_3_3_1_1_1_reflection.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/P_3_3_2_1_cycle.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_9/P_3_3_2_1_cycle.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/P_3_3_2_1_reflection.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_9/P_3_3_2_1_reflection.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/P_3_3_3_cycle.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_9/P_3_3_3_cycle.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/P_3_3_3_reflection.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_9/P_3_3_3_reflection.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/P_4_1_1_1_1_1_cycle.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_9/P_4_1_1_1_1_1_cycle.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/P_4_1_1_1_1_1_reflection.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_9/P_4_1_1_1_1_1_reflection.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/P_4_2_1_1_1_cycle.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_9/P_4_2_1_1_1_cycle.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/P_4_2_1_1_1_reflection.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_9/P_4_2_1_1_1_reflection.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/P_4_2_2_1_cycle.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_9/P_4_2_2_1_cycle.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/P_4_2_2_1_reflection.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_9/P_4_2_2_1_reflection.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/P_4_3_1_1_cycle.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_9/P_4_3_1_1_cycle.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/P_4_3_1_1_reflection.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_9/P_4_3_1_1_reflection.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/P_4_3_2_cycle.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_9/P_4_3_2_cycle.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/P_4_3_2_reflection.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_9/P_4_3_2_reflection.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/P_4_4_1_cycle.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_9/P_4_4_1_cycle.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/P_4_4_1_reflection.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_9/P_4_4_1_reflection.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/P_5_1_1_1_1_cycle.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_9/P_5_1_1_1_1_cycle.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/P_5_1_1_1_1_reflection.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_9/P_5_1_1_1_1_reflection.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/P_5_2_1_1_cycle.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_9/P_5_2_1_1_cycle.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/P_5_2_1_1_reflection.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_9/P_5_2_1_1_reflection.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/P_5_2_2_cycle.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_9/P_5_2_2_cycle.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/P_5_2_2_reflection.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_9/P_5_2_2_reflection.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/P_5_3_1_cycle.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_9/P_5_3_1_cycle.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/P_5_3_1_reflection.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_9/P_5_3_1_reflection.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/P_5_4_cycle.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_9/P_5_4_cycle.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/P_5_4_reflection.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_9/P_5_4_reflection.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/P_6_1_1_1_cycle.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_9/P_6_1_1_1_cycle.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/P_6_1_1_1_reflection.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_9/P_6_1_1_1_reflection.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/P_6_2_1_cycle.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_9/P_6_2_1_cycle.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/P_6_2_1_reflection.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_9/P_6_2_1_reflection.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/P_6_3_cycle.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_9/P_6_3_cycle.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/P_6_3_reflection.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_9/P_6_3_reflection.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/P_7_1_1_cycle.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_9/P_7_1_1_cycle.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/P_7_1_1_reflection.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_9/P_7_1_1_reflection.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/P_7_2_cycle.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_9/P_7_2_cycle.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/P_7_2_reflection.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_9/P_7_2_reflection.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/P_8_1_cycle.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_9/P_8_1_cycle.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/P_8_1_reflection.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_9/P_8_1_reflection.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/P_9_cycle.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_9/P_9_cycle.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/combinatorics/gens/S_9/P_9_reflection.npz` & `autoeft-1.0.1/autoeft/combinatorics/gens/S_9/P_9_reflection.npz`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/construction/invariants.py` & `autoeft-1.0.1/autoeft/construction/invariants.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import itertools
 from collections import Counter
 from math import ceil
 from math import floor
 from typing import Counter as Count
 from typing import Iterable
 from typing import Iterator
 from typing import List
@@ -26,26 +27,26 @@
 ) -> Iterator[tensors.SUNTableau]:
     """Modified Littlewood-Richardson rule.
 
     Return the product of two tableaux
     using a modified version of the Littlewood-Richardson rule.
     """
     for part, coeff in combinat.lr_rule(lhs.shape, rhs.shape, N).items():
-        assert (
-            len(skew_tableaux := combinat.lr_skew_tableaux(part, lhs.shape, rhs.shape))
-            == coeff
-        )
+        skew_tableaux = combinat.lr_skew_tableaux(part, lhs.shape, rhs.shape)
+        assert len(skew_tableaux) == coeff
         for skew_tab in skew_tableaux:
             rhs_idx = [list(row) for row in rhs]
             yield tensors.SUNTableau(
                 (
                     (
-                        lhs[row, col]
-                        if row < len(lhs) and col < len(lhs[row])
-                        else rhs_idx[skew_tab[row, col] - 1].pop(0)
+                        (
+                            lhs[row, col]
+                            if row < len(lhs) and col < len(lhs[row])
+                            else rhs_idx[skew_tab[row, col] - 1].pop(0)
+                        )
                         for col in range(row_len)
                     )
                     for row, row_len in enumerate(part)
                 ),
             )
 
 
@@ -117,14 +118,15 @@
     errmsg = "Lorentz"
     raise exceptions.NoContractionException(errmsg)  # no invariant contractions found
 
 
 def construct_types(
     family: classes.Family,
     model: ir_model.Model,
+    hc_flag: bool = True,
 ) -> Iterator[classes.Type]:
     def _con_types(
         f_counts: Count[ir_model.Field],
         h_counts: Count[utils.Fraction],
         fields: List[ir_model.Field],
     ):
         if sum(h_counts.values()) == 0:  # all helicity slots are filled
@@ -140,15 +142,17 @@
                     sum(f.representations[name].partition) * m
                     for f, m in f_counts.items()
                 )
                 if tot_indices % group.N != 0:
                     # reject operators where the total number of SU(N) fundamental
                     # indices is not a multiple of N
                     return
-            yield classes.Type(f_counts, family)
+            con_type = classes.Type(f_counts, family)
+            if hc_flag or con_type.is_normal():
+                yield con_type
         while fields:
             field = fields.pop(0)
             hel = field.helicity
             for nh in range(1, h_counts[hel] + 1):
                 new_h_counts = h_counts.copy()
                 new_h_counts[hel] -= nh
                 new_f_counts = f_counts.copy()
@@ -165,61 +169,67 @@
     N: int,
     nl: int,
     nr: int,
     hc_flag: bool = True,
 ) -> Iterator[classes.Family]:
     for nD in range(2 * min(nl, nr) + 1):
         for nFR in range(nr - ceil(nD / 2) + 1):
-            boundFL = nl - ceil(nD / 2) if hc_flag or nl != nr else nFR
-            for nFL in range(boundFL + 1):
+            for nFL in range(nl - ceil(nD / 2) + 1):
                 nPsiD = 2 * nr - 2 * nFR - nD
                 nPsi = 2 * nl - 2 * nFL - nD
                 nPhi = N - nFR - nFL - nPsiD - nPsi
                 n_hel = (nFL, nPsi, nPhi, nPsiD, nFR)
-                fh2 = sum(
-                    ([h2] * n for h2, n in zip((-2, -1, 0, 1, 2), n_hel)),
-                    start=[],
+                fh2 = list(
+                    itertools.chain.from_iterable(
+                        itertools.repeat(h2, n)
+                        for h2, n in zip((-2, -1, 0, 1, 2), n_hel)
+                    ),
                 )
                 if (
                     all(nh >= 0 for nh in n_hel)
                     and nD >= max(nPsiD % 2, -nPsi % 2)
                     and nD >= -2 * min(fh2) - (2 * nFL + nPsi)
                     and nD >= 2 * max(fh2) - (2 * nFR + nPsiD)
                 ):
-                    yield classes.Family(n_hel, nD)
+                    con_family = classes.Family(n_hel, nD)
+                    if hc_flag or con_family.is_normal():
+                        yield con_family
 
 
 def _construct_families_gr(
     N: int,
     nl: int,
     nr: int,
     nGR: int,
     hc_flag: bool = True,
 ) -> Iterator[classes.Family]:
     for nD in range(2 * min(nl, nr) + 1):
         for nCR in range(ceil(nr / 2 - nD / 4) + 1):
             nCL = nGR - nCR
             for nFR in range(nr - 2 * nCR - ceil(nD / 2) + 1):
-                boundFL = nl - 2 * nCL - ceil(nD / 2) if hc_flag or nl != nr else nFR
-                for nFL in range(boundFL + 1):
+                for nFL in range(nl - 2 * nCL - ceil(nD / 2) + 1):
                     nPsiD = 2 * nr - 4 * nCR - 2 * nFR - nD
                     nPsi = 2 * nl - 4 * nCL - 2 * nFL - nD
                     nPhi = N - nCR - nCL - nFR - nFL - nPsiD - nPsi
                     n_hel = (nCL, nFL, nPsi, nPhi, nPsiD, nFR, nCR)
-                    fh2 = sum(
-                        ([h2] * n for h2, n in zip((-4, -2, -1, 0, 1, 2, 4), n_hel)),
-                        start=[],
+                    fh2 = list(
+                        itertools.chain.from_iterable(
+                            itertools.repeat(h2, n)
+                            for h2, n in zip((-4, -2, -1, 0, 1, 2, 4), n_hel)
+                        ),
                     )
                     if (
                         all(nh >= 0 for nh in n_hel)
                         and nD >= max(nPsiD % 2, -nPsi % 2)
                         and nD >= -2 * min(fh2) - (4 * nCL + 2 * nFL + nPsi)
                         and nD >= 2 * max(fh2) - (4 * nCR + 2 * nFR + nPsiD)
                     ):
-                        yield classes.FamilyGR(n_hel, nD)
+                        con_family = classes.FamilyGR(n_hel, nD)
+                        if hc_flag or con_family.is_normal():
+                            yield con_family
 
 
 def construct_families(
     d: int,
     hc_flag: bool = True,
     gr_flag: bool = False,
 ) -> Iterator[classes.Family]:
```

### Comparing `autoeft-1.0.0rc0/autoeft/construction/main.py` & `autoeft-1.0.1/autoeft/construction/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -121,20 +121,21 @@
 
 
 def plain_main(
     model: ir_model.Model,
     dimension: int,
     hc_flag: bool,
     gr_flag: bool,
-    basis_file: io_basis.BasisFile,
+    basis_file: Optional[io_basis.BasisFile] = None,
     select: Optional[list] = None,
     ignore: Optional[list] = None,
     overwrite: bool = False,
     threads: Optional[int] = None,
-) -> Tuple[Counter, Counter, Counter, Counter]:
+) -> Tuple[eft_basis.Basis, Tuple[Counter, Counter, Counter, Counter]]:
+    basis = eft_basis.Basis(model)
     ct_family, ct_type, ct_term, ct_operator = (
         Counter(),
         Counter(),
         Counter(),
         Counter(),
     )
     tct_family, tct_type, tct_term, tct_operator = (
@@ -148,55 +149,71 @@
         rich.progress.TextColumn("{task.description}", style="bold"),
     )
     status_task = operator_status.add_task("")
     stats_progress = rich.progress.Progress(
         rich.progress.TextColumn(
             "#[repr.attrib_name]{task.description}[/repr.attrib_name]"
             "="
-            "[repr.number]{task.total:,}[/repr.number]([repr.number]{task.completed:,})[/repr.number]",
+            "[repr.number]{task.total:,}[/repr.number]"
+            " ([repr.number]{task.fields[exist]:,}[/repr.number] existing,"
+            " [repr.number]{task.completed:,}[/repr.number] constructed in this run)",
         ),
     )
-    families_task = stats_progress.add_task("families", total=0)
-    types_task = stats_progress.add_task("types", total=0)
-    terms_task = stats_progress.add_task("terms", total=0)
-    operators_task = stats_progress.add_task("operators", total=0)
+    families_task = stats_progress.add_task("families", total=0, exist=0)
+    types_task = stats_progress.add_task("types", total=0, exist=0)
+    terms_task = stats_progress.add_task("terms", total=0, exist=0)
+    operators_task = stats_progress.add_task("operators", total=0, exist=0)
     progress_group = rich.console.Group(
         operator_status,
         stats_progress,
     )
     with rich.live.Live(
         progress_group,
         console=autoeft.console,
         transient=True,
     ) as live:
         for family in invariants.construct_families(dimension, hc_flag, gr_flag):
-            hc_mod = 1 if hc_flag or family.is_real() else 2
-            for op_type in invariants.construct_types(family, model):
+            hc_mod_f = 1 if hc_flag or family.is_real() else 2
+            for op_type in invariants.construct_types(family, model, hc_flag):
+                hc_mod_t = 1 if hc_flag or op_type.is_real() else 2
                 operator_status.update(status_task, description=str(op_type))
                 live.refresh()
-                op_stats = basis_file.get_operator_raw_numbers(op_type.full_path())
-                if op_stats:
-                    terms_per_type, operators_per_type = op_stats
-                    if terms_per_type:
-                        tct_family[family] = hc_mod
-                        tct_type[op_type] = hc_mod
-                        tct_term[op_type] = hc_mod * terms_per_type
-                        tct_operator[op_type] = hc_mod * operators_per_type
-                        stats_progress.update(
-                            families_task,
-                            total=sum(tct_family.values()),
-                        )
-                        stats_progress.update(types_task, total=sum(tct_type.values()))
-                        stats_progress.update(terms_task, total=sum(tct_term.values()))
-                        stats_progress.update(
-                            operators_task,
-                            total=sum(tct_operator.values()),
-                        )
-                    if not overwrite:
-                        continue
+                if basis_file:
+                    op_stats = basis_file.get_operator_raw_numbers(op_type.full_path())
+                    if op_stats:
+                        terms_per_type, operators_per_type = op_stats
+                        if terms_per_type:
+                            tct_family[family] = hc_mod_f
+                            tct_type[op_type] = hc_mod_t
+                            tct_term[op_type] = hc_mod_t * terms_per_type
+                            tct_operator[op_type] = hc_mod_t * operators_per_type
+                            stats_progress.update(
+                                families_task,
+                                total=sum(tct_family.values()),
+                                exist=sum(tct_family.values())
+                                - sum(ct_family.values()),
+                            )
+                            stats_progress.update(
+                                types_task,
+                                total=sum(tct_type.values()),
+                                exist=sum(tct_type.values()) - sum(ct_type.values()),
+                            )
+                            stats_progress.update(
+                                terms_task,
+                                total=sum(tct_term.values()),
+                                exist=sum(tct_term.values()) - sum(ct_term.values()),
+                            )
+                            stats_progress.update(
+                                operators_task,
+                                total=sum(tct_operator.values()),
+                                exist=sum(tct_operator.values())
+                                - sum(ct_operator.values()),
+                            )
+                        if not overwrite:
+                            continue
                 if select and not utils.type_matches(op_type, select):
                     continue
                 if ignore and utils.type_matches(op_type, ignore):
                     continue
                 try:
                     lorentz_tableaux = invariants.construct_lorentz_tableaux(family)
                     sun_groups_tableaux = {
@@ -254,15 +271,15 @@
                             )
                             permutations_info.append(permutation_info)
                             terms_per_type += terms_per_symmetry
                             operators_per_type += operators_per_symmetry
                 if terms_per_type:
                     type_info = (
                         op_type.to_counter(),
-                        "real" if op_type.is_real(model) else "complex",
+                        "real" if op_type.is_real() else "complex",
                     )
                     generations_info = Counter(
                         {f.name: f.generations for f, _ in op_type},
                     )
                     invariants_info = {
                         model.symmetries.lorentz_group.name: list(
                             zip(lorentz_tableaux, itertools.repeat(1)),
@@ -279,75 +296,92 @@
                         type=type_info,
                         generations=generations_info,
                         n_terms=terms_per_type,
                         n_operators=operators_per_type,
                         invariants=invariants_info,
                         permutation_symmetries=permutations_info,
                     )
-                    basis_file.add_operator_info(operator_info)
+                    basis[repr(operator_info)] = operator_info
+                    if basis_file:
+                        basis_file.add_operator_info(operator_info)
                     print(repr(op_type), dest="log")
-                    ct_family[family] = hc_mod
-                    ct_type[op_type] = hc_mod
-                    ct_term[op_type] = hc_mod * terms_per_type
-                    ct_operator[op_type] = hc_mod * operators_per_type
-                    tct_family[family] = hc_mod
-                    tct_type[op_type] = hc_mod
-                    tct_term[op_type] = hc_mod * terms_per_type
-                    tct_operator[op_type] = hc_mod * operators_per_type
+                    ct_family[family] = hc_mod_f
+                    ct_type[op_type] = hc_mod_t
+                    ct_term[op_type] = hc_mod_t * terms_per_type
+                    ct_operator[op_type] = hc_mod_t * operators_per_type
+                    tct_family[family] = hc_mod_f
+                    tct_type[op_type] = hc_mod_t
+                    tct_term[op_type] = hc_mod_t * terms_per_type
+                    tct_operator[op_type] = hc_mod_t * operators_per_type
                     stats_progress.update(
                         families_task,
                         total=sum(tct_family.values()),
                         completed=sum(ct_family.values()),
+                        exist=sum(tct_family.values()) - sum(ct_family.values()),
                     )
                     stats_progress.update(
                         types_task,
                         total=sum(tct_type.values()),
                         advance=ct_type[op_type],
+                        exist=sum(tct_type.values()) - sum(ct_type.values()),
                     )
                     stats_progress.update(
                         terms_task,
                         total=sum(tct_term.values()),
                         advance=ct_term[op_type],
+                        exist=sum(tct_term.values()) - sum(ct_term.values()),
                     )
                     stats_progress.update(
                         operators_task,
                         total=sum(tct_operator.values()),
                         advance=ct_operator[op_type],
+                        exist=sum(tct_operator.values()) - sum(ct_operator.values()),
                     )
         operator_status.update(status_task, visible=False)
+    fam_total, fam_constructed = sum(tct_family.values()), sum(ct_family.values())
+    type_total, type_constructed = sum(tct_type.values()), sum(ct_type.values())
+    term_total, term_constructed = sum(tct_term.values()), sum(ct_term.values())
+    op_total, op_constructed = sum(tct_operator.values()), sum(ct_operator.values())
     print(
-        f"[b]#[/b]families=[repr.number]{sum(tct_family.values()):,}[/repr.number]"
-        f"([repr.number]{sum(ct_family.values()):,}[/repr.number])",
+        f"[b]#[/b]families=[repr.number]{fam_total:,}[/repr.number]"
+        f" ([repr.number]{fam_total-fam_constructed:,}[/repr.number] existing,"
+        f" [repr.number]{fam_constructed:,}[/repr.number] constructed in this run)",
     )
     print(
-        f"[b]#[/b]types=[repr.number]{sum(tct_type.values()):,}[/repr.number]"
-        f"([repr.number]{sum(ct_type.values()):,}[/repr.number])",
+        f"[b]#[/b]types=[repr.number]{type_total:,}[/repr.number]"
+        f" ([repr.number]{type_total-type_constructed:,}[/repr.number] existing,"
+        f" [repr.number]{type_constructed:,}[/repr.number] constructed in this run)",
     )
     print(
-        f"[b]#[/b]terms=[repr.number]{sum(tct_term.values()):,}[/repr.number]"
-        f"([repr.number]{sum(ct_term.values()):,}[/repr.number])",
+        f"[b]#[/b]terms=[repr.number]{term_total:,}[/repr.number]"
+        f" ([repr.number]{term_total-term_constructed:,}[/repr.number] existing,"
+        f" [repr.number]{term_constructed:,}[/repr.number] constructed in this run)",
     )
     print(
-        f"[b]#[/b]operators=[repr.number]{sum(tct_operator.values()):,}[/repr.number]"
-        f"([repr.number]{sum(ct_operator.values()):,}[/repr.number])",
+        f"[b]#[/b]operators=[repr.number]{op_total:,}[/repr.number]"
+        f" ([repr.number]{op_total-op_constructed:,}[/repr.number] existing,"
+        f" [repr.number]{op_constructed:,}[/repr.number] constructed in this run)",
     )
-    return tct_family, tct_type, tct_term, tct_operator
+    if basis_file and op_constructed:
+        print(f"Saved operators in {basis_file.basis_path}")
+    return basis, (tct_family, tct_type, tct_term, tct_operator)
 
 
-def verbose_main(  # noqa: C901
+def verbose_main(
     model: ir_model.Model,
     dimension: int,
     hc_flag: bool,
     gr_flag: bool,
-    basis_file: io_basis.BasisFile,
+    basis_file: Optional[io_basis.BasisFile] = None,
     select: Optional[list] = None,
     ignore: Optional[list] = None,
     overwrite: bool = False,
     threads: Optional[int] = None,
-) -> Tuple[Counter, Counter, Counter, Counter]:
+) -> Tuple[eft_basis.Basis, Tuple[Counter, Counter, Counter, Counter]]:
+    basis = eft_basis.Basis(model)
     ct_family, ct_type, ct_term, ct_operator = (
         Counter(),
         Counter(),
         Counter(),
         Counter(),
     )
     tct_family, tct_type, tct_term, tct_operator = (
@@ -381,15 +415,15 @@
     )
     tree_height = layout.render(autoeft.console, autoeft.console.options)[
         layout["tree"]
     ].region.height
     with rich.live.Live(layout, console=autoeft.console, transient=True) as live:
         for family in invariants.construct_families(dimension, hc_flag, gr_flag):
             layout["header"].update(rich.rule.Rule(family.tuple_repr()))
-            hc_mod = 1 if hc_flag or family.is_real() else 2
+            hc_mod_f = 1 if hc_flag or family.is_real() else 2
             hc_str = (
                 "" if hc_flag or family.is_real() else "[dim italic not bold] + h.c.[/]"
             )
             family_tree = eft_tree.add(
                 str(family) + hc_str,
                 style="bold",
                 highlight=True,
@@ -397,48 +431,55 @@
             render_family_tree = render_eft_tree.add(
                 str(family) + hc_str,
                 style="bold",
                 highlight=True,
             )
             render_family_tree.children = deque(maxlen=(tree_height - 2) // 3)
 
-            for op_type in invariants.construct_types(family, model):
-                operator_status.update(status_task, description=str(op_type) + hc_str)
+            for op_type in invariants.construct_types(family, model, hc_flag):
+                hc_mod_t = 1 if hc_flag or op_type.is_real() else 2
+                hc_str = (
+                    ""
+                    if hc_flag or op_type.is_real()
+                    else "[dim italic not bold] + h.c.[/]"
+                )
+                operator_status.update(status_task, description=str(op_type))
                 live.refresh()
-                op_stats = basis_file.get_operator_raw_numbers(op_type.full_path())
-                if op_stats:
-                    terms_per_type, operators_per_type = op_stats
-                    if terms_per_type:
-                        tct_family[family] = hc_mod
-                        tct_type[op_type] = hc_mod
-                        tct_term[op_type] = hc_mod * terms_per_type
-                        tct_operator[op_type] = hc_mod * operators_per_type
-                    if not overwrite:
-                        if tct_term[op_type]:
-                            type_tree = family_tree.add(str(op_type) + hc_str)
-                            type_tree.add(
-                                f"#terms={tct_term[op_type]}",
-                                style="not bold dim",
-                            )
-                            type_tree.add(
-                                f"#operators={tct_operator[op_type]}",
-                                style="not bold dim",
-                            )
-                            render_type_tree = render_family_tree.add(
-                                str(op_type) + hc_str,
-                            )
-                            render_type_tree.add(
-                                f"#terms={tct_term[op_type]}",
-                                style="not bold dim",
-                            )
-                            render_type_tree.add(
-                                f"#operators={tct_operator[op_type]}",
-                                style="not bold dim",
-                            )
-                        continue
+                if basis_file:
+                    op_stats = basis_file.get_operator_raw_numbers(op_type.full_path())
+                    if op_stats:
+                        terms_per_type, operators_per_type = op_stats
+                        if terms_per_type:
+                            tct_family[family] = hc_mod_f
+                            tct_type[op_type] = hc_mod_t
+                            tct_term[op_type] = hc_mod_t * terms_per_type
+                            tct_operator[op_type] = hc_mod_t * operators_per_type
+                        if not overwrite:
+                            if tct_term[op_type]:
+                                type_tree = family_tree.add(str(op_type) + hc_str)
+                                type_tree.add(
+                                    f"#terms={tct_term[op_type]}",
+                                    style="not bold dim",
+                                )
+                                type_tree.add(
+                                    f"#operators={tct_operator[op_type]}",
+                                    style="not bold dim",
+                                )
+                                render_type_tree = render_family_tree.add(
+                                    str(op_type) + hc_str,
+                                )
+                                render_type_tree.add(
+                                    f"#terms={tct_term[op_type]}",
+                                    style="not bold dim",
+                                )
+                                render_type_tree.add(
+                                    f"#operators={tct_operator[op_type]}",
+                                    style="not bold dim",
+                                )
+                            continue
                 if select and not utils.type_matches(op_type, select):
                     if tct_term[op_type]:
                         type_tree = family_tree.add(str(op_type) + hc_str)
                         type_tree.add(
                             f"#terms={tct_term[op_type]}",
                             style="not bold dim",
                         )
@@ -534,15 +575,15 @@
                             )
                             permutations_info.append(permutation_info)
                             terms_per_type += terms_per_symmetry
                             operators_per_type += operators_per_symmetry
                 if terms_per_type:
                     type_info = (
                         op_type.to_counter(),
-                        "real" if op_type.is_real(model) else "complex",
+                        "real" if op_type.is_real() else "complex",
                     )
                     generations_info = Counter(
                         {f.name: f.generations for f, _ in op_type},
                     )
                     invariants_info = {
                         model.symmetries.lorentz_group.name: list(
                             zip(lorentz_tableaux, itertools.repeat(1)),
@@ -559,24 +600,26 @@
                         type=type_info,
                         generations=generations_info,
                         n_terms=terms_per_type,
                         n_operators=operators_per_type,
                         invariants=invariants_info,
                         permutation_symmetries=permutations_info,
                     )
-                    basis_file.add_operator_info(operator_info)
+                    basis[repr(operator_info)] = operator_info
+                    if basis_file:
+                        basis_file.add_operator_info(operator_info)
                     print(repr(op_type), dest="log")
-                    ct_family[family] = hc_mod
-                    ct_type[op_type] = hc_mod
-                    ct_term[op_type] = hc_mod * terms_per_type
-                    ct_operator[op_type] = hc_mod * operators_per_type
-                    tct_family[family] = hc_mod
-                    tct_type[op_type] = hc_mod
-                    tct_term[op_type] = hc_mod * terms_per_type
-                    tct_operator[op_type] = hc_mod * operators_per_type
+                    ct_family[family] = hc_mod_f
+                    ct_type[op_type] = hc_mod_t
+                    ct_term[op_type] = hc_mod_t * terms_per_type
+                    ct_operator[op_type] = hc_mod_t * operators_per_type
+                    tct_family[family] = hc_mod_f
+                    tct_type[op_type] = hc_mod_t
+                    tct_term[op_type] = hc_mod_t * terms_per_type
+                    tct_operator[op_type] = hc_mod_t * operators_per_type
                     type_tree = family_tree.add(str(op_type) + hc_str)
                     type_tree.add(f"#terms={ct_term[op_type]}", style="not bold")
                     type_tree.add(
                         f"#operators={ct_operator[op_type]}",
                         style="not bold",
                     )
                     render_type_tree = render_family_tree.add(str(op_type) + hc_str)
@@ -584,43 +627,53 @@
                     render_type_tree.add(
                         f"#operators={ct_operator[op_type]}",
                         style="not bold",
                     )
         layout["header"].update(rich.rule.Rule())
     print(eft_tree)
     autoeft.console.rule()
+    fam_total, fam_constructed = sum(tct_family.values()), sum(ct_family.values())
+    type_total, type_constructed = sum(tct_type.values()), sum(ct_type.values())
+    term_total, term_constructed = sum(tct_term.values()), sum(ct_term.values())
+    op_total, op_constructed = sum(tct_operator.values()), sum(ct_operator.values())
     print(
-        f"[b]#[/b]families=[repr.number]{sum(tct_family.values()):,}[/repr.number]"
-        f"([repr.number]{sum(ct_family.values()):,}[/repr.number])",
+        f"[b]#[/b]families=[repr.number]{fam_total:,}[/repr.number]"
+        f" ([repr.number]{fam_total-fam_constructed:,}[/repr.number] existing,"
+        f" [repr.number]{fam_constructed:,}[/repr.number] constructed in this run)",
     )
     print(
-        f"[b]#[/b]types=[repr.number]{sum(tct_type.values()):,}[/repr.number]"
-        f"([repr.number]{sum(ct_type.values()):,}[/repr.number])",
+        f"[b]#[/b]types=[repr.number]{type_total:,}[/repr.number]"
+        f" ([repr.number]{type_total-type_constructed:,}[/repr.number] existing,"
+        f" [repr.number]{type_constructed:,}[/repr.number] constructed in this run)",
     )
     print(
-        f"[b]#[/b]terms=[repr.number]{sum(tct_term.values()):,}[/repr.number]"
-        f"([repr.number]{sum(ct_term.values()):,}[/repr.number])",
+        f"[b]#[/b]terms=[repr.number]{term_total:,}[/repr.number]"
+        f" ([repr.number]{term_total-term_constructed:,}[/repr.number] existing,"
+        f" [repr.number]{term_constructed:,}[/repr.number] constructed in this run)",
     )
     print(
-        f"[b]#[/b]operators=[repr.number]{sum(tct_operator.values()):,}[/repr.number]"
-        f"([repr.number]{sum(ct_operator.values()):,}[/repr.number])",
-    )
-    return tct_family, tct_type, tct_term, tct_operator
+        f"[b]#[/b]operators=[repr.number]{op_total:,}[/repr.number]"
+        f" ([repr.number]{op_total-op_constructed:,}[/repr.number] existing,"
+        f" [repr.number]{op_constructed:,}[/repr.number] constructed in this run)",
+    )
+    if basis_file and op_constructed:
+        print(f"Saved operators in {basis_file.basis_path}")
+    return basis, (tct_family, tct_type, tct_term, tct_operator)
 
 
 def dry_run(
     model: ir_model.Model,
     dimension: int,
     hc_flag: bool,
     gr_flag: bool,
     select: Optional[list] = None,
     ignore: Optional[list] = None,
 ):
     for family in invariants.construct_families(dimension, hc_flag, gr_flag):
-        for op_type in invariants.construct_types(family, model):
+        for op_type in invariants.construct_types(family, model, hc_flag):
             if select and not utils.type_matches(op_type, select):
                 continue
             if ignore and utils.type_matches(op_type, ignore):
                 continue
             yield op_type
 
 
@@ -632,15 +685,18 @@
             "\n"
             f"Please install FORM version {form_version_min} or higher."
         )
         raise exceptions.RequirementVersionError(errmsg)
     model_path = args.model.resolve()
     dimension = args.dimension
     output_path = args.output.resolve()
-    output_path /= f"{model_path.stem}-eft"
+    if args.name:
+        output_path /= args.name
+    else:
+        output_path /= f"{model_path.stem}-eft"
     generators.default_path = args.generators.resolve()
     try:
         with model_path.open("r") as model_file:
             model = ir_model.Model(**yaml.safe_load(model_file))
     except (FileNotFoundError, IsADirectoryError):
         errmsg = f"Model file not found {model_path}."
         print(errmsg)
@@ -690,47 +746,76 @@
             select,
             ignore,
         ):
             print(f"[bold white]{op_type}[/bold white]", dest="terminal")
             print(op_type, dest="log")
         return 0
 
+    if args.threads <= 0:
+        errmsg = f"Number of threads must be greater than 0, not '{args.threads}'."
+        print(errmsg)
+        return 1
+
     wd = output_path / ascii(dimension)
     wd.mkdir(parents=True, exist_ok=True)
     basis_path = wd / "basis"
     basis_file = io_basis.BasisFile(basis_path)
     if basis_file:
+        extra = basis_file.get_extra()
+        print(f"Existing operators found in {basis_path}")
+        print(f"Last run at {extra.timestamp}")
         existing_model = basis_file.get_model()
         if model != existing_model:
             errmsg = (
                 "Incompatible model files."
                 "\n"
                 f"The basis directory {basis_path} already exists"
                 " but it was created using a different model."
                 "\n"
                 "Please delete the existing basis directory"
-                " or provide the same model as before."
+                " or provide a different output path using"
+                " the --name or --output option."
             )
             print(errmsg)
             return 1
+        extra_diff = {
+            k: (v, vars(args)[k])
+            for k, v in extra.args.items()
+            if k in {"select", "ignore", "no_hc"} and v != vars(args)[k]
+        }
+        if extra_diff:
+            erropt = "\n".join(
+                f" - {option}: {prev} -> {curr}"
+                for option, (prev, curr) in extra_diff.items()
+            )
+            errmsg = (
+                "Incompatible options:"
+                f"\n{erropt}\n"
+                f"The basis directory {basis_path} already exists"
+                " but it was created using different options."
+                "\n"
+                "Please delete the existing basis directory"
+                " or provide a different output path using"
+                " the --name or --output option."
+            )
+            print(errmsg)
+            return 1
+        print()
     else:
         basis_file.set_model(model)
     basis_file.set_extra(output_path.name, dimension, args)
 
-    if args.threads <= 0:
-        errmsg = f"Number of threads must be greater than 0, not '{args.threads}'."
-        print(errmsg)
-        return 1
-
     print(
         f"Constructing operator basis for "
         f"[b]{rich.markup.escape(model.name)}[/b] @ [i]d={dimension}[/i]",
     )
+    if not hc_flag:
+        print("(Hermitian conjugation implied)")
     main_func = verbose_main if not args.quiet and args.verbose else plain_main
-    ct_family, ct_type, ct_term, ct_operator = main_func(
+    basis, (ct_family, ct_type, ct_term, ct_operator) = main_func(
         model,
         dimension,
         hc_flag,
         gr_flag,
         basis_file,
         select,
         ignore,
@@ -740,9 +825,8 @@
     stats = {}
     stats["n_families"] = int(sum(ct_family.values()))
     stats["n_types"] = int(sum(ct_type.values()))
     stats["n_terms"] = int(sum(ct_term.values()))
     stats["n_operators"] = int(sum(ct_operator.values()))
     stats_path = wd / "stats.yml"
     stats_path.write_text(yaml.safe_dump(stats, sort_keys=False))
-    print(f"Saved operators in {basis_file.basis_path}")
     return 0
```

### Comparing `autoeft-1.0.0rc0/autoeft/construction/permutation_symmetries.py` & `autoeft-1.0.1/autoeft/construction/permutation_symmetries.py`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/construction/symmetrizers.py` & `autoeft-1.0.1/autoeft/construction/symmetrizers.py`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/form/__init__.py` & `autoeft-1.0.1/autoeft/form/__init__.py`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/form/contract.py` & `autoeft-1.0.1/autoeft/form/contract.py`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/autoeft/io/basis.py` & `autoeft-1.0.1/autoeft/io/basis.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,14 +16,21 @@
 
 class MetaData(pydantic.BaseModel):
     timestamp: datetime.datetime
     eft_name: str
     dimension: int
     args: dict
 
+    @pydantic.validator("args")
+    def validate_args(cls, v):
+        for k in "model", "output", "generators":
+            if k in v:
+                v[k] = Path(v[k])
+        return v
+
 
 class BasisFile:
     basis_path: Path
     model_path: Path
     extra_path: Path
 
     def __init__(self, basis_path: Path):
@@ -67,15 +74,15 @@
 
     def set_extra(
         self,
         eft_name: str,
         dimension: int,
         args: argparse.Namespace,
     ):
-        exclude = {"main_func", "quiet", "verbose", "dry_run", "no_hc"}
+        exclude = {"main_func", "quiet", "verbose", "dry_run", "name"}
         args_dict = {k: v for k, v in vars(args).items() if k not in exclude}
         meta = MetaData.construct(
             timestamp=datetime.datetime.now().isoformat(timespec="seconds"),
             eft_name=eft_name,
             dimension=dimension,
             args=args_dict,
         )
@@ -90,15 +97,15 @@
         operator_path = self.basis_path / operator_info.path()
         operator_path.parent.mkdir(parents=True, exist_ok=True)
         data = (
             f"# '{operator_path.name}' generated by "
             f"{autoeft.program} {autoeft.version}\n"
         )
         data += operator_info.yaml()
-        tmp_operator_path = operator_path.with_stem("tmp")
+        tmp_operator_path = operator_path.with_suffix(".tmp")
         tmp_operator_path.write_text(data)
         tmp_operator_path.rename(operator_path)
 
     def get_operator_info(self, rel_path: Path) -> eft_basis.OperatorInfoPermutation:
         model = self.get_model()
         operator_path = self.basis_path / rel_path
         try:
```

### Comparing `autoeft-1.0.0rc0/autoeft/tex/main.py` & `autoeft-1.0.1/autoeft/tex/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -63,14 +63,15 @@
         return 1
     output_path = args.output.resolve()
     output_path /= f"{metadata.eft_name}"
     output_path /= ascii(metadata.dimension)
     output_path.mkdir(parents=True, exist_ok=True)
     operators_path = output_path / "operators"
     operators_path.mkdir(exist_ok=True)
+    hc_flag = not metadata.args["no_hc"]
     try:
         select = (
             [yaml.safe_load(s.replace(":", ": ")) for s in args.select]
             if args.select
             else None
         )
         ignore = (
@@ -114,29 +115,40 @@
     for op_info in basis.values():
         if select and not utils.type_matches(op_info.op_type, select):
             continue
         if ignore and utils.type_matches(op_info.op_type, ignore):
             continue
         op_type = op_info.op_type
         family = op_type.family
-        tex_family = tex(family) if family.is_normal() else tex(family.conjugated())
-        if family.is_complex():
-            tex_family += r" + \hc"
-            families[tex_family] = 2
-        else:
+        if hc_flag:
+            tex_family = tex(family)
+            tex_type = tex(op_type)
+            hilbert_series[tex_type] = op_info.n_operators
             families[tex_family] = 1
-        types[tex_family] += 1
-        terms[tex_family] += op_info.n_terms
-        operators[tex_family] += op_info.n_operators
-        hilbert_series[tex(op_type)] = op_info.n_operators
+            types[tex_family] += 1
+            terms[tex_family] += op_info.n_terms
+            operators[tex_family] += op_info.n_operators
+        else:
+            tex_family = tex(family)
+            tex_type = tex(op_type)
+            hilbert_series[tex_type] = op_info.n_operators
+            hc_mod = 2 if op_type.is_complex() else 1
+            if family.is_complex():
+                tex_family += r" + \hc"
+                families[tex_family] = 2
+            else:
+                families[tex_family] = 1
+            types[tex_family] += 1 * hc_mod
+            terms[tex_family] += op_info.n_terms * hc_mod
+            operators[tex_family] += op_info.n_operators * hc_mod
         operator_path = operators_path / f"{op_type.path('tex')}"
         produce_texfile(
             operator_path,
             [
-                rf"\subsection{{\texorpdfstring{{${tex(op_info.op_type)}$}}"
+                rf"\subsection{{\texorpdfstring{{${tex(op_type)}$}}"
                 f"{{{op_info.op_type!s}}}}}",
                 tex(op_info),
             ],
         )
         operator_files.append(rf"\input{{operators/{operator_path.stem}}}")
     produce_texfile(
         output_path / "header.tex",
@@ -148,15 +160,15 @@
     )
     produce_texfile(
         output_path / "numbers_table.tex",
         tex_table(families, types, terms, operators),
     )
     produce_texfile(
         output_path / "hilbert_series.tex",
-        tex_series(hilbert_series, metadata.dimension),
+        tex_series(hilbert_series, metadata.dimension, not hc_flag),
     )
     produce_texfile(
         output_path / "operators.tex",
         [tensor_product, *operator_files],
     )
     if texfile_path.is_file():
         if not (output_path / "main.tex").is_file():
@@ -208,21 +220,27 @@
         rf"{sum(families.values())} & {sum(types.values())}"
         rf" & {sum(terms.values())} & {sum(operators.values())} \\"
     )
     yield r"\bottomrule"
     yield r"\end{longtable}"
 
 
-def tex_series(hilbert_series: Count[str], dimension: int) -> Iterator[str]:
+def tex_series(
+    hilbert_series: Count[str],
+    dimension: int,
+    add_hc: bool = False,
+) -> Iterator[str]:
     yield r"\begin{align*}"
     yield r"\begin{autobreak}"
     yield rf"\hat{{H}}_{{{dimension}}} = "
     yield "  " + "\n+ ".join(
         rf"{co}\,{op}" if co > 1 else op for op, co in hilbert_series.items()
     )
+    if add_hc:
+        yield r"  + \hc"
     yield r"\end{autobreak}"
     yield r"\end{align*}"
 
 
 def produce_texfile(path: Path, content: Iterable):
     disclaimer = f"% '{path.name}' generated by {autoeft.program} {autoeft.version}\n"
     path.write_text(disclaimer + "\n".join(content))
```

### Comparing `autoeft-1.0.0rc0/models/README.md` & `autoeft-1.0.1/models/README.md`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/models/all-left_sm.yml` & `autoeft-1.0.1/models/all-left_sm.yml`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/models/bno_nf1_sm.yml` & `autoeft-1.0.1/models/bno_nf1_sm.yml`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/models/bno_sm.yml` & `autoeft-1.0.1/models/bno_sm.yml`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/models/dynkin_sm.yml` & `autoeft-1.0.1/models/dynkin_sm.yml`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/models/grsm.yml` & `autoeft-1.0.1/models/grsm.yml`

 * *Files 2% similar despite different names*

```diff
@@ -76,7 +76,8 @@
       SU2: [1]
       U1: 1/2
     tex: H
   CL:
     representations:
       Lorentz: -2
     tex: C_{\mathrm{L}}
+    tex_hc: C_{\mathrm{R}}
```

### Comparing `autoeft-1.0.0rc0/models/mfv-sm.yml` & `autoeft-1.0.1/models/bsm/lqc2+sm.yml`

 * *Files 15% similar despite different names*

```diff
@@ -1,36 +1,26 @@
 # AutoEFT model file
-name: MVF-SMEFT
-description: Minimal Flavor Violation Standard Model Effective Field Theory
+name: LQC2+SMEFT
+description: Lepto-Quark chi2 + Standard Model Effective Field Theory
 
 symmetries:
   lorentz_group:
     tex: SO^+(1,3)
   sun_groups:
     SU3:
       N: 3
       tex: SU(3)
       indices: [a,b,c,d,e,f,g,h]
     SU2:
       N: 2
       tex: SU(2)
       indices: [i,j,k,l,m,n,p,q]
-    q3: {N: 3}
-    u3: {N: 3}
-    d3: {N: 3}
-    l3: {N: 3}
-    e3: {N: 3}
   u1_groups:
     U1:
       tex: U(1)
-    q1: {}
-    u1: {}
-    d1: {}
-    l1: {}
-    e1: {}
 
 fields:
   GL:
     representations:
       Lorentz: -1
       SU3: [2,1]
     tex: G_{\mathrm{L}}
@@ -48,46 +38,49 @@
     tex_hc: B_{\mathrm{R}}
   QL:
     representations:
       Lorentz: -1/2
       SU3: [1]
       SU2: [1]
       U1: 1/6
-      q3: [1]
-      q1: 1
+    generations: 3
     tex: Q_{\mathrm{L}}
   uR:
     representations:
       Lorentz: 1/2
       SU3: [1]
       U1: 2/3
-      u3: [1]
-      u1: 1
+    generations: 3
     tex: u_{\mathrm{R}}
   dR:
     representations:
       Lorentz: 1/2
       SU3: [1]
       U1: -1/3
-      d3: [1]
-      d1: 1
+    generations: 3
     tex: d_{\mathrm{R}}
   LL:
     representations:
       Lorentz: -1/2
       SU2: [1]
       U1: -1/2
-      l3: [1]
-      l1: 1
+    generations: 3
     tex: L_{\mathrm{L}}
   eR:
     representations:
       Lorentz: 1/2
       U1: -1
-      e3: [1]
-      e1: 1
+    generations: 3
     tex: e_{\mathrm{R}}
   H:
     representations:
       SU2: [1]
       U1: 1/2
     tex: H
+
+  # BSM
+  chi2:
+    representations:
+      SU3: [1]
+      SU2: [1]
+      U1: 7/6
+    tex: \chi_2
```

### Comparing `autoeft-1.0.0rc0/models/nf1_sm.yml` & `autoeft-1.0.1/models/nf1_sm.yml`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/models/sm.yml` & `autoeft-1.0.1/models/sm.yml`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/models/bsm/cqs+sm.yml` & `autoeft-1.0.1/models/bsm/cqs+sm.yml`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/models/bsm/cts+sm.yml` & `autoeft-1.0.1/models/bsm/cts+sm.yml`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/models/bsm/dcs+sm.yml` & `autoeft-1.0.1/models/bsm/dcs+sm.yml`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/models/bsm/lqc1+sm.yml` & `autoeft-1.0.1/models/bsm/lqc1+sm.yml`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/models/bsm/lqc2+sm.yml` & `autoeft-1.0.1/models/bsm/lqp2+sm.yml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # AutoEFT model file
-name: LQC2+SMEFT
-description: Lepto-Quark chi2 + Standard Model Effective Field Theory
+name: LQP2+SMEFT
+description: Lepto-Quark phi2 + Standard Model Effective Field Theory
 
 symmetries:
   lorentz_group:
     tex: SO^+(1,3)
   sun_groups:
     SU3:
       N: 3
@@ -74,13 +74,12 @@
   H:
     representations:
       SU2: [1]
       U1: 1/2
     tex: H
 
   # BSM
-  chi2:
+  phi2:
     representations:
       SU3: [1]
-      SU2: [1]
-      U1: 7/6
-    tex: \chi_2
+      U1: -1/3
+    tex: \phi_2
```

### Comparing `autoeft-1.0.0rc0/models/bsm/lqp1+sm.yml` & `autoeft-1.0.1/models/bsm/lqp1+sm.yml`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/models/bsm/lqp2+sm.yml` & `autoeft-1.0.1/models/bsm/scs+sm.yml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # AutoEFT model file
-name: LQP2+SMEFT
-description: Lepto-Quark phi2 + Standard Model Effective Field Theory
+name: SCS+SMEFT
+description: Singly Charged Scalar + Standard Model Effective Field Theory
 
 symmetries:
   lorentz_group:
     tex: SO^+(1,3)
   sun_groups:
     SU3:
       N: 3
@@ -74,12 +74,11 @@
   H:
     representations:
       SU2: [1]
       U1: 1/2
     tex: H
 
   # BSM
-  phi2:
+  del:
     representations:
-      SU3: [1]
-      U1: -1/3
-    tex: \phi_2
+      U1: 1
+    tex: \delta^+
```

### Comparing `autoeft-1.0.0rc0/models/bsm/ltf+sm.yml` & `autoeft-1.0.1/models/bsm/ltf+sm.yml`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/models/bsm/scs+sm.yml` & `autoeft-1.0.1/models/bsm/u1-u1-sm.yml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # AutoEFT model file
-name: SCS+SMEFT
-description: Singly Charged Scalar + Standard Model Effective Field Theory
+name: U(1)-U(1)-SMEFT
+description: U(1)' x U(1)'' extended Standard Model Effective Field Theory
 
 symmetries:
   lorentz_group:
     tex: SO^+(1,3)
   sun_groups:
     SU3:
       N: 3
@@ -13,14 +13,20 @@
     SU2:
       N: 2
       tex: SU(2)
       indices: [i,j,k,l,m,n,p,q]
   u1_groups:
     U1:
       tex: U(1)
+    U1p:
+      tex: U(1)^\prime
+    U1pp:
+      tex: U(1)^{\prime\prime}
+    Bno: {}
+    Lno: {}
 
 fields:
   GL:
     representations:
       Lorentz: -1
       SU3: [2,1]
     tex: G_{\mathrm{L}}
@@ -32,53 +38,62 @@
     tex: W_{\mathrm{L}}
     tex_hc: W_{\mathrm{R}}
   BL:
     representations:
       Lorentz: -1
     tex: B_{\mathrm{L}}
     tex_hc: B_{\mathrm{R}}
+  XL:
+    representations:
+      Lorentz: -1
+    tex: X_{\mathrm{L}}
+    tex_hc: X_{\mathrm{R}}
+  YL:
+    representations:
+      Lorentz: -1
+    tex: Y_{\mathrm{L}}
+    tex_hc: Y_{\mathrm{R}}
   QL:
     representations:
       Lorentz: -1/2
       SU3: [1]
       SU2: [1]
       U1: 1/6
+      Bno: 1/3
     generations: 3
     tex: Q_{\mathrm{L}}
   uR:
     representations:
       Lorentz: 1/2
       SU3: [1]
       U1: 2/3
+      Bno: 1/3
     generations: 3
     tex: u_{\mathrm{R}}
   dR:
     representations:
       Lorentz: 1/2
       SU3: [1]
       U1: -1/3
+      Bno: 1/3
     generations: 3
     tex: d_{\mathrm{R}}
   LL:
     representations:
       Lorentz: -1/2
       SU2: [1]
       U1: -1/2
+      Lno: -1
     generations: 3
     tex: L_{\mathrm{L}}
   eR:
     representations:
       Lorentz: 1/2
       U1: -1
+      Lno: -1
     generations: 3
     tex: e_{\mathrm{R}}
   H:
     representations:
       SU2: [1]
       U1: 1/2
     tex: H
-
-  # BSM
-  del:
-    representations:
-      U1: 1
-    tex: \delta^+
```

### Comparing `autoeft-1.0.0rc0/models/bsm/u1-u1-sm.yml` & `autoeft-1.0.1/models/all-left_grsm.yml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # AutoEFT model file
-name: U(1)-U(1)-SMEFT
-description: U(1)' x U(1)'' extended Standard Model Effective Field Theory
+name: GRSMEFT
+description: Gravitational Interactions + Standard Model Effective Field Theory in the all-left chirality convention
 
 symmetries:
   lorentz_group:
     tex: SO^+(1,3)
   sun_groups:
     SU3:
       N: 3
@@ -13,20 +13,14 @@
     SU2:
       N: 2
       tex: SU(2)
       indices: [i,j,k,l,m,n,p,q]
   u1_groups:
     U1:
       tex: U(1)
-    U1p:
-      tex: U(1)^\prime
-    U1pp:
-      tex: U(1)^{\prime\prime}
-    Bno: {}
-    Lno: {}
 
 fields:
   GL:
     representations:
       Lorentz: -1
       SU3: [2,1]
     tex: G_{\mathrm{L}}
@@ -38,62 +32,52 @@
     tex: W_{\mathrm{L}}
     tex_hc: W_{\mathrm{R}}
   BL:
     representations:
       Lorentz: -1
     tex: B_{\mathrm{L}}
     tex_hc: B_{\mathrm{R}}
-  XL:
-    representations:
-      Lorentz: -1
-    tex: X_{\mathrm{L}}
-    tex_hc: X_{\mathrm{R}}
-  YL:
-    representations:
-      Lorentz: -1
-    tex: Y_{\mathrm{L}}
-    tex_hc: Y_{\mathrm{R}}
-  QL:
+  Q:
     representations:
       Lorentz: -1/2
       SU3: [1]
       SU2: [1]
       U1: 1/6
-      Bno: 1/3
     generations: 3
-    tex: Q_{\mathrm{L}}
-  uR:
+    tex: Q
+  uC:
     representations:
-      Lorentz: 1/2
-      SU3: [1]
-      U1: 2/3
-      Bno: 1/3
+      Lorentz: -1/2
+      SU3: [1,1]
+      U1: -2/3
     generations: 3
-    tex: u_{\mathrm{R}}
-  dR:
+    tex: u_{\mathbb{C}}
+  dC:
     representations:
-      Lorentz: 1/2
-      SU3: [1]
-      U1: -1/3
-      Bno: 1/3
+      Lorentz: -1/2
+      SU3: [1,1]
+      U1: 1/3
     generations: 3
-    tex: d_{\mathrm{R}}
-  LL:
+    tex: d_{\mathbb{C}}
+  L:
     representations:
       Lorentz: -1/2
       SU2: [1]
       U1: -1/2
-      Lno: -1
     generations: 3
-    tex: L_{\mathrm{L}}
-  eR:
+    tex: L
+  eC:
     representations:
-      Lorentz: 1/2
-      U1: -1
-      Lno: -1
+      Lorentz: -1/2
+      U1: 1
     generations: 3
-    tex: e_{\mathrm{R}}
+    tex: e_{\mathbb{C}}
   H:
     representations:
       SU2: [1]
       U1: 1/2
     tex: H
+  CL:
+    representations:
+      Lorentz: -2
+    tex: C_{\mathrm{L}}
+    tex_hc: C_{\mathrm{R}}
```

### Comparing `autoeft-1.0.0rc0/models/bsm/vll+sm.yml` & `autoeft-1.0.1/models/bsm/vll+sm.yml`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/resources/theme.ini` & `autoeft-1.0.1/resources/theme.ini`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/resources/tex/main.tex` & `autoeft-1.0.1/resources/tex/main.tex`

 * *Files identical despite different names*

### Comparing `autoeft-1.0.0rc0/.gitignore` & `autoeft-1.0.1/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 *.so
 
 # Distribution / packaging
 .Python
 build/
 develop-eggs/
 dist/
+dist-*/
 downloads/
 eggs/
 .eggs/
 lib/
 lib64/
 parts/
 sdist/
@@ -153,8 +154,8 @@
 cython_debug/
 
 # PyCharm
 #  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
-.idea/
+.idea/
```

### Comparing `autoeft-1.0.0rc0/LICENSE` & `autoeft-1.0.1/LICENSE`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Robert V. Harlander and Magnus C. Schaaf
+Copyright (c) 2023, 2024 Robert V. Harlander and Magnus C. Schaaf
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `autoeft-1.0.0rc0/PyPI_README.md` & `autoeft-1.0.1/PyPI_README.md`

 * *Files 14% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 
 Automated operator construction for effective field theories.
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
 [![Hatch project](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg)](https://github.com/pypa/hatch)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+[![PyPI - Version](https://img.shields.io/pypi/v/autoeft)](https://pypi.org/project/autoeft/)
+[![Conda (channel only)](https://img.shields.io/conda/vn/conda-forge/autoeft)](https://anaconda.org/conda-forge/autoeft)
 
 ## Installation
 AutoEFT is available on the [Python Package Index (PyPI)](https://pypi.org/) and the [conda-forge](https://conda-forge.org/) channel.
 
 ### Requirements
 - [Python](https://www.python.org/) >= 3.8
 - [SageMath](https://www.sagemath.org/) >= 9.3
@@ -23,14 +25,15 @@
 To install *autoeft* and its dependencies, run:
 ```shell
 sage -pip install autoeft
 ```
 
 On *macOS* using [Homebrew](https://brew.sh/), it may be necessary to precede this statement by `PYTHONEXECUTABLE=</path/to/sage>` with the proper path to the SageMath executable inserted.
 In addition, it may be necessary to add the path to SageMath’s executables to the `$PATH` environment variable.
+See also [here](https://gitlab.com/auto_eft/autoeft/-/issues?label_name=installation) for a collection of potential installation issues.
 
 ### Installing AutoEFT from conda-forge
 To install *autoeft* and its dependencies, run:
 - with [conda](https://conda.io/):
 ```shell
 conda install autoeft -c conda-forge
 ```
@@ -49,14 +52,18 @@
 ```
 
 ## Usage
 Verify the installation by running:
 ```shell
 autoeft --help
 ```
+and
+```shell
+autoeft check
+```
 
 ### Model Files
 The *model file* defines the symmetry groups and field content of a low-energy theory in the [YAML](https://yaml.org/) format.
 To produce a sample *model file*, run:
 ```shell
 autoeft sample-model > sm.yml
 ```
@@ -103,19 +110,26 @@
 print(model)
 # SMEFT: Standard Model Effective Field Theory
 
 LQQQ = basis[{"LL": 1, "QL": 3}]
 print(LQQQ)
 # LL (1) QL(3)
 
-print(LQQQ.n_terms , LQQQ.n_operators , sep=" & ")
+print(LQQQ.n_terms, LQQQ.n_operators, sep=" & ")
 # 3 & 57
 ```
 
 ## Authors
-- Robert V. Harlander (RWTH Aachen University)
-- Magnus C. Schaaf (RWTH Aachen University)
+- **Robert V. Harlander** (_RWTH Aachen University_)
+- **Magnus C. Schaaf** (_RWTH Aachen University_)
 
 ## Cite
-If you use AutoEFT in your project, please refer to:
-- <!DOCTYPE html> <html> <body> <p><b> <a href="https://inspirehep.net/literature/2658915"> Standard model effective field theory up to mass dimension 12 </a> </b></p>  <p><a href="https://inspirehep.net/authors/1006678">R.V. Harlander</a> (<a href="https://inspirehep.net/institutions/910724">RWTH Aachen U.</a>), <a href="https://inspirehep.net/authors/2658916">T. Kempkens</a> (<a href="https://inspirehep.net/institutions/910724">RWTH Aachen U.</a>), <a href="https://inspirehep.net/authors/2658917">M.C. Schaaf</a> (<a href="https://inspirehep.net/institutions/910724">RWTH Aachen U.</a>)</p>  <p> e-Print: <a href="https://arxiv.org/abs/2305.06832"> 2305.06832 </a>[hep-ph]</p> <p> DOI: <a href="https://doi.org/10.1103/PhysRevD.108.055020"> 10.1103/PhysRevD.108.055020 </a>(publication) </p> <p> Published in:<span> Phys.Rev.D 108 (2023) 5, 055020</span></p> <br> </body> </html>
+- [**Standard model effective field theory up to mass dimension 12**](https://inspirehep.net/literature/2658915)  
+R.V. Harlander, T. Kempkens, M.C. Schaaf  
+[_Phys. Rev. D_ **108** (2023) 055020](https://doi.org/10.1103/PhysRevD.108.055020),
+[arXiv:2305.06832 [hep-ph]](https://arxiv.org/abs/2305.06832)
+
+- [**AutoEFT: Automated operator construction for effective field theories**](https://inspirehep.net/literature/2703514)  
+R.V. Harlander, M.C. Schaaf  
+[_Comput. Phys. Commun._ **300** (2024) 109198](https://doi.org/10.1016/j.cpc.2024.109198),
+[arXiv:2309.15783 [hep-ph]](https://arxiv.org/abs/2309.15783)
 ---
```

### Comparing `autoeft-1.0.0rc0/pyproject.toml` & `autoeft-1.0.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "autoeft"
-version = "1.0.0rc0"
+version = "1.0.1"
 description = "Automated operator construction for effective field theories."
 readme = "PyPI_README.md"
 requires-python = ">=3.8"
-license = "MIT"
-license-files = { paths = ["LICENSE"] }
+license.file = "LICENSE"
 authors = [
     { name="Robert V. Harlander", email="harlander@physik.rwth-aachen.de" },
     { name="Magnus C. Schaaf", email="magnus.schaaf@rwth-aachen.de" },
 ]
 maintainers = [
     { name="Magnus C. Schaaf", email="magnus.schaaf@rwth-aachen.de" },
 ]
@@ -80,14 +79,17 @@
 
 [tool.hatch.envs.docs]
 extra-dependencies = [
     "sphinx",
 ]
 
 [tool.ruff]
+namespace-packages = ["tests/*"]
+
+[tool.ruff.lint]
 select = [
     "F",      # Pyflakes
     "E","W",  # pycodestyle
     "C90",    # mccabe
     "I",      # isort
     "D",      # pydocstyle
     "UP",     # pyupgrade
@@ -142,22 +144,21 @@
 ]
 unfixable = [
     "F401",      # unused-import
     "F841",      # unused-variable
     "E731",      # lambda-assignment
     "ERA001",    # commented out code
 ]
-namespace-packages = ["tests/*"]
 
-[tool.ruff.isort]
+[tool.ruff.lint.isort]
 force-single-line = true
 
-[tool.ruff.pydocstyle]
+[tool.ruff.lint.pydocstyle]
 convention = "google"
 
-[tool.ruff.mccabe]
-max-complexity = 15
+[tool.ruff.lint.mccabe]
+max-complexity = 20
 
 [tool.pytest.ini_options]
 addopts = [
     "--import-mode=importlib",
 ]
```

### Comparing `autoeft-1.0.0rc0/PKG-INFO` & `autoeft-1.0.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,35 @@
 Metadata-Version: 2.1
 Name: autoeft
-Version: 1.0.0rc0
+Version: 1.0.1
 Summary: Automated operator construction for effective field theories.
 Project-URL: Homepage, https://gitlab.com/auto_eft/autoeft
 Author-email: "Robert V. Harlander" <harlander@physik.rwth-aachen.de>, "Magnus C. Schaaf" <magnus.schaaf@rwth-aachen.de>
 Maintainer-email: "Magnus C. Schaaf" <magnus.schaaf@rwth-aachen.de>
-License-Expression: MIT
+License: MIT License
+        
+        Copyright (c) 2023, 2024 Robert V. Harlander and Magnus C. Schaaf
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
 License-File: LICENSE
 Keywords: basis,eft,hep,operators,physics,qft
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix
@@ -36,14 +56,16 @@
 
 Automated operator construction for effective field theories.
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
 [![Hatch project](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg)](https://github.com/pypa/hatch)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+[![PyPI - Version](https://img.shields.io/pypi/v/autoeft)](https://pypi.org/project/autoeft/)
+[![Conda (channel only)](https://img.shields.io/conda/vn/conda-forge/autoeft)](https://anaconda.org/conda-forge/autoeft)
 
 ## Installation
 AutoEFT is available on the [Python Package Index (PyPI)](https://pypi.org/) and the [conda-forge](https://conda-forge.org/) channel.
 
 ### Requirements
 - [Python](https://www.python.org/) >= 3.8
 - [SageMath](https://www.sagemath.org/) >= 9.3
@@ -55,14 +77,15 @@
 To install *autoeft* and its dependencies, run:
 ```shell
 sage -pip install autoeft
 ```
 
 On *macOS* using [Homebrew](https://brew.sh/), it may be necessary to precede this statement by `PYTHONEXECUTABLE=</path/to/sage>` with the proper path to the SageMath executable inserted.
 In addition, it may be necessary to add the path to SageMath’s executables to the `$PATH` environment variable.
+See also [here](https://gitlab.com/auto_eft/autoeft/-/issues?label_name=installation) for a collection of potential installation issues.
 
 ### Installing AutoEFT from conda-forge
 To install *autoeft* and its dependencies, run:
 - with [conda](https://conda.io/):
 ```shell
 conda install autoeft -c conda-forge
 ```
@@ -81,14 +104,18 @@
 ```
 
 ## Usage
 Verify the installation by running:
 ```shell
 autoeft --help
 ```
+and
+```shell
+autoeft check
+```
 
 ### Model Files
 The *model file* defines the symmetry groups and field content of a low-energy theory in the [YAML](https://yaml.org/) format.
 To produce a sample *model file*, run:
 ```shell
 autoeft sample-model > sm.yml
 ```
@@ -135,19 +162,26 @@
 print(model)
 # SMEFT: Standard Model Effective Field Theory
 
 LQQQ = basis[{"LL": 1, "QL": 3}]
 print(LQQQ)
 # LL (1) QL(3)
 
-print(LQQQ.n_terms , LQQQ.n_operators , sep=" & ")
+print(LQQQ.n_terms, LQQQ.n_operators, sep=" & ")
 # 3 & 57
 ```
 
 ## Authors
-- Robert V. Harlander (RWTH Aachen University)
-- Magnus C. Schaaf (RWTH Aachen University)
+- **Robert V. Harlander** (_RWTH Aachen University_)
+- **Magnus C. Schaaf** (_RWTH Aachen University_)
 
 ## Cite
-If you use AutoEFT in your project, please refer to:
-- <!DOCTYPE html> <html> <body> <p><b> <a href="https://inspirehep.net/literature/2658915"> Standard model effective field theory up to mass dimension 12 </a> </b></p>  <p><a href="https://inspirehep.net/authors/1006678">R.V. Harlander</a> (<a href="https://inspirehep.net/institutions/910724">RWTH Aachen U.</a>), <a href="https://inspirehep.net/authors/2658916">T. Kempkens</a> (<a href="https://inspirehep.net/institutions/910724">RWTH Aachen U.</a>), <a href="https://inspirehep.net/authors/2658917">M.C. Schaaf</a> (<a href="https://inspirehep.net/institutions/910724">RWTH Aachen U.</a>)</p>  <p> e-Print: <a href="https://arxiv.org/abs/2305.06832"> 2305.06832 </a>[hep-ph]</p> <p> DOI: <a href="https://doi.org/10.1103/PhysRevD.108.055020"> 10.1103/PhysRevD.108.055020 </a>(publication) </p> <p> Published in:<span> Phys.Rev.D 108 (2023) 5, 055020</span></p> <br> </body> </html>
+- [**Standard model effective field theory up to mass dimension 12**](https://inspirehep.net/literature/2658915)  
+R.V. Harlander, T. Kempkens, M.C. Schaaf  
+[_Phys. Rev. D_ **108** (2023) 055020](https://doi.org/10.1103/PhysRevD.108.055020),
+[arXiv:2305.06832 [hep-ph]](https://arxiv.org/abs/2305.06832)
+
+- [**AutoEFT: Automated operator construction for effective field theories**](https://inspirehep.net/literature/2703514)  
+R.V. Harlander, M.C. Schaaf  
+[_Comput. Phys. Commun._ **300** (2024) 109198](https://doi.org/10.1016/j.cpc.2024.109198),
+[arXiv:2309.15783 [hep-ph]](https://arxiv.org/abs/2309.15783)
 ---
```

