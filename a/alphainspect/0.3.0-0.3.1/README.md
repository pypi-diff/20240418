# Comparing `tmp/alphainspect-0.3.0.tar.gz` & `tmp/alphainspect-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alphainspect-0.3.0.tar", last modified: Sat Mar 23 06:10:52 2024, max compression
+gzip compressed data, was "alphainspect-0.3.1.tar", last modified: Thu Apr 18 03:37:59 2024, max compression
```

## Comparing `alphainspect-0.3.0.tar` & `alphainspect-0.3.1.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 06:10:52.516769 alphainspect-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-03-23 06:10:42.000000 alphainspect-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5115 2024-03-23 06:10:52.516769 alphainspect-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-03-23 06:10:42.000000 alphainspect-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 06:10:52.516769 alphainspect-0.3.0/alphainspect/
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-03-23 06:10:42.000000 alphainspect-0.3.0/alphainspect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3260 2024-03-23 06:10:42.000000 alphainspect-0.3.0/alphainspect/_nb.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-23 06:10:42.000000 alphainspect-0.3.0/alphainspect/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     4111 2024-03-23 06:10:42.000000 alphainspect-0.3.0/alphainspect/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     7058 2024-03-23 06:10:42.000000 alphainspect-0.3.0/alphainspect/ic.py
--rw-r--r--   0 runner    (1001) docker     (127)     7609 2024-03-23 06:10:42.000000 alphainspect-0.3.0/alphainspect/portfolio.py
--rw-r--r--   0 runner    (1001) docker     (127)     8824 2024-03-23 06:10:42.000000 alphainspect-0.3.0/alphainspect/reports.py
--rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-03-23 06:10:42.000000 alphainspect-0.3.0/alphainspect/returns.py
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-03-23 06:10:42.000000 alphainspect-0.3.0/alphainspect/selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-03-23 06:10:42.000000 alphainspect-0.3.0/alphainspect/turnover.py
--rw-r--r--   0 runner    (1001) docker     (127)     6695 2024-03-23 06:10:42.000000 alphainspect-0.3.0/alphainspect/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 06:10:52.516769 alphainspect-0.3.0/alphainspect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5115 2024-03-23 06:10:52.000000 alphainspect-0.3.0/alphainspect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-03-23 06:10:52.000000 alphainspect-0.3.0/alphainspect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-23 06:10:52.000000 alphainspect-0.3.0/alphainspect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-03-23 06:10:52.000000 alphainspect-0.3.0/alphainspect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-23 06:10:52.000000 alphainspect-0.3.0/alphainspect.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-03-23 06:10:42.000000 alphainspect-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-23 06:10:52.516769 alphainspect-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:37:59.239461 alphainspect-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-18 03:37:54.000000 alphainspect-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5115 2024-04-18 03:37:59.239461 alphainspect-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-04-18 03:37:54.000000 alphainspect-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:37:59.235461 alphainspect-0.3.1/alphainspect/
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-18 03:37:54.000000 alphainspect-0.3.1/alphainspect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3260 2024-04-18 03:37:54.000000 alphainspect-0.3.1/alphainspect/_nb.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-18 03:37:54.000000 alphainspect-0.3.1/alphainspect/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4032 2024-04-18 03:37:54.000000 alphainspect-0.3.1/alphainspect/dtree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4111 2024-04-18 03:37:54.000000 alphainspect-0.3.1/alphainspect/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7492 2024-04-18 03:37:54.000000 alphainspect-0.3.1/alphainspect/ic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7639 2024-04-18 03:37:54.000000 alphainspect-0.3.1/alphainspect/portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9951 2024-04-18 03:37:54.000000 alphainspect-0.3.1/alphainspect/reports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-04-18 03:37:54.000000 alphainspect-0.3.1/alphainspect/returns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-04-18 03:37:54.000000 alphainspect-0.3.1/alphainspect/selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-04-18 03:37:54.000000 alphainspect-0.3.1/alphainspect/turnover.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7824 2024-04-18 03:37:54.000000 alphainspect-0.3.1/alphainspect/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:37:59.239461 alphainspect-0.3.1/alphainspect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5115 2024-04-18 03:37:59.000000 alphainspect-0.3.1/alphainspect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-18 03:37:59.000000 alphainspect-0.3.1/alphainspect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 03:37:59.000000 alphainspect-0.3.1/alphainspect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-18 03:37:59.000000 alphainspect-0.3.1/alphainspect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-18 03:37:59.000000 alphainspect-0.3.1/alphainspect.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-18 03:37:54.000000 alphainspect-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 03:37:59.239461 alphainspect-0.3.1/setup.cfg
```

### Comparing `alphainspect-0.3.0/LICENSE` & `alphainspect-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alphainspect-0.3.0/PKG-INFO` & `alphainspect-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alphainspect
-Version: 0.3.0
+Version: 0.3.1
 Summary: factor performance visualization
 Author-email: wukan <wu-kan@163.com>
 License: MIT License
         
         Copyright (c) 2024 wukan
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `alphainspect-0.3.0/README.md` & `alphainspect-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `alphainspect-0.3.0/alphainspect/_nb.py` & `alphainspect-0.3.1/alphainspect/_nb.py`

 * *Files identical despite different names*

### Comparing `alphainspect-0.3.0/alphainspect/events.py` & `alphainspect-0.3.1/alphainspect/events.py`

 * *Files identical despite different names*

### Comparing `alphainspect-0.3.0/alphainspect/ic.py` & `alphainspect-0.3.1/alphainspect/ic.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import itertools
-from typing import Sequence, Literal
+from typing import Sequence, Literal, Dict
 
 import numpy as np
 import pandas as pd
 import polars as pl
 from loguru import logger
 from matplotlib import pyplot as plt
 from polars import Expr
