# Comparing `tmp/resaid-0.1.6.tar.gz` & `tmp/resaid-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resaid-0.1.6.tar", last modified: Wed Apr 10 22:54:40 2024, max compression
+gzip compressed data, was "resaid-0.1.7.tar", last modified: Thu Apr 18 16:39:12 2024, max compression
```

## Comparing `resaid-0.1.6.tar` & `resaid-0.1.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 22:54:40.770402 resaid-0.1.6/
--rw-rw-rw-   0        0        0     1067 2023-10-05 19:55:40.000000 resaid-0.1.6/LICENSE
--rw-rw-rw-   0        0        0      704 2024-04-10 22:54:40.762871 resaid-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0       70 2022-02-28 19:33:00.000000 resaid-0.1.6/README.md
--rw-rw-rw-   0        0        0      103 2023-10-09 21:04:28.000000 resaid-0.1.6/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-04-10 22:54:40.696797 resaid-0.1.6/resaid/
--rw-rw-rw-   0        0        0        0 2021-10-06 19:02:31.000000 resaid-0.1.6/resaid/__init__.py
--rw-rw-rw-   0        0        0    42266 2023-12-01 16:38:17.000000 resaid-0.1.6/resaid/dca.py
--rw-rw-rw-   0        0        0    19951 2024-03-27 20:04:24.000000 resaid-0.1.6/resaid/econ.py
-drwxrwxrwx   0        0        0        0 2024-04-10 22:54:40.756429 resaid-0.1.6/resaid.egg-info/
--rw-rw-rw-   0        0        0      704 2024-04-10 22:54:40.000000 resaid-0.1.6/resaid.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      238 2024-04-10 22:54:40.000000 resaid-0.1.6/resaid.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 22:54:40.000000 resaid-0.1.6/resaid.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       72 2024-04-10 22:54:40.000000 resaid-0.1.6/resaid.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-10 22:54:40.000000 resaid-0.1.6/resaid.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-10 22:54:40.772404 resaid-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0     1177 2024-04-08 16:46:50.000000 resaid-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 16:39:12.113599 resaid-0.1.7/
+-rw-rw-rw-   0        0        0     1067 2023-10-05 19:55:40.000000 resaid-0.1.7/LICENSE
+-rw-rw-rw-   0        0        0      704 2024-04-18 16:39:12.109607 resaid-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0       70 2022-02-28 19:33:00.000000 resaid-0.1.7/README.md
+-rw-rw-rw-   0        0        0      103 2023-10-09 21:04:28.000000 resaid-0.1.7/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-04-18 16:39:12.062637 resaid-0.1.7/resaid/
+-rw-rw-rw-   0        0        0        0 2021-10-06 19:02:31.000000 resaid-0.1.7/resaid/__init__.py
+-rw-rw-rw-   0        0        0    42266 2023-12-01 16:38:17.000000 resaid-0.1.7/resaid/dca.py
+-rw-rw-rw-   0        0        0    23130 2024-04-18 13:52:40.000000 resaid-0.1.7/resaid/econ.py
+drwxrwxrwx   0        0        0        0 2024-04-18 16:39:12.102592 resaid-0.1.7/resaid.egg-info/
+-rw-rw-rw-   0        0        0      704 2024-04-18 16:39:11.000000 resaid-0.1.7/resaid.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      238 2024-04-18 16:39:11.000000 resaid-0.1.7/resaid.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 16:39:11.000000 resaid-0.1.7/resaid.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       72 2024-04-18 16:39:11.000000 resaid-0.1.7/resaid.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-18 16:39:11.000000 resaid-0.1.7/resaid.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-18 16:39:12.115600 resaid-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0     1177 2024-04-17 20:59:08.000000 resaid-0.1.7/setup.py
```

### Comparing `resaid-0.1.6/LICENSE` & `resaid-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `resaid-0.1.6/PKG-INFO` & `resaid-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resaid
-Version: 0.1.6
+Version: 0.1.7
 Summary: Reservoir engineering tools
 Home-page: https://github.com/gregeasley/resaid
 Author: Greg Easley
 Author-email: greg@easley.dev
 Project-URL: Bug Tracker, https://github.com/gregeasley/resaid/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `resaid-0.1.6/resaid/dca.py` & `resaid-0.1.7/resaid/dca.py`

 * *Files identical despite different names*

### Comparing `resaid-0.1.6/resaid/econ.py` & `resaid-0.1.7/resaid/econ.py`

 * *Files 6% similar despite different names*

```diff
@@ -81,14 +81,15 @@
         
         self._discount_rate = None
 
         self._breakeven_phase = None
 
         # optional variables
         self._royalty_col = None
