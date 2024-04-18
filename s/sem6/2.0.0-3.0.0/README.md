# Comparing `tmp/sem6-2.0.0.tar.gz` & `tmp/sem6-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sem6-2.0.0.tar", last modified: Sun Apr 14 15:07:10 2024, max compression
+gzip compressed data, was "sem6-3.0.0.tar", last modified: Thu Apr 18 17:58:05 2024, max compression
```

## Comparing `sem6-2.0.0.tar` & `sem6-3.0.0.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-04-14 15:07:10.219230 sem6-2.0.0/
--rw-rw-rw-   0        0        0       51 2024-04-14 15:07:10.219230 sem6-2.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-14 15:07:10.158338 sem6-2.0.0/sem6/
--rw-rw-rw-   0        0        0        0 2024-04-13 12:06:54.000000 sem6-2.0.0/sem6/__init__.py
--rw-rw-rw-   0        0        0     1712 2024-04-13 12:00:16.000000 sem6-2.0.0/sem6/adaboost.py
--rw-rw-rw-   0        0        0     5770 2024-04-13 13:17:40.000000 sem6-2.0.0/sem6/clustering.py
--rw-rw-rw-   0        0        0     3604 2024-04-14 14:55:04.000000 sem6-2.0.0/sem6/decisiontree.py
--rw-rw-rw-   0        0        0     3100 2024-04-14 15:02:18.000000 sem6-2.0.0/sem6/ensemble_classification.py
--rw-rw-rw-   0        0        0     2193 2024-04-13 12:00:57.000000 sem6-2.0.0/sem6/ensemble_regression.py
--rw-rw-rw-   0        0        0     3263 2024-04-14 14:55:06.000000 sem6-2.0.0/sem6/gradientboosting.py
--rw-rw-rw-   0        0        0     3418 2024-04-14 14:55:07.000000 sem6-2.0.0/sem6/lightgbm.py
--rw-rw-rw-   0        0        0     3314 2024-04-14 14:55:09.000000 sem6-2.0.0/sem6/linearreg.py
--rw-rw-rw-   0        0        0     3315 2024-04-14 14:55:10.000000 sem6-2.0.0/sem6/logisticreg.py
--rw-rw-rw-   0        0        0     3666 2024-04-14 14:55:12.000000 sem6-2.0.0/sem6/randomforest.py
--rw-rw-rw-   0        0        0     4379 2024-04-14 14:55:14.000000 sem6-2.0.0/sem6/svm.py
--rw-rw-rw-   0        0        0     3441 2024-04-14 15:03:40.000000 sem6-2.0.0/sem6/xgb.py
-drwxrwxrwx   0        0        0        0 2024-04-14 15:07:10.213037 sem6-2.0.0/sem6.egg-info/
--rw-rw-rw-   0        0        0       51 2024-04-14 15:07:09.000000 sem6-2.0.0/sem6.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      406 2024-04-14 15:07:09.000000 sem6-2.0.0/sem6.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-14 15:07:09.000000 sem6-2.0.0/sem6.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-04-14 15:07:09.000000 sem6-2.0.0/sem6.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-04-14 15:07:09.000000 sem6-2.0.0/sem6.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-14 15:07:10.219230 sem6-2.0.0/setup.cfg
--rw-rw-rw-   0        0        0      235 2024-04-14 14:59:21.000000 sem6-2.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 17:58:05.621381 sem6-3.0.0/
+-rw-rw-rw-   0        0        0       51 2024-04-18 17:58:05.620382 sem6-3.0.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-18 17:58:05.591281 sem6-3.0.0/sem6/
+-rw-rw-rw-   0        0        0        0 2024-04-13 12:06:54.000000 sem6-3.0.0/sem6/__init__.py
+-rw-rw-rw-   0        0        0     1494 2024-04-18 17:11:23.000000 sem6-3.0.0/sem6/adaboost.py
+-rw-rw-rw-   0        0        0     2934 2024-04-18 16:25:34.000000 sem6-3.0.0/sem6/clustering.py
+-rw-rw-rw-   0        0        0     4128 2024-04-18 12:55:58.000000 sem6-3.0.0/sem6/decisiontree.py
+-rw-rw-rw-   0        0        0     2666 2024-04-18 15:51:46.000000 sem6-3.0.0/sem6/ensemble_classification.py
+-rw-rw-rw-   0        0        0     1855 2024-04-18 15:53:22.000000 sem6-3.0.0/sem6/ensemble_regression.py
+-rw-rw-rw-   0        0        0     3651 2024-04-18 17:55:45.000000 sem6-3.0.0/sem6/gradientboosting.py
+-rw-rw-rw-   0        0        0     3418 2024-04-14 14:55:07.000000 sem6-3.0.0/sem6/lightgbm.py
+-rw-rw-rw-   0        0        0     3314 2024-04-14 14:55:09.000000 sem6-3.0.0/sem6/linearreg.py
+-rw-rw-rw-   0        0        0     3315 2024-04-14 14:55:10.000000 sem6-3.0.0/sem6/logisticreg.py
+-rw-rw-rw-   0        0        0     3666 2024-04-14 14:55:12.000000 sem6-3.0.0/sem6/randomforest.py
+-rw-rw-rw-   0        0        0     4379 2024-04-18 16:32:26.000000 sem6-3.0.0/sem6/svm.py
+-rw-rw-rw-   0        0        0    38016 2024-04-18 17:55:01.000000 sem6-3.0.0/sem6/theory.py
+-rw-rw-rw-   0        0        0     3441 2024-04-18 16:33:42.000000 sem6-3.0.0/sem6/xgb.py
+drwxrwxrwx   0        0        0        0 2024-04-18 17:58:05.618379 sem6-3.0.0/sem6.egg-info/
+-rw-rw-rw-   0        0        0       51 2024-04-18 17:58:05.000000 sem6-3.0.0/sem6.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      421 2024-04-18 17:58:05.000000 sem6-3.0.0/sem6.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 17:58:05.000000 sem6-3.0.0/sem6.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-04-18 17:58:05.000000 sem6-3.0.0/sem6.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-04-18 17:58:05.000000 sem6-3.0.0/sem6.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-18 17:58:05.621381 sem6-3.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      235 2024-04-18 17:56:54.000000 sem6-3.0.0/setup.py
```

### Comparing `sem6-2.0.0/sem6/decisiontree.py` & `sem6-3.0.0/sem6/decisiontree.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,58 +27,79 @@
     # plt.title('Feature Correlation Heatmap')
     # plt.show()
 
     # 3. Preprocessing
     from sklearn.preprocessing import LabelEncoder, StandardScaler
 
     # a. Label Encoding for categorical variables if any
