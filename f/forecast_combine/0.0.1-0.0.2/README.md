# Comparing `tmp/forecast_combine-0.0.1.tar.gz` & `tmp/forecast_combine-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "forecast_combine-0.0.1.tar", max compression
+gzip compressed data, was "forecast_combine-0.0.2.tar", max compression
```

## Comparing `forecast_combine-0.0.1.tar` & `forecast_combine-0.0.2.tar`

### file list

```diff
@@ -1,9 +1,11 @@
--rw-r--r--   0        0        0     1069 2023-08-09 11:13:58.574534 forecast_combine-0.0.1/LICENSE
--rw-r--r--   0        0        0     3666 2023-08-11 11:00:35.281961 forecast_combine-0.0.1/README.md
--rw-r--r--   0        0        0        0 2023-08-10 11:20:30.403617 forecast_combine-0.0.1/forecast_combine/__init__.py
--rwxr-xr-x   0        0        0    42753 2023-08-11 11:01:35.066849 forecast_combine-0.0.1/forecast_combine/forecast.py
--rwxr-xr-x   0        0        0    29640 2023-08-11 11:01:32.614812 forecast_combine-0.0.1/forecast_combine/model_select.py
--rwxr-xr-x   0        0        0     5670 2023-08-10 06:46:13.018293 forecast_combine-0.0.1/forecast_combine/utils/plotting.py
--rw-r--r--   0        0        0     1246 2023-08-11 11:00:54.578248 forecast_combine-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     4823 1970-01-01 00:00:00.000000 forecast_combine-0.0.1/setup.py
--rw-r--r--   0        0        0     4977 1970-01-01 00:00:00.000000 forecast_combine-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-08-09 11:13:58.574534 forecast_combine-0.0.2/LICENSE
+-rw-r--r--   0        0        0     3791 2024-04-18 10:16:14.517329 forecast_combine-0.0.2/README.md
+-rw-r--r--   0        0        0        0 2023-08-10 11:20:30.403617 forecast_combine-0.0.2/forecast_combine/__init__.py
+-rwxr-xr-x   0        0        0    40996 2024-04-17 11:25:40.057693 forecast_combine-0.0.2/forecast_combine/forecast.py
+-rwxr-xr-x   0        0        0    44575 2024-04-18 09:45:41.518588 forecast_combine-0.0.2/forecast_combine/model_select.py
+-rw-r--r--   0        0        0    13643 2024-04-17 11:56:30.131379 forecast_combine-0.0.2/forecast_combine/reconcile.py
+-rw-r--r--   0        0        0     5534 2024-04-12 15:21:42.963039 forecast_combine-0.0.2/forecast_combine/utils/explore.py
+-rw-r--r--   0        0        0     3194 2024-04-17 09:26:53.214931 forecast_combine-0.0.2/forecast_combine/utils/metrics.py
+-rwxr-xr-x   0        0        0     9434 2024-04-15 11:32:24.768704 forecast_combine-0.0.2/forecast_combine/utils/plotting.py
+-rw-r--r--   0        0        0     1282 2024-04-18 10:16:12.237370 forecast_combine-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     5082 1970-01-01 00:00:00.000000 forecast_combine-0.0.2/PKG-INFO
```

### Comparing `forecast_combine-0.0.1/LICENSE` & `forecast_combine-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `forecast_combine-0.0.1/README.md` & `forecast_combine-0.0.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -20,55 +20,63 @@
 ```bash
 pip install forecast_combine
 ```
 
 ## Usage
 
 ```python
-# Import the necessary classes from your-package-name
+# Read the data
+import pandas as pd
+import numpy as np
 data = pd.Series(np.cumsum(np.random.normal(0, 1, size=1000)), 
-                 index=pd.date_range(end='31/12/2022', periods=1000)).rename('y').to_frame()
+                 index=pd.date_range(end='31/12/2022', periods=1000)
+                ).rename('y').to_frame()
 
+# Import the package
 from forecast_combine.model_select import ForecastModelSelect
-# models necessary to define the forecasting models 
+
+# Import the packages of the models to test
 from sktime.forecasting.naive import NaiveForecaster
 from sktime.forecasting.statsforecast import (
     StatsForecastAutoARIMA,
     StatsForecastAutoETS, 
-    StatsForecastAutoTheta
+    StatsForecastAutoTheta,
+    StatsForecastAutoTBATS
 )
-from sktime.forecasting.tbats import TBATS
-from sktime.forecasting.fbprophet import Prophet
 
+# Define the forecasting models 
 ForecastingModels = {
-"Naive": NaiveForecaster(),
-"AutoARIMA": StatsForecastAutoARIMA(),
-"AutoETS": StatsForecastAutoETS(),
-"AutoTheta": StatsForecastAutoTheta(),
-"TBATS": TBATS(),
-"Prophet": Prophet(),
+    "Naive": NaiveForecaster(),
+    "AutoARIMA": StatsForecastAutoARIMA(),
+    "AutoETS": StatsForecastAutoETS(),
+    "AutoTheta": StatsForecastAutoTheta(),
+    "AutoTBATS": StatsForecastAutoTBATS(seasonal_periods=1),
 }
+
 model = ForecastModelSelect(
             data= data,
             depvar_str = 'y',                 
             exog_l=None,
             fh = 10,
             pct_initial_window=0.75,
-            step_length = 25,
-            models_d = ForecastingModels,
+            step_length = 5,
+            forecasters_d = ForecastingModels,
             freq = 'B',
-            mode = 'nbest_average_horizon',
-            score = 'RMSE', 
-            nbest = 2)
+            mode = 'best_horizon',
+            score = 'RMSE', )
+
+# evaluate all the models out-of-sample
+summary_horizon, summary_results = model.evaluate()
 
 # compare models
-model.select_best(score = 'MAPE')
+rank, score = model.select_best(score = 'MAPE')
+
 # Visualize model comparison
-model.plot_model_compare(score='MAPE', view='horizon')
-model.plot_model_compare(score='MAPE', view='cutoff')
+model.plot_model_compare(score ='MAPE', view = 'cutoff')
+model.plot_model_compare(score ='MAPE', view = 'horizon')
 
 # Generate prediction
 y_pred, y_pred_ints, preds, pred_ints =  model.predict(score='RMSE', ret_underlying=True)
 
 # Visualize prediction
 model.plot_prediction(y_pred = y_pred,
                      models_preds = preds,
```

### Comparing `forecast_combine-0.0.1/forecast_combine/forecast.py` & `forecast_combine-0.0.2/forecast_combine/forecast.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,93 +1,85 @@
+""" Timeseries Forecasting with Insample, Validation and Out-of-Sample predictions"""
+__description__ = "Time Series Forecast"
+__author__ = "Amine Raboun - amineraboun@github.io"
+
+# Filter Warnings
+import logging
+logging.getLogger().setLevel(logging.ERROR)
+import warnings
+warnings.simplefilter('ignore')
+warnings.filterwarnings("ignore")
+
+##############################################################################
+# Import Libraries & default configuration 
+##############################################################################
 # Standard Inports
+from typing import Optional, Tuple, List
 import pandas as pd
 import numpy as np
-import os
 
-from typing import Optional, Tuple, List
+# Iteration tools
 from collections.abc import Iterable
-from tqdm.autonotebook import tqdm
+from multiprocessing import Pool
+from tqdm import tqdm
 import time
 
-# Plotting packages
+# Plotting packages & configuration
+from forecast_combine.utils.plotting import plot_series, plot_windows
 import matplotlib.pyplot as plt
-from matplotlib.ticker import MaxNLocator
-import seaborn as sns
-sns.set(style='white', font_scale=1)
 plt.rc('axes', titlesize='large')    
 plt.rc('axes', labelsize='large')   
 plt.rc('xtick', labelsize='large')   
 plt.rc('ytick', labelsize='large')   
 plt.rc('legend', fontsize='large')   
 plt.rc('figure', titlesize='x-large') 
-from forecast_combine.utils.plotting import plot_series
+import seaborn as sns
+sns.set_theme(style='white', font_scale=1)
+
+# Cross Validation tools
+from sktime.forecasting.base import ForecastingHorizon
+from sktime.forecasting.model_evaluation import evaluate
+from sktime.split import CutoffSplitter
+from sktime.forecasting.model_selection import (
+ExpandingWindowSplitter, 
+temporal_train_test_split
+)
+
+# Performance Metrics
+from .utils.metrics import summary_perf, calculate_prediction_interval
+from sktime.performance_metrics.forecasting import (
+MeanSquaredError,
+MeanAbsoluteError, 
+MeanAbsolutePercentageError, 
+MedianAbsoluteError
+)
 
-# Forcast models
+##############################################################################
+# Default values
+##############################################################################
+# Common Forcasting models
 from sktime.forecasting.naive import NaiveForecaster
+from sktime.forecasting.fbprophet import Prophet
 from sktime.forecasting.statsforecast import (
 StatsForecastAutoARIMA,
 StatsForecastAutoETS, 
-StatsForecastAutoTheta
+StatsForecastAutoCES,
+StatsForecastAutoTheta,
+StatsForecastAutoTBATS, 
 )
-from sktime.forecasting.tbats import TBATS
-from sktime.forecasting.fbprophet import Prophet
-
-ForecastingModels = {
+CommonForecastingModels = {
 "Naive": NaiveForecaster(),
+"Seasonal_Naive": NaiveForecaster(sp = 5),
 "AutoARIMA": StatsForecastAutoARIMA(),
 "AutoETS": StatsForecastAutoETS(),
+"AutoCES": StatsForecastAutoCES(),
 "AutoTheta": StatsForecastAutoTheta(),
-"TBATS": TBATS(),
+"AutoTBATS": StatsForecastAutoTBATS(seasonal_periods = 1),
 "Prophet": Prophet(),
 }
-
-# Cross Validation
-from sktime.forecasting.base import ForecastingHorizon
-from sktime.forecasting.model_selection import (
-CutoffSplitter, 
-ExpandingWindowSplitter, 
-temporal_train_test_split
-)
-from sktime.forecasting.model_evaluation import evaluate
-# Performance Metrics
-from sktime.performance_metrics.forecasting import (
-MeanAbsolutePercentageError, 
-MeanSquaredError,
-)
-
-# Filter Warnings
-from warnings import simplefilter
-simplefilter('ignore')
-
-def summary_perf(insample_result_df, 
-			 grouper, 
-			 y_true_col = 'y_true',
-			 y_pred_col = 'y_pred',
-			):
-
-	"""
-	Compute summary performance metrics for a given forecast.
-
-	Parameters:
-		- insample_result_df (DataFrame): A DataFrame containing the forecast results.
-		- grouper (str): The column name to group the forecast results for computing summary metrics.
-		- y_true_col (str, optional): The column name representing the true values. Default is 'y_true'.
-		- y_pred_col (str, optional): The column name representing the predicted values. Default is 'y_pred'.
-
-	Returns:
-		DataFrame: A DataFrame containing summary performance metrics, including RMSE and MAPE.
-	"""
-
-	rmse = MeanSquaredError(square_root=True)
-	mape = MeanAbsolutePercentageError()
-	horizon_metrics = pd.concat([insample_result_df.groupby(grouper).apply(lambda x: rmse(x[y_true_col], x[y_pred_col])).rename('RMSE'),
-									 insample_result_df.groupby(grouper).apply(lambda x: mape(x[y_true_col], x[y_pred_col])).rename('MAPE')
-									], axis=1)
-	return horizon_metrics
-
 # Pandas frequencies
 pandas_frequency_dict = {
     "D": "daily",
     "B": "business days",
     "W": "weekly (end of week, default on Sunday)",
     "M": "monthly (end of month)",
     "Q": "quarterly (end of quarter)",
@@ -97,136 +89,80 @@
     "S": "secondly",
     "L": "millisecondly",
     "U": "microsecondly",
     "BQ": "business quarterly (business quarter-end)",
     "BA": "business annual (business year-end)",
     "BH": "business hourly (business hour)"
 }
+
 ##############################################################################
 # Master Class Definition and Plot
 ##############################################################################
-
 class Forecast(object):
     """
     Forecast class for managing and evaluating forecast models.
 
-    Parameters
-    
-        data : pd.DataFrame
-            A DataFrame containing the input data for forecasting.
-        depvar_str : str
-            The column name representing the dependent variable for forecasting.
-        fh : int
-            The forecast horizon, i.e., the number of periods ahead to forecast.
-        pct_initial_window : float
-            The percentage of data used as the initial training window.
-        step_length : int
-            The step size for expanding window cross-validation.
-        forecaster_name : str, optional
-            The name of the forecasting model. Default is 'Naive'.
-        forecaster : object, optional
-            The forecasting model object. Default is None, which will use the model corresponding to forecaster_name.
-        exog_l : list, optional
-            List of exogenous variables for forecasting. Default is None.
-        freq : str, optional
-            The frequency of the time series data. Default is 'B' (business days).
-        random_state : int, optional
-            Random state for reproducibility. Default is 0.
-
-    Attributes
-    
-        y : pd.Series
-            The time series data representing the dependent variable.
-        X : pd.DataFrame or None
-            The DataFrame containing exogenous variables or None if there are no exogenous variables.
-        forecaster_name : str
-            The name of the forecasting model used.
-        forecaster : object
-            The forecasting model object used for forecasting.
-        fh : ForecastingHorizon
-            The forecast horizon, i.e., the number of periods ahead to forecast.
-        initial_window : int
-            The size of the initial training window.
-        step_length : int
-            The step size for expanding window cross-validation.
-        cv : ExpandingWindowSplitter
-            The cross-validation window used for expanding window validation.
-        X_train : pd.DataFrame or None
-            The DataFrame containing exogenous variables for the training set or None if there are no exogenous variables.
-        X_test : pd.DataFrame or None
-            The DataFrame containing exogenous variables for the test set or None if there are no exogenous variables.
-        y_train : pd.Series
-            The dependent variable values for the training set.
-        y_test : pd.Series
-            The dependent variable values for the test set.
-        is_fitted : bool
-            True if the forecaster is fitted, False otherwise.
-        is_evaluated : bool
-            True if the forecaster is evaluated on the test set, False otherwise.
-        rs : numpy.random.RandomState
-            Random state for reproducibility.
-        plot : ForecastPlot
-            An instance of the ForecastPlot class for plotting utility.
+    Parameters:
+    -----------
+    - data (pd.DataFrame): A DataFrame containing the input data for forecasting.
+    - depvar_str (str): The column name representing the dependent variable for forecasting.
+    - fh (int): The forecast horizon, i.e., the number of periods ahead to forecast.
+    - pct_initial_window (float): The percentage of data used as the initial training window.
+    - step_length (int): The step size for expanding window cross-validation.
+    - forecaster_name (str, optional): The name of the forecasting model. Default is 'Naive'.
+    - forecaster (object, optional): The forecasting model object. Default is None, which will use the model corresponding to forecaster_name.
+    - exog_l (list, optional): List of exogenous variables for forecasting. Default is None.
+    - freq (str, optional): The frequency of the time series data. Default is 'B' (business days).
+
+    Attributes:
+    -----------
+    - y (pd.Series): The time series data representing the dependent variable.
+    - X (pd.DataFrame or None): The DataFrame containing exogenous variables or None if there are no exogenous variables.
+    - forecaster_name (str): The name of the forecasting model used.
+    - forecaster (object): The forecasting model object used for forecasting.
+    - fh (ForecastingHorizon): The forecast horizon, i.e., the number of periods ahead to forecast.
+    - initial_window (int): The size of the initial training window.
+    - step_length (int): The step size for expanding window cross-validation.
+    - cv (ExpandingWindowSplitter): The cross-validation window used for expanding window validation.
+    - X_train (pd.DataFrame or None): The DataFrame containing exogenous variables for the training set or None if there are no exogenous variables.
+    - X_test (pd.DataFrame or None): The DataFrame containing exogenous variables for the test set or None if there are no exogenous variables.
+    - y_train (pd.Series): The dependent variable values for the training set.
+    - y_test (pd.Series): The dependent variable values for the test set.
+    - is_fitted (bool): True if the forecaster is fitted, False otherwise.
+    - is_evaluated (bool): True if the forecaster is evaluated on the test set, False otherwise.
+    - rs (numpy.random.RandomState): Random state for reproducibility.
+    - plot (ForecastPlot): An instance of the ForecastPlot class for plotting utility.
     """
 
-    __description = "Time Series Forecast"
-    __author = "Amine Raboun - amineraboun@github.io"
-
     # Initializer
     def __init__(self,
                  data: pd.DataFrame,
                  depvar_str: str,
                  fh: int,
                  pct_initial_window: float,
                  step_length: int,
-                 forecaster_name: str = 'Naive',
+                 forecaster_name: Optional[str] = 'Naive',
                  forecaster: Optional[object] = None,
                  exog_l: Optional[list] = None,
-                 freq: str = 'B',
-                 random_state: int = 0) -> None:
-        """
-        Initialize the Forecast instance.
-
-        Parameters
-        
-            data : pd.DataFrame
-                A DataFrame containing the input data for forecasting.
-            depvar_str : str
-                The column name representing the dependent variable for forecasting.
-            fh : int
-                The forecast horizon, i.e., the number of periods ahead to forecast.
-            pct_initial_window : float
-                The percentage of data used as the initial training window.
-            step_length : int
-                The step size for expanding window cross-validation.
-            forecaster_name : str, optional
-                The name of the forecasting model. Default is 'Naive'.
-            forecaster : object, optional
-                The forecasting model object. Default is None, which will use the model corresponding to forecaster_name.
-            exog_l : list, optional
-                List of exogenous variables for forecasting. Default is None.
-            freq : str, optional
-                The frequency of the time series data. Default is 'B' (business days).
-            random_state : int, optional
-                Random state for reproducibility. Default is 0.
-        """
-        
+                 freq: Optional[str] = 'D',
+                 ) -> None:
+        """Initializes the Forecast class with the provided parameters."""
         self.__init_test(data, depvar_str, exog_l, freq)
         self.y, self.X = self.__clean_data(data=data, 
-                                       depvar_str=depvar_str,
-                                       exog_l=exog_l,
-                                       freq=freq)
+                                           depvar_str=depvar_str,
+                                           exog_l=exog_l,
+                                           freq=freq)
         # Forecasting Model Parameters
         self.forecaster_name = forecaster_name
 
         if forecaster is None:
             # Name of the forecaster should be known only if the forecaster is null