+        self._owned_royalty_col = None
 
         self._wi_col = None
         self._nri_col = None
 
         self._gas_shrink = 0 
         self._ngl_yield = 0 # input as b/M post shrink
         self._ngl_price_fraction = 0
@@ -216,14 +217,22 @@
         return self._royalty_col
 
 
     @royalty_col.setter
     def royalty_col(self,value):
         self._royalty_col = value
         
+    @property
+    def owned_royalty_col(self):
+        return self._owned_royalty_col
+
+
+    @owned_royalty_col.setter
+    def owned_royalty_col(self,value):
+        self._owned_royalty_col = value
 
     @property
     def flowstreams(self):
         return self._flowstreams
 
 
     @flowstreams.setter
@@ -526,51 +535,72 @@
         l_flow['ngl_volume'] = l_flow['gas_sold']*self._ngl_yield
         t_series = np.array(range(len(l_flow)))
 
         l_flow['oil_price'] = self.generate_oil_price(t_series)
         l_flow['gas_price'] = self.generate_gas_price(t_series)
         l_flow['ngl_price'] = l_flow['oil_price'] * self._ngl_price_fraction
 
+        l_flow['oil_revenue'] = l_flow[self.OIL_COL]*l_flow['oil_price']
+        l_flow['gas_revenue'] = l_flow['gas_sold']*l_flow['gas_price']
+        l_flow['ngl_revenue'] = l_flow['ngl_volume']*l_flow['ngl_price']
+
         l_flow['revenue'] = (
             l_flow[self.OIL_COL]*l_flow['oil_price']
             +l_flow['gas_sold']*l_flow['gas_price']
             +l_flow['ngl_volume']*l_flow['ngl_price']
         )
 
-        if self._wi_col and self._nri_col:
+        
+        if self._wi_col and self._nri_col and self._owned_royalty_col and self._royalty_col:
             l_nri = self._header_data[self._header_data[self._header_uwi_col]==input_well].iloc[0][self._nri_col]
             l_wi = self._header_data[self._header_data[self._header_uwi_col]==input_well].iloc[0][self._wi_col]
+            l_ori = self._header_data[self._header_data[self._header_uwi_col]==input_well].iloc[0][self._owned_royalty_col]
+            l_royalty = self._header_data[self._header_data[self._header_uwi_col]==input_well].iloc[0][self._royalty_col]
+            if l_nri+l_royalty>1:
+                raise Exception(ValueError, f"Sum of royalty and NRI must be less than or equal to 1, currently {l_nri+l_royalty}")
+            l_flow['royalty'] = l_flow['revenue']*l_royalty
+            
+        elif self._wi_col and self._nri_col:  
+            l_nri = self._header_data[self._header_data[self._header_uwi_col]==input_well].iloc[0][self._nri_col]
+            l_wi = self._header_data[self._header_data[self._header_uwi_col]==input_well].iloc[0][self._wi_col]
+            l_ori = 0
             l_royalty = 1-l_nri/l_wi
             l_flow['royalty'] = l_flow['revenue']*l_royalty
         elif self._royalty_col:
             l_royalty = self._header_data[self._header_data[self._header_uwi_col]==input_well].iloc[0][self._royalty_col]
+            l_ori = 0
             l_flow['royalty'] = l_flow['revenue']*l_royalty
             l_wi = 1
+            l_nri = 1-l_royalty
         else:
             l_royalty = self._royalty
             l_flow['royalty'] = l_flow['revenue']*self._royalty
             l_wi = 1
-
-        l_flow['net_oil'] = l_flow[self.OIL_COL]*l_royalty
-        l_flow['net_gas'] = l_flow['gas_sold']*l_royalty
-        l_flow['net_ngl'] = l_flow['ngl_volume']*l_royalty
+            l_nri = 1-l_royalty
 
         l_flow['expense'] = (
             self._opc_t
             + self._opc_gas*l_flow['gas_sold']
             + self._opc_oil*l_flow[self.OIL_COL]
             + self._opc_water*l_flow[self.WATER_COL]
         )
 
         l_flow['expense'] = np.where(
             l_flow[self._flowstream_t_index] < start_val+n,
             0,
             l_flow['expense']
         )
 
+        l_flow['severance_tax'] = (
+            self._sev_gas*l_flow[self.GAS_COL]*l_flow['gas_price']
+            + self._sev_oil*l_flow[self.OIL_COL]*l_flow['oil_price']
+        )*(1-l_royalty)
+
+        l_flow['ad_val_tax'] = self._atx*l_flow['revenue']*(1-l_royalty)
+
         l_flow['taxes'] = (
             self._atx*l_flow['revenue']
             + self._sev_gas*l_flow[self.GAS_COL]*l_flow['gas_price']
             + self._sev_oil*l_flow[self.OIL_COL]*l_flow['oil_price']
         )*(1-l_royalty)
 
         l_flow['capex'] = self.generate_capex(len(l_flow),input_well)