@@ -33,14 +33,24 @@
         # TODO 使用此函数是否合理？
         mi = mutual_info_regression(yx_[:, 0].reshape(-1, 1), yx_[:, 1], n_neighbors=3)
         return float(mi[0])
 
     return pl.map_groups([a, b], lambda xx: mutual_info_func(xx))
 
 
+def w_corr(a: str, b: str, w: str) -> pl.Expr:
+    def _w_corr(xx):
+        x, y, weights = xx
+        cov_matrix = np.cov(x, y, aweights=weights)
+        weighted_corr = cov_matrix[0, 1] / np.sqrt(cov_matrix[0, 0] * cov_matrix[1, 1])
+        return weighted_corr
+
+    return pl.map_groups([a, b, w], lambda xx: _w_corr(xx))
+
+
 def calc_ic(df_pl: pl.DataFrame, factors: Sequence[str], forward_returns: Sequence[str],
             method: Literal['rank_ic', 'mutual_info'] = 'rank_ic') -> pl.DataFrame:
     """多因子多收益的IC矩阵。方便部分用户统计大量因子信息"""
     if method == 'mutual_info':
         # 互信息，非线性因子。注意，有点慢
         func = mutual_info
     else:
@@ -71,15 +81,15 @@
     """一行值堆叠成一个矩阵"""
     return pd.DataFrame(df_pl.to_numpy().reshape(len(factors), len(forward_returns)),
                         index=factors, columns=forward_returns)
 
 
 def plot_ic_ts(df_pl: pl.DataFrame, col: str,
                *,
-               axvlines=(), ax=None) -> None:
+               axvlines=(), ax=None) -> Dict[str, float]:
     """IC时序图
 
     Examples
     --------
     >>> plot_ic_ts(df_pd, 'RETURN_OO_1')
     """
     df_pl = df_pl.select([_DATE_, col])
@@ -91,30 +101,32 @@
         pl.col(col).fill_nan(0).cum_sum().alias('cum_sum'),
     ])
     df_pd = df_pl.to_pandas().replace([-np.inf, np.inf], np.nan).dropna(subset='ic')
     s: pd.Series = df_pd['ic']
 
     ic = s.mean()
     ir = s.mean() / s.std()
-    rate = (s.abs() > 0.02).mean()
+    ratio = (s.abs() > 0.02).mean()
     t_stat, p_value = stats.ttest_1samp(s, 0)
 