-            _err_msg = f'unsupported forecaster! Known forcasters are {list(ForecastingModels.keys())}'
-            assert forecaster_name in ForecastingModels.keys(), _err_msg
-            self.forecaster = ForecastingModels[forecaster_name]
+            _err_msg = f'unsupported forecaster! Known forcasters are {list(CommonForecastingModels.keys())}'
+            assert forecaster_name in CommonForecastingModels.keys(), _err_msg
+            self.forecaster = CommonForecastingModels[forecaster_name]
         else:
             self.forecaster = forecaster
 
         # Forecasting parameters
         #1. horizon
         self.fh = ForecastingHorizon(np.arange(1, fh+1))
         #2. Initial training window
@@ -239,75 +175,86 @@
                                           step_length=self.step_length,
                                           fh=self.fh)
 
         # Create the train test sets
         if self.X is None:
             self.X_train =  None
             self.X_test = None
-            self.y_train, self.y_test = temporal_train_test_split(
-                y=self.y,
-                train_size=self.initial_window)
+            self.y_train, self.y_test = temporal_train_test_split(y=self.y, 
+                                                                  train_size=self.initial_window)
         else:
             self.y_train, self.y_test, self.X_train, self.X_test = temporal_train_test_split(
             y=self.y, 
             X=self.X,
             train_size=self.initial_window)
 
         self.is_fitted = False
+        self.fitted = None
         self.is_evaluated = False
-        self.rs = np.random.RandomState(random_state) 
+        self.eval = None
+
         # Plots
         self.plot = self.__plot()
 
-
-    def split_procedure_summary(self) -> dict:
+    def split_procedure_summary(self, verbose: bool=True) -> dict:
         """
         Generate a summary of the cross-validation procedure.
 
-        Returns
-        
-            dict:
-                A dictionary containing details of the cross-validation procedure, including the number of folds, initial window size, step length, and forecast period.
+        Parameters:
+        -----------        
+            verbose : bool, optional
+                If True, print the summary. Default is True.
+
+        Returns:
+        --------        
+            dict
+                A dictionary containing the summary of the cross-validation procedure.
         """
 
-        _n_splits = cv.get_n_splits(self.y)
-        cutoffs = [_train[0] for (_train, _test) in self.cv.split(self.y.index)]
+        _n_splits = self.cv.get_n_splits(self.y)
+        cutoffs = [self.y.index[_train[-1]] for (_train, _) in self.cv.split(self.y.index)]
         _split_proc= {'Number of Folds': _n_splits,
-                      'Initial Window Size': cv.initial_window,
-                      'Step Length': cv.step_length,
-                      'Forecast period': len(cv.fh),
+                      'Initial Window Size': self.cv.initial_window,
+                      'Step Length': self.cv.step_length,
+                      'Forecast Horizon': len(self.cv.fh),
                       'First Cutoff': cutoffs[0],
                       'Last Curoff': cutoffs[-1]
                      }
+        if verbose:
+            for k, v in _split_proc.items():
+                print(f"{k:<21}: {v}")
         return _split_proc    
 
     def __plot(self): #-> ForecastPlot
         """
         Create an instance of the ForecastPlot class for plotting utility.
 
         Returns:
+        --------
             ForecastPlot:
                 An instance of the ForecastPlot class.
         """
         return ForecastPlot(self)  
 
     def fit(self, 
             on: str = 'all', 
             fh: Optional[ForecastingHorizon] = None
            ): #-> ForecastFit
         """
         Fit the forecaster and compute insample results.
 
         Parameters:
+        --------
             on : str, optional
                 Either 'train' or 'all'. Sample on which the model is fitted. By default, it is fitted on the entire sample.
             fh : ForecastingHorizon, optional
                 Forecast horizon.
 
         Returns:
+        --------
             ForecastFit:
                 An instance of the ForecastFit class containing the fitted model and insample performance metrics.
         """
 
         if fh is None:
             fh =  self.fh
 
@@ -318,130 +265,158 @@
         elif on=='train':
             self.forecaster.fit(y=self.y_train, X=self.X_train, fh=fh)
             self.is_fitted = False
 
         else: 
             on_values =['all', 'train']
             raise ValueError(f'argument takes 2 possible values {on_values}')
-
-        return ForecastFit(self)  
+        self.fitted = ForecastFit(self)   
+        return self.fitted
 
     def evaluate(self): #-> ForecastEval
         """
         Evaluate the forecaster out-of-sample.
 
         Returns:
+        --------
             ForecastEval:
                 An instance of the ForecastEval class containing the out-of-sample evaluation results.
         """
 
         self.eval = ForecastEval(self)  
         self.is_evaluated = True
         return self.eval
 
     def predict(self, 
                 X: Optional[pd.DataFrame] = None, 
                 fh: Optional[ForecastingHorizon] = None, 
-                coverage: float = 0.9
+                coverage: float = 0.9,
+                verbose = False
                ) -> Tuple[pd.DataFrame, pd.DataFrame]:
         """
         Generate predictions (Average and confidence interval) using the fitted model.
 
-        Parameters
-        
+        Parameters:
+        -----------        
             X : pd.DataFrame, optional
-                Exogenous variables for forecasting. Default is None and takes the exogenous variables defined at instantiation.
+                Exogenous variables for forecasting. Default is None
             fh : ForecastingHorizon, optional
                 Forecast horizon. Default is None and takes the horizon defined at instantiation.
             coverage : float, optional
                 The coverage of the confidence interval. Default is 0.9.
 
-        Returns
-        
+        Returns:
+        --------        
             Tuple[pd.DataFrame, pd.DataFrame]:
                 A tuple containing the predictions and the confidence intervals.
         """
         if self.is_fitted==False:
-            print("\nModel not fitted yet, or fitted on training sample alone")
-            print("Fitting the model on the whole sample ...")
+            if verbose:
+                print(f"\n{self.forecaster_name} model not fitted yet, or fitted on a subset only")
+                print("Fitting the model on the entire sample ...")
             self.fit(on='all', fh=fh)
 
         if fh is None:
             fh =  self.fh
         if X is None:
             X = self.X
 
         y_pred = self.forecaster.predict(X=X, fh=fh)
-        y_pred_ints = self.forecaster.predict_interval(X=X, fh=fh, coverage=coverage)
+        try:
+            y_pred_ints = self.forecaster.predict_interval(X=X, fh=fh, coverage=coverage)
+        except Exception as e:
+            if verbose:
+                print(f"{self.forecaster_name} does not support prediction intervals")
+                print(f"Error: {e}")
+                print("Computing the prediction intervals based on historical errors distribution")
+            
+            historical_errors = self.get_pred_errors()
+            y_pred_ints = calculate_prediction_interval(historical_errors, y_pred, coverage=coverage)
 
         return y_pred, y_pred_ints
 
     def update(self, 
-               newdata: pd.DataFrame, 
+               new_y: pd.Series,
+               new_X: Optional[pd.DataFrame] = None,
                fh: Optional[ForecastingHorizon] = None, 
                coverage: float = 0.9, 
-               refit: bool = False
+               refit: bool = False,
               ) -> Tuple[pd.DataFrame, pd.DataFrame]:
         """
         Update cutoff value to forecast new dates.
         Possibility to refit the model.
 
-        Parameters
-        
-            newdata : pd.DataFrame
-                The new data containing the same columns as the original data.
+        Parameters:
+        -----------        
+            new_y : pd.Series
+                The new dependent variable values.
+            new_X : pd.DataFrame, optional
+                The new exogenous variables. Default is None.
             fh : ForecastingHorizon, optional
                 Forecast horizon. Default is None and takes the horizon defined at instantiation.
             coverage : float, optional
                 The coverage of the confidence interval. Default is 0.9.
             refit : bool, optional
-                If True, the model will be refitted on the new training data. Default is False.
+                If True, refit the model. Default is False.
 
-        Returns
-        
+        Returns:
+        --------        
             Tuple[pd.DataFrame, pd.DataFrame]:
                 A tuple containing the updated predictions and the updated confidence intervals.
         """
-
-        new_y, new_X = self.__clean_data(data=newdata, 
-                                           depvar_str=self.depvar,
-                                           exog_l = self.exog_l,
-                                           freq = self.freq)
-
+        new_y = new_y.resample(self.freq).last().ffill()
+        if new_X is not None:
+            new_X = new_X.resample(self.freq).last().ffill()
         self.forecaster.update(y=new_y, X=new_X, update_params=refit)
         y_pred, y_pred_ints = self.predict(X=new_X, fh=fh, coverage=coverage)
         return y_pred, y_pred_ints
 
+    def get_pred_errors(self):
+        """
+        Get the prediction errors.
+        Returns:
+        --------        
+            pd.DataFrame:
+                A DataFrame containing the prediction errors.
+        """
+        if (self.is_evaluated is False) or (self.eval is None):
+            self.eval = self.evaluate()        
+        try:
+            pred_errors = self.eval.oos_horizon_df[['cutoff', 'horizon', 'error']]
+        except Exception as e:
+            return None
+        return pred_errors
+        
 
     def __init_test(self,
                     data: pd.DataFrame, 
                     depvar_str: str, 
                     exog_l: Optional[list], 
                     freq: str
                    ) -> None:
         """
         Perform checks for the provided data, dependent variable, exogenous variables, and frequency.
 
-        Parameters
-        
+        Parameters:
+        -----------        
             data : pd.DataFrame
                 A DataFrame containing the input data for forecasting.
             depvar_str : str
                 The column name representing the dependent variable for forecasting.
             exog_l : list or None
                 List of exogenous variables for forecasting.
             freq : str
                 The frequency of the time series data.
 
-        Returns
-        
+        Returns:
+        --------
             None
 
-        Raises
-        
+        Raises:
+        -------        
             AssertionError:
                 If the provided data is not a DataFrame, or if depvar_str is not a valid column in the data,
                 or if exog_l is not None or an iterable.
             AssertionError:
                 If any column in exog_l is not present in the data.
             AssertionError:
                 If freq is not a recognized pandas frequency.
@@ -452,15 +427,15 @@
         assert depvar_str in data.columns, 'the dependent varible must be a column in the data'
         self.depvar = depvar_str
 
         cond1 = exog_l is None
         cond2 = isinstance(exog_l, Iterable)
         assert cond1 or cond2, 'exog_l is either None, meaning no X or an iterable object'
         if cond2:
-            assert all([c in data.columns for c in exog_l]), 'not all columns are not in the data'
+            assert all([c in data.columns for c in exog_l]), 'not all exog variables are in the data'
             self.exog_l = exog_l
         else:
             self.exog_l = exog_l
 
         assert freq in pandas_frequency_dict.keys(), f'Not a pandas recognized frequency. List of pandas frequencies:\n{pandas_frequency_dict}'
         self.freq = freq
 
@@ -470,138 +445,140 @@
                      data: pd.DataFrame, 
                      depvar_str: str, 
                      exog_l: Optional[list],
                      freq: str
                     ) -> Tuple[pd.Series, pd.DataFrame]:
         """
         Reformat the data taking into account the requested frequency.
-
-        Returns the X and y for the rest of forecasting operations.
         """
 
+        _df = data.dropna().resample(freq).last().copy()
         # Declare and stage the variable to forecast
-        y = data[depvar_str].dropna().resample(freq).last().ffill()
+        y = _df[depvar_str]
 
         # List of Exogenous variables if any
         if exog_l is None:
             X = None
         else:
-            assert all([c in data.columns for c in exog_l]), 'not all columns are not in the data'
-            X = data[exog_l].resample(freq).last().ffill()
-            X = X.loc[y.index]
-
+            assert all([c in _df.columns for c in exog_l]), 'not all columns are not in the data'
+            X = _df[exog_l]
         return y, X
 
-
 class ForecastPlot:
     """
     Plotting utility class for Forecast.
 