-    # encoder = LabelEncoder()
-    # df['categorical_column'] = encoder.fit_transform(df['categorical_column'])
+    encoder = LabelEncoder()
+     df['categorical_column'] = encoder.fit_transform(df['categorical_column'])
 
     # b. Feature engineering - Create or transform features while avoiding introduction of noise
-    # df['engineered_feature'] = df['existing_feature'] ** 2 # example for polynomial feature
+     df['engineered_feature'] = df['existing_feature'] ** 2 # example for polynomial feature
 
     # c. Standard scaler - Standardize features by removing the mean and scaling to unit variance
-    # scaler = StandardScaler()
-    # df[['feature1', 'feature2', 'feature3']] = scaler.fit_transform(df[['feature1', 'feature2', 'feature3']])
+     scaler = StandardScaler()
+     df[['feature1', 'feature2', 'feature3']] = scaler.fit_transform(df[['feature1', 'feature2', 'feature3']])
 
     # 4. Decision Tree classifier
     from sklearn.tree import DecisionTreeClassifier
 
     # a. Import and declare the model
     # Decision Trees are a type of non-parametric supervised learning method used for classification and regression.
 
     # b. Instantiate the Decision Tree classifier with a criterion
-    # dt_model = DecisionTreeClassifier(criterion='gini')  # or criterion='entropy'
+    dt_model = DecisionTreeClassifier(criterion='gini')  # or criterion='entropy'
 
     # 5. Train/Test/Split
     from sklearn.model_selection import train_test_split
 