@@ -599,49 +629,80 @@
 
         zero_cols = [
             self.OIL_COL,
             self.GAS_COL,
             'gas_sold',
             self.WATER_COL,
             'ngl_volume',
-            'net_oil',
-            'net_gas',
-            'net_ngl',
+            'oil_revenue',
+            'gas_revenue',
+            'ngl_revenue',
             'revenue',
             'royalty',
             'expense',
+            'severance_tax',
+            'ad_val_tax',
             'taxes',
             'capex',
             'cf',
             'dcf'
         ]
 
         l_flow = self.zero_below(l_flow,last_cf,zero_cols)
 
-        l_flow[['wi_net_oil',
-            'wi_net_gas',
-            'wi_net_ngl',
+        # calculate WI vales
+        l_flow[['wi_oil',
+            'wi_gas',
+            'wi_ngl',
             'wi_revenue',
             'wi_royalty',
             'wi_expense',
+            'wi_severance_tax',
+            'wi_ad_val_tax',
             'wi_taxes',
             'wi_capex',
             'wi_cf',
-            'wi_dcf']] = l_flow[['net_oil',
-            'net_gas',
-            'net_ngl',
+            'wi_dcf']] = l_flow[[self.OIL_COL,
+            'gas_sold',
+            'ngl_volume',
             'revenue',
             'royalty',
             'expense',
+            'severance_tax',
+            'ad_val_tax',
             'taxes',
             'capex',
             'cf',
             'dcf']].mul(l_wi)
+        
+        l_flow['net_oil'] = l_flow[self.OIL_COL]*(l_nri+l_royalty*l_ori)
+        l_flow['net_gas'] = l_flow['gas_sold']*(l_nri+l_royalty*l_ori)
+        l_flow['net_ngl'] = l_flow['ngl_volume']*(l_nri+l_royalty*l_ori)
+        l_flow['net_oil_revenue'] = l_flow['oil_revenue']*(l_nri+l_royalty*l_ori)
+        l_flow['net_gas_revenue'] = l_flow['gas_revenue']*(l_nri+l_royalty*l_ori)
+        l_flow['net_ngl_revenue'] = l_flow['ngl_revenue']*(l_nri+l_royalty*l_ori)
+        l_flow['net_revenue'] = l_flow['revenue']*(l_nri+l_royalty*l_ori)
+        l_flow['net_royalty'] = 0
+        l_flow['net_expense'] = l_flow['wi_expense']
+        l_flow['net_severance_tax'] = l_flow['severance_tax']/(1-l_royalty)*(l_nri+l_royalty*l_ori)
+        l_flow['net_ad_val_tax'] = l_flow['ad_val_tax']/(1-l_royalty)*(l_nri+l_royalty*l_ori)
+        l_flow['net_taxes'] = l_flow['taxes']/(1-l_royalty)*(l_nri+l_royalty*l_ori)
+        l_flow['net_capex'] = l_flow['wi_capex']
+        l_flow['net_cf'] = (
+            l_flow['net_revenue']
+            - l_flow['net_royalty']
+            - l_flow['net_expense']
+            - l_flow['net_taxes']
+            - l_flow['net_capex']
+        )
+        l_flow['net_dcf'] = (l_flow['net_cf'].to_numpy() / (1+self._discount_rate)**np.arange(0, len(l_flow['cf'].to_numpy())))
 
-        # calculate WI vales
+        l_flow['wi_net_oil'] = l_flow[self.OIL_COL]*(l_nri+l_royalty*l_ori)
+        l_flow['wi_net_gas'] = l_flow['gas_sold']*(l_nri+l_royalty*l_ori)
+        l_flow['wi_net_ngl'] = l_flow['ngl_volume']*(l_nri+l_royalty*l_ori)
 
         return l_flow
 
 
     def generate_indicators(self):
 
         ind_dict = {
```

### Comparing `resaid-0.1.6/resaid.egg-info/PKG-INFO` & `resaid-0.1.7/resaid.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resaid
-Version: 0.1.6
+Version: 0.1.7
 Summary: Reservoir engineering tools
 Home-page: https://github.com/gregeasley/resaid
 Author: Greg Easley
 Author-email: greg@easley.dev
 Project-URL: Bug Tracker, https://github.com/gregeasley/resaid/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `resaid-0.1.6/setup.py` & `resaid-0.1.7/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="resaid",
-    version="0.1.6",
+    version="0.1.7",
     author="Greg Easley",
     author_email="greg@easley.dev",
     description="Reservoir engineering tools",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/gregeasley/resaid",
     project_urls={
```