-    Parameters
-    
+    Parameters:
+    -----------    
         LF : Forecast
-            An instance of the Forecast class.
-
-    Returns:
-        None
+            An instance of the Forecast class
     """
 
     def __init__(self, LF: Forecast):
-        self.__dict__.update(LF.__dict__)
-
+        self.y_train = LF.y_train
+        self.y_test = LF.y_test
+        self.y = LF.y
+        self.cv = LF.cv
+        return None
 
     def plot_train_test(self,
-                        labels: List[str] = ["y_train", "y_test"],
+                        labels: List[str] = None,
                         xlabel: Optional[str] = None,
                         ylabel: Optional[str] = None,
                         title: str = 'Train-Test sets',
                         ax: Optional[plt.Axes] = None,
                         figsize: Tuple[float, float] = (15, 6)) -> None:
         """
         Plot the dependent variable separating the train from the test windows.
 
-        Parameters
-        
+        Parameters:
+        -----------
             labels : List[str], optional
                 Labels for the plot. Default is ["y_train", "y_test"].
             xlabel : str, optional
                 Label for the x-axis.
             ylabel : str, optional
                 Label for the y-axis.
             title : str, optional
                 The title of the plot. Default is 'Train-Test sets'.
             ax : plt.Axes, optional
                 The Axes object for the plot.
             figsize : Tuple[float, float], optional
                 The figure size. Default is (15, 6).
 
-        Returns
-        
+        Returns:
+        --------        
             None
         """
+        if labels is None:
+            labels = ["y_train", "y_test"]
         return plot_series(self.y_train, self.y_test, 
                            labels =labels, 
                            ax = ax, 
                            xlabel = xlabel,
                            ylabel = ylabel,
                            title = title,
                            figsize = figsize)
 
-
     def plot_cv_procedure(self,
                           ax: Optional[plt.Axes] = None,
-                          labels: List[str] = ["Window", "Forecasting horizon"],
+                          labels: List[str] = None,
                           ylabel: str = "Window number",
                           xlabel: str = "Time",
-                          title: str = "Cross Validation Procedure") -> None:
+                          title: str = "Cross Validation Procedure"
+                          ) -> None:
         """
         Plot the cross-validation procedure.
 
-        Parameters
-        
+        Parameters:
+        -----------        
             ax : plt.Axes, optional
                 The Axes object for the plot.
             labels : List[str], optional
                 Labels for the plot. Default is ["Window", "Forecasting horizon"].
             ylabel : str, optional
                 Label for the y-axis. Default is "Window number".
             xlabel : str, optional
                 Label for the x-axis. Default is "Time".
             title : str, optional
                 The title of the plot. Default is "Cross Validation Procedure".
 
-        Returns
-        
+        Returns:
+        --------        
             None
         """
 
         _train_windows, _test_windows = self._get_windows()
-        self._plot_windows(_train_windows, _test_windows,
-                           ax = ax,
-                           labels = labels,
-                           xlabel = xlabel, 
-                           ylabel = ylabel,
-                           title = title)
-
+        if labels is None:
+            labels = ["Window", "Forecasting horizon"]
+            
+        return plot_windows(self.y, 
+                            _train_windows,
+                            _test_windows,
+                            ax = ax,
+                            labels = labels,
+                            xlabel = xlabel, 
+                            ylabel = ylabel,
+                            title = title)
 
     def plot_prediction(self,
                         y_pred: pd.Series,
                         y_pred_ints: Optional[pd.DataFrame] = None,
-                        interval_label: str = 'prediction interval',
-                        labels: List[str] = ["y_train", "y_pred"],
+                        interval_label: str = 'CI',
+                        labels: List[str] = None,
                         xlabel: Optional[str] = None,
                         ylabel: Optional[str] = None,
                         title: str = 'Prediction',
                         ax: Optional[plt.Axes] = None,
                         figsize: Tuple[float, float] = (15, 6)):
         """
         Plot the forecast predictions and the confidence intervals.
 
-        Parameters
-        
+        Parameters:
+        ----------        
             y_pred : pd.Series
                 The predicted values.
             y_pred_ints : pd.DataFrame, optional
                 The DataFrame containing the prediction intervals.
             interval_label : str, optional
                 Label for the prediction interval. Default is 'prediction interval'.
             labels : List[str], optional
@@ -613,48 +590,50 @@
             title : str, optional
                 The title of the plot. Default is 'Prediction'.
             ax : plt.Axes, optional
                 The Axes object for the plot.
             figsize : Tuple[float, float], optional
                 The figure size. Default is (15, 6).
 
-        Returns
-        
+        Returns:
+        -------        
             None
         """
 
         y = self.y
         y_train = y.loc[y.index<y_pred.index[0]]
-        zoom_y_train = y_train.iloc[-5*len(y_pred):]	
+        zoom_y_train = y_train.iloc[-3*len(y_pred):]	
+        if labels is None:
+            labels = ["y_train", "y_pred"]
         return plot_series(zoom_y_train, y_pred,
                            labels= labels,
                            pred_interval=y_pred_ints,	
-                           interval_label ='prediction interval',
+                           interval_label = interval_label,
                            xlabel = xlabel,
                            ylabel = ylabel,
                            title = title, 
                            ax = ax,
                            figsize = figsize
                           )
 
     def plot_prediction_true(self,
                              y_pred: pd.Series,
                              y_pred_ints: Optional[pd.DataFrame] = None,
-                             interval_label: str = 'prediction interval',
-                             labels: List[str] = ["y_train", "y_true", "y_pred"],
+                             interval_label: str = 'CI',
+                             labels: List[str] = None,
                              xlabel: Optional[str] = None,
                              ylabel: Optional[str] = None,
                              title: str = 'Prediction',
                              ax: Optional[plt.Axes] = None,
                              figsize: Tuple[float, float] = (15, 6)):
         """
         Plot the forecast predictions, true values, and the confidence intervals.
 
-        Parameters
-        
+        Parameters:
+        -----------        
             y_pred : pd.Series
                 The predicted values.
             y_pred_ints : pd.DataFrame, optional
                 The DataFrame containing the prediction intervals.
             interval_label : str, optional
                 Label for the prediction interval. Default is 'prediction interval'.
             labels : List[str], optional
@@ -666,504 +645,401 @@
             title : str, optional
                 The title of the plot. Default is 'Prediction'.
             ax : plt.Axes, optional
                 The Axes object for the plot.
             figsize : Tuple[float, float], optional
                 The figure size. Default is (15, 6).
 
-        Returns
-        
+        Returns:
+        --------        
             None
         """
 
         y = self.y
         y_train = y.loc[y.index<y_pred.index[0]]
         zoom_y_train = y_train.iloc[-5*len(y_pred):]
         true_pred_idx = np.intersect1d(y.index, y_pred.index)
         err_msg = 'No overlap between true values and predicted values.\nIf you want to plot prediction alone use the function plot_prediction'
         assert len(true_pred_idx)>0, err_msg
         y_true = self.y[true_pred_idx]
+        if labels is None:
+            labels = ["y_train", "y_true", "y_pred"]
 
         return plot_series(zoom_y_train, y_true, y_pred,
                            pred_interval=y_pred_ints,
-                           interval_label ='prediction interval',
+                           interval_label =interval_label,
                            labels=labels, 
                            xlabel = xlabel,
                            ylabel = ylabel,
                            title = title, 
                            ax = ax,
                            figsize = figsize)
 
-    def _plot_windows(self,
-                      train_windows: List[np.ndarray],
-                      test_windows: List[np.ndarray],
-                      ax: plt.Axes,
-                      labels: List[str],
-                      ylabel: str,
-                      xlabel: str,
-                      title: str) -> None:
-        """
-        Visualize training and test windows.
-
-        Parameters
-        
-            train_windows : List[np.ndarray]
-                List of training window indices.
-            test_windows : List[np.ndarray]
-                List of test window indices.
-            ax : plt.Axes
-                The Axes object for the plot.
-            labels : List[str]
-                Labels for the plot.
-            ylabel : str
-                Label for the y-axis.
-            xlabel : str
-                Label for the x-axis.
-            title : str
-                The title of the plot.
-
-        Returns
-        
-            None
-        """
-        assert len(labels)==2, 'wrong number of labels'
-        simplefilter("ignore", category=UserWarning)
-
-        def get_y(length, split):
-            # Create a constant vector based on the split for y-axis."""
-            return np.ones(length) * split
-        reformat_xticks = lambda x: x if x=='' else pd.to_datetime(x).strftime('%Y-%m-%d')
-
-        n_splits = len(train_windows)
-        n_timepoints = len(self.y)
-        len_test = len(test_windows[0])
-
-        train_color, test_color = sns.color_palette("colorblind")[:2]
-
-        if ax is None:
-            f, ax = plt.subplots(figsize=plt.figaspect(0.3))
-
-        for i in range(n_splits):
-            train = train_windows[i]
-            test = test_windows[i]
-
-            ax.plot(
-                np.arange(n_timepoints), get_y(n_timepoints, i), marker="o", c="lightgray"
-            )
-            ax.plot(
-                train,
-                get_y(len(train), i),
-                marker="o",
-                c=train_color,
-                label=labels[0],
-            )
-            ax.plot(
-                test,
-                get_y(len_test, i),
-                marker="o",
-                c=test_color,
-                label=labels[1],
-            )
-        #import pdb; pdb.set_trace()
-        xticklabels = [int(item) for item in ax.get_xticks()[1:-1]]
-        xticklabels = [''] + [self.y.index[i].strftime('%Y-%m-%d') for i in xticklabels] + ['']
-        ax.invert_yaxis()
-        ax.yaxis.set_major_locator(MaxNLocator(integer=True))
-        ax.set(
-            title=title,
-            ylabel=ylabel,
-            xlabel=xlabel,
-            xticklabels = xticklabels,
-        )
-        # remove duplicate labels/handles
-        handles, labels = [(leg[:2]) for leg in ax.get_legend_handles_labels()]
-        ax.legend(handles, labels, frameon=False)
-
-        if ax is None:			
-            return f, ax
-        else:
-            return ax
-
-
     def _get_windows(self) -> Tuple[List[np.ndarray], List[np.ndarray]]:
         """
         Generate windows for the cross-validation procedure.
 
-        Returns
-        
+        Returns:
+        --------
             tuple:
                 A tuple containing two lists: train_windows and test_windows.
         """
         _train_windows = []
         _test_windows = []
         _y_index = self.y.index 
-        for i, (_train, _test) in enumerate(self.cv.split(_y_index)):
+        for _train, _test in self.cv.split(_y_index):
             _train_windows.append(_train)
             _test_windows.append(_test)
         return _train_windows, _test_windows 
 
-
 ##############################################################################
 # Model Fit and Insample Performance
 ##############################################################################
+def compute_predictions(params):
+    forecaster, X, intrain, intest, verbose = params
+    fh = ForecastingHorizon(intest.index, is_relative=False)
+    try:
+        in_pred = forecaster.predict(fh=fh, X=X).rename('y_pred').reset_index()
+        in_pred['y_true'] = intest.values
+        in_pred['error'] = in_pred['y_true'] - in_pred['y_pred']
+        in_pred['error_pct'] = in_pred['error'].abs()/in_pred['y_true']
+        in_pred.insert(0, 'horizon', np.arange(1, len(in_pred) + 1))
+        in_pred.insert(0, 'cutoff', intrain.index[-1])        
+    except Exception as e:
+        if verbose:
+            print(f"Error occured in {intrain.index[-1]}: {e}")
+        in_pred = pd.DataFrame()
+    return in_pred
 class ForecastFit:
     """
     Class for fitting the forecast model and computing insample performance metrics.
 
-    Parameters
-    
+    Parameters:
+    -----------    
         Forecast : Forecast
             An instance of the Forecast class.
-
-    Returns
-    
-        None
     """
 
-    def __init__(self, Forecast: Forecast):
-        """
-        Initialize the ForecastFit object.
-
-        Parameters
-        
-            Forecast : Forecast
-                An instance of the Forecast class.
-        """
-
-        self.__dict__.update(Forecast.__dict__)
-
+    def __init__(self, LF: Forecast):
+        self.forecaster = LF.forecaster
+        self.forecaster_name = LF.forecaster_name
+        self.is_fitted = LF.is_fitted
+        self.y_train = LF.y_train
+        self.y = LF.y
+        self.X = LF.X
+        self.fh = LF.fh
+        self.cv = LF.cv
         self.plot = self.__plot()
 
+        self.insample_result_df = None
+        self.insample_perf_summary = None
 
-    def insample_predictions(self, nsample: int = 100) -> pd.DataFrame:
+    def insample_predictions(self, random_sample=False, nsample: int = 100, verbose=False) -> pd.DataFrame:
         """
         Compute the insample predictions for the fitted model.
 
-        Parameters
-        
+        Parameters:
+        -----------        
             nsample : int, optional
                 The number of samples to compute. Default is 100.
 
-        Returns
-        
+        Returns:
+        --------        
             pd.DataFrame
                 A DataFrame containing the insample predictions.
         """
 
-        assert self.forecaster.is_fitted, 'Fit the forecast on the training window first before you can evaluate the insample performance'
-
-        _cutoffs = np.random.choice(len(self.y_train)-len(self.fh), size=nsample, replace=False)
-
-        cv_in = CutoffSplitter(cutoffs=_cutoffs, window_length=1, fh=self.fh)
-
-        insample_result = []                
-        for i, (intrain, intest) in tqdm(enumerate(cv_in.split_series(self.y_train))):
-            fh = ForecastingHorizon(intest.index, is_relative=False)
-
-            # Apply forecaster to predict the past
-            in_pred = self.forecaster.predict(fh=fh, X=self.X).rename('y_pred').reset_index()
-            in_pred['y_true'] = intest.values
-            in_pred['Abs_diff'] = (in_pred['y_true'] - in_pred['y_pred']).abs()
-            in_pred['horizon'] = np.arange(1, len(in_pred)+1)
-            in_pred['cutoff'] = intrain.index[-1]
+        if self.is_fitted:
+            _y = self.y
+        else:
+            _y = self.y_train
 
-            insample_result.append(in_pred)
+        insample_eval_window = len(_y) - len(self.fh)
+        if random_sample:            
+            nsample = max(insample_eval_window, nsample)
+            # Randomly selecting cutoff points
+            _cutoffs = np.random.choice(insample_eval_window, size=nsample, replace=False)
+            cv_in = CutoffSplitter(cutoffs=_cutoffs, window_length=1, fh=self.fh)
+        else:
+            _cutoffs = np.arange(insample_eval_window)
+            cv_in = ExpandingWindowSplitter(initial_window=1, step_length=1, fh=self.fh)
+        if verbose:
+            print(f"\nComputing {self.forecaster_name} forecaster historic predictions....")        
+
+        params = [(self.forecaster, self.X, intrain, intest, verbose) for intrain, intest in cv_in.split_series(_y)]                
+        with Pool() as pool:
+            insample_result = list(tqdm(pool.imap(compute_predictions, params), total=len(params)))
 
         insample_result_df = pd.concat(insample_result)