-    title = f"{col},IC={ic:0.4f},>0.02={rate:0.2f},IR={ir:0.4f},t_stat={t_stat:0.4f},p_value={p_value:0.4f}"
+    title = f"{col},IC={ic:0.4f},>0.02={ratio:0.2f},IR={ir:0.4f},t_stat={t_stat:0.4f},p_value={p_value:0.4f}"
     logger.info(title)
     ax1 = df_pd.plot.line(x=_DATE_, y=['ic', 'sma_20'], alpha=0.5, lw=1,
                           title=title,
                           ax=ax)
     ax2 = df_pd.plot.line(x=_DATE_, y=['cum_sum'], alpha=0.9, lw=1,
                           secondary_y='cum_sum', c='r',
                           ax=ax1)
     ax1.axhline(y=ic, c="r", ls="--", lw=1)
     ax.set_xlabel('')
     for v in axvlines:
         ax1.axvline(x=v, c="b", ls="--", lw=1)
 
+    return {'IC': ic, 'IR': ir, 'ratio': ratio, 't_stat': t_stat, 'p_value': p_value}
+
 
 def plot_ic_qq(df_pl: pl.DataFrame, col: str,
                *,
                ax=None) -> None:
     """IC QQ图
 
     Examples
```

### Comparing `alphainspect-0.3.0/alphainspect/portfolio.py` & `alphainspect-0.3.1/alphainspect/portfolio.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from typing import Optional
+
 import numpy as np
 import pandas as pd
 import polars as pl
 from loguru import logger
 from matplotlib import pyplot as plt
 
 from alphainspect import _QUANTILE_, _DATE_, _ASSET_, _WEIGHT_
@@ -32,14 +34,15 @@
     logger.info('累计收益计算完成,period={}\n{}', period, out.tail(1).to_string())
     return out
 
 
 def calc_cum_return_spread(df_pl: pl.DataFrame, fwd_ret_1: str, period: int = 5, factor_quantile: str = _QUANTILE_) -> pd.DataFrame:
     """分层计算收益。分成N层，层内等权。
     取Top层和Bottom层。比较不同的计算方法多空收益的区别"""
+
     q_max = df_pl.select(pl.max(factor_quantile)).to_series(0)[0]
     rr = df_pl.pivot(index=_DATE_, columns=_ASSET_, values=fwd_ret_1, aggregate_function='first', sort_columns=True).sort(_DATE_).fill_nan(0)
     qq = df_pl.pivot(index=_DATE_, columns=_ASSET_, values=factor_quantile, aggregate_function='first', sort_columns=True).sort(_DATE_).fill_nan(-1)
 
     out = pd.DataFrame(index=rr[_DATE_])
     rr = rr.select(pl.exclude(_DATE_)).to_numpy() + 1  # 日收益
     qq = qq.select(pl.exclude(_DATE_)).to_numpy()  # 分组编号
```

### Comparing `alphainspect-0.3.0/alphainspect/reports.py` & `alphainspect-0.3.1/alphainspect/reports.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,59 @@
+"""
+问题：明日涨跌停是否要过滤?
+
+1. 回测分层累计收益时应当过滤掉涨跌停
+    因为开盘前预测出股票后，开盘后才发现涨跌停无法交易影响曲线
+2. IC计算，是否要过滤掉涨跌停呢？个人认为不能过滤掉
+    因为IC用于评价预测能力，能不能交易不是它能实现的
+3. 机器学习。应当保留涨跌停。原因与IC一样
+    涨跌停的记录全删了后，失去学习涨跌停相关信息的机会。
+
+有不同观点的朋友可以提issue
+
+"""
+import base64
+import io
 import os
 from math import ceil
 from pathlib import Path
-from typing import Sequence, Tuple
+from typing import Sequence, Tuple, Any, Optional
 
 import polars as pl
 from loguru import logger  # noqa
 from matplotlib import pyplot as plt
 
 from alphainspect import _QUANTILE_
 from alphainspect.ic import calc_ic, plot_ic_ts, plot_ic_heatmap_monthly
 from alphainspect.portfolio import calc_cum_return_by_quantile, plot_quantile_portfolio
 from alphainspect.turnover import calc_auto_correlation, calc_quantile_turnover, plot_factor_auto_correlation, plot_turnover_quantile
 from alphainspect.utils import plot_hist
 
+html_template = """
+<html>
+<head>
+<style>
+table { border-collapse: collapse;}
+img {border: 1px solid;}
+</style>
+</head>
+<body>
+{{body}}
+</body>
+</html>
+"""
+
+
+def fig_to_img(fig, format: str = "png") -> str:
+    """图片转HTML字符串"""
+    buf = io.BytesIO()
+    fig.savefig(buf, format=format)
+    return '<img src="data:image/{};base64,{}" />'.format(format,
+                                                          base64.b64encode(buf.getvalue()).decode())
+
 
 def ipynb_to_html(template: str, output: str = None,
                   no_input: bool = False, no_prompt: bool = False, execute: bool = True,
                   timeout: int = 120,
                   open_browser: bool = True,
                   **kwargs) -> int:
     """将`ipynb`导出成`HTML`格式。生成有点慢，也许自己生成html更好
