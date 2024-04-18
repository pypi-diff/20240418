# Comparing `tmp/masspds2024-0.0.3.tar.gz` & `tmp/masspds2024-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "masspds2024-0.0.3.tar", last modified: Sat Apr 13 06:22:14 2024, max compression
+gzip compressed data, was "masspds2024-0.0.4.tar", last modified: Thu Apr 18 12:37:34 2024, max compression
```

## Comparing `masspds2024-0.0.3.tar` & `masspds2024-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-13 06:22:14.884133 masspds2024-0.0.3/
--rw-rw-rw-   0        0        0     1077 2024-04-13 04:56:25.000000 masspds2024-0.0.3/LICENSE.txt
--rw-rw-rw-   0        0        0      589 2024-04-13 06:22:14.884133 masspds2024-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       79 2024-04-13 04:55:53.000000 masspds2024-0.0.3/README.md
--rw-rw-rw-   0        0        0       86 2024-04-13 04:55:16.000000 masspds2024-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0      707 2024-04-13 06:22:14.886190 masspds2024-0.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-13 06:22:14.860126 masspds2024-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2024-04-13 06:22:14.876123 masspds2024-0.0.3/src/masspds2024/
--rw-rw-rw-   0        0        0        0 2024-04-13 04:33:04.000000 masspds2024-0.0.3/src/masspds2024/__init__.py
--rw-rw-rw-   0        0        0     3483 2024-04-13 06:09:59.000000 masspds2024-0.0.3/src/masspds2024/data_generation.py
-drwxrwxrwx   0        0        0        0 2024-04-13 06:22:14.883123 masspds2024-0.0.3/src/masspds2024.egg-info/
--rw-rw-rw-   0        0        0      589 2024-04-13 06:22:14.000000 masspds2024-0.0.3/src/masspds2024.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      265 2024-04-13 06:22:14.000000 masspds2024-0.0.3/src/masspds2024.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-13 06:22:14.000000 masspds2024-0.0.3/src/masspds2024.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-04-13 06:22:14.000000 masspds2024-0.0.3/src/masspds2024.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-18 12:37:34.866117 masspds2024-0.0.4/
+-rw-rw-rw-   0        0        0     1077 2024-04-13 04:56:25.000000 masspds2024-0.0.4/LICENSE.txt
+-rw-rw-rw-   0        0        0      589 2024-04-18 12:37:34.866117 masspds2024-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       79 2024-04-13 04:55:53.000000 masspds2024-0.0.4/README.md
+-rw-rw-rw-   0        0        0       86 2024-04-13 04:55:16.000000 masspds2024-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0      707 2024-04-18 12:37:34.867116 masspds2024-0.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-18 12:37:34.850747 masspds2024-0.0.4/src/
+drwxrwxrwx   0        0        0        0 2024-04-18 12:37:34.859158 masspds2024-0.0.4/src/masspds2024/
+-rw-rw-rw-   0        0        0        0 2024-04-13 04:33:04.000000 masspds2024-0.0.4/src/masspds2024/__init__.py
+-rw-rw-rw-   0        0        0     4342 2024-04-18 12:35:17.000000 masspds2024-0.0.4/src/masspds2024/data.py
+drwxrwxrwx   0        0        0        0 2024-04-18 12:37:34.865117 masspds2024-0.0.4/src/masspds2024.egg-info/
+-rw-rw-rw-   0        0        0      589 2024-04-18 12:37:34.000000 masspds2024-0.0.4/src/masspds2024.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      254 2024-04-18 12:37:34.000000 masspds2024-0.0.4/src/masspds2024.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 12:37:34.000000 masspds2024-0.0.4/src/masspds2024.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-04-18 12:37:34.000000 masspds2024-0.0.4/src/masspds2024.egg-info/top_level.txt
```

### Comparing `masspds2024-0.0.3/LICENSE.txt` & `masspds2024-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `masspds2024-0.0.3/PKG-INFO` & `masspds2024-0.0.4/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: masspds2024
-Version: 0.0.3
+Version: 0.0.4
 Summary: Package contains useful commands for mentee MaSSP DS 2024
 Home-page: https://github/
 Author: MaSSP Mathematics and Computer Science 2024
 Author-email: nghi08122003@gmail.com
 Project-URL: repository, https://github/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `masspds2024-0.0.3/setup.cfg` & `masspds2024-0.0.4/setup.cfg`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206d 6173 7370 6473 3230 3234 0d0a   = masspds2024..
-00000020: 7665 7273 696f 6e20 3d20 302e 302e 330d  version = 0.0.3.
+00000020: 7665 7273 696f 6e20 3d20 302e 302e 340d  version = 0.0.4.
 00000030: 0a61 7574 686f 7220 3d20 4d61 5353 5020  .author = MaSSP 
 00000040: 4d61 7468 656d 6174 6963 7320 616e 6420  Mathematics and 
 00000050: 436f 6d70 7574 6572 2053 6369 656e 6365  Computer Science
 00000060: 2032 3032 340d 0a61 7574 686f 725f 656d   2024..author_em
 00000070: 6169 6c20 3d20 6e67 6869 3038 3132 3230  ail = nghi081220
 00000080: 3033 4067 6d61 696c 2e63 6f6d 0d0a 6465  03@gmail.com..de
 00000090: 7363 7269 7074 696f 6e20 3d20 5061 636b  scription = Pack
```