-    # a. Hold out method - Split the dataset into training and testing sets
-    # X = df.drop('target', axis=1)
-    # y = df['target']
-    # X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.2, random_state=42)
+     #a. Hold out method - Split the dataset into training and testing sets
+     X = df.drop('target', axis=1)
+     y = df['target']
+     X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.2, random_state=42)
 
     # c. Fit the model on the training data and predict on the test data
-    # dt_model.fit(X_train, y_train)
-    # predictions = dt_model.predict(X_test)
+
+    dt_model.fit(X_train, y_train)
+    gini_index = dt.tree_.impurity[0]
+
+    print("Gini Index:", gini_index)
+    predictions = dt_model.predict(X_test)
 
     # 6. Use appropriate accuracy metrics
     from sklearn.metrics import accuracy_score, classification_report, confusion_matrix
 
     # Calculate metrics
-    # acc = accuracy_score(y_test, predictions)
-    # report = classification_report(y_test, predictions)
-    # conf_mat = confusion_matrix(y_test, predictions)
-    # print(f'Accuracy Score: {acc}')
-    # print(f'Classification Report:\n{report}')
-    # print(f'Confusion Matrix:\n{conf_mat}')
-
-    # 7. Compare and comment on model performances
-    # Comment on the performance and potentially compare with other models or the same model with different parameters.
-    # Also, consider plotting the decision tree or other insightful visualizations.
-    # from sklearn.tree import plot_tree
-    # plt.figure(figsize=(20,10))
-    # plot_tree(dt_model, filled=True, feature_names=X.columns, class_names=['Class1', 'Class2'])
-    # plt.show()
+     acc = accuracy_score(y_test, predictions)
+     report = classification_report(y_test, predictions)
+     conf_mat = confusion_matrix(y_test, predictions)
+     print(f'Accuracy Score: {acc}')
+     print(f'Classification Report:\n{report}')
+     print(f'Confusion Matrix:\n{conf_mat}')
+
+     7. Compare and comment on model performances
+     Comment on the performance and potentially compare with other models or the same model with different parameters.
+    
+     from sklearn.tree import plot_tree
+     plt.figure(figsize=(20,10))
+     plot_tree(dt_model, filled=True, feature_names=X.columns, class_names=['Class1', 'Class2'])
+     plt.show()
+
+     8.Adding hyperparameter:
+            param_grid={
+            'criterion':['gini','entropy'],
+            'min_samples_split': [2, 5, 10],
+            'max_depth':[3,5,7,9,10]
+        }
+
+        grid_search=GridSearchCV(dt,param_grid,cv=5,n_jobs=-1)
+        grid_search.fit(x_train,y_train)
+        print('Best',grid_search.best_params_)
+
+        best_dt = grid_search.best_estimator_
+        y_pred = best_dt.predict(x_test)
+        accuracy = accuracy_score(y_test, y_pred)
+        print("Accuracy on test set:", accuracy)
+
     """
     print(code)
```

### Comparing `sem6-2.0.0/sem6/ensemble_classification.py` & `sem6-3.0.0/sem6/ensemble_classification.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,59 +5,53 @@
     import numpy as np
     import pandas as pd
     import os
     from sklearn.preprocessing import LabelEncoder
     import seaborn as sns
     from sklearn.model_selection import cross_val_score
     from sklearn.linear_model import LogisticRegression
-    from sklearn.neighbors import KNeighborsClassifier
+    from sklearn.ensemble import GradientBoostingClassification
     from sklearn.ensemble import RandomForestClassifier, VotingClassifier
     from sklearn.svm import SVC
     from sklearn.datasets import make_classification
 
-    # Load Iris dataset
-    df = pd.read_csv('Iris.csv')
-    df = df.iloc[:, 1:]  # Remove Id column
+    # Load  dataset
+    df = pd.read_csv('.csv')
+    
 
-    # Label encode Species
+    # Label encode categorical variable
     encoder = LabelEncoder()
-    df['Species'] = encoder.fit_transform(df['Species'])
+    df[''] = encoder.fit_transform(df[''])
 
-    # Visualize data
-    sns.pairplot(df, hue='Species')
+    # standardise numerical variable
+    scaler = StandardScaler()
+    df[''] = scaler.fit_transform(df[''])
 
     # Prepare data for classification
-    X = df.iloc[:, :2]
-    y = df.iloc[:, -1]
+    X = df.drop(['target'],axis=1)
+    y = df['target']
 
     # Define classifiers
     clf1 = LogisticRegression()
     clf2 = RandomForestClassifier()
-    clf3 = KNeighborsClassifier()
+    clf3 = GradientBoostingClassifier()
 
     # Perform cross-validation for individual classifiers
-    estimators = [('lr', clf1), ('rf', clf2), ('knn', clf3)]
+    estimators = [('lr', clf1), ('rf', clf2), ('gb', clf3)]
     for estimator in estimators:
         scores = cross_val_score(estimator[1], X, y, cv=10, scoring='accuracy')
         print(estimator[0], np.round(np.mean(scores), 2))
 
     # Perform cross-validation for Voting Classifier
     vc_hard = VotingClassifier(estimators=estimators, voting='hard')
     vc_soft = VotingClassifier(estimators=estimators, voting='soft')
     print("Hard Voting:", np.round(np.mean(cross_val_score(vc_hard, X, y, cv=10, scoring='accuracy')), 2))
     print("Soft Voting:", np.round(np.mean(cross_val_score(vc_soft, X, y, cv=10, scoring='accuracy')), 2))
 
-    # Perform cross-validation for Weighted Voting Classifier
-    for i in range(1, 4):
-        for j in range(1, 4):
-            for k in range(1, 4):
-                weights = [i, j, k]
-                vc_weighted = VotingClassifier(estimators=estimators, voting='soft', weights=weights)
-                scores = cross_val_score(vc_weighted, X, y, cv=10, scoring='accuracy')
-                print("Weights:", weights, "Accuracy:", np.round(np.mean(scores), 2))
+
 
     # Classifiers of the same algorithm (SVC)
     X, y = make_classification(n_samples=1000, n_features=20, n_informative=15, n_redundant=5, random_state=2)
     svm1 = SVC(probability=True, kernel='poly', degree=1)
     svm2 = SVC(probability=True, kernel='poly', degree=2)
     svm3 = SVC(probability=True, kernel='poly', degree=3)
     svm4 = SVC(probability=True, kernel='poly', degree=4)
```

### Comparing `sem6-2.0.0/sem6/ensemble_regression.py` & `sem6-3.0.0/sem6/ensemble_regression.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,44 +2,37 @@
 def ensemble_regression():
     code = """
 
     from sklearn.datasets import load_boston
     import numpy as np
     from sklearn.linear_model import LinearRegression
     from sklearn.tree import DecisionTreeRegressor