+        if insample_result_df.empty:
+            print(f"No insample predictions computed {self.forecaster_name}")
+        if verbose:
+            print(f"\n{self.forecaster_name} forecaster historic predictions completed")        
         self.insample_result_df = insample_result_df
         return insample_result_df
 
     def insample_perf(self) -> dict:
         """
         Compute insample performance metrics (RMSE and MAPE) for the fitted model.
 
-        Returns
-        
+        Returns:
+        --------        
             dict
                 A dictionary containing the computed insample performance metrics.
         """
 
-        if 'insample_result_df' in self.__dict__.keys():
-            pass
-        else:           
-            self.insample_result_df = self.insample_predictions()
+        if self.insample_result_df is None:
+            self.insample_predictions()
 
         insample_perf_summary = {
             'cutoff': summary_perf(self.insample_result_df, grouper = 'cutoff', y_true_col = 'y_true', y_pred_col = 'y_pred'),
-            'horizon': summary_perf(self.insample_result_df, grouper = 'horizon', y_true_col = 'y_true', y_pred_col = 'y_pred')
+            'horizon':summary_perf(self.insample_result_df, grouper = 'horizon', y_true_col = 'y_true', y_pred_col = 'y_pred')
         }
         self.insample_perf_summary = insample_perf_summary
         return insample_perf_summary
 
     def __plot(self):
         return ForecastFitPlot(self)
 
 class ForecastFitPlot:
     """
     Plotting utility class for ForecastFit.
 
-    Parameters
-    
+    Parameters:
+    -----------    
         LFF : ForecastFit
             An instance of the ForecastFit class.
-
-    Returns
-    
-        None
     """
 
     def __init__(self, LFF: ForecastFit):
-        """
-        Initialize the ForecastFitPlot object.
-
-        Parameters
-        
-            LFF : ForecastFit
-                An instance of the ForecastFit class.
-        """
-
-        self.__dict__.update(LFF.__dict__)
         self.LFF = LFF
 
     def plot_insample_performance(self,
                                   metric: str = 'RMSE',
                                   title: str = 'Insample Performance'):
         """
         Plot the insample performance metrics.
 
-        Parameters
-        
+        Parameters:
+        -----------        
             metric : str, optional
                 The performance metric to plot. Default is 'RMSE'.
             title : str, optional
                 The title of the plot. Default is 'Insample Performance'.
+
+        Returns:
+        --------        
+            fig : plt.Figure
+                The Figure object containing the plot.
+            axes : np.array
+                An array of Axes objects containing the plot.
         """
 
         assert metric in ['RMSE', 'MAPE'], f'{metric} not in summary performance'
         if 'insample_perf_summary' not in self.__dict__.keys():
             insample_perf_summary = self.LFF.insample_perf()
 
         f, axes = plt.subplots(1,2,figsize=(15,5))
         for i, (_grouper, _df) in enumerate(insample_perf_summary.items()):
             _df[metric].plot(ax= axes[i], style = '-o', title = f'{metric} By {_grouper}')
             axes[i].set_xlabel('')
 
         plt.suptitle(title)
         plt.tight_layout()                   
-
+        return f, axes
 
 ##############################################################################
 # Model Out of Sample Evaluation
 ##############################################################################
-
 class ForecastEval:
     """
     Class for evaluating the forecaster out-of-sample.
 
-    Parameters
-    
+    Parameters:
+    -----------    
         Forecast : Forecast
             An instance of the Forecast class.
-
-    Returns
-    
-        None
     """
 
-    def __init__(self, Forecast: Forecast):
-        """
-        Initialize the ForecastEval object.
-
-        Parameters
+    def __init__(self, LF: Forecast):
         
-            Forecast : Forecast
-                An instance of the Forecast class.
-        """
-
-        self.__dict__.update(Forecast.__dict__)     
+        self.forecaster = LF.forecaster
+        self.forecaster_name = LF.forecaster_name
+        self.y = LF.y
+        self.X = LF.X
+        self.cv = LF.cv
 
         self.scoring_metrics = [MeanSquaredError(square_root=True),
-                                MeanAbsolutePercentageError()]
+                                MeanAbsoluteError(),
+                                MeanAbsolutePercentageError(), 
+                                MedianAbsoluteError(),
+                                ]
+
         _rename_metrics = {
             'test_MeanSquaredError':'RMSE', 
-            'test_MeanAbsolutePercentageError':'MAPE'
+            'test_MeanAbsoluteError':'MAE',
+            'test_MeanAbsolutePercentageError':'MAPE',
+            'test_MedianAbsoluteError':'MedianAE',
         }
-        print(f"\nStart forecaster {self.forecaster_name} evalution....")
-        print(" Depending on the forecaster this step may take couple of minutes. Please don't kill the kernel")
+        print(f"\nStart {self.forecaster_name} forecaster evalution....")
         st = time.time()
         self.oos_eval = evaluate(forecaster=self.forecaster, 
                             y=self.y,
                             X = self.X,
                             cv=self.cv,
                             strategy="refit",
                             return_data=True,
                             scoring = self.scoring_metrics,
                             backend ='loky',
                            )
         self.oos_eval = self.oos_eval.set_index('cutoff').sort_index()
         self.oos_eval = self.oos_eval.rename(columns = _rename_metrics)
         et = time.time()
         elapsed_time = et - st
-        print(f"Evaluation time: {np.around(elapsed_time / 60,3)} minutes")
+        print(f"Evaluation completed in: {np.around(elapsed_time / 60,3)} minutes")
 
         convert_horizon = self.oos_eval.apply(self.__eval_horizon, axis=1)
+        
         self.oos_horizon_df = pd.concat(convert_horizon.values)
+        self.oos_horizon_perf = summary_perf(self.oos_horizon_df, 
+                                             grouper='horizon', 
+                                             y_true_col = 'y_test', 
+                                             y_pred_col = 'y_pred')
+        self.oos_cutoff_perf = summary_perf(self.oos_horizon_df, 
+                                             grouper='cutoff', 
+                                             y_true_col = 'y_test', 
+                                             y_pred_col = 'y_pred')
 
         self.plot = self.__plot()
-
+        return None
 
     def summary_results(self) -> pd.DataFrame:
         """
         Generate a summary of out-of-sample forecast results.
 
-        Returns
-        
+        Returns:
+        --------        
             pd.DataFrame
                 A DataFrame containing various summary statistics of the out-of-sample forecasts.
         """
 