@@ -129,15 +166,15 @@
 def create_1x3_sheet(df_pl: pl.DataFrame,
                      factor: str,
                      forward_return: str, fwd_ret_1: str,
                      *,
                      period: int = 5,
                      factor_quantile: str = _QUANTILE_,
                      figsize=(12, 4),
-                     axvlines: Sequence[str] = ()) -> None:
+                     axvlines: Sequence[str] = ()) -> Tuple[Any, Any, Any, Any]:
     """画2*2的图表。含IC时序、IC直方图、IC热力图、累积收益图
 
     Parameters
     ----------
     df_pl
     factor
     forward_return: str
@@ -155,25 +192,27 @@
     fig, axes = plt.subplots(1, 3, figsize=figsize, squeeze=False)
     axes = axes.flatten()
 
     # 画IC信息
     # logger.info('计算IC')
     df_ic = calc_ic(df_pl, [factor], [forward_return])
     col = df_ic.columns[1]
-    plot_ic_ts(df_ic, col, axvlines=axvlines, ax=axes[0])
+    ic_dict = plot_ic_ts(df_ic, col, axvlines=axvlines, ax=axes[0])
 
     # 画累计收益
     df_cum_ret = calc_cum_return_by_quantile(df_pl, fwd_ret_1, period, factor_quantile)
     plot_quantile_portfolio(df_cum_ret, fwd_ret_1, period, axvlines=axvlines, ax=axes[1])
 
     # 画因子直方图
-    plot_hist(df_pl, factor, ax=axes[2])
+    hist_dict = plot_hist(df_pl, factor, ax=axes[2])
 
     fig.tight_layout()
 
+    return fig, ic_dict, hist_dict, df_cum_ret
+
 
 def create_2x3_sheet(df_pl: pl.DataFrame,
                      factor: str,
                      forward_return: str, fwd_ret_1: str,
                      *,
                      periods: Tuple = (2, 5, 10),
                      factor_quantile: str = _QUANTILE_,
@@ -188,15 +227,14 @@
     forward_return: str
         用于记算IC的远期收益率
     fwd_ret_1:str
         用于记算累计收益的1期远期收益率
     periods:Tuple
         累计收益时持仓天数与资金份数
     factor_quantile: str
-
     axvlines
 
     """
     count = len(periods) + 3
     fig, axes = plt.subplots(2, ceil(count / 2), figsize=figsize, squeeze=False)
     axes = axes.flatten()
 
@@ -237,15 +275,14 @@
     fwd_ret_1:str
         用于记算累计收益的1期远期收益率
     period: int
         累计收益时持仓天数与资金份数
     periods:
         换手率，多期比较
     factor_quantile:str