-    from sklearn.svm import SVR
+    from sklearn.ensemble import RandomForestRegressor
     from sklearn.model_selection import cross_val_score
     from sklearn.ensemble import VotingRegressor
 
     # Load Boston housing dataset
     X, y = load_boston(return_X_y=True)
 
     # Define estimators
     lr = LinearRegression()
     dt = DecisionTreeRegressor()
-    svr = SVR()
-    estimators = [('lr', lr), ('dt', dt), ('svr', svr)]
+    rf = RandomForestRegressor()
+    estimators = [('lr', lr), ('dt', dt), ('gb', svr)]
 
     # Evaluate individual estimators
     for estimator in estimators:
         scores = cross_val_score(estimator[1], X, y, scoring='r2', cv=10)
         print(estimator[0], np.round(np.mean(scores), 2))
 
     # Evaluate Voting Regressor
     vr = VotingRegressor(estimators)
     scores = cross_val_score(vr, X, y, scoring='r2', cv=10)
     print("Voting Regressor", np.round(np.mean(scores), 2))
 
-    # Evaluate Voting Regressor with different weights
-    for i in range(1, 4):
-        for j in range(1, 4):
-            for k in range(1, 4):
-                vr = VotingRegressor(estimators, weights=[i, j, k])
-                scores = cross_val_score(vr, X, y, scoring='r2', cv=10)
-                print("For i={}, j={}, k={}".format(i, j, k), np.round(np.mean(scores), 2))
 
     # Using different depths for Decision Trees
     dt1 = DecisionTreeRegressor(max_depth=1)
     dt2 = DecisionTreeRegressor(max_depth=3)
     dt3 = DecisionTreeRegressor(max_depth=5)
     dt4 = DecisionTreeRegressor(max_depth=7)
     dt5 = DecisionTreeRegressor(max_depth=None)