-        _summary = {'Number of Folds':  self.oos_eval.shape[0], 
+        _summary = {
+         'Number of Folds':  self.oos_eval.shape[0], 
          'Avg Fit time (s)': self.oos_eval.fit_time.mean(),
          'Avg_pred_time (s)': self.oos_eval.pred_time.mean(),
          'Smallest training window': self.oos_eval.len_train_window.min(),
          'Largest training window':self.oos_eval.len_train_window.max(),
          'First cutoff': self.oos_eval.index[0],
          'Last cutoff': self.oos_eval.index[-1],
-         'Avg MAPE': self.oos_eval.MAPE.mean(),
-         'Avg RMSE': self.oos_eval.RMSE.mean()
         }
+        for _s in self.oos_cutoff_perf.columns:
+            _summary[f'Avg {_s}'] = self.oos_cutoff_perf[_s].mean()
         return pd.Series(_summary).to_frame().T
 
-    def summary_horizon(self) -> pd.DataFrame:
+    def summary_cutoff(self) -> pd.DataFrame:
         """
-        Generate a summary of out-of-sample forecast results per horizon.
+        Generate a summary of out-of-sample performance per cutoff.
 
-        Returns
-        
+        Returns:
+        --------        
             pd.DataFrame
                 A DataFrame containing summary performance metrics (RMSE and MAPE) for each horizon.
+        """        
+        return self.oos_cutoff_perf
+
+    def summary_horizon(self) -> pd.DataFrame:
         """
+        Generate a summary of out-of-sample performance per horizon.
 
-        self.oos_horizon_perf = summary_perf(self.oos_horizon_df, grouper='horizon', y_true_col = 'y_test', y_pred_col = 'y_pred')        
+        Returns:
+        --------        
+            pd.DataFrame
+                A DataFrame containing summary performance metrics (RMSE and MAPE) for each horizon.
+        """        
         return self.oos_horizon_perf
 
     def __eval_horizon(self, x):
-            _fct = pd.concat([x['y_test'], x['y_pred']], keys=['y_test', 'y_pred'], axis=1)
-            _fct['Abs_diff'] = (_fct['y_test'] - _fct['y_pred']).abs()        
-            _fct['horizon'] = np.arange(1, len(_fct)+1)    
-            _fct['cutoff'] = x.name
-            return _fct
+        _fct = pd.concat([x['y_test'], x['y_pred']], keys=['y_test', 'y_pred'], axis=1)
+        _fct['error'] = _fct['y_test'] - _fct['y_pred']
+        _fct['error_pct'] = _fct['error'].abs()/ _fct['y_test']
+        _fct['horizon'] = np.arange(1, len(_fct)+1)    
+        _fct['cutoff'] = x.name
+        return _fct
 
     def __plot(self):
         return ForecastEvalPlot(self)
 
 class ForecastEvalPlot:
     """
     Plotting utility class for ForecastEval.
 
-    Parameters
-    
+    Parameters:
+    -----------    
         LFE : ForecastEval
             An instance of the ForecastEval class.
-
-    Returns
-    
-        None
     """
 
     def __init__(self, LFE: ForecastEval):
-        """
-        Initialize the ForecastEvalPlot object.
-
-        Parameters
-        
-            LFE : ForecastEval
-                An instance of the ForecastEval class.
-        """
-
-        self.__dict__.update(LFE.__dict__)
-        self.LFE = LFE
+        self.oos_horizon_perf = LFE.oos_horizon_perf
+        self.oos_cutoff_perf = LFE.oos_cutoff_perf
+        return None
 
     def plot_oos_score(self,
                        score: str = 'RMSE',
+                       view: str = 'horizon', 
                        xlabel: str = None,
                        ylabel: str = None,
-                       title: str = 'Out of Sample Performance - Average on All Horizons',
+                       title: str = 'Out of Sample Performance',
                        ax: Optional[plt.Axes] = None,
                        figsize: Tuple[float, float] = (15, 6)):
         """
         Plot out-of-sample performance metric historically.
 
-        Parameters
-        
+        Parameters:
+        -----------        
             score : str, optional
                 The performance metric to plot. Default is 'RMSE'.
+            view: str, optional
+                The view of the plot. It must be either 
+                    - horizon: the function plots the average score per forecast horizon
+                    - cutoff: the function plots the average across all horizons for each cutoff                
+                Default is 'horizon'.
             xlabel : str, optional
                 Label for the x-axis.
             ylabel : str, optional
                 Label for the y-axis.
             title : str, optional
-                The title of the plot. Default is 'Out of Sample Performance - Average on All Horizons'.
+                The title of the plot. Default is 'Out of Sample Performance'.
             ax : plt.Axes, optional
                 The Axes object for the plot.
             figsize : Tuple[float, float], optional
                 The figure size. Default is (15, 6).
-        """
-
-        assert score in self.oos_eval.columns, 'score not computed'
-        if ax is None:
-            f, ax = plt.subplots(1,1,figsize=figsize)
-
-        ylabel = score if ylabel is None else ylabel
-        xlabel = '' if xlabel is None else xlabel
-        self.oos_eval[score].plot(ax = ax, style = '-o')
-        ax.set(xlabel = xlabel, ylabel=ylabel, title =title)
-
-        if ax is None:
-            return f, ax
-        else:
-            return ax
-
-    def plot_oos_horizon(self,
-                         score: str = 'RMSE',
-                         xlabel: str = None,
-                         ylabel: str = None,
-                         title: str = 'Out of Sample Performance - Average per Horizons',
-                         ax: Optional[plt.Axes] = None,
-                         figsize: Tuple[float, float] = (15, 6)):
-        """
-        Plot out-of-sample performance metric per horizon.
-
-        Parameters
         
-            score : str, optional
-                The performance metric to plot. Default is 'RMSE'.
-            xlabel : str, optional
-                Label for the x-axis.
-            ylabel : str, optional
-                Label for the y-axis.
-            title : str, optional
-                The title of the plot. Default is 'Out of Sample Performance - Average per Horizons'.
-            ax : plt.Axes, optional
-                The Axes object for the plot.
-            figsize : Tuple[float, float], optional
-                The figure size. Default is (15, 6).
-        """
-        if 'oos_horizon_perf' not in self.__dict__.keys():
-            oos_horizon_perf = self.LFE.summary_horizon()
+        Returns:
+        --------        
+            fig : plt.Figure
+                The Figure object containing the plot.
+            axes : np.array
+                An array of Axes objects containing the plot.
 
-        assert score in oos_horizon_perf.columns, 'score not computed'
+        """
+        if view == 'horizon':
+            assert score in self.oos_horizon_perf.columns, 'score not computed'
+            to_plot = self.oos_horizon_perf[score]
+        elif view == 'cutoff':
+            assert score in self.oos_cutoff_perf.columns, 'score not computed'
+            to_plot = self.oos_cutoff_perf[score]
+        else:
+            raise ValueError('view should be either horizon or cutoff')
 
         if ax is None:
             f, ax = plt.subplots(1,1,figsize=figsize)
 
         ylabel = score if ylabel is None else ylabel
-        xlabel = '' if xlabel is None else xlabel
-        
-        oos_horizon_perf[score].plot(ax = ax, style = '-o')
-        ax.set(xlabel = xlabel, ylabel=ylabel, title =title)
-
+        xlabel = '' if xlabel is None else xlabel        
+        to_plot.plot(ax = ax, style = '-o')                    
+        ax.set(xlabel = xlabel, ylabel=ylabel)
+        ax.set_title(title, size ='xx-large')
         if ax is None:
             return f, ax
         else:
-            return ax
-
+            return ax
```

### Comparing `forecast_combine-0.0.1/forecast_combine/model_select.py` & `forecast_combine-0.0.2/forecast_combine/model_select.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,332 +1,415 @@
+""" Combination of timeseries Forecasts"""
+__description__ = "Time Series Forecast Combination"
+__author__ = "Amine Raboun - amineraboun@github.io"
+
+import logging
+logging.getLogger().setLevel(logging.ERROR)
+import warnings
+warnings.filterwarnings("ignore")
+warnings.simplefilter("ignore", category=FutureWarning)
+warnings.simplefilter("ignore", category=DeprecationWarning)
+
+##############################################################################
+# Import Libraries & default configuration 
+##############################################################################
 import pandas as pd
 import numpy as np
-import os
-import matplotlib.pyplot as plt
-import seaborn as sns
-
 from typing import Union, Optional, Tuple, List, Dict, Any
 
-from warnings import simplefilter
-simplefilter('ignore')
+from .forecast import Forecast
+from .forecast import CommonForecastingModels
+from .utils.plotting import plot_series
+from sktime.forecasting.base import ForecastingHorizon
 
-from forecast_combine.forecast import *
-from forecast_combine.utils.plotting import plot_series
+import matplotlib.pyplot as plt
+plt.rc('axes', titlesize='x-large')    
+plt.rc('axes', labelsize='large')   
+plt.rc('xtick', labelsize='large')   
+plt.rc('ytick', labelsize='large')   
+plt.rc('legend', fontsize='large')   
+plt.rc('figure', titlesize='x-large') 
+import seaborn as sns
+sns.set_theme(style='white', font_scale=1)
 
-##############################################################################
-# Model Selection
-##############################################################################
+from concurrent.futures import ProcessPoolExecutor
+def fetch_errors(item):
+    _fname, _lf = item
+    return _fname, _lf.get_pred_errors()
 
-class ForecastModelSelect:
 
+class ForecastModelSelect:
     """
     Class for model selection and comparison based on out-of-sample performance.
     Evaluate how to best combine the different models based on their oos performance.
 
     The class can be initialized in 2 ways. 
         Method 1: Requires a list of Forecast objects. It is the preferable instantiation if the models have already been evaluated out of sample.
 
         Method 2: Requires all the arguments taken by Forecast plus a dictionary where the keys are names of forecasts and the values are the forecast_models.
 
-    Parameters
-    
-        LF_list : list[Forecast], optional
-            List of Forecast objects. Default is None.
-        models_d : dict, optional
-            A dictionary containing various forecasting models for comparison. Default is None.
+    Parameters:
+    -----------    
+        forecasters_d : dict, optional
+            A dictionary containing various forecasting models for comparison. 
+            Default is None and assess the most common forecasting models.
+                Naive: NaiveForecaster - Keep the latest value
+                AutoARIMA: StatsForecastAutoARIMA - Auto ARIMA model
+                AutoETS: StatsForecastAutoETS - Auto ETS model
+                AutoTheta: StatsForecastAutoTheta - Auto Theta model
+                TBATS: StatsForecastAutoTBATS - TBATS model
+                LOESS: StatsForecastMSTL - LOESS model
+                Prophet: Prophet - Prophet model
+        trained_forecasters_d : dict, optional
+            A dictionary containing trained Forecast objects. Default is None.
         mode : str, optional
             The aggregation mode. Default is 'nbest_average_horizon'.
         score : str, optional
             The performance score. Default is 'RMSE'.
         nbest : int, optional
             Number of best models to aggregate. Default is 2.
         kwargs
             Additional keyword arguments to be passed to the Forecast initialization.
 
-    Raises
-    
+    Raises:
+    -------    
         AssertionError
             If the mode, score, or nbest values are not recognized or do not meet the requirements.
-            If both LF_list and models_d are None.
+            If both LF_list and forecasters_d are None.
     """
 
     def __init__(self, 
-                 LF_list: Optional[List[Forecast]] = None,
-                 models_d: Optional[Dict] = None,
-                 mode: str = 'nbest_average_horizon',
+                 forecasters_d: Optional[Dict] = None,
+                 trained_forecasters_d: Optional[Dict] = None,
+                 model_exog_d: Optional[Dict] = None,
+                 mode: str = 'best_horizon',
                  score: str = 'RMSE',
-                 nbest: int = 2,
+                 nbest: int = None,
                  **kwargs: Any
                 ) -> None:
-        """
-        Initialize the ForecastModelSelect instance.
-
-        Parameters
-        
-            LF_list : list[Forecast], optional
-                List of Forecast objects. Default is None.
-            models_d : dict, optional
-                A dictionary containing various forecasting models for comparison. Default is None.
-            mode : str, optional
-                The aggregation mode. Default is 'nbest_average_horizon'.
-            score : str, optional
-                The performance score. Default is 'RMSE'.
-            nbest : int, optional
-                Number of best models to aggregate. Default is 2.
-            **kwargs
-                Additional keyword arguments to be passed to the Forecast initialization.
 
-        Raises
+        lf_d = {}
+        if (trained_forecasters_d is not None):
+            # Trained Models must be istance of Forecast object
+            assert len(set(forecasters_d.keys()).intersection(set(trained_forecasters_d.keys()))) == 0, 'There is an overlap between the two trained and non trainded dictionaries' 
+            if (forecasters_d is not None):
+                # There must be no overlap between the two dictionaries
+                assert all([isinstance(_lf, Forecast) for _lf in trained_forecasters_d.values()]), 'Trained models must be instances of Forecast object'
+            for forecaster_name, _lf in trained_forecasters_d.items():
+                lf_d[forecaster_name] = _lf        
+        else:
+            if (forecasters_d is None):
+                forecasters_d = CommonForecastingModels
         
-            AssertionError
-                If the mode, score, or nbest values are not recognized or do not meet the requirements.
-                If both LF_list and models_d are None.
-        """
-        self.__init_test(mode, score, nbest)
-
-        if LF_list is not None:
-            self.LF_list = LF_list
-
+        # Define the Forecasters exogenous variables
+        exog_l = kwargs.pop('exog_l', None)
+        if model_exog_d is None:
+            model_exog_d = {forecaster_name: exog_l for forecaster_name in forecasters_d.keys()}
         else:
-
-            assert models_d is not None, 'You must have either the models_d or the LF_list not empty'
-            lf_l = []
-            for forecaster_name, forecaster in models_d.items():            
+            exog_l = [] if exog_l is None else exog_l
+            for forecaster_name in forecasters_d.keys():
+                model_exog_d[forecaster_name] = exog_l + model_exog_d.get(forecaster_name, [])
+        
+        if forecasters_d is not None:
+            for forecaster_name, forecaster in forecasters_d.items():            
                 _lf =  Forecast(
                     forecaster_name = forecaster_name,
                     forecaster = forecaster,
+                    exog_l = model_exog_d[forecaster_name],
                     **kwargs
                 )
-                lf_l.append(_lf)
-            self.LF_list = lf_l		
+                lf_d[forecaster_name] = _lf
+                           
+        self.LF_d = lf_d
+
+        assert isinstance(mode, str), 'mode must be a sting'
+        recog_modes = ['best', 'best_horizon', 'average', 'inverse_score', 
+                           'nbest_average', 'nbest_average_horizon']
+        assert mode in recog_modes, f'mode function not implemented!. Recognized modes are {recog_modes}'
+        self.mode = mode
+
+        recog_scores = ['RMSE', 'MAE', 'MAPE', 'R2', 'MedianAE']
+        assert score in recog_scores, f'performance score not implemented!. Recognized scores are {recog_scores}'		
+        self.score = score
+
+        if nbest is None:
+            nbest = 2
+        else:
+            assert isinstance(nbest, int), 'n best must be an integer'		
+        self.nbest = min(nbest, len(self.LF_d))	
+
+        self.eval_models = None
+        self.summary_horizon = None
+        self.summary_results = None
+        self.best_x_overall = None
+        self.model_rank_perhorizon = None
+        self.avg_oos_horizon = None
+        self.avg_oos_hist = None
         return None
 
-    def add_forecast(self, 
-                     lf: Forecast) -> None:
+    def split_procedure_summary(self):
+        """
+        Print the summary of the split procedure for each model.
+
+        Returns:
+        --------        
+            dict:
+                A dictionary containing details of the cross-validation procedure, including:
+                the number of folds, initial window size, step length, and forecast period.
+        """
+        _lf  = list(self.LF_d.values())[0]
+        return _lf.split_procedure_summary()
+    
+    def add_forecaster(self, 
+                       forecaster_name: str,
+                       lf: Forecast) -> None:
         """
         Add a Forecast Object to the list of models to evaluate.
 
         Parameters:
+        -----------
             lf : Forecast
                 The Forecast object to be added.
         """
-        self.LF_list.append(lf)
-        return self.LF_list
-
+        assert forecaster_name not in self.LF_d.keys(), 'Forecaster name already exists in the considered list of model'
+        self.LF_d[forecaster_name] = lf
+        return self.LF_d
 
     def fit(self, 
             on: str = 'all', 
             fh: Optional[ForecastingHorizon] = None, 
-            force: bool = False
+            force: bool = False,
+            verbose: bool = False
            ) -> None:
         """
         Fit the forecasting models for all the underlying Forecast objects.
 
-        Parameters
-        
+        Parameters:
+        -----------        
             on : str, optional
                 The period for the in-sample fitting. Default is 'all'.
             fh : ForecastingHorizon, optional
                 The forecasting horizon. Default is None and it takes the value entered at initialization..
             force : bool, optional
                 If True, force fitting even if the models are already fitted. Default is False.
 
-        Returns
-        
+        Returns:
+        --------        
             None
         """
-        for _lf in self.LF_list:
+        for _lfname, _lf in self.LF_d.items():
+            if verbose:
+                print(f'Fitting {_lfname} ...')
             if (_lf.is_fitted) and force ==False:
                 pass
             else:
                 _lf.fit(on=on, fh=fh)
         return None
 
     def evaluate(self,
                  force: bool = False
                 ) -> Tuple:
         """
         Evaluate the underlying Forecast models out of sample.
 
-        Parameters
-        
+        Parameters:
+        -----------
             force : bool, optional
                 If True, force the evaluation even if the models are already evaluated. Default is False.
 
-        Returns
-        
+        Returns:
+        --------
             tuple
                 A tuple containing the summary of out-of-sample performance per horizon and per model.
         """
         #Step 1: Loop on all models and evaluate them
         _model_evals = []
-        for _lf in self.LF_list:
+        _todrop_evals = []
+        for _fname, _lf in self.LF_d.items():
             if (_lf.is_evaluated) and force ==False:
                 _model_evals.append(_lf.eval)
-                pass
             else:
-                _model_evals.append(_lf.evaluate())
+                try:
+                    _eval = _lf.evaluate()
+                    _model_evals.append(_eval)
+                except Exception as e:
+                    print(f'Error evaluating {_fname}: {e}')
+                    print(f'\nmodel {_fname} cannot be evaluated. It will be removed from the list of models')
+                    _todrop_evals.append(_fname)
+                    continue                
+        if len(_todrop_evals)>0:
+            for _fname in _todrop_evals:
+                self.LF_d.pop(_fname)
         self.eval_models = _model_evals
 
         # Step 2: Get the OOS Summary of Performance 
         #per horizon and per model
         _sum_h = {}; _sum_T = {}
         for _lf_eval in self.eval_models:            
             _sum_T[_lf_eval.forecaster_name] = _lf_eval.summary_results().squeeze()
             _sum_h[_lf_eval.forecaster_name] = _lf_eval.summary_horizon()
 
-        self.summary_horizon = pd.concat(_sum_h.values(),
-                                         axis=1,
-                                         keys = _sum_h.keys())
-        self.summary_results = pd.concat(_sum_T.values(), 
-                                         axis=1,
-                                         keys = _sum_T.keys())
-
+        self.summary_horizon = pd.concat(_sum_h.values(), axis=1, keys = _sum_h.keys())
+        self.summary_results = pd.concat(_sum_T.values(), axis=1, keys = _sum_T.keys())
         return self.summary_horizon, self.summary_results
 
     def select_best(self,
-
                     score: Optional[str] = None,
-
-                    nbest: Optional[int] = None
-
+                    reestimate = False,
                    ) -> pd.DataFrame:
         """
         Select the best model based on horizon and overall performance.
 
-        Parameters
-        
+        Parameters:
+        -----------        
             score : str, optional
-                The performance metric to use for model comparison. Should be either 'RMSE' or 'MAPE'. Default is None and it takes the value entered at initialization.
+                The performance metric to use for model comparison. Default is None and it takes the value entered at initialization.
             nbest : int, optional
                 The number of best models to select based on horizon performance. Default is None and it takes the value entered at initialization.
 
-        Returns
-        
+        Returns:
+        --------        
             pd.DataFrame
                 model_rank_perhorizon. Rank of models per horizon based on performance.
         """
-
         if score is None:
             score = self.score
 
-        if nbest is None:
-            nbest = self.nbest
+        if (self.model_rank_perhorizon is None) or (self.avg_oos_horizon is None) or reestimate:
 
-        nevals = len(self.LF_list)
-        if nbest > nevals:
-            print(f'\nnbest ={nbest} is higher than the number of models evaluated {nevals}')
-            print(f'The average performance of best models will be computed on {nevals} models instead')
-            nbest = max(nbest, nevals)
-
-        cond1 = 'eval_models' not in self.__dict__.keys()
-        cond2 = 'summary_horizon' not in self.__dict__.keys()
-        if cond1 & cond2:	
-            print('\nTo select best. We have to evaluate the models out of sample')
-            print('Run evaluate ...')
-            self.evaluate()
-
-        self.best_x_overall = {}
-        self.model_rank_perhorizon = {}
-        self.avg_oos_horizon = {}
-        for score in ['RMSE', 'MAPE']:
-
-            r = self.summary_horizon.unstack().unstack(1)[score].unstack()
-
-            # Select best x models based on their average performance on all horizons 
-            best_x_overall = list(r.mean(axis=1).sort_values(ascending=True).index[:nbest])
-
-            # Compute the rank of the models per horizon
-            model_rank_perhorizon = r.apply(lambda x: x.nsmallest(nevals).index.tolist(), axis=0)
-            model_rank_perhorizon = model_rank_perhorizon.reset_index(drop=True)\
-            .rename(index={i: f'Best_{i+1}' for i in range(nevals)})
-
-            # Summary Model average
-            avg_oos_horizon = pd.concat([r.mean(), 
-                                           r.loc[best_x_overall].mean(),
-                                           r.apply(lambda x: x.nsmallest(nbest).mean(), axis=0)
-                                          ], 
-                                         keys = ['Model Avg (all models)',  
-                                          f'Best {nbest} Model (over all)',
-                                          f'Best {nbest} Model (per horizon)'], 
-                                         axis = 1)
-
-            self.avg_oos_horizon[score] = pd.concat([r.T, avg_oos_horizon], axis=1)
-            self.model_rank_perhorizon[score] = model_rank_perhorizon
-            self.best_x_overall[score] = best_x_overall
+            # if models are not evaluated yet, run evaluate
+            cond1 = self.eval_models is None
+            cond2 = self.summary_horizon is None
+            if cond1 or cond2:	
+                print('\nRun evaluate ...')
+                self.evaluate()
 
-        return self.model_rank_perhorizon[score]
+            nevals = len(self.LF_d)
+            nbest = self.nbest
+            if nbest > nevals:
+                print(f'\nnbest ={nbest} is higher than the number of models evaluated {nevals}')
+                print('All models will be considered. The average best models will be equal to the simple average')
+                nbest = max(nbest, nevals)
+
+            best_x_overall = {}
+            model_rank_perhorizon = {}
+            avg_oos_horizon = {}
+            _perf_metrics = list(self.summary_horizon.columns.levels[1])
+            for _s in _perf_metrics:
+                r = self.summary_horizon.unstack().unstack(1)[_s].unstack()
+
+                # Select best x models based on their average performance on all horizons 
+                overall_score = r.mean(axis=1).sort_values(ascending=True)
+                best_overall = overall_score.index[0]
+                _s_best_x_overall = list(overall_score.index[:nbest])
+
+                # Summary Model average
+                _avg_oos_horizon = pd.concat([r.loc[best_overall],
+                                            r.min(),
+                                            r.loc[_s_best_x_overall].mean(),
+                                            r.apply(lambda x: x.nsmallest(nbest).mean(), axis=0),
+                                            r.mean(), 
+                                            ], 
+                                            keys = [
+                                            'Best Model (over all)',
+                                            'Best Model (per horizon)',
+                                            f'Best {nbest} Models (over all)',
+                                            f'Best {nbest} Models (per horizon)',
+                                            'Model Avg (all models)'
+                                            ], 
+                                            axis = 1)
+
+                avg_oos_horizon[_s] = pd.concat([r.T, _avg_oos_horizon], axis=1)
+
+                # Compute the rank of the models per horizon
+                _rank_perhorizon = r.apply(lambda x: x.nsmallest(nevals).index.tolist(), axis=0)\
+                    .reset_index(drop=True).rename(index={i: f'Best_{i+1}' for i in range(nevals)})
+                model_rank_perhorizon[_s] = _rank_perhorizon
+                best_x_overall[_s] = _s_best_x_overall
+            
+            self.best_x_overall = best_x_overall
+            self.model_rank_perhorizon = model_rank_perhorizon
+            self.avg_oos_horizon = avg_oos_horizon
 
+        return self.model_rank_perhorizon[score], self.avg_oos_horizon[score]
 
     def oos_per_cutoff(self,
-                       score: Optional[str] = None,
-                       nbest: Optional[int] = None
+                       score: Optional[str] = None
                       ) -> pd.DataFrame:
         """
         Calculate and return the out-of-sample performance based on cutoffs.
 
-        Parameters
-        
+        Parameters:
+        -----------        
             score : str, optional
                 The performance metric to use for model comparison. Should be either 'RMSE' or 'MAPE'. Default is None and it takes the value entered at initialization.
             nbest : int, optional
                 The number of best models to select based on horizon performance. Default is None and it takes the value entered at initialization.
 
-        Returns
-        
+        Returns:
+        --------        
             pd.DataFrame
                 A DataFrame containing the out-of-sample performance per horizon and per model based on the specified score and nbest values.
-        """
+        """    
         if score is None:
             score = self.score
-
-        if nbest is None:
+        
+        if self.avg_oos_hist is None:
             nbest = self.nbest
-
-        nevals = len(self.LF_list)
-        if nbest > nevals:
-            print(f'\nnbest ={nbest} is higher than the number of models evaluated {nevals}')
-            print(f'The average performance of best models will be computed on {nevals} models instead')
-            nbest = max(nbest, nevals)
-
-        cond = 'eval_models' not in self.__dict__.keys()
-        if cond:
-            print('\nTo select best. We have to evaluate the models out of sample')
-            print('Run evaluate ...')
-            self.evaluate()
-
-        avg_oos_hist = {}
-        for score in ['RMSE', 'MAPE']:
-            _oos = {_lf_eval.forecaster_name:_lf_eval.oos_eval[score] for _lf_eval in self.eval_models}
-            _oos = pd.concat(_oos.values(),  axis=1, keys= _oos.keys())
-
-            nbest_mods = list(_oos.mean().nsmallest(nbest).index)
-            _aggs = pd.concat([_oos.mean(axis=1), 
-                                             _oos[nbest_mods].mean(axis=1)
-                                            ], axis = 1,  keys = ['Model Avg (all models)',  
-                                                                  f'Best {nbest} Model (over all)']
-                                           )
-            avg_oos_hist[score] = pd.concat([_oos, _aggs], axis=1)
-        self.avg_oos_hist = avg_oos_hist
+            nevals = len(self.LF_d)
+            if nbest > nevals:
+                print(f'\nnbest ={nbest} is higher than the number of models evaluated {nevals}')
+                print(f'The average performance of best models will be computed on {nevals} models instead')
+                nbest = max(nbest, nevals)
+
+            if self.eval_models is None:
+                print('Run evaluate ...')
+                self.evaluate()
+
+            avg_oos_hist = {}
+            _perf_metrics = list(self.summary_horizon.columns.levels[1])
+            for _s in _perf_metrics:
+                _oos = {_lf_eval.forecaster_name: _lf_eval.oos_cutoff_perf[_s] for _lf_eval in self.eval_models}
+                _oos = pd.concat(_oos.values(),  axis=1, keys= _oos.keys())
+
+                best_mod = _oos.mean().idxmin()
+                nbest_mods = list(_oos.mean().nsmallest(nbest).index)
+                _aggs = pd.concat([_oos[best_mod], _oos[nbest_mods].mean(axis=1), _oos.mean(axis=1)], axis = 1,
+                                  keys = ['Best Model (over all)', f'Best {nbest} Models (over all)','Model Avg (all models)'])
+                avg_oos_hist[_s] = pd.concat([_oos, _aggs], axis=1)
+            self.avg_oos_hist = avg_oos_hist
+        
         return avg_oos_hist[score]
 
+    def __stage_X(self,
+                  LF:Forecast,
+                  X: pd.DataFrame
+                  ) -> None:
+        if LF.X is not None:
+            _lf_exogs = LF.X.columns
+            assert all([_ex in X.columns for _ex in _lf_exogs]), f'Some exogenous variables are missing for model {LF.forecaster_name}'
+            _lf_X = X[_lf_exogs]
+        else:
+            _lf_X = None
+        return _lf_X
+        
     def predict(self,
                 X: Optional[pd.DataFrame] = None, 
                 fh: Optional[ForecastingHorizon] = None,
                 coverage: float = 0.9,
                 mode: Optional[str] = None,
                 score: Optional[str] = None,
-                nbest: Optional[int] = None,
+                model_name = None,
                 ret_underlying: bool = False
                ) -> Tuple[pd.Series, pd.DataFrame]:
         """
         Make forecasts using the specified aggregation mode.
 
-        Parameters
-        
+        Parameters:
+        -----------        
             X : pd.DataFrame, optional
                 The exogenous variables used for prediction. Default is None and it takes the value entered at initialization..
             fh : ForecastingHorizon, optional
                 The forecasting horizon. Default is None and it takes the value entered at initialization..
             coverage : float, optional
                 The prediction interval coverage. Default is 0.9.
             mode : str, optional
@@ -334,114 +417,245 @@
                 Available values:
                 * 'best': The prediction is based on the best model.
                 * 'best_horizon': The prediction is based on the best model for each horizon.
                 * 'average': The average of the prediction of all models.
                 * 'inverse_score': The weighted average prediction, where weights are inversely proportional to the model performance score.
                 * 'nbest_average': Average of the n best models. The n is given by the parameter nbest.
                 * 'nbest_average_horizon': Average of the n best models for each horizon. The n is given by the parameter nbest.
+                * 'model': Returns the prediction of a specific model. The model name must be provided in the model_name parameter.
             score : str, optional
                 The performance metric to use for model comparison. Should be either 'RMSE' or 'MAPE'. Default is None and it takes the value entered at initialization..
             nbest : int, optional
                 The number of best models to select based on horizon performance. Default is None and it takes the value entered at initialization..
+            model_name: str, optional
+                The model name to use for prediction if mode='model'. Default is None.
             ret_underlying : bool, optional
                 If True, return the underlying predictions and prediction intervals for each model. Default is False.
 
-        Returns
-        
+        Returns:
+        --------        
             tuple
                 A tuple containing the aggregated prediction and prediction intervals.
         """
-        preds = {}; pred_ints = {};
-
-        for _lf in self.LF_list:
-            _y_pred, _y_pred_ints = _lf.predict(X=X, fh=fh, coverage=coverage)
-            preds[_lf.forecaster_name] = _y_pred;
-            pred_ints[_lf.forecaster_name] =_y_pred_ints; 
-
-        preds = pd.concat(preds.values(), keys = preds.keys(), axis=1)
-        pred_ints = pd.concat(pred_ints.values(), keys = pred_ints.keys(), axis=1)
+        if mode is None:
+            mode = self.mode
+        if mode == 'model':
+            assert model_name in self.LF_d.keys(), 'Model name not in the list of models'
+            _lf_X = self.__stage_X(self.LF_d[model_name], X)
+            return self.LF_d[model_name].predict(X=_lf_X, fh=fh, coverage=coverage)
+        else:
+            preds = {}; pred_ints = {}
+            for _fname, _lf in self.LF_d.items():
+                _lf_X = self.__stage_X(self.LF_d[_fname], X)                
+                _y_pred, _y_pred_ints = _lf.predict(X=_lf_X, fh=fh, coverage=coverage)
+                preds[_fname] = _y_pred
+                pred_ints[_fname] =_y_pred_ints
 
+            preds = pd.concat(preds.values(), keys = preds.keys(), axis=1)
+            pred_ints = pd.concat(pred_ints.values(), keys = pred_ints.keys(), axis=1)
 
-        return self.__aggregate_pred(mode=mode, preds=preds, pred_ints=pred_ints, score=score, nbest=nbest, ret_underlying=ret_underlying)
+            return self.__aggregate_pred(mode=mode, preds=preds, pred_ints=pred_ints, score=score, ret_underlying=ret_underlying)
 
     def update(self,
-               newdata: pd.DataFrame,
+               new_y: pd.Series,
+               new_X: Optional[pd.DataFrame] = None,
                refit: bool = False, 
+               reevaluate:bool = False, 
                fh: Optional[ForecastingHorizon] = None, 
                coverage: float = 0.9, 
                mode: Optional[str] = None,
                score: Optional[str] = None,
-               nbest: Optional[int] = None,
+               model_name = None,
                ret_underlying: bool = False
               ) -> Tuple[pd.Series, pd.DataFrame]:
         """
         Function to update the prediction for all the models and aggregate them based on the specific mode.
 
-        Parameters
-        
+        Parameters:
+        -----------        
             newdata : pd.DataFrame
                 The new data for updating the predictions.
             refit : bool, optional
-                If False, generate the prediction without fitting the model. If True, fit the underlying models again, evaluate them out of sample, select the best models, and aggregate the predictions. Default is False.
+                If False, generate the prediction without fitting the model. If True, fits the underlying models again on the entire sample
+                Default is False
+            reevaluate: bool, optional    
+                Reapply the cross-validateion, evaluate the models out of sample, select the best models, then aggregate the predictions according the setup.
+                Default is False.
             fh : ForecastingHorizon, optional
                 The forecasting horizon. Default is None and it takes the value entered at initialization..
             coverage : float, optional
                 The prediction interval coverage. Default is 0.9.
             mode : str, optional
                 The aggregation mode for predictions. Default is None and it takes the value entered at initialization..
                 Available values:
                 * 'best': The prediction is based on the best model.
                 * 'best_horizon': The prediction is based on the best model for each horizon.
                 * 'average': The average of the prediction of all models.
                 * 'inverse_score': The weighted average prediction, where weights are inversely proportional to the model performance score.
                 * 'nbest_average': Average of the n best models. The n is given by the parameter nbest.
                 * 'nbest_average_horizon': Average of the n best models for each horizon. The n is given by the parameter nbest.
+                * 'model': Returns the prediction of a specific model. The model name must be provided in the model_name parameter.
             score : str, optional
                 The performance metric to use for model comparison. Should be either 'RMSE' or 'MAPE'. Default is None and it takes the value entered at initialization..
             nbest : int, optional
                 The number of best models to select based on horizon performance. Default is None and it takes the value entered at initialization. and it takes the value entered at initialization..
+            model_name: str, optional
+                The model name to use for prediction if mode='model'. Default is None.
             ret_underlying : bool, optional
                 If True, return the underlying predictions and prediction intervals for each model. Default is False.
 
-        Returns
-        
+        Returns:
+        -------
             tuple
                 A tuple containing the aggregated prediction and prediction intervals.
         """
-        preds = {}; pred_ints = {};
-        for _lf in self.LF_list:
-            _y_pred, _y_pred_ints = _lf.update(newdata = newdata, fh=fh, coverage=coverage, refit=refit)
-            preds[_lf.forecaster_name] = _y_pred;
-            pred_ints[_lf.forecaster_name] =_y_pred_ints; 
-
-        preds = pd.concat(preds.values(), keys = preds.keys(), axis=1)
-        pred_ints = pd.concat(pred_ints.values(), keys = pred_ints.keys(), axis=1)
-
-        if refit == False:
-            return self.__aggregate_pred(mode=mode, preds=preds, pred_ints=pred_ints, score=score, nbest=nbest, ret_underlying=ret_underlying)
-        else:
-            self.evalutate(force=True)
-            self.select_best(score = score, nbest = nbest)
-            return self.__aggregate_pred(mode=mode, preds=preds, pred_ints=pred_ints, score=score, nbest=nbest, ret_underlying=ret_underlying)
+        if mode is None:
+            mode = self.mode
 
+        if mode == 'model':
+            assert model_name in self.LF_d.keys(), 'Model name not in the list of models'
+            _lf_X = self.__stage_X(self.LF_d[model_name], new_X)
+            return self.LF_d[model_name].update(new_y=new_y, new_X=_lf_X, fh=fh, coverage=coverage, refit=refit)
+        else:
+            if reevaluate == False:            
+                preds = {}; pred_ints = {}
+                for _lf in self.LF_d.values():
+                    _lf_X = self.__stage_X(_lf, new_X)
+                    try:
+                        _y_pred, _y_pred_ints = _lf.update(new_y=new_y, new_X=_lf_X, 
+                                                           fh=fh, coverage=coverage, refit=refit)
+                        preds[_lf.forecaster_name] = _y_pred
+                        pred_ints[_lf.forecaster_name] =_y_pred_ints
+                    except Exception as e:
+                        print(f'Error updating {_lf.forecaster_name}: {e}')
+                        print(f"model {_lf.forecaster_name} cannot be updated. It won't be considered for forecasts")
+                        continue                   
+
+                preds = pd.concat(preds.values(), keys = preds.keys(), axis=1)
+                pred_ints = pd.concat(pred_ints.values(), keys = pred_ints.keys(), axis=1)
+                return self.__aggregate_pred(mode=mode, preds=preds, pred_ints=pred_ints, score=score, ret_underlying=ret_underlying)
+            else:
+                self.evaluate(force=True)
+                self.select_best(score = score, reestimate=True)
+                preds = {}; pred_ints = {}
+                for _lf in self.LF_d.values():
+                    _lf_X = self.__stage_X(_lf, new_X)
+                    try:
+                        _y_pred, _y_pred_ints = _lf.update(new_y=new_y, new_X=_lf_X, fh=fh, coverage=coverage, refit=refit)
+                        preds[_lf.forecaster_name] = _y_pred
+                        pred_ints[_lf.forecaster_name] =_y_pred_ints
+                    except Exception as e:
+                        print(f'Error updating {_lf.forecaster_name}: {e}')
+                        print(f'model {_lf.forecaster_name} cannot be updated. It will be considered for forecasts')
+                        continue                   
+                preds = pd.concat(preds.values(), keys = preds.keys(), axis=1)
+                pred_ints = pd.concat(pred_ints.values(), keys = pred_ints.keys(), axis=1)
+                return self.__aggregate_pred(mode=mode, preds=preds, pred_ints=pred_ints, score=score, ret_underlying=ret_underlying)
 
+    def save(self, path: str):
+        """
+        Save the model to a file.
+        Parameters:
+        -----------
+            path : str
+                The path to save the model.
+        Returns:
+        --------
+            None
+        """
+        import pickle
+        with open(path, 'wb') as f:
+            pickle.dump(self, f)
+        return None
+    
+    def get_pred_errors(self, 
+                        mode: Optional[str] = None,
+                        score: Optional[str] = None,
+                        model_name = None, 
+                        ):
+        """
+        Get the prediction errors.
+        """
+        if mode is None:
+            mode = self.mode
+        if mode == 'model':
+            assert model_name in self.LF_d.keys(), 'Model name not in the list of models'
+            return self.LF_d[model_name].get_pred_errors()
+        else:
+            if score is None:
+                score = self.score
+            
+            # Using ProcessPoolExecutor to execute computation-heavy tasks in parallel
+            with ProcessPoolExecutor() as executor:
+                results = executor.map(fetch_errors, self.LF_d.items())
+            errors = {fname: err for fname, err in results}
+            for _fname, _lf in self.LF_d.items():
+                _lf.fitted.insample_result_df = errors[_fname]
+
+            # Convert results to dictionary            
+            errors_df = pd.concat(errors.values(), keys = errors.keys(), axis=0).reset_index()
+            errors_df = errors_df.rename(columns = {'level_0': 'forecaster'})
+
+
+            if mode =='best':
+                return errors[self.best_x_overall[score][0]].reset_index(drop=True)
+            
+            elif mode =='best_horizon':
+                if self.model_rank_perhorizon is None:
+                    self.select_best()
+                best_horizon = self.model_rank_perhorizon[score].loc['Best_1'].to_dict()
+                error_horizon_l = [errors[best_mod_h].loc[errors[best_mod_h]['horizon']==h] for h, best_mod_h in best_horizon.items()]
+                return pd.concat(error_horizon_l, axis=0).reset_index(drop=True)
+            
+            elif mode =='average':
+                return errors_df.groupby(['cutoff', 'horizon']).error.mean().reset_index()               
+            
+            elif mode =='inverse_score':
+                if self.summary_results is None:
+                    self.evaluate()
+                _score = self.summary_results.loc[f'Avg {score}']
+                _score = _score/_score.sum()
+                errors_df['_score'] = errors_df['forecaster'].map(_score.to_dict())
+                errors_df['weighted_error'] = errors_df['_score']*errors_df['error']
+                return errors_df.groupby(['cutoff', 'horizon']).weighted_error.sum().reset_index()
+            
+            elif mode =='nbest_average':
+                if self.best_x_overall is None:
+                    self.select_best()
+                return errors_df.loc[errors_df.forecaster.isin(self.best_x_overall[score])].groupby(['cutoff', 'horizon']).error.mean().reset_index()
+            
+            elif mode =='nbest_average_horizon':
+                if self.model_rank_perhorizon is None:
+                    self.select_best()
+                best_horizon = self.model_rank_perhorizon[score].iloc[:self.nbest].T
+                best_horizon = best_horizon.apply(lambda x: x.values, axis=1).to_dict()
+                errors_best_horizon = []
+                for h, best_mod_h in best_horizon.items():
+                    errors_best_horizon.append(errors_df.loc[(errors_df.horizon==h) & errors_df.forecaster.isin(best_mod_h)]\
+                        .groupby(['cutoff', 'horizon']).error.mean().reset_index())
+                return pd.concat(errors_best_horizon, axis=0).reset_index(drop=True)            
+            
+            else:
+                raise ValueError('mode can take the foloowing values: best, best_horizon, average, inverse_score, nbest_average, nbest_average_horizon, model')        
+    
     def plot_model_compare(self, 
                            score: str = 'RMSE', 
                            view: str = 'horizon', 
+                           model_subset: Optional[List[str]] = None,
                            xlabel: Optional[str] = None, 
                            ylabel: Optional[str] = None,
                            title: str = 'Out of Sample Performance', 
                            ax: Optional[plt.Axes] = None, 
                            figsize: Tuple[int, int] = (15, 6)
                           ) -> Union[plt.Figure, plt.Axes]:
         """
         Plot a comparison of models based on their out-of-sample performance.
 
-        Parameters
-        
+        Parameters:
+        -----------        
             score : str, optional
                 The performance metric for comparison. Should be either 'RMSE' or 'MAPE'. Default is 'RMSE'.
             view : str, optional
                 The view mode for comparison, either 'horizon' or 'cutoff'. Default is 'horizon'.
             xlabel : str, optional
                 The label for the x-axis. Default is an empty string.
             ylabel : str, optional
@@ -449,67 +663,90 @@
             title : str, optional
                 The title of the plot. Default is 'Out of Sample Performance'.
             ax : matplotlib.axes._subplots.AxesSubplot, optional
                 The matplotlib axes to use for plotting. Default is None.
             figsize : tuple, optional
                 The size of the figure in inches (width, height). Default is (15, 6).
 
-        Returns
-        
+        Returns:
+        --------        
             matplotlib.figure.Figure or matplotlib.axes._subplots.AxesSubplot
                 The figure and axes of the plot.
         """
+        
         if view =='horizon':
-            if 'avg_oos_horizon' not in self.__dict__.keys():
+            if self.avg_oos_horizon is None:
                 self.select_best()
             toplot = self.avg_oos_horizon[score]
 
         elif view=='cutoff':
-            if 'avg_oos_hist' not in self.__dict__.keys():
+            if self.avg_oos_hist is None:
                 self.oos_per_cutoff()
             toplot = self.avg_oos_hist[score]
 
         else:
             raise ValueError('view can take only 2 values: horizon or cutoff')
 
+        if model_subset is not None:
+            assert all([m in toplot.columns for m in model_subset]), 'Some models are not in the list of models'
+            toplot = toplot[model_subset]
         if ax is None:
             f, ax = plt.subplots(1,1,figsize=figsize)
         if ylabel is None:
             ylabel = score
         if xlabel is None:
             xlabel = view
+        
+        nseries = len(toplot.columns)
+        def expand_color_palette(colors, n_colors_needed):
+            base_array = sns.color_palette(colors, n_colors=len(colors))
+            color_array = np.array(base_array)
+            
+            # Interpolating colors
+            new_colors = np.vstack([np.interp(np.linspace(0, len(color_array)-1, num=n_colors_needed),
+                                            np.arange(len(color_array)), color_array[:, i])
+                                    for i in range(color_array.shape[1])]).T
+            return new_colors
+
+        # Get the initial colorblind palette
+        initial_palette = sns.color_palette("colorblind")
+
+        # Expand the palette if more colors are needed
+        if len(initial_palette) < nseries:
+            expanded_colors = expand_color_palette("colorblind", n_colors_needed=nseries)
+        else:
+            expanded_colors = initial_palette
 
-        toplot.plot(ax=ax, style = '-o')
-        ax.set(xlabel = xlabel, ylabel=ylabel, title =title)
-        ax.legend(frameon=False)
-
+        toplot.plot(ax=ax, style = '-o', color= expanded_colors)
+        ax.set(xlabel = xlabel, ylabel=ylabel)
+        ax.set_title(title, size="xx-large")
+        ax.legend(frameon=False, bbox_to_anchor=(1, 1))
         if ax is None:
             return f, ax
         else:
             return ax
 
-
     def plot_prediction(self, 
                         y_pred: pd.Series, 
                         models_preds: Optional[pd.DataFrame] = None, 
                         y_pred_interval: Optional[Tuple] = None, 
-                        interval_label: str = 'prediction interval', 
+                        interval_label: str = 'CI', 
                         aggregation_label: str = 'Model Agg', 
                         xlabel: str = '', 
                         ylabel: str = '', 
                         title: str = 'Prediction', 
                         ax: Optional[plt.Axes] = None, 
                         figsize: Tuple[int, int] = (15, 6)
 
                        ) -> Union[plt.Figure, plt.Axes]:
         """
         Plot forecast predictions and aggregated prediction.
 
-        Parameters
-        
+        Parameters:
+        -----------        
             y_pred : pd.Series
                 The aggregated prediction.
             models_preds : pd.DataFrame, optional
                 The DataFrame containing predictions from different models. Default is None.
             y_pred_interval : tuple, optional
                 Prediction interval for the aggregated prediction. Default is None.
             interval_label : str, optional
@@ -523,159 +760,181 @@
             title : str, optional
                 Title of the plot. Default is 'Prediction'.
             ax : matplotlib.axes._subplots.AxesSubplot, optional
                 Matplotlib axes to use for plotting. Default is None.
             figsize : tuple, optional
                 Size of the figure in inches (width, height). Default is (15, 6).
 
-        Returns
-        
+        Returns:
+        --------        
             matplotlib.figure.Figure or matplotlib.axes._subplots.AxesSubplot
                 The figure and axes of the plot.
         """
 
-        y = self.LF_list[0].y
+        y = list(self.LF_d.values())[0].y
         y_train = y.loc[y.index<y_pred.index[0]]
-        zoom_y_train = y_train.iloc[-5*len(y_pred):]
+        zoom_y_train = y_train.iloc[-3*len(y_pred):]
     
         if models_preds is not None:
             model_names = models_preds.columns
             models_preds = [models_preds[c] for c in model_names]
             labels = ['y'] + list(model_names) + [aggregation_label]
 
-            return plot_series(zoom_y_train, *models_preds, y_pred,
+            plt_res = plot_series(zoom_y_train, *models_preds, y_pred,
                                labels =labels,
                                xlabel =xlabel,
                                ylabel =ylabel,
                                title =title,
                                ax=ax, 
                                figsize =figsize,
                                pred_interval = y_pred_interval,
-                               interval_label ='prediction interval')
+                               interval_label =interval_label)
         else:
-
-            return plot_series(zoom_y_train, y_pred,
+            plt_res = plot_series(zoom_y_train, y_pred,
                                labels =['y', aggregation_label],
                                xlabel =xlabel,
                                ylabel =ylabel,
                                title =title,
                                ax=ax, 
                                figsize =figsize,
                                pred_interval = y_pred_interval,
-                              interval_label ='prediction interval')
+                              interval_label =interval_label)
+        if ax is None:
+            f, ax = plt_res
+            ax.legend(frameon=False, bbox_to_anchor=(1, 1))
+            return f, ax
+        else:
+            ax = plt_res
+            ax.legend(frameon=False, bbox_to_anchor=(1, 1))
+            return ax
+
+    def plot_train_test(self, **kwargs: Any):
+        """
+        Plot the training and test windows for each model.
+
+        Parameters:
+        -----------        
+            kwargs
+                Additional keyword arguments to be passed to the plot function.
+
+        Returns:
+        --------        
+            fig : plt.Figure
+                If ax was None, a new figure is created and returned
+                If ax was not None, the same ax is returned with plot added
+            ax : plt.Axis             
+                Axes containing the plot             
+        """
+        _lf  = list(self.LF_d.values())[0]
+        return _lf.plot.plot_train_test(**kwargs)
+    
+    def plot_cv_procedure(self,**kwargs: Any):
+        """
+        Plot the cross-validation procedure for each model.
 
-    def __aggregate_pred(self, mode, preds, pred_ints, score=None, nbest=None, ret_underlying=False):
+        Parameters:
+        -----------        
+            kwargs
+                Additional keyword arguments to be passed to the plot function.
+
+        Returns:
+        --------
+            fig : plt.Figure
+                If ax was None, a new figure is created and returned
+                If ax was not None, the same ax is returned with plot added
+            ax : plt.Axis             
+                Axes containing the plot             
+        """
+        _lf  = list(self.LF_d.values())[0]
+        return _lf.plot.plot_cv_procedure(**kwargs)
+    
+    def __aggregate_pred(self, mode, preds, pred_ints, score=None, ret_underlying=False):
 
         if score is None:
             score = self.score
-        if nbest is None:
-            nbest = self.nbest
+ 
+        nbest = self.nbest
         if mode is None:
             mode = self.mode
 
-        if  (mode !='average') & ('best_x_overall' not in self.__dict__.keys()):
-            print('\nIdentify best models and their oos performance ...')
-            self.select_best(score = score, nbest = nbest)
+        if  (mode !='average') & (self.best_x_overall is None):
+            self.select_best(score = score)
 
         if mode =='best':
-
-            "returns the prediction of the best model"
-            y_pred = preds[self.best_x_overall[score][0]]
-            y_pred_int = pred_ints[self.best_x_overall[score][0]]
-
+            # returns the prediction of the best model
+            _best_model = self.best_x_overall[score][0]
+            y_pred = preds[_best_model]            
+            if _best_model in pred_ints.columns:
+                y_pred_int = pred_ints[_best_model]
+            else:
+                print(f'Prediction intervals for {_best_model} are not available')
+                y_pred_int = pd.DataFrame()
 
         elif mode =='best_horizon':
-
-            "returns the prediction of the best model for each forecast horizon"
+            # returns the prediction of the best model for each forecast horizon
             best_horizon = self.model_rank_perhorizon[score].loc['Best_1'].to_dict()
             y_pred = pd.Series([preds[v].iloc[k-1] for k, v in best_horizon.items()], 
                    index=preds.index)
-            y_pred_int = pd.concat([pred_ints[v].iloc[k-1].to_frame().T for k, v in best_horizon.items()])
-
+            if all([v in pred_ints.columns for v in best_horizon.values()]):
+                y_pred_int = pd.concat([pred_ints[v].iloc[k-1].to_frame().T for k, v in best_horizon.items()])
+            else:
+                print('One or several model that are best in their respective horizon are not available')
+                y_pred_int = pd.DataFrame() 
 
         elif mode == 'average':
-
-            "returns the average prediction of all models"
+            # returns the average prediction of all models
             y_pred = preds.mean(axis=1)
             y_pred_int = pred_ints.unstack().unstack(0).mean(axis=1).unstack().T
 
         elif mode == 'inverse_score':
-
-            "returns the Average models proportionals to performance score"
+            # returns the Average models proportionals to performance score
             _score = self.summary_results.loc[f'Avg {score}'].sort_values()
             _score = _score/_score.sum()
 
             _weigh_preds =  preds.mul(_score, axis=1).sum(axis=1)
             y_pred = _weigh_preds.astype('float')
 
             _weigh_preds_ints = 0
             for m, w in _score.to_dict().items():
-                _weigh_preds_ints = _weigh_preds_ints+ pred_ints[m]*w
+                if m not in pred_ints.columns:
+                    print(f'Prediction intervals for model {m} are not available.') 
+                    print('It will be droped in the aggregation of prediction intervals')
+                    continue
+                else:
+                    _weigh_preds_ints = _weigh_preds_ints+ pred_ints[m]*w
             y_pred_int = _weigh_preds_ints.astype('float')
 
         elif mode == 'nbest_average':
-
-            "return the average prediction of nbest models"
+            # return the average prediction of nbest models
             y_pred = preds[self.best_x_overall[score]].mean(axis=1)
-            y_pred_int = pred_ints[self.best_x_overall[score]]\
+            if all([v in pred_ints.columns for v in self.best_x_overall[score]]):
+                y_pred_int = pred_ints[self.best_x_overall[score]]\
             .unstack().unstack(0).mean(axis=1).unstack().T
-
+            else:
+                print(f'Prediction intervals for {nbest} best models are not available')
+                y_pred_int = None
 
         elif mode == 'nbest_average_horizon':
-
-            "return the average prediction on the nbest models per horizon"
+            # return the average prediction on the nbest models per horizon
             best_horizon = self.model_rank_perhorizon[score].iloc[:nbest].T
             best_horizon = best_horizon.apply(lambda x: x.values, axis=1).to_dict()
 
             y_pred = pd.Series([preds[v].iloc[k-1].mean() for k, v in best_horizon.items()], 
                                index=preds.index)
-
-            y_pred_int = pd.concat([pred_ints[v].iloc[k-1].unstack(0).mean(axis=1).to_frame().T for k, v in best_horizon.items()])
-            y_pred_int.index = y_pred.index
-
+            if all([v in pred_ints.columns for v in best_horizon.values()]):
+                y_pred_int = pd.concat([pred_ints[v].iloc[k-1].unstack(0).mean(axis=1).to_frame().T for k, v in best_horizon.items()])
+                y_pred_int.index = y_pred.index        
+            else:
+                print(f'Prediction intervals for {nbest} best models are not available')
+                y_pred_int = None
+                
         else:
             recog_modes = ['best', 'best_horizon', 'average', 'inverse_score', 
                            'nbest_average', 'nbest_average_horizon']
             _error_msg = f'Aggregation mode not recognized. Recognized prediction aggregation are {recog_modes}'
             raise ValueError(_error_msg)
 
         if ret_underlying:
             return y_pred, y_pred_int, preds, pred_ints
         else:
             return y_pred, y_pred_int
 
-
-    def __init_test(self, 
-                    mode: str, 
-                    score: str,
-                    nbest: int
-                   ) -> None:
-        """
-        Check the validity of mode, score, and nbest values.
-
-        Parameters
-        
-            mode : str
-                The aggregation mode.
-            score : str
-                The performance score.
-            nbest : int
-                Number of best models to aggregate.
-
-        Raises
-        
-            AssertionError
-                If the mode, score, or nbest values are not recognized or do not meet the requirements.
-        """
-        assert isinstance(mode, str), 'mode must be a sting'
-        recog_modes = ['best', 'best_horizon', 'average', 'inverse_score', 
-                           'nbest_average', 'nbest_average_horizon']
-        assert mode in recog_modes, f'mode function not implemented!. Recognized modes are {recog_modes}'
-        self.mode = mode
-
-        recog_scores = ['RMSE', 'MAPE']
-        assert score in ['RMSE', 'MAPE'], f'performance score not implemented!. Recognized scores are {recog_scores}'		
-        self.score = score
-
-        assert isinstance(nbest, int), 'n best must be an integer'		
-        self.nbest = nbest	
-        return None
```

### Comparing `forecast_combine-0.0.1/pyproject.toml` & `forecast_combine-0.0.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "forecast_combine"
-version = "0.0.1"
+version = "0.0.2"
 description = "Automation of forecast models testing, combining and predicting"
 authors = ["amineraboun <amineraboun@gmail.com>"]
 repository ="https://github.com/amineraboun/forecast"
 homepage  ="https://github.com/amineraboun/forecast"
 
 readme = "README.md"
 keywords = ["arima", "ets", "theta", "tbats", "prophet"]
@@ -13,27 +13,29 @@
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 
 [tool.poetry.dependencies]
-python = ">=3.8,<3.12"
-sktime = "^0.21.0"
-statsforecast = "^1.5.0"
+python = ">=3.9,<3.12"
+sktime = "^0.28.0"
+statsforecast = "^1.7.4"
 tbats = "^1.1.3"
 prophet = "^1.1.4"
+arch = "^6.3.0"
 statsmodels = "^0.14.0"
 tqdm = "^4.66.0"
 matplotlib = "^3.7.2"
 seaborn = "^0.12.2"
 sphinx = "^7.1.2"
 nbsphinx = "^0.9.2"
 sphinx-mdinclude = "^0.5.3"
 pandoc = "^2.3"
+openpyxl = "^3.1.2"
 
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.3"
 pytest-cov = "^3.0"
 
 [tool.pytest.ini_options]
```

### Comparing `forecast_combine-0.0.1/setup.py` & `forecast_combine-0.0.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,41 +1,134 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: forecast_combine
+Version: 0.0.2
+Summary: Automation of forecast models testing, combining and predicting
+Home-page: https://github.com/amineraboun/forecast
+Keywords: arima,ets,theta,tbats,prophet
+Author: amineraboun
+Author-email: amineraboun@gmail.com
+Requires-Python: >=3.9,<3.12
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: arch (>=6.3.0,<7.0.0)
+Requires-Dist: matplotlib (>=3.7.2,<4.0.0)
+Requires-Dist: nbsphinx (>=0.9.2,<0.10.0)
+Requires-Dist: openpyxl (>=3.1.2,<4.0.0)
+Requires-Dist: pandoc (>=2.3,<3.0)
+Requires-Dist: prophet (>=1.1.4,<2.0.0)
+Requires-Dist: seaborn (>=0.12.2,<0.13.0)
+Requires-Dist: sktime (>=0.28.0,<0.29.0)
+Requires-Dist: sphinx (>=7.1.2,<8.0.0)
+Requires-Dist: sphinx-mdinclude (>=0.5.3,<0.6.0)
+Requires-Dist: statsforecast (>=1.7.4,<2.0.0)
+Requires-Dist: statsmodels (>=0.14.0,<0.15.0)
+Requires-Dist: tbats (>=1.1.3,<2.0.0)
+Requires-Dist: tqdm (>=4.66.0,<5.0.0)
+Project-URL: Repository, https://github.com/amineraboun/forecast
+Description-Content-Type: text/markdown
+
+# forecast_combine
+
+[![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
+
+## Overview
+
+forecast_combine is a Python library built upon the foundation of the sktime library, designed to simplify and streamline the process of forecasting and prediction model aggregation. It provides tools for aggregating predictions from multiple models, evaluating their performance, and visualizing the results. Whether you're working on time series forecasting, data analysis, or any other predictive modeling task, forecast_combine offers a convenient and efficient way to handle aggregation and comparison.
+
+## Key Features
+
+- **Model Aggregation:** Easily aggregate predictions from multiple models using various aggregation modes such as best model overall, best model per horizon, inverse score weighted average model, and more.
+- **Out-of-Sample Evaluation:** Evaluate model performance using out-of-sample data and choose the best models based on user-defined performance metrics.
+- **Visualization:** Visualize model performance, aggregated predictions, and prediction intervals with built-in plotting functions.
+- **Flexibility:** Accommodate various aggregation strategies, forecast horizons, and performance metrics to cater to your specific use case.
+
+## Installation
+
+Install Your Package Name using pip:
+
+```bash
+pip install forecast_combine
+```
+
+## Usage
+
+```python
+# Read the data
+import pandas as pd
+import numpy as np
+data = pd.Series(np.cumsum(np.random.normal(0, 1, size=1000)), 
+                 index=pd.date_range(end='31/12/2022', periods=1000)
+                ).rename('y').to_frame()
+
+# Import the package
+from forecast_combine.model_select import ForecastModelSelect
+
+# Import the packages of the models to test
+from sktime.forecasting.naive import NaiveForecaster
+from sktime.forecasting.statsforecast import (
+    StatsForecastAutoARIMA,
+    StatsForecastAutoETS, 
+    StatsForecastAutoTheta,
+    StatsForecastAutoTBATS
+)
+
+# Define the forecasting models 
+ForecastingModels = {
+    "Naive": NaiveForecaster(),
+    "AutoARIMA": StatsForecastAutoARIMA(),
+    "AutoETS": StatsForecastAutoETS(),
+    "AutoTheta": StatsForecastAutoTheta(),
+    "AutoTBATS": StatsForecastAutoTBATS(seasonal_periods=1),
+}
 
-packages = \
-['forecast_combine', 'forecast_combine.utils']
+model = ForecastModelSelect(
+            data= data,
+            depvar_str = 'y',                 
+            exog_l=None,
+            fh = 10,
+            pct_initial_window=0.75,
+            step_length = 5,
+            forecasters_d = ForecastingModels,
+            freq = 'B',
+            mode = 'best_horizon',
+            score = 'RMSE', )
 
-package_data = \
-{'': ['*']}
+# evaluate all the models out-of-sample
+summary_horizon, summary_results = model.evaluate()
 
-install_requires = \
-['matplotlib>=3.7.2,<4.0.0',
- 'nbsphinx>=0.9.2,<0.10.0',
- 'pandoc>=2.3,<3.0',
- 'prophet>=1.1.4,<2.0.0',
- 'seaborn>=0.12.2,<0.13.0',
- 'sktime>=0.21.0,<0.22.0',
- 'sphinx-mdinclude>=0.5.3,<0.6.0',
- 'sphinx>=7.1.2,<8.0.0',
- 'statsforecast>=1.5.0,<2.0.0',
- 'statsmodels>=0.14.0,<0.15.0',
- 'tbats>=1.1.3,<2.0.0',
- 'tqdm>=4.66.0,<5.0.0']
-
-setup_kwargs = {
-    'name': 'forecast-combine',
-    'version': '0.0.1',
-    'description': 'Automation of forecast models testing, combining and predicting',
-    'long_description': '# forecast_combine\n\n[![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)\n\n## Overview\n\nforecast_combine is a Python library built upon the foundation of the sktime library, designed to simplify and streamline the process of forecasting and prediction model aggregation. It provides tools for aggregating predictions from multiple models, evaluating their performance, and visualizing the results. Whether you\'re working on time series forecasting, data analysis, or any other predictive modeling task, forecast_combine offers a convenient and efficient way to handle aggregation and comparison.\n\n## Key Features\n\n- **Model Aggregation:** Easily aggregate predictions from multiple models using various aggregation modes such as best model overall, best model per horizon, inverse score weighted average model, and more.\n- **Out-of-Sample Evaluation:** Evaluate model performance using out-of-sample data and choose the best models based on user-defined performance metrics.\n- **Visualization:** Visualize model performance, aggregated predictions, and prediction intervals with built-in plotting functions.\n- **Flexibility:** Accommodate various aggregation strategies, forecast horizons, and performance metrics to cater to your specific use case.\n\n## Installation\n\nInstall Your Package Name using pip:\n\n```bash\npip install forecast_combine\n```\n\n## Usage\n\n```python\n# Import the necessary classes from your-package-name\ndata = pd.Series(np.cumsum(np.random.normal(0, 1, size=1000)), \n                 index=pd.date_range(end=\'31/12/2022\', periods=1000)).rename(\'y\').to_frame()\n\nfrom forecast_combine.model_select import ForecastModelSelect\n# models necessary to define the forecasting models \nfrom sktime.forecasting.naive import NaiveForecaster\nfrom sktime.forecasting.statsforecast import (\n    StatsForecastAutoARIMA,\n    StatsForecastAutoETS, \n    StatsForecastAutoTheta\n)\nfrom sktime.forecasting.tbats import TBATS\nfrom sktime.forecasting.fbprophet import Prophet\n\nForecastingModels = {\n"Naive": NaiveForecaster(),\n"AutoARIMA": StatsForecastAutoARIMA(),\n"AutoETS": StatsForecastAutoETS(),\n"AutoTheta": StatsForecastAutoTheta(),\n"TBATS": TBATS(),\n"Prophet": Prophet(),\n}\nmodel = ForecastModelSelect(\n            data= data,\n            depvar_str = \'y\',                 \n            exog_l=None,\n            fh = 10,\n            pct_initial_window=0.75,\n            step_length = 25,\n            models_d = ForecastingModels,\n            freq = \'B\',\n            mode = \'nbest_average_horizon\',\n            score = \'RMSE\', \n            nbest = 2)\n\n# compare models\nmodel.select_best(score = \'MAPE\')\n# Visualize model comparison\nmodel.plot_model_compare(score=\'MAPE\', view=\'horizon\')\nmodel.plot_model_compare(score=\'MAPE\', view=\'cutoff\')\n\n# Generate prediction\ny_pred, y_pred_ints, preds, pred_ints =  model.predict(score=\'RMSE\', ret_underlying=True)\n\n# Visualize prediction\nmodel.plot_prediction(y_pred = y_pred,\n                     models_preds = preds,\n                     y_pred_interval = y_pred_ints, \n                     title = \'Prediction\')\n```\n\n## Documentation\n\nFor detailed information about available classes, methods, and parameters, please refer to the [Documentation](https://amineraboun.github.io/forecast/).\n\n## License\n\nThis project is licensed under the [MIT License](LICENSE).\n\n## Contributing\n\nWe welcome contributions from the community! If you have suggestions, bug reports, or feature requests, please open an issue or submit a pull request. \n\n## Contact\n\nFor queries, support, or general inquiries, please feel free to reach me at [amineraboun@gmail.com](mailto:amineraboun@gmail.com).\n',
-    'author': 'amineraboun',
-    'author_email': 'amineraboun@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/amineraboun/forecast',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<3.12',
-}
+# compare models
+rank, score = model.select_best(score = 'MAPE')
+
+# Visualize model comparison
+model.plot_model_compare(score ='MAPE', view = 'cutoff')
+model.plot_model_compare(score ='MAPE', view = 'horizon')
+
+# Generate prediction
+y_pred, y_pred_ints, preds, pred_ints =  model.predict(score='RMSE', ret_underlying=True)
+
+# Visualize prediction
+model.plot_prediction(y_pred = y_pred,
+                     models_preds = preds,
+                     y_pred_interval = y_pred_ints, 
+                     title = 'Prediction')
+```
+
+## Documentation
+
+For detailed information about available classes, methods, and parameters, please refer to the [Documentation](https://amineraboun.github.io/forecast/).
+
+## License
+
+This project is licensed under the [MIT License](LICENSE).
+
+## Contributing
+
+We welcome contributions from the community! If you have suggestions, bug reports, or feature requests, please open an issue or submit a pull request. 
+
+## Contact
 
+For queries, support, or general inquiries, please feel free to reach me at [amineraboun@gmail.com](mailto:amineraboun@gmail.com).
 
-setup(**setup_kwargs)
```