-
     axvlines
 
     """
     fig, axes = plt.subplots(3, 2, figsize=figsize)
 
     # 画IC信息
     # logger.info('计算IC')
```

### Comparing `alphainspect-0.3.0/alphainspect/returns.py` & `alphainspect-0.3.1/alphainspect/returns.py`

 * *Files identical despite different names*

### Comparing `alphainspect-0.3.0/alphainspect/selection.py` & `alphainspect-0.3.1/alphainspect/selection.py`

 * *Files identical despite different names*

### Comparing `alphainspect-0.3.0/alphainspect/turnover.py` & `alphainspect-0.3.1/alphainspect/turnover.py`

 * *Files identical despite different names*

### Comparing `alphainspect-0.3.0/alphainspect/utils.py` & `alphainspect-0.3.1/alphainspect/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import math
+from typing import Dict
 
 import numpy as np
 import pandas as pd
 import polars as pl
 import seaborn as sns
 from loguru import logger
 from polars import selectors as cs
@@ -50,14 +51,35 @@
 
     if by_group:
         return df_pl.group_by(by=[_DATE_, _GROUP_]).map_groups(_func_cs)
     else:
         return df_pl.group_by(_DATE_).map_groups(_func_cs)
 
 
+def with_quantile_tradable(df_pl: pl.DataFrame, factor_quantile: str, next_doji: str = 'NEXT_DOJI') -> pl.DataFrame:
+    """是否可以交易，将不可产易的分到其它分组
+
+    Parameters
+    ----------
+    df_pl: pl.DataFrame
+    factor_quantile: str
+        分组名
+    next_doji: str
+        明日涨跌停。修改factor_quantile到-1组
+
+    Returns
+    -------
+    pl.DataFrame
+
+    """
+    if next_doji is not None:
+        pl.when(pl.col(next_doji)).then(-1).otherwise(pl.col(factor_quantile)).name.keep(),
+    return df_pl
+
+
 def cumulative_returns(returns: np.ndarray, weights: np.ndarray,
                        funds: int = 3, freq: int = 3,
                        benchmark: np.ndarray = None,
                        ret_mean: bool = True,
                        init_cash: float = 1.0,
                        risk_free: float = 1.0,  # 1.0 + 0.025 / 250
                        ) -> np.ndarray:
@@ -174,15 +196,15 @@
     """选择指定前缀的所有因子"""
     return df_pl.select(cs.starts_with(name).name.map(lambda x: x[len(name):]))
 
 
 def plot_hist(df_pl: pl.DataFrame, col: str,
               *,
               kde: bool = False,  # 启用kde后速度慢了非常多
-              ax=None) -> None:
+              ax=None) -> Dict[str, float]:
     """直方图
 
     Examples
     --------
     >>> plot_hist(df_pl, 'RETURN_OO_1')
     """
     a = df_pl[col].to_pandas().replace([-np.inf, np.inf], np.nan).dropna()
@@ -201,7 +223,25 @@
     ax.axvline(x=mean, c="r", ls="--", lw=1)
     ax.axvline(x=mean + std * 3, c="r", ls="--", lw=1)
     ax.axvline(x=mean - std * 3, c="r", ls="--", lw=1)
     title = f"{col},mean={mean:0.4f},std={std:0.4f},skew={skew:0.4f},kurt={kurt:0.4f}"
     logger.info(title)
     ax.set_title(title)
     ax.set_xlabel('')
+
+    return {'mean': mean, 'std': std, 'skew': skew, 'kurt': kurt}
+
+
+# =================================
+# 没分好类的函数先放这，等以后再移动
+def symmetric_orthogonal(matrix):
+    # 计算特征值和特征向量
+    eigenvalues, eigenvectors = np.linalg.eigh(matrix)
+
+    # 按照特征值的大小排序
+    sorted_indices = np.argsort(eigenvalues)[::-1]
+    sorted_eigenvectors = eigenvectors[:, sorted_indices]
+
+    # 正交化矩阵
+    orthogonal_matrix = np.linalg.qr(sorted_eigenvectors)[0]
+
+    return orthogonal_matrix
```

### Comparing `alphainspect-0.3.0/alphainspect.egg-info/PKG-INFO` & `alphainspect-0.3.1/alphainspect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alphainspect
-Version: 0.3.0
+Version: 0.3.1
 Summary: factor performance visualization
 Author-email: wukan <wu-kan@163.com>
 License: MIT License
         
         Copyright (c) 2024 wukan
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `alphainspect-0.3.0/pyproject.toml` & `alphainspect-0.3.1/pyproject.toml`

 * *Files identical despite different names*