```

### Comparing `sem6-2.0.0/sem6/gradientboosting.py` & `sem6-3.0.0/sem6/gradientboosting.py`

 * *Files 8% similar despite different names*

```diff
@@ -71,12 +71,30 @@
     from sklearn.metrics import accuracy_score, classification_report, confusion_matrix
 
     # Calculate metrics
     print("Accuracy:", accuracy_score(y_test, predictions))
     print("Confusion Matrix:\n", confusion_matrix(y_test, predictions))
     print("Classification Report:\n", classification_report(y_test, predictions))
 
-    # 7. Compare and comment on model performances
-    # Comment on the accuracy, precision, recall, and F1-score.
-    # Compare these metrics against a baseline model or domain expectations.
+    #8 Adding Gridsearch:
+    param_grid = {
+    'learning_rate': [0.01, 0.1, 0.2],
+    'n_estimators': [50, 100, 150],
+    'max_depth': [1,3, 5, 7],
+    }
+
+    
+    grid_search = GridSearchCV(gb_model, param_grid, cv=5, n_jobs=-1)
+
+    grid_search.fit(x_train, y_train)
+
+    # Print the best parameters found
+    print("Best parameters:", grid_search.best_params_)
+
+    # Evaluate the model with the best parameters on the test set
+    best_lgb = grid_search.best_estimator_
+    y_pred = best_lgb.predict(x_test)
+    accuracy = accuracy_score(y_test, y_pred)
+
+
     """
     print(code)
```

### Comparing `sem6-2.0.0/sem6/lightgbm.py` & `sem6-3.0.0/sem6/lightgbm.py`

 * *Files identical despite different names*

### Comparing `sem6-2.0.0/sem6/linearreg.py` & `sem6-3.0.0/sem6/linearreg.py`

 * *Files identical despite different names*

### Comparing `sem6-2.0.0/sem6/logisticreg.py` & `sem6-3.0.0/sem6/logisticreg.py`

 * *Files identical despite different names*

### Comparing `sem6-2.0.0/sem6/randomforest.py` & `sem6-3.0.0/sem6/randomforest.py`

 * *Files identical despite different names*

### Comparing `sem6-2.0.0/sem6/svm.py` & `sem6-3.0.0/sem6/svm.py`

 * *Files identical despite different names*

### Comparing `sem6-2.0.0/sem6/xgb.py` & `sem6-3.0.0/sem6/xgb.py`

 * *Files identical despite different names*