### Comparing `masspds2024-0.0.3/src/masspds2024/data_generation.py` & `masspds2024-0.0.4/src/masspds2024/data.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,91 +1,114 @@
 import numpy as np
 import pandas as pd
 import matplotlib.pyplot as plt
 import requests
 import random
 
-def CAE_generator(n_student = 100000, random_seed = 1):
-    np.random.seed(random_seed)
-    if (n_student < 1000 or n_student > 100000):
-        raise Exception("n_student have to greater than 1000 and smaller than 100000!")
-    p_top = 0.05
-    p_bot = 0.95
-    p = []
-    temp_p = np.linspace(p_top, p_bot, 40)
-    np.random.shuffle(temp_p)
-    for i in range(40):
-        p.append((i, temp_p[i]))
-    temp_p = np.linspace(p_top, p_bot, 30)
-    np.random.shuffle(temp_p)
-    for i in range(30):
-        p.append((i+40, temp_p[i]))
-    temp_p = np.linspace(p_top, p_bot, 50)
-    np.random.shuffle(temp_p)
-    for i in range(50):
-        p.append((i+70,temp_p[i]))
-    p = sorted(p, key = lambda x : x[1], reverse=True)
-    solutions = []
-    answers = ['A', 'B', 'C', 'D']
-    for i in range(120):
-        solutions.append(answers[np.random.randint(0, 3)])
-    results = np.full((n_student, 120), 'E')
-    student_performances = list(map(int,np.random.normal(65, 11.1, n_student)))
-    
-    points = []
-    point_per_question = []
-    for question in range(120):
-        point_per_question.append(np.log(p[question][1]/(1-p[question][1])))
-
-    for student in range(n_student):
-        student_perf = student_performances[student]
-        points.append(0)
-        for i, item in enumerate(p):
-            remain = 120 - i
-            _p = np.random.rand()
-            if (remain <= student_perf):
-                results[student, item[0]] = solutions[item[0]]
-                points[-1]+=10 + point_per_question[item[0]]
-                student_perf -= 1
-            elif (_p <= 0.9 and student_perf > 0):
-                results[student, item[0]] = solutions[item[0]]
-                points[-1]+=10 + point_per_question[item[0]]
-                student_perf -= 1
-            else:
-                results[student, item[0]] = solutions[item[0]]
-                while (results[student, item[0]] == solutions[item[0]]):
-                    results[student, item[0]] = answers[np.random.randint(0, 3)]
-        points[-1] = np.round(points[-1], 2)
-
-    # fig, ax = plt.subplots(1, 2, figsize=(14, 5))
-    # ax[0].hist(points, bins=30)
-    # ax[1].boxplot(points)
-    # fig.savefig("hist.png")
-    # print(f'max : {max(point_per_question)} | min : {min(point_per_question)} | median : {np.median(point_per_question)}')
-    # print(f'max : {max(points)} | min : {min(points)} | median : {np.median(points)}')
-    # print(points)
-
-    return results, solutions
-
-def name_generator(n_student = 100000, random_seed = 1):
-    np.random.seed(random_seed)
-    data = ""
-    response = requests.get("https://raw.githubusercontent.com/nprm1243/MaSSP-DS-2023/main/ProjectData/names.txt")
-    data = response.text
-    data = data.split('\r\n')
-    random.shuffle(data)
-    return data[:n_student]
-
-def CAE_data_generator(n_student = 100000, random_seed = 1):
-    if (random_seed == 1):
-        raise Exception("You have to change random_seed as required in the assignment!")
-    CAE_data, sols = CAE_generator(n_student, random_seed)
-    names = name_generator(n_student, random_seed)
-    df = pd.DataFrame(CAE_data)
-    df.columns += 1
-    df.insert(0, "Name", names)
-    return df, sols
+class APT_dataset:
+
+    def __init__(self, n_student:int = 100000, random_seed:int = 1):
+        if (n_student < 1000 or n_student > 100000):
+            raise Exception("n_student have to greater than 1000 and smaller than 100000!")
+        if (random_seed == 1):
+            raise Exception("You have to change random_seed as required in the assignment!")
+        self.n_student = n_student
+        self.random_seed = random_seed
+        self.answers, self.solution = self.APT_data_generator()
+
+    def APT_generator(self)->tuple[np.ndarray, list]:
+        """
+        Function to generate a simulation Advanced Placement Test solutions and answers of participants
+
+        Returns:
+        student_answers: 2D ndarray
+        solution: 1D ndarray
+        """
+        np.random.seed(self.random_seed)
+        p_top = 0.05
+        p_bot = 0.95
+        p = []
+        temp_p = np.linspace(p_top, p_bot, 40)
+        np.random.shuffle(temp_p)
+        for i in range(40):
+            p.append((i, temp_p[i]))
+        temp_p = np.linspace(p_top, p_bot, 30)
+        np.random.shuffle(temp_p)
+        for i in range(30):
+            p.append((i+40, temp_p[i]))
+        temp_p = np.linspace(p_top, p_bot, 50)
+        np.random.shuffle(temp_p)
+        for i in range(50):
+            p.append((i+70,temp_p[i]))
+        p = sorted(p, key = lambda x : x[1], reverse=True)
+        solutions = []
+        answers = ['A', 'B', 'C', 'D']
+        for i in range(120):
+            solutions.append(answers[np.random.randint(0, 3)])
+        student_answers = np.full((self.n_student, 120), 'E')
+        student_performances = list(map(int,np.random.normal(65, 11.1, self.n_student)))
+        
+        points = []
+        point_per_question = []
+        for question in range(120):
+            point_per_question.append(np.log(p[question][1]/(1-p[question][1])))
+
+        for student in range(self.n_student):
+            student_perf = student_performances[student]
+            points.append(0)
+            for i, item in enumerate(p):
+                remain = 120 - i
+                _p = np.random.rand()
+                if (remain <= student_perf):
+                    student_answers[student, item[0]] = solutions[item[0]]
+                    points[-1]+=10 + point_per_question[item[0]]
+                    student_perf -= 1
+                elif (_p <= 0.9 and student_perf > 0):
+                    student_answers[student, item[0]] = solutions[item[0]]
+                    points[-1]+=10 + point_per_question[item[0]]
+                    student_perf -= 1
+                else:
+                    student_answers[student, item[0]] = solutions[item[0]]
+                    while (student_answers[student, item[0]] == solutions[item[0]]):
+                        student_answers[student, item[0]] = answers[np.random.randint(0, 3)]
+            points[-1] = np.round(points[-1], 2)
+
+        return student_answers, solutions
+
+    def name_generator(self)->list:
+        """
+        Function to generate a list of Vietnamese name
+
+        Returns:
+        list of Vietnamese name
+        """
+        np.random.seed(self.random_seed)
+        random.seed(self.random_seed)
+        data = ""
+        response = requests.get("https://raw.githubusercontent.com/nprm1243/MaSSP-DS-2023/main/ProjectData/names.txt")
+        data = response.text
+        data = data.split('\r\n')
+        random.shuffle(data)
+        return data[:self.n_student]
+
+    def APT_data_generator(self)->tuple[pd.DataFrame, list]:
+        """
+        Function to generate a simulation APT DataFrame contain students's answer and list of solution
+
+        Returns:
+        DataFrame
+        list of solution
+        """
+        np.random.seed(self.random_seed)
+        CAE_data, sols = self.APT_generator()
+        names = self.name_generator()
+        df = pd.DataFrame(CAE_data)
+        df.columns += 1
+        df.insert(0, "Name", names)
+        return df, sols
 
 if __name__ == '__main__':
-    table, sols = CAE_data_generator(5000, 2024)
+    APT_dataset = APT_dataset(n_student=5000, random_seed=20022002)
+    table = APT_dataset.answers
+    solution = APT_dataset.solution
     print(table.head(5))
-    print(sols)
+    print(solution)
```

### Comparing `masspds2024-0.0.3/src/masspds2024.egg-info/PKG-INFO` & `masspds2024-0.0.4/src/masspds2024.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: masspds2024
-Version: 0.0.3
+Version: 0.0.4
 Summary: Package contains useful commands for mentee MaSSP DS 2024
 Home-page: https://github/
 Author: MaSSP Mathematics and Computer Science 2024
 Author-email: nghi08122003@gmail.com
 Project-URL: repository, https://github/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

