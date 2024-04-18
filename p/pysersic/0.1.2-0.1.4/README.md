# Comparing `tmp/pysersic-0.1.2.tar.gz` & `tmp/pysersic-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysersic-0.1.2.tar", last modified: Mon Jul 17 05:06:10 2023, max compression
+gzip compressed data, was "pysersic-0.1.4.tar", last modified: Thu Apr 18 19:37:58 2024, max compression
```

## Comparing `pysersic-0.1.2.tar` & `pysersic-0.1.4.tar`

### file list

```diff
@@ -1,26 +1,29 @@
-drwxr-xr-x   0 ipasha     (501) staff       (20)        0 2023-07-17 05:06:10.825367 pysersic-0.1.2/
--rw-r--r--   0 ipasha     (501) staff       (20)     1065 2023-01-18 18:39:41.000000 pysersic-0.1.2/LICENSE
--rw-r--r--   0 ipasha     (501) staff       (20)      277 2023-07-17 05:06:10.825508 pysersic-0.1.2/PKG-INFO
--rw-r--r--   0 ipasha     (501) staff       (20)     3717 2023-06-30 17:38:35.000000 pysersic-0.1.2/README.md
-drwxr-xr-x   0 ipasha     (501) staff       (20)        0 2023-07-17 05:06:10.819848 pysersic-0.1.2/pysersic/
--rw-r--r--   0 ipasha     (501) staff       (20)      289 2023-06-30 20:31:35.000000 pysersic-0.1.2/pysersic/__init__.py
--rw-r--r--   0 ipasha     (501) staff       (20)      204 2023-06-30 20:09:06.000000 pysersic-0.1.2/pysersic/exceptions.py
--rw-r--r--   0 ipasha     (501) staff       (20)     6804 2023-06-06 01:01:14.000000 pysersic-0.1.2/pysersic/galfit.py
--rw-r--r--   0 ipasha     (501) staff       (20)    10866 2023-06-06 01:01:14.000000 pysersic-0.1.2/pysersic/loss.py
--rw-r--r--   0 ipasha     (501) staff       (20)    29883 2023-06-06 01:01:14.000000 pysersic-0.1.2/pysersic/priors.py
--rw-r--r--   0 ipasha     (501) staff       (20)    25249 2023-06-30 20:46:02.000000 pysersic-0.1.2/pysersic/pysersic.py
--rw-r--r--   0 ipasha     (501) staff       (20)    42318 2023-06-30 17:58:46.000000 pysersic-0.1.2/pysersic/rendering.py
--rw-r--r--   0 ipasha     (501) staff       (20)    20176 2023-06-06 01:01:14.000000 pysersic-0.1.2/pysersic/results.py
-drwxr-xr-x   0 ipasha     (501) staff       (20)        0 2023-07-17 05:06:10.822282 pysersic-0.1.2/pysersic.egg-info/
--rw-r--r--   0 ipasha     (501) staff       (20)      277 2023-07-17 05:06:10.000000 pysersic-0.1.2/pysersic.egg-info/PKG-INFO
--rw-r--r--   0 ipasha     (501) staff       (20)      443 2023-07-17 05:06:10.000000 pysersic-0.1.2/pysersic.egg-info/SOURCES.txt
--rw-r--r--   0 ipasha     (501) staff       (20)        1 2023-07-17 05:06:10.000000 pysersic-0.1.2/pysersic.egg-info/dependency_links.txt
--rw-r--r--   0 ipasha     (501) staff       (20)       89 2023-07-17 05:06:10.000000 pysersic-0.1.2/pysersic.egg-info/requires.txt
--rw-r--r--   0 ipasha     (501) staff       (20)        9 2023-07-17 05:06:10.000000 pysersic-0.1.2/pysersic.egg-info/top_level.txt
--rw-r--r--   0 ipasha     (501) staff       (20)       79 2023-07-17 05:06:10.826076 pysersic-0.1.2/setup.cfg
--rw-r--r--   0 ipasha     (501) staff       (20)      586 2023-07-17 05:04:59.000000 pysersic-0.1.2/setup.py
-drwxr-xr-x   0 ipasha     (501) staff       (20)        0 2023-07-17 05:06:10.824824 pysersic-0.1.2/tests/
--rw-r--r--   0 ipasha     (501) staff       (20)     6001 2023-06-06 01:01:14.000000 pysersic-0.1.2/tests/test_fitters.py
--rw-r--r--   0 ipasha     (501) staff       (20)      676 2023-06-06 01:01:14.000000 pysersic-0.1.2/tests/test_loss.py
--rw-r--r--   0 ipasha     (501) staff       (20)     3444 2023-06-06 01:01:14.000000 pysersic-0.1.2/tests/test_priors.py
--rw-r--r--   0 ipasha     (501) staff       (20)     3652 2023-06-06 01:01:14.000000 pysersic-0.1.2/tests/test_renderers.py
+drwxr-xr-x   0 ipasha     (501) staff       (20)        0 2024-04-18 19:37:58.071461 pysersic-0.1.4/
+-rw-r--r--   0 ipasha     (501) staff       (20)     1065 2023-01-18 18:39:41.000000 pysersic-0.1.4/LICENSE
+-rw-r--r--   0 ipasha     (501) staff       (20)     1810 2024-04-18 19:37:58.071277 pysersic-0.1.4/PKG-INFO
+-rw-r--r--   0 ipasha     (501) staff       (20)     5310 2024-01-30 18:45:38.000000 pysersic-0.1.4/README.md
+-rw-r--r--   0 ipasha     (501) staff       (20)      709 2024-04-18 18:01:53.000000 pysersic-0.1.4/pyproject.toml
+drwxr-xr-x   0 ipasha     (501) staff       (20)        0 2024-04-18 19:37:58.069141 pysersic-0.1.4/pysersic/
+-rw-r--r--   0 ipasha     (501) staff       (20)      289 2024-04-18 18:01:51.000000 pysersic-0.1.4/pysersic/__init__.py
+-rw-r--r--   0 ipasha     (501) staff       (20)      204 2023-08-10 18:12:29.000000 pysersic-0.1.4/pysersic/exceptions.py
+-rw-r--r--   0 ipasha     (501) staff       (20)     6804 2023-06-06 01:01:14.000000 pysersic-0.1.4/pysersic/galfit.py
+-rw-r--r--   0 ipasha     (501) staff       (20)    11326 2024-01-30 18:45:38.000000 pysersic-0.1.4/pysersic/loss.py
+-rw-r--r--   0 ipasha     (501) staff       (20)    21344 2024-01-30 18:45:38.000000 pysersic-0.1.4/pysersic/multiband.py
+-rw-r--r--   0 ipasha     (501) staff       (20)    36198 2024-04-18 19:37:28.000000 pysersic-0.1.4/pysersic/priors.py
+-rw-r--r--   0 ipasha     (501) staff       (20)    27213 2024-04-18 19:37:28.000000 pysersic-0.1.4/pysersic/pysersic.py
+-rw-r--r--   0 ipasha     (501) staff       (20)    33668 2024-04-18 19:37:28.000000 pysersic-0.1.4/pysersic/rendering.py
+-rw-r--r--   0 ipasha     (501) staff       (20)    19587 2024-04-18 18:01:53.000000 pysersic-0.1.4/pysersic/results.py
+drwxr-xr-x   0 ipasha     (501) staff       (20)        0 2024-04-18 19:37:58.069982 pysersic-0.1.4/pysersic.egg-info/
+-rw-r--r--   0 ipasha     (501) staff       (20)     1810 2024-04-18 19:37:58.000000 pysersic-0.1.4/pysersic.egg-info/PKG-INFO
+-rw-r--r--   0 ipasha     (501) staff       (20)      494 2024-04-18 19:37:58.000000 pysersic-0.1.4/pysersic.egg-info/SOURCES.txt
+-rw-r--r--   0 ipasha     (501) staff       (20)        1 2024-04-18 19:37:58.000000 pysersic-0.1.4/pysersic.egg-info/dependency_links.txt
+-rw-r--r--   0 ipasha     (501) staff       (20)      112 2024-04-18 19:37:58.000000 pysersic-0.1.4/pysersic.egg-info/requires.txt
+-rw-r--r--   0 ipasha     (501) staff       (20)        9 2024-04-18 19:37:58.000000 pysersic-0.1.4/pysersic.egg-info/top_level.txt
+-rw-r--r--   0 ipasha     (501) staff       (20)       38 2024-04-18 19:37:58.071499 pysersic-0.1.4/setup.cfg
+-rw-r--r--   0 ipasha     (501) staff       (20)       38 2024-01-30 18:45:38.000000 pysersic-0.1.4/setup.py
+drwxr-xr-x   0 ipasha     (501) staff       (20)        0 2024-04-18 19:37:58.070923 pysersic-0.1.4/tests/
+-rw-r--r--   0 ipasha     (501) staff       (20)     7002 2024-04-18 18:01:53.000000 pysersic-0.1.4/tests/test_fitters.py
+-rw-r--r--   0 ipasha     (501) staff       (20)      676 2023-06-06 01:01:14.000000 pysersic-0.1.4/tests/test_loss.py
+-rw-r--r--   0 ipasha     (501) staff       (20)     2588 2024-04-18 18:01:53.000000 pysersic-0.1.4/tests/test_multiband.py
+-rw-r--r--   0 ipasha     (501) staff       (20)     4090 2024-01-30 18:45:38.000000 pysersic-0.1.4/tests/test_priors.py
+-rw-r--r--   0 ipasha     (501) staff       (20)     3524 2024-01-30 18:45:38.000000 pysersic-0.1.4/tests/test_renderers.py
```

### Comparing `pysersic-0.1.2/LICENSE` & `pysersic-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pysersic-0.1.2/pysersic/galfit.py` & `pysersic-0.1.4/pysersic/galfit.py`

 * *Files identical despite different names*

### Comparing `pysersic-0.1.2/pysersic/loss.py` & `pysersic-0.1.4/pysersic/loss.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import jax.numpy as jnp
 from numpyro import distributions as dist, sample, handlers, factor,deterministic
 from typing import Optional
 
 def gaussian_loss(mod: jnp.array,
                 data: jnp.array,
                 rms: jnp.array,
-                mask: jnp.array)-> float:
+                mask: jnp.array,
+                suffix: str = "")-> float:
     """Basic Gaussian loss function using given uncertainties
 
     Parameters
     ----------
     mod : jnp.array
         Model image
     data : jnp.array
@@ -20,21 +21,22 @@
     Returns
     -------
     float
         Sampled loss function
     """
 
     with handlers.mask(mask = mask):
-        loss = sample("Loss", dist.Normal(mod, rms), obs=data)
+        loss = sample(f"Loss{suffix}", dist.Normal(mod, rms), obs=data)
     return loss
 
 def cash_loss(mod: jnp.array,
                 data: jnp.array,
                 rms: jnp.array,
-                mask: jnp.array)-> float:
+                mask: jnp.array,
+                suffix: str = "")-> float:
     """
     Cash statistic based on Poisson statistics derived in Cash (1979) (DOI 10.1086/156922) and advocated for in Erwin (2015) (https://arxiv.org/abs/1408.1097) for use in Sersic fitting. Since the is based on Poisson statistics, scaling of the image will produce different confidence intervals. Additionally, since a logarithm is taken of the model image, negative values associated with different sky models will cause issues.
 
     Parameters
     ----------
     mod : jnp.array
         Model image
@@ -46,21 +48,22 @@
     Returns
     -------
     float
         Sampled loss function
     """
     
     with handlers.mask(mask = mask):
-        loss = factor('cash_loss', -1*(mod - data*jnp.log(mod)))
+        loss = factor(f'cash_loss{suffix}', -1*(mod - data*jnp.log(mod)))
     return loss
 
 def gaussian_loss_w_frac(mod: jnp.array,
                 data: jnp.array,
                 rms: jnp.array,
-                mask: jnp.array)-> float:
+                mask: jnp.array,
+                suffix: str = "")-> float:
     """Gaussian loss with and additional fractional increase to all uncertainties such that,
 
     $$ \sigma_{new,i} = (1 + f) * \sigma_{old,i} $$
 
     f is a free parameter varied between -0.5 and 2
 
     Parameters
@@ -74,23 +77,24 @@
 
     Returns
     -------
     float
         Sampled loss function
     """
     
-    scatter_frac = sample('frac_scatter_increase', dist.TruncatedNormal(low = -0.5, high = 2) )
+    scatter_frac = sample(f'frac_rms_increase{suffix}', dist.TruncatedNormal(low = -0.5, high = 2) )
     with handlers.mask(mask = mask):
-        loss =  sample("Loss", dist.Normal(mod, (1+ scatter_frac)*rms), obs=data)    
+        loss =  sample(f"Loss{suffix}", dist.Normal(mod, (1+ scatter_frac)*rms), obs=data)    
     return loss
 
 def gaussian_loss_w_sys(mod: jnp.array,
                 data: jnp.array,
                 rms: jnp.array,
-                mask: jnp.array)-> float:
+                mask: jnp.array,
+                suffix: str = "")-> float:
     """Gaussian loss with and additional systematic increase such_that
 
     $$ \sigma_{new,i}^2 = \sigma_{old,i}^2 + \sigma_{sys}^2 $$
 
     \sigma_{sys} is a free parameter with a Normal prior, with loc = 0 and scale = mean(rms) truncated to ensure > 0
 
     Parameters
@@ -104,25 +108,26 @@
 
     Returns
     -------
     float
         Sampled loss function
     """
     
-    sys_scatter_base = sample('sys_scatter_base', dist.TruncatedNormal(low = 0, scale = 1 ) )
-    sys_scatter = deterministic('sys_scatter', sys_scatter_base*jnp.mean(rms))
+    sys_scatter_base = sample(f'sys_rms_base{suffix}', dist.TruncatedNormal(low = 0, scale = 1 ) )
+    sys_scatter = deterministic(f'sys_rms{suffix}', sys_scatter_base*jnp.mean(rms))
     with handlers.mask(mask = mask):
-        loss =  sample("Loss", dist.Normal(mod, jnp.sqrt(rms**2 + sys_scatter**2)), obs=data)    
+        loss =  sample(f"Loss{suffix}", dist.Normal(mod, jnp.sqrt(rms**2 + sys_scatter**2)), obs=data)    
     return loss
 
 def student_t_loss(mod: jnp.array,
                 data: jnp.array,
                 rms: jnp.array,
                 mask: jnp.array,
-                nu: Optional[int] = 5)-> float:
+                nu: Optional[int] = 5,
+                suffix: str = "")-> float:
     """
     Student T loss, with a df = 5 by default. This has fatter tails than Gaussian loss (or chi squared) so is more resilient to outliers
 
     Parameters
     ----------
     mod : jnp.array
         Model image
@@ -134,22 +139,23 @@
     Returns
     -------
     float
         Sampled loss function
     """
     nu = 5.
     with handlers.mask(mask = mask):
-        loss =  sample("Loss", dist.StudentT(nu,mod,jnp.sqrt((nu-2.)/2.)*rms), obs=data)    
+        loss =  sample(f"Loss{suffix}", dist.StudentT(nu,mod,jnp.sqrt((nu-2.)/2.)*rms), obs=data)    
     return loss
 
 def student_t_loss_free_sys(mod: jnp.array,
                 data: jnp.array,
                 rms: jnp.array,
                 mask: jnp.array,
-                nu: Optional[int] = 5)-> float:
+                nu: Optional[int] = 5,
+                suffix: str = "")-> float:
     """
     Student T loss, which has fatter tails than Gaussian loss (or chi squared) so is so is more resilient to outliers. In addition, add additional systematic increase such that
 
     $$ \sigma_{new,i}^2 = \sigma_{old,i}^2 + \sigma_{sys}^2 $$
 
     \sigma_{sys} is a free parameter with a Normal prior, with loc = 0 and scale = mean(rms) truncated to ensure > 0
 
@@ -164,28 +170,28 @@
         per pixel 1-sigma uncertainties
 
     Returns
     -------
     float
         Sampled loss function
     """
-    sys_scatter_base = sample('sys_scatter_base', dist.TruncatedNormal(low = 0, scale = 1 ) )
-    sys_scatter = deterministic('sys_scatter', sys_scatter_base*jnp.mean(rms))
+    sys_scatter_base = sample(f'sys_rms_base{suffix}', dist.TruncatedNormal(low = 0, scale = 1 ) )
+    sys_scatter = deterministic(f'sys_rms{suffix}', sys_scatter_base*jnp.mean(rms))
     rms_new = jnp.sqrt((nu-2.)/2.)*jnp.sqrt(rms**2 + sys_scatter**2)
 
     with handlers.mask(mask = mask):
-        loss =  sample("Loss", dist.StudentT(nu, mod, rms_new), obs=data)    
+        loss =  sample(f"Loss{suffix}", dist.StudentT(nu, mod, rms_new), obs=data)    
     return loss
 
 def pseudo_huber_loss(mod: jnp.array,
                 data: jnp.array,
                 rms: jnp.array,
                 mask: jnp.array,
-                delta: Optional[int] = 3
-                )-> float:
+                delta: Optional[int] = 3,
+                suffix: str = "")-> float:
     """
     Pseudo huber loss function of the form:
 
     $$ L = \delta^2 * ( \sqrt{1 + (a/\delta)^2} - 1) $$
 
     where a is the residuals scaled by the rms and delta can be chosen. This loss function is more robust to outliers than the Gaussian loss function as it is meant to transition for L2 to L1 loss at residuals greater than delta. The delta parameter is 3 by default but can be varied.
 
@@ -202,23 +208,23 @@
     -------
     float
         Sampled loss function
     """
     
     with handlers.mask(mask = mask):
         res = (data-mod)/rms
-        loss = factor('pseudo_huber_loss', -1.*(jnp.sqrt(1 + ( res/delta )**2) - 1) )
+        loss = factor(f'pseudo_huber_loss{suffix}', -1.*(jnp.sqrt(1 + ( res/delta )**2) - 1) )
     return loss
 
 def gaussian_mixture(mod: jnp.array,
                 data: jnp.array,
                 rms: jnp.array,
                 mask: jnp.array,
-                c: Optional[float] = 5.
-                )-> float:
+                c: Optional[float] = 5.,
+                suffix: str = "")-> float:
     """
     Gaussian mixture loss function, with one representing a "contaminating" outlier distribution with standard deviation equal to c*rms where c is 5 by default. The "contaminating fraction" or fraction of outliers is a free parameter with a Uniform prior between 0 and 0.25.
 
     Parameters
     ----------
     Parameters
     ----------
@@ -232,30 +238,30 @@
         factor to increase rms for outlier distribution, by default 5
 
     Returns
     -------
     float
         _description_
     """
-    contam_frac_base = sample('outlier_frac_base', dist.TruncatedNormal(low = 0, scale = 1., high = 5.) )
-    contam_frac = deterministic('outlier_frac', contam_frac_base*0.05 )
+    contam_frac_base = sample(f'outlier_frac_base{suffix}', dist.TruncatedNormal(low = 0, scale = 1., high = 5.) )
+    contam_frac = deterministic(f'outlier_frac{suffix}', contam_frac_base*0.05 )
 
     mixture_dists = dist.Categorical(probs = jnp.array([1-contam_frac, contam_frac]))
     component_dists = dist.Normal(jnp.stack([mod,mod],axis = -1), jnp.stack([rms,c*rms],axis = -1) )
 
     with handlers.mask(mask = mask):
-        loss = sample("Loss", dist.MixtureSameFamily(mixture_dists, component_dists), obs=data)
+        loss = sample(f"Loss{suffix}", dist.MixtureSameFamily(mixture_dists, component_dists), obs=data)
     return loss
 
 def gaussian_mixture_w_sys(mod: jnp.array,
                 data: jnp.array,
                 rms: jnp.array,
                 mask: jnp.array,
-                c: Optional[float] = 5.
-                )-> float:
+                c: Optional[float] = 5.,
+                suffix: str = "")-> float:
     """
     Gaussian mixture loss function, with one representing a "contaminating" outlier distribution with standard deviation equal to c*rms where c is 5 by default. The "outlier fraction" or fraction of outliers is a free parameter with a Uniform prior between 0 and 0.25.
 
     Parameters
     ----------
     Parameters
     ----------
@@ -269,34 +275,34 @@
         factor to increase rms for outlier distribution, by default 5
 
     Returns
     -------
     float
         _description_
     """
-    contam_frac_base = sample('outlier_frac_base', dist.TruncatedNormal(low = 0, scale = 1., high = 5.) )
-    contam_frac = deterministic('outlier_frac', contam_frac_base*0.05 )
+    contam_frac_base = sample(f'outlier_frac_base{suffix}', dist.TruncatedNormal(low = 0, scale = 1., high = 5.) )
+    contam_frac = deterministic(f'outlier_frac{suffix}', contam_frac_base*0.05 )
 
-    sys_scatter_base = sample('sys_scatter_base', dist.TruncatedNormal(low = 0, scale = 1 ) )
-    sys_scatter = deterministic('sys_scatter', sys_scatter_base*jnp.mean(rms))
+    sys_scatter_base = sample(f'sys_rms_base{suffix}', dist.TruncatedNormal(low = 0, scale = 1 ) )
+    sys_scatter = deterministic(f'sys_rms{suffix}', sys_scatter_base*jnp.mean(rms))
 
     rms_new = jnp.sqrt(rms**2 + sys_scatter**2)
     mixture_dists = dist.Categorical(probs = jnp.array([1-contam_frac, contam_frac]))
     component_dists = dist.Normal(jnp.stack([mod,mod],axis = -1), jnp.stack([rms_new,c*rms_new],axis = -1) )
 
     with handlers.mask(mask = mask):
-        loss = sample("Loss", dist.MixtureSameFamily(mixture_dists, component_dists), obs=data)
+        loss = sample(f"Loss{suffix}", dist.MixtureSameFamily(mixture_dists, component_dists), obs=data)
     return loss
 
 def gaussian_mixture_w_frac(mod: jnp.array,
                 data: jnp.array,
                 rms: jnp.array,
                 mask: jnp.array,
-                c: Optional[float] = 5.
-                )-> float:
+                c: Optional[float] = 5.,
+                suffix: str = "")-> float:
     """
     Gaussian mixture loss function, with one representing a "contaminating" outlier distribution with standard deviation equal to c*rms where c is 5 by default. The "outlier fraction" or fraction of outliers is a free parameter with a Uniform prior between 0 and 0.25.
 
     Parameters
     ----------
     Parameters
     ----------
@@ -310,19 +316,19 @@
         factor to increase rms for outlier distribution, by default 5
 
     Returns
     -------
     float
         _description_
     """
-    contam_frac_base = sample('outlier_frac_base', dist.TruncatedNormal(low = 0, scale = 1., high = 5.) )
-    contam_frac = deterministic('outlier_frac', contam_frac_base*0.05 )
+    contam_frac_base = sample(f'outlier_frac_base{suffix}', dist.TruncatedNormal(low = 0, scale = 1., high = 5.) )
+    contam_frac = deterministic(f'outlier_frac{suffix}', contam_frac_base*0.05 )
 
-    sig_frac = sample('sig_frac', dist.TruncatedNormal(low = -2./3., high = 2., loc = 0, scale = 0.5 ) )
+    sig_frac = sample(f'rms_frac{suffix}', dist.TruncatedNormal(low = -2./3., high = 2., loc = 0, scale = 0.5 ) )
 
     rms_new = (1+sig_frac)*rms
     mixture_dists = dist.Categorical(probs = jnp.array([1-contam_frac, contam_frac]))
     component_dists = dist.Normal(jnp.stack([mod,mod],axis = -1), jnp.stack([rms_new,c*rms],axis = -1) )
 
     with handlers.mask(mask = mask):
-        loss = sample("Loss", dist.MixtureSameFamily(mixture_dists, component_dists), obs=data)
+        loss = sample(f"Loss{suffix}", dist.MixtureSameFamily(mixture_dists, component_dists), obs=data)
     return loss
```

### Comparing `pysersic-0.1.2/pysersic/priors.py` & `pysersic-0.1.4/pysersic/priors.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,294 +1,367 @@
-
 from __future__ import annotations
-from abc import ABC
-from typing import Iterable, Optional, Union, Tuple
+
+from abc import abstractmethod
+from copy import copy
+from typing import Iterable, Optional, Tuple, Union
 
 import astropy.units as u
-from astropy.stats import biweight_scale as bws
+import equinox as eqx
 import jax
 import jax.numpy as jnp
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas
-from numpyro import distributions as dist, infer, sample
+from astropy.stats import biweight_scale as bws
+from numpyro import distributions as dist
+from numpyro import infer, sample
 from photutils.morphology import data_properties
 
-base_sky_types = ['none','flat','tilted-plane']
+base_sky_types = ["none", "flat", "tilted-plane"]
 base_sky_params = dict(
-    zip(base_sky_types,
-    [ [],['sky_back',], ['sky_back','sky_x_sl','sky_y_sl'] ]
+    zip(
+        base_sky_types,
+        [
+            [],
+            [
+                "sky_back",
+            ],
+            ["sky_back", "sky_x_sl", "sky_y_sl"],
+        ],
     )
 )
 
-@jax.jit
-def render_tilted_plane_sky(X,Y,back,x_sl,y_sl ):
-    xmid = float(X.shape[0]/2.)
-    ymid = float(Y.shape[0]/2.)
-    return back + (X-xmid)*x_sl + (Y-ymid)*y_sl
 
-
-base_profile_types = ['sersic','doublesersic','pointsource','exp','dev']
-base_profile_params =dict( 
-    zip(base_profile_types,
-    [ ['xc','yc','flux','r_eff','n','ellip','theta'],
-    ['xc','yc','flux','f_1', 'r_eff_1','n_1','ellip_1', 'r_eff_2','n_2','ellip_2','theta'],
-    ['xc','yc','flux'],
-    ['xc','yc','flux','r_eff','ellip','theta'],
-    ['xc','yc','flux','r_eff','ellip','theta'],]
+def render_tilted_plane_sky(X, Y, back, x_sl, y_sl):
+    xmid = float(X.shape[0] / 2.0)
+    ymid = float(Y.shape[0] / 2.0)
+    return back + (X - xmid) * x_sl + (Y - ymid) * y_sl
+
+
+base_profile_types = [
+    "sersic",
+    "doublesersic",
+    "sersic_pointsource",
+    "pointsource",
+    "exp",
+    "dev",
+]
+base_profile_params = dict(
+    zip(
+        base_profile_types,
+        [
+            ["xc", "yc", "flux", "r_eff", "n", "ellip", "theta"],
+            [
+                "xc",
+                "yc",
+                "flux",
+                "f_1",
+                "r_eff_1",
+                "n_1",
+                "ellip_1",
+                "r_eff_2",
+                "n_2",
+                "ellip_2",
+                "theta",
+            ],
+            ["xc", "yc", "flux", "f_ps", "r_eff", "n", "ellip", "theta"],
+            ["xc", "yc", "flux"],
+            ["xc", "yc", "flux", "r_eff", "ellip", "theta"],
+            ["xc", "yc", "flux", "r_eff", "ellip", "theta"],
+        ],
     )
 )
 
 
-class BasePrior(ABC):
+class BaseSkyPrior(eqx.Module):
+    type: eqx.AbstractClassVar()
+    repr_dict: dict = eqx.field(static=True)
+    suffix: str
+    dist_dict: dict
+    reparam_dict: dict
+
+    def __init__(self, sky_guess: float, sky_guess_err: float, suffix: str = ""):
+        """Base class for sky priors
+
+        Parameters
+        ----------
+        sky_guess : float
+            Initial guess for level of background, by default None
+        sky_guess_err : float
+            Uncertainty on initial guess, by default None
+        suffix : str, optional
+            suffix to be added on end of variables, by default ''
+        """
+
+        self.reparam_dict = {}
+        self.dist_dict = {}
+        self.suffix = suffix
+        self.repr_dict = {}
+
+    @abstractmethod
+    def sample(self, X: jnp.array, Y: jnp.array):
+        return NotImplementedError
+
+    def update_prior(self, name: str, mu: float, sigma: float):
+        """Update prior for a given parameter, assumed to be Gaussian with mu and sigma
+
+        Parameters
+        ----------
+        name : str
+            Name of parameter
+        mu : float
+            Location for prior
+        sigma : float
+            width of prior
+        """
+        self.reparam_dict[f"{name}{self.suffix}"] = infer.reparam.TransformReparam()
+        self.dist_dict[f"{name}{self.suffix}"] = dist.TransformedDistribution(
+            dist.Normal(),
+            dist.transforms.AffineTransform(
+                mu,
+                sigma,
+            ),
+        )
+        self.repr_dict[name] = f"Normal with mu = {mu:.3e} and sd = {sigma:.3e}"
+
+    def __repr__(
+        self,
+    ):
+        string = f"sky type - {self.type}\n"
+        for k, v in self.repr_dict.items():
+            string += f"{k} --- {v}\n"
+        return string
+
+
+class NoSkyPrior(BaseSkyPrior):
+    type: str = "None"
+
+    def __init__(self, sky_guess: float, sky_guess_err: float, suffix: str = ""):
+        """Class for no sky model
+
+        Parameters
+        ----------
+        sky_guess : float
+            Initial guess for level of background, by default None
+        sky_guess_err : float
+            Uncertainty on initial guess, by default None
+        suffix : str, optional
+            suffix to be added on end of variables, by default ''
+        """
+        super().__init__(sky_guess, sky_guess_err, suffix)
+        self.type = "None"
+
+    def sample(self, X, Y):
+        return 0.0
+
+
+class FlatSkyPrior(BaseSkyPrior):
+    type: str = "flat"
+
+    def __init__(self, sky_guess: float, sky_guess_err: float, suffix: str = ""):
+        """Class for sky model of constant background
+
+        Parameters
+        ----------
+        sky_guess : float
+            Initial guess for level of background, by default None
+        sky_guess_err : float
+            Uncertainty on initial guess, by default None
+        suffix : str, optional
+            suffix to be added on end of variables, by default ''
+        """
+        super().__init__(sky_guess, sky_guess_err, suffix)
+        self.update_prior("sky_back", sky_guess, sky_guess_err)
+
+    def sample(self, X, Y):
+        return sample(
+            "sky_back" + self.suffix, self.dist_dict["sky_back" + self.suffix]
+        )
+
+
+class TiltedPlaneSkyPrior(BaseSkyPrior):
+    type: str = "TiltedPlane"
+
+    def __init__(self, sky_guess: float, sky_guess_err: float, suffix: str = ""):
+        """Class for tilted-plane sky model
+
+        Parameters
+        ----------
+        sky_guess : float
+            Initial guess for level of background, by default None
+        sky_guess_err : float
+            Uncertainty on initial guess, by default None
+        suffix : str, optional
+            suffix to be added on end of variables, by default ''
+        """
+        super().__init__(sky_guess, sky_guess_err, suffix)
+
+        self.update_prior("sky_back", sky_guess, sky_guess_err)
+        self.update_prior("sky_x_sl", 0.0, 0.1 * sky_guess_err)
+        self.update_prior("sky_y_sl", 0.0, 0.1 * sky_guess_err)
+
+    def sample(self, X, Y):
+        back = sample(
+            "sky_back" + self.suffix, self.dist_dict["sky_back" + self.suffix]
+        )
+        x_sl = sample(
+            "sky_x_sl" + self.suffix, self.dist_dict["sky_x_sl" + self.suffix]
+        )
+        y_sl = sample(
+            "sky_y_sl" + self.suffix, self.dist_dict["sky_y_sl" + self.suffix]
+        )
+
+        x_mid = float(X.shape[0] / 2.0)
+        y_mid = float(Y.shape[0] / 2.0)
+
+        return back + (X - x_mid) * x_sl + (Y - y_mid) * y_sl
+
+
+class BasePrior(eqx.Module):
+    sky_type: str = eqx.field(static=True)
+    repr_dict: dict = eqx.field(static=True)
+    suffix: str
+    dist_dict: dict
+    reparam_dict: dict
+    sky_prior: eqx.Module
+
     """
     Base class for priors with sky sampling included
     """
-    def __init__(self, sky_type = 'none',sky_guess=None,sky_guess_err=None) -> None:
+
+    def __init__(
+        self, sky_type="none", sky_guess=None, sky_guess_err=None, suffix=""
+    ) -> None:
         """Initialize a base prior class
 
         Parameters
         ----------
         sky_type : str, optional
-            Type of sky modle to use, one of: none,flat or tilted-plane, by default 'none'
+            Type of sky mode to use, one of: none,flat or tilted-plane, by default 'none'
+        sky_guess : float
+            Initial guess for level of background, by default None
+        sky_guess_err : float
+            Uncertainty on initial guess, by default None
+        suffix : str, optional
+            suffix to be added on end of variables, by default ''
         """
         self.reparam_dict = {}
+        self.dist_dict = {}
+        self.repr_dict = {}
         self.sky_type = sky_type
+        self.suffix = suffix
+
         if sky_guess is None:
-            self.sky_guess = 0.0 
+            sky_guess = 0.0
+            sky_guess_err = 0.0
         else:
-            assert sky_guess is not None and sky_guess_err is not None, 'If using fitting a sky then must supply a guess and uncertainty on the background value'
-            self.sky_guess = sky_guess
-            self.sky_guess_err = sky_guess_err
+            assert (
+                sky_guess is not None and sky_guess_err is not None
+            ), "If using fitting a sky then must supply a guess and uncertainty on the background value"
 
         if self.sky_type not in base_sky_types:
             raise AssertionError("Sky type must be one of: ", base_sky_types)
-        elif self.sky_type == 'none':
-            self.sample_sky = self.sample_sky_none
-    
-        elif self.sky_type == 'flat':
-            
-            self._set_dist('sky_back',dist.TransformedDistribution(
-                                dist.Normal(),
-                                dist.transforms.AffineTransform(sky_guess,sky_guess_err),)
-                            )
-            self.reparam_dict['sky_back'] = infer.reparam.TransformReparam()
-            self.sample_sky = self.sample_sky_flat
-            
-        elif self.sky_type == 'tilted-plane':
-            self._set_dist('sky_back',dist.TransformedDistribution(
-                                dist.Normal(),
-                                dist.transforms.AffineTransform(sky_guess,sky_guess_err),)
-                            )
-            self._set_dist('sky_x_sl',  dist.TransformedDistribution(
-                                dist.Normal(),
-                                dist.transforms.AffineTransform(0.0,0.1*sky_guess_err),)
-            )
 
-            self._set_dist('sky_y_sl',dist.TransformedDistribution(
-                                dist.Normal(),
-                                dist.transforms.AffineTransform(0.0,0.1*sky_guess_err),)
+        elif self.sky_type == "none":
+            self.sky_prior = NoSkyPrior(0.0, 0.0)
+
+        elif self.sky_type == "flat":
+            self.sky_prior = FlatSkyPrior(
+                sky_guess=sky_guess, sky_guess_err=sky_guess_err, suffix=suffix
             )
-            
-            self.reparam_dict['sky_back'] = infer.reparam.TransformReparam()
-            self.reparam_dict['sky_x_sl'] = infer.reparam.TransformReparam()
-            self.reparam_dict['sky_y_sl'] = infer.reparam.TransformReparam()
-            self.sample_sky = self.sample_sky_tilted_plane
 
-    def sample_sky_none(self,X: jax.numpy.array,Y: jax.numpy.array)-> float:
-        """Simple wrapper to generate no sky
+        elif self.sky_type == "tilted-plane":
+            self.sky_prior = TiltedPlaneSkyPrior(
+                sky_guess=sky_guess, sky_guess_err=sky_guess_err, suffix=suffix
+            )
 
-        Parameters
-        ----------
-        X : jax.numpy.array
-            2d array, X pixel values
-        Y : jax.numpy.array
-            2d array, Y pixel values
+    @property
+    def param_names(self):
+        return list(self.dist_dict.keys())
 
-        Returns
-        -------
-        float = 0
-            returns 0
-        """
-        return 0.
-    
-    def sample_sky_flat(self,X: jax.numpy.array,Y: jax.numpy.array)-> float:
-        """
-        Sample and generate a flat sky background
+    def sample_sky(self, X: jax.numpy.array, Y: jax.numpy.array) -> float:
+        """Sample sky parameters and return sky model
 
         Parameters
         ----------
         X : jax.numpy.array
-            2d array, X pixel values
+            2D mesh grid of pixel x pixel indices
         Y : jax.numpy.array
-            2d array, Y pixel values
+            2D mesh grid of pixel y pixel indices
 
-        Returns
-        -------
-        float
-            sampled background value
-        """
-        sky_back = sample('sky_back', self.sky_back_prior_dist)
-        return sky_back
-    
-    def sample_sky_tilted_plane(self,X: jax.numpy.array,Y: jax.numpy.array)-> jax.numpy.array:
-        """
-        Sample and generate a tilted-plane sky background
-
-        Parameters
-        ----------
-        X : jax.numpy.array
-            2d array, X pixel values
-        Y : jax.numpy.array
-            2d array, Y pixel values
 
         Returns
         -------
-        jax.numpy.array
-            renderned sky background
+        float
+            sampled and rendered sky model
         """
-        sky_back = sample('sky_back', self.sky_back_prior_dist)
-        sky_x_sl = sample('sky_x_sl', self.sky_x_sl_prior_dist)
-        sky_y_sl = sample('sky_y_sl', self.sky_y_sl_prior_dist)
-        return render_tilted_plane_sky(X,Y, sky_back,sky_x_sl,sky_y_sl)
+        return self.sky_prior.sample(X, Y)
 
-    def _set_dist(self, var_name: str, dist: dist.Distribution)-> None:
+    def _set_dist(self, var_name: str, dist: dist.Distribution) -> None:
         """Set prior for a given variable
 
         Parameters
         ----------
         var_name : str
             variable name
         dist : dist.Distribution
             Numpyro distribution object specifying prior
         """
-        self.__setattr__(var_name+'_prior_dist', dist)
+        self.dist_dict[var_name] = dist
 
-    def _get_dist(self, var_name: str)-> dist.Distribution:
+    def _get_dist(self, var_name: str) -> dist.Distribution:
         """
         Get prior for a given variable
 
         Parameters
         ----------
         var_name : str
             variable name
 
         Returns
         -------
         dist.Distribution
             Numpyro distribution clas describing prior
         """
-        return self.__getattribute__(var_name +'_prior_dist')
-    
-
-class PySersicSourcePrior(BasePrior):
-    """
-    Class used for priors for single source fitting in PySersic
-    """
-    def __init__(self, 
-                profile_type: str, 
-                sky_type: Optional[str] = 'none',
-                sky_guess: Optional[float]=None,
-                sky_guess_err: Optional[float] = None,
-                suffix: Optional[str] =  "") -> None:
-        """Initialize PySersicSourcePrior class
-
-        Parameters
-        ----------
-        profile_type : str
-            Type of profile
-        sky_type : Optional[str], optional
-            Type of sky model to use, one of: none, flat, tilted-plane, by default 'none'
-        suffix : Optional[str], optional
-            Additional suffix to add to each variable name, used in PySersicMultiPrior, by default ""
-        """
-        super().__init__(sky_type= sky_type,sky_guess=sky_guess,sky_guess_err=sky_guess_err)
-        assert profile_type in base_profile_types
-        self.profile_type = profile_type
-        self.param_names = base_profile_params[self.profile_type]
-        self.repr_dict = {}
-        self.built = False
-        self.suffix = suffix
-
-    def __repr__(self, print_sky = True) -> str:
-        out = f"Prior for a {self.profile_type} source:"
-        num_dash = len(out)
-        out += "\n" + "-"*num_dash + "\n"
-        for (var, descrip) in self.repr_dict.items():
-            out += var + " ---  " + descrip + "\n"    
-        if print_sky: # This is not as dynamic as the parameter ones so will not update once set
-            out+= f'\nSky Type: {self.sky_type}\n'
-            if not self.sky_type == 'none':
-                out+=f'Sky level --- Normal w/ mu = {self.sky_guess:.1e}, sigma = {self.sky_guess_err:.1e}\n'
-                if self.sky_type == 'tilted-plane':
-                    out+=f'Sky x slope --- Normal w/ mu = {0}, sigma = {self.sky_guess_err*0.1:.1e}\n'
-                    out+=f'Sky y slope --- Normal w/ mu = {0}, sigma = {self.sky_guess_err*0.1:.1e}\n'
-        return out
-    
-    def _build_dist_list(self)-> None:
-        """
-        Function to combine all distributions into list, sets self.dist_list
-        """
-        self.dist_list = []
-        assert self.check_vars() # check and make sure all is good
-
-        for param in self.param_names:
-            self.dist_list.append(self._get_dist(param+self.suffix))
-        
-        self.built = True
-    
-    def __call__(self) -> jax.numpy.array:
-        """
-        Sample variables from prior
-
-        Returns
-        -------
-        jax.numpy.array
-            sampled variables
-        """
-        if not self.built: 
-            self._build_dist_list()
-
-        arr = []
-        for (param,prior) in zip(self.param_names,self.dist_list):
-            if issubclass(type(prior), dist.Distribution):
-                arr.append(sample(param+self.suffix, prior) )
-            else:
-                arr.append(prior)
-        return jnp.array(arr)      
+        return self.dist_dict[var_name]
 
-    def set_gaussian_prior(self,var_name: str, loc: float, scale: float) -> "PySersicSourcePrior":
+    def set_gaussian_prior(
+        self, var_name: str, loc: float, scale: float
+    ) -> "PySersicSourcePrior":
         """
         Set a Gaussian prior for a variable
 
         Parameters
         ----------
         var_name : str
             variable name
         loc : float
-            mean 
+            mean
         scale : float
             standard deviation
 
         Returns
         -------
         PySersicSourcePrior
             returns self to allow chaining
         """
 
         prior_dist = dist.TransformedDistribution(
             dist.Normal(),
-            dist.transforms.AffineTransform(loc,scale),)
-        
+            dist.transforms.AffineTransform(loc, scale),
+        )
+
         self._set_dist(var_name + self.suffix, prior_dist)
-        self.reparam_dict[var_name  + self.suffix] = infer.reparam.TransformReparam()
+        self.reparam_dict[var_name + self.suffix] = infer.reparam.TransformReparam()
         self.repr_dict[var_name] = f"Normal w/ mu = {loc:.2f}, sigma = {scale:.2f}"
         return self
-    
-    def set_uniform_prior(self, var_name:str, low: float,high: float)-> "PySersicSourcePrior":
+
+    def set_uniform_prior(
+        self, var_name: str, low: float, high: float
+    ) -> "PySersicSourcePrior":
         """
         Set a uniform prior for a variable
 
         Parameters
         ----------
         var_name : str
             variable name
@@ -300,29 +373,32 @@
         Returns
         -------
         PySersicSourcePrior
             returns self to allow chaining
 
         """
         shift = low
-        scale = high-low
+        scale = high - low
         prior_dist = dist.TransformedDistribution(
             dist.Uniform(),
-            dist.transforms.AffineTransform(shift,scale),)
+            dist.transforms.AffineTransform(shift, scale),
+        )
         self._set_dist(var_name + self.suffix, prior_dist)
         self.reparam_dict[var_name + self.suffix] = infer.reparam.TransformReparam()
         self.repr_dict[var_name] = f"Uniform between: {low:.2f} -> {high:.2f}"
         return self
-    
-    def set_truncated_gaussian_prior(self,
-            var_name:str, 
-            loc: float,
-            scale:float, 
-            low: Optional[float] = None,
-            high: Optional[float] = None) -> "PySersicSourcePrior":
+
+    def set_truncated_gaussian_prior(
+        self,
+        var_name: str,
+        loc: float,
+        scale: float,
+        low: Optional[float] = None,
+        high: Optional[float] = None,
+    ) -> "PySersicSourcePrior":
         """
         Set a truncated Gaussian prior for a given variable
 
         Parameters
         ----------
         var_name : str
             variable name
@@ -337,37 +413,42 @@
 
         Returns
         -------
         PySersicSourcePrior
             Returns self to allow chaining
         """
         if low is not None:
-            low_scaled = (low - loc)/scale
+            low_scaled = (low - loc) / scale
         else:
             low = -jnp.inf
             low_scaled = None
-        
+
         if high is not None:
-            high_scaled = (high - loc)/scale
+            high_scaled = (high - loc) / scale
         else:
             high_scaled = None
             high = jnp.inf
         prior_dist = dist.TransformedDistribution(
-            dist.TruncatedNormal(low= low_scaled, high = high_scaled),
-            dist.transforms.AffineTransform(loc,scale),)
-    
+            dist.TruncatedNormal(low=low_scaled, high=high_scaled),
+            dist.transforms.AffineTransform(loc, scale),
+        )
+
         self._set_dist(var_name + self.suffix, prior_dist)
         self.reparam_dict[var_name + self.suffix] = infer.reparam.TransformReparam()
-        self.repr_dict[var_name] = f"Truncated Normal w/ mu = {loc:.2f}, sigma = {scale:.2f}, between: {low:.2f} -> {high:.2f}"
+        self.repr_dict[var_name] = (
+            f"Truncated Normal w/ mu = {loc:.2f}, sigma = {scale:.2f}, between: {low:.2f} -> {high:.2f}"
+        )
         return self
 
-    def set_custom_prior(self, 
-            var_name: str, 
-            prior_dist: dist.Distribution, 
-            reparam: Optional[infer.reparam.Reparam] = None)-> "PySersicSourcePrior":
+    def set_custom_prior(
+        self,
+        var_name: str,
+        prior_dist: dist.Distribution,
+        reparam: Optional[infer.reparam.Reparam] = None,
+    ) -> "PySersicSourcePrior":
         """Set a custom distribution as the prior for a given variable
 
         Parameters
         ----------
         var_name : str
             variable name
         prior_dist : dist.Distribution
@@ -379,173 +460,323 @@
         -------
         PySersicSourcePrior
             Returns self to allow chaining
         """
         self._set_dist(var_name + self.suffix, prior_dist)
         if reparam is not None:
             self.reparam_dict[var_name + self.suffix] = reparam
-        self.repr_dict[var_name] = "Custom prior of type: "+ str(prior_dist.__class__)
+        self.repr_dict[var_name] = "Custom prior of type: " + str(prior_dist.__class__)
         return self
-    
-    def check_vars(self, verbose = False) -> bool:
+
+    def __call__(self) -> jax.numpy.array:
+        """
+        Sample variables from prior
+
+        Returns
+        -------
+        jax.numpy.array
+            sampled variables
+        """
+
+        res_dict = {}
+        for param, prior in self.dist_dict.items():
+            res_dict[param] = sample(param, prior)
+        return res_dict
+
+
+class PySersicSourcePrior(BasePrior):
+    """
+    Class used for priors for single source fitting in PySersic
+    """
+
+    profile_type: str = eqx.field(static=True)
+
+    def __init__(
+        self,
+        profile_type: str,
+        sky_type: Optional[str] = "none",
+        sky_guess: Optional[float] = None,
+        sky_guess_err: Optional[float] = None,
+        suffix: Optional[str] = "",
+    ) -> None:
+        """Initialize PySersicSourcePrior class
+
+        Parameters
+        ----------
+        profile_type : str
+            Type of profile
+        sky_type : Optional[str], optional
+            Type of sky model to use, one of: none, flat, tilted-plane, by default 'none'
+        sky_guess : float
+            Initial guess for level of background, by default None
+        sky_guess_err : float
+            Uncertainty on initial guess, by default None
+        suffix : Optional[str], optional
+            Additional suffix to add to each variable name, by default ""
+        """
+        super().__init__(
+            sky_type=sky_type,
+            sky_guess=sky_guess,
+            sky_guess_err=sky_guess_err,
+            suffix=suffix,
+        )
+        assert profile_type in base_profile_types
+        self.profile_type = profile_type
+
+    def __repr__(self) -> str:
+        out = f"Prior for a {self.profile_type} source:"
+        num_dash = len(out)
+        out += "\n" + "-" * num_dash + "\n"
+        for var, descrip in self.repr_dict.items():
+            out += var + " ---  " + descrip + "\n"
+        out += self.sky_prior.__repr__()
+        return out
+
+    def check_vars(self, verbose=False) -> bool:
         """
         Function to check if all variable for the specified profile type are set with no extras
 
         Parameters
         ----------
         verbose : bool, optional
             Wheter to print out missing and extra variables, by default False
 
         Returns
         -------
         bool
             True if all variable for given type are present with no extra, False otherwise
         """
         missing = []
-        for var in self.param_names:
-            if not hasattr(self, f"{var + self.suffix}_prior_dist"):
+        param_names = base_profile_params[self.profile_type]
+        for var in param_names:
+            if var not in self.dist_dict.keys():
                 missing.append(var)
-        
+
         extra = []
-        for (name, descrip) in self.repr_dict.items():
-            if (name not in self.param_names) and ('sky' not in name):
+        for name, descrip in self.dist_dict.items():
+            if (name not in param_names) and ("sky" not in name):
                 extra.append(name)
         if verbose:
-            print ("Missing params for profile: ", missing)
-            print ("Extra params, will not be used: ", extra)
-        
-        if len(missing)== 0 and len(extra)==0:
+            print("Missing params for profile: ", missing)
+            print("Extra params, will not be used: ", extra)
+
+        if len(missing) == 0 and len(extra) == 0:
             out = True
         else:
             out = False
         return out
-    
-        
+
+
 class PySersicMultiPrior(BasePrior):
     """
     Class used for priors for multi source fitting in PySersic
     """
-    def __init__(self, 
-            catalog: Union[pandas.DataFrame,dict, np.recarray],
-            sky_type: Optional[str] = 'none', 
-            sky_guess: Optional[float] = None,
-            sky_guess_err: Optional[float] = None    
-            )-> None:
+
+    catalog: dict = eqx.field(static=True)
+    N_sources: int
+
+    def __init__(
+        self,
+        catalog: Union[pandas.DataFrame, dict, np.recarray],
+        sky_type: Optional[str] = "none",
+        sky_guess: Optional[float] = None,
+        sky_guess_err: Optional[float] = None,
+        suffix: Optional[str] = "",
+    ) -> None:
         """
-        Ingest a catalog-like data structure containing prior positions and parameters for multiple sources in a single image. 
-        The format of the catalog can be a `pandas.DataFrame`, `numpy` RecordArray, dictionary, or any other format so-long as 
+        Ingest a catalog-like data structure containing prior positions and parameters for multiple sources in a single image.
+        The format of the catalog can be a `pandas.DataFrame`, `numpy` RecordArray, dictionary, or any other format so-long as
         the following fields exist and can be directly indexed: 'x', 'y', 'flux', 'r' and 'type'
 
         Parameters
         ----------
         image : jax.numpy.array
             science image
         catalog : Union[pandas.DataFrame,dict, np.recarray]
-            Object containing information about the sources to be fit
-        Returns
-        -------
-        prior_list : Iterable
-            List containing a prior dictionary for each source
+            Object containing information about the sources to be
+        sky_type : Optional[str], optional
+            Type of sky model to use, one of: none, flat, tilted-plane, by default 'none'
+        sky_guess : float
+            Initial guess for level of background, by default None
+        sky_guess_err : float
+            Uncertainty on initial guess, by default None
+        suffix : Optional[str], optional
+            Additional suffix to add to each variable name, by default ""
         """
-        image = jnp.zeros((100,100)) # dummy image
-        properties = SourceProperties(image)
-        if sky_type != 'none':
-                assert sky_guess is not None and sky_guess_err is not None, "If using a sky model must provide initial guess and uncertainty"
+        properties = SourceProperties(-99)
+
+        if sky_type != "none":
+            assert (
+                sky_guess is not None and sky_guess_err is not None
+            ), "If using a sky model must provide initial guess and uncertainty"
+            properties.set_sky_guess(sky_guess=sky_guess, sky_guess_err=sky_guess_err)
+        else:
+            properties.set_sky_guess(sky_guess=0.0, sky_guess_err=0.0)
+
+        super().__init__(
+            sky_type=sky_type, sky_guess=sky_guess, sky_guess_err=sky_guess_err
+        )
 
-        super().__init__(sky_type = sky_type,sky_guess=sky_guess,sky_guess_err=sky_guess_err)
-        
         self.catalog = catalog
-        self.all_priors = []
-        self.N_sources = len(catalog['x'])
-        image = jnp.zeros((100,100)) # dummy image
-        
-        #Loop through catalog to generate priors
-        for ind in range(len(catalog['x'])):
-            properties.set_flux_guess(catalog['flux'][ind])
-            properties.set_r_eff_guess(r_eff_guess = catalog['r'][ind])
-            properties.set_position_guess((catalog['x'][ind],catalog['y'][ind]) )
-            
+        self.N_sources = len(catalog["x"])
+        self.suffix = suffix
+
+        # Loop through catalog to generate priors
+        for ind in range(len(catalog["x"])):
+            properties.set_flux_guess(catalog["flux"][ind])
+            properties.set_r_eff_guess(r_eff_guess=catalog["r"][ind])
+            properties.set_position_guess((catalog["x"][ind], catalog["y"][ind]))
             try:
-                properties.set_theta_guess(catalog['theta'][ind])
-            except:
-                pass 
-            
-            prior = properties.generate_prior(catalog['type'][ind], sky_type= 'none', suffix  = f'_{ind:d}')
-
-            self.all_priors.append(prior)
-            self.reparam_dict.update(prior.reparam_dict)
-    
-    def __repr__(self,)-> str:
-        out = f"PySersicMultiPrior containing {len(self.all_priors):d} sources \n"
-        for i, source_prior in enumerate(self.all_priors):
-            out += f"\nSource {i:d} : " + source_prior.__repr__(print_sky = False)
-        out+= f'\nSky Type: {self.sky_type}\n'
-        if not self.sky_type == 'none':
-            out+=f'Sky level --- Normal w/ mu = {self.sky_guess:.1e}, sigma = {self.sky_guess_err:.1e}\n'
-            if self.sky_type == 'tilted-plane':
-                out+=f'Sky x slope --- Normal w/ mu = {0}, sigma = {self.sky_guess_err*0.1:.1e}\n'
-                out+=f'Sky y slope --- Normal w/ mu = {0}, sigma = {self.sky_guess_err*0.1:.1e}\n'
+                properties.set_theta_guess(catalog["theta"][ind])
+            except KeyError:
+                properties.set_theta_guess(0)
+
+            dummy_prior = properties.generate_prior(
+                catalog["type"][ind], sky_type="none", suffix=f"_{ind:d}{suffix}"
+            )
+
+            for k, v in dummy_prior.dist_dict.items():
+                self._set_dist(k, v)
+
+            for k, v in dummy_prior.reparam_dict.items():
+                self.reparam_dict[k] = v
+
+            for k, v in dummy_prior.repr_dict.items():
+                self.repr_dict[f"{k}_{ind}"] = v
+            del dummy_prior
+
+    def __repr__(
+        self,
+    ) -> str:
+        out = f"PySersicMultiPrior containing {self.N_sources:d} sources \n"
+        for i, profile_type in enumerate(self.catalog["type"]):
+            out_cur = f"Source #{i} of type - {profile_type}:"
+            num_dash = len(out_cur)
+            out_cur += "\n" + "-" * num_dash + "\n"
+
+            for var in base_profile_params[profile_type]:
+                descrip = self.repr_dict[f"{var}_{i}"]
+                out_cur += f"{var}_{i} ---  {descrip}\n"
+
+            out += out_cur
+        out += self.sky_prior.__repr__()
         return out
-    
-    def __call__(self) -> list:
-        """Sample prior for all sources
 
-        Returns
-        -------
-        list
-            a list of jax.numpy.arrays containing sampled variables for each source
-        """
-        all_params = []
-        for prior_cur in self.all_priors:
-            all_params.append(prior_cur())
-        return all_params
 
+def update_prior_suffix(prior: BasePrior, new_suffix: str) -> BasePrior:
+    """Change the suffix of a pysersic prior
 
+    Parameters
+    ----------
+    prior : BasePrior
+        Either a Source or Multi Prior,
+    new_suffix : str
+        new suffix for variables
 
-class SourceProperties():
+    Returns
+    -------
+    BasePrior
+        Prior with updated suffix
     """
-    A Class used to estimate initial guesses for source properties. If no guesses are provided, then the class will estimate them using the `photutls` package and the `data_properties()` function.
+    old_suffix = copy(prior.suffix)
+
+    def name_change(s: str) -> str:
+        new_s = copy(s)
+        if len(old_suffix) == 0:
+            new_s += new_suffix
+        else:
+            new_s = new_s.replace(old_suffix, new_suffix)
+        return new_s
+
+    new_dist_dict = {}
+    for k, v in prior.dist_dict.items():
+        new_dist_dict[name_change(k)] = prior.dist_dict[k]
+
+    new_reparam_dict = {}
+    for k, v in prior.dist_dict.items():
+        new_reparam_dict[name_change(k)] = prior.reparam_dict[k]
+
+    new_prior = eqx.tree_at(lambda t: t.reparam_dict, prior, new_reparam_dict)
+    new_prior = eqx.tree_at(lambda t: t.dist_dict, new_prior, new_dist_dict)
+    new_prior = eqx.tree_at(lambda t: t.suffix, new_prior, new_suffix)
+
+    new_dist_dict = {}
+    for k, v in prior.sky_prior.dist_dict.items():
+        new_dist_dict[name_change(k)] = prior.sky_prior.dist_dict[k]
+
+    new_reparam_dict = {}
+    for k, v in prior.sky_prior.dist_dict.items():
+        new_reparam_dict[name_change(k)] = prior.sky_prior.reparam_dict[k]
+
+    new_prior = eqx.tree_at(
+        lambda t: t.sky_prior.reparam_dict, new_prior, new_reparam_dict
+    )
+    new_prior = eqx.tree_at(lambda t: t.sky_prior.dist_dict, new_prior, new_dist_dict)
+    new_prior = eqx.tree_at(lambda t: t.sky_prior.suffix, new_prior, new_suffix)
+    return new_prior
+
+
+class SourceProperties:
+    """
+    A Class used to estimate initial guesses for source properties.
+    If no guesses are provided, then the class will estimate them
+    using the `photutls` package and the `data_properties()` function.
     """
-    def __init__(self,image: np.array, mask:np.array =None):
+
+    def __init__(
+        self, image: Union[np.array, jnp.array], mask: Union[np.array, jnp.array] = None
+    ):
         """Initialize the a SourceProperties object
 
         Parameters
         ----------
         image : np.array
             science image
         mask : np.array, optional
             pixel by pixel mask, by default None
         """
-        self.image = image 
-        self.mask = mask 
-        
-        if self.mask is not None:
-            self.cat = data_properties(self.image,mask=self.mask.astype(bool))
-            self.image = np.ma.masked_array(self.image, self.mask )
-        else:
-            self.cat = data_properties(self.image)
-        _ = self.measure_properties() 
+        # Force back to numpy for photutils compatibility
+        if not isinstance(image, int):
+            self.image = np.array(image)
+            if mask is not None:
+                self.mask = np.array(mask)
+            else:
+                self.mask = None
+
+            if self.mask is not None:
+                self.cat = data_properties(self.image, mask=self.mask.astype(bool))
+                self.image = np.ma.masked_array(self.image, self.mask)
+            else:
+                self.cat = data_properties(self.image)
+            _ = self.measure_properties()
 
-    def measure_properties(self,**kwargs) -> SourceProperties:
+    def measure_properties(self, **kwargs) -> SourceProperties:
         """Measure default properties of the source
 
         Returns
         -------
         SourceProperties
             returns self
         """
         self.set_flux_guess(**kwargs)
         self.set_r_eff_guess(**kwargs)
         self.set_theta_guess(**kwargs)
         self.set_position_guess(**kwargs)
         self.set_sky_guess(**kwargs)
         return self
-    
-    def set_sky_guess(self,sky_guess: Optional[float] = None,sky_guess_err:Optional[float] = None,n_pix_sample:int = 5, **kwargs)-> SourceProperties:
-        """Measure or set guess for initial sky background level. If no estimate is provided, the median of the n_pix_sample number of pixels around each edge is used
+
+    def set_sky_guess(
+        self,
+        sky_guess: Optional[float] = None,
+        sky_guess_err: Optional[float] = None,
+        n_pix_sample: int = 5,
+        **kwargs,
+    ) -> SourceProperties:
+        """Measure or set guess for initial sky background level.
+        If no estimate is provided, the median of the n_pix_sample number of pixels around each edge is used
 
         Parameters
         ----------
         sky_guess : Optional[float], optional
             Initial guess for level of background, by default None
         sky_guess_err : Optional[float], optional
             Uncertainity on inital guess, by default None
@@ -553,23 +784,44 @@
             Number of pixels around each edge to use to estimate sky level if neccesary, by default 5
 
         Returns
         -------
         SourceProperties
             returns self
         """
-        med, std, npix = estimate_sky(self.image, n_pix_sample= n_pix_sample)
-        if sky_guess is None:
+
+        if sky_guess is None and hasattr(self, "image"):
+            med, std, npix = estimate_sky(self.image, n_pix_sample=n_pix_sample)
             self.sky_guess = med
-        if sky_guess_err is None:
-            self.sky_guess_err = 2*std/np.sqrt(npix)
+        elif sky_guess is not None:
+            self.sky_guess = sky_guess
+        else:
+            raise RuntimeError(
+                "Need to either supply image or sky_guess_err to source_properties class"
+            )
+        if sky_guess_err is None and hasattr(self, "image"):
+            med, std, npix = estimate_sky(self.image, n_pix_sample=n_pix_sample)
+            self.sky_guess_err = 2 * std / np.sqrt(npix)
+        elif sky_guess_err is not None:
+            self.sky_guess_err = sky_guess_err
+        else:
+            raise RuntimeError(
+                "Need to either supply image or sky_guess_Err to source_properties class"
+            )
         return self
 
-    def set_flux_guess(self,flux_guess: Optional[float] =None,flux_guess_err: Optional[float] = None,**kwargs)-> SourceProperties:
-        """Measure or set guess for initial flux. If no estimate is provided, the flux of the source in estimated as the total flux within the sgmentatated region for the source
+    def set_flux_guess(
+        self,
+        flux_guess: Optional[float] = None,
+        flux_guess_err: Optional[float] = None,
+        **kwargs,
+    ) -> SourceProperties:
+        """Measure or set guess for initial flux.
+        If no estimate is provided, the flux of the source in estimated as the total flux
+        within the sgmentatated region for the source
 
         Parameters
         ----------
         flux_guess : Optional[float], optional
             Initial guess for flux, by default None
         flux_guess_err : Optional[float], optional
             Uncertainty on initial guess, by default None
@@ -581,25 +833,31 @@
         """
         if flux_guess is None:
             flux_guess = self.cat.segment_flux
         if flux_guess_err is not None:
             flux_guess_err = flux_guess_err
         else:
             if flux_guess > 0:
-                flux_guess_err = 2*np.sqrt( flux_guess )
+                flux_guess_err = 2 * np.sqrt(flux_guess)
             else:
-                flux_guess_err = 2*np.sqrt(np.abs(flux_guess))
-                flux_guess = 0.
-        
-        self.flux_guess = flux_guess 
+                flux_guess_err = 2 * np.sqrt(np.abs(flux_guess))
+                flux_guess = 0.0
+
+        self.flux_guess = flux_guess
         self.flux_guess_err = flux_guess_err
-        return self 
-    
-    def set_r_eff_guess(self,r_eff_guess:Optional[float] = None, r_eff_guess_err:Optional[float] = None, **kwargs)-> SourceProperties:
-        """Measure or set guess for effective radius. If no estimate is provided, the r_eff of the source in estimated using photutils
+        return self
+
+    def set_r_eff_guess(
+        self,
+        r_eff_guess: Optional[float] = None,
+        r_eff_guess_err: Optional[float] = None,
+        **kwargs,
+    ) -> SourceProperties:
+        """Measure or set guess for effective radius.
+        If no estimate is provided, the r_eff of the source in estimated using photutils
 
         Parameters
         ----------
         r_eff_guess : Optional[float], optional
             Initial guess for effective radius, by default None
         r_eff_guess_err : Optional[float], optional
             Uncertainty on initial guess, by default None
@@ -607,47 +865,57 @@
         Returns
         -------
         SourceProperties
             returns self
         """
         if r_eff_guess is None:
             r_eff_guess = self.cat.fluxfrac_radius(0.5).to(u.pixel).value
-        
+
         if r_eff_guess_err is not None:
             self.r_eff_guess_err = r_eff_guess_err
         else:
-            self.r_eff_guess_err = 2*np.sqrt(r_eff_guess) 
+            self.r_eff_guess_err = 2 * np.sqrt(r_eff_guess)
 
         self.r_eff_guess = r_eff_guess
         return self
 
-    def set_theta_guess(self,theta_guess: Optional[float] = None,**kwargs)-> SourceProperties:
-        """Measure or set guess for initial position angle. If no estimate is provided, the position angle of the source in estimated using the data_properties() function from photutils
+    def set_theta_guess(
+        self, theta_guess: Optional[float] = None, **kwargs
+    ) -> SourceProperties:
+        """Measure or set guess for initial position angle.
+        If no estimate is provided, the position angle of the source in estimated
+        using the data_properties() function from photutils
 
         Parameters
         ----------
         theta_guess : Optional[float], optional
             Estimate of the position angle in radians, by default None
 
         Returns
         -------
         SourceProperties
             returns self
         """
 
         if theta_guess is None:
-            theta_guess = self.cat.orientation.to(u.rad).value
+            theta_guess = self.cat.orientation.to(u.rad).value + (
+                np.pi / 2
+            )  # make north 0
 
         if np.isnan(theta_guess):
             theta_guess = 0
-        self.theta_guess = theta_guess 
+        self.theta_guess = theta_guess
         return self
-    
-    def set_position_guess(self,position_guess: Optional[Iterable[float,float]]=None,**kwargs)-> SourceProperties:
-        """Measure or set guess for initial position. If no estimate is provided, the position of the source in estimated using the data_properties() function from photutils
+
+    def set_position_guess(
+        self, position_guess: Optional[Iterable[float, float]] = None, **kwargs
+    ) -> SourceProperties:
+        """Measure or set guess for initial position.
+        If no estimate is provided, the position of the source in estimated
+        using the data_properties() function from photutils
 
         Parameters
         ----------
         position_guess : Optional[Iterable[float,float]], optional
             A 2 element list, tuple or array which contain the x,y pixel values of the inital guess for the centroid, by default None
 
         Returns
@@ -658,19 +926,21 @@
         if position_guess is None:
             self.xc_guess = self.cat.centroid_win[0]
             self.yc_guess = self.cat.centroid_win[1]
         else:
             self.xc_guess = position_guess[0]
             self.yc_guess = position_guess[1]
         return self
-    
-    def generate_prior(self,
-                profile_type: str,
-                sky_type: Optional[str] = 'none',
-                suffix: Optional[str] = '')-> PySersicSourcePrior:
+
+    def generate_prior(
+        self,
+        profile_type: str,
+        sky_type: Optional[str] = "none",
+        suffix: Optional[str] = "",
+    ) -> PySersicSourcePrior:
         """Function to generate default priors based on a given image and profile type
 
         Parameters
         ----------
         profile_type : str
             Type of profile
         sky_type : str, default 'none'
@@ -678,94 +948,122 @@
         suffix : str, default ''
             Add suffix onto all source related variables, generally only used to number sources in MultiPrior
         Returns
         -------
         PySersicSourcePrior
             Pysersic prior object to be used to initialize FitSingle
         """
-        
-        prior = PySersicSourcePrior(profile_type=profile_type, sky_type= sky_type,sky_guess=self.sky_guess,sky_guess_err=self.sky_guess_err, suffix=suffix)
-
-        # 3 properties common to all sources
-        prior.set_gaussian_prior('flux',self.flux_guess,self.flux_guess_err)
-        prior.set_gaussian_prior('xc', self.xc_guess, 1.)
-        prior.set_gaussian_prior('yc', self.yc_guess, 1.)
-
-        if profile_type in ['exp','dev','sersic']:
-            prior.set_truncated_gaussian_prior('r_eff', self.r_eff_guess,self.r_eff_guess_err, low = 0.5)
-            prior.set_uniform_prior('ellip', 0, 0.9)
-            prior.set_custom_prior('theta', dist.VonMises(loc = self.theta_guess,concentration=2), reparam= infer.reparam.CircularReparam() )
-            if profile_type == 'sersic':
-                prior.set_uniform_prior('n', 0.65, 8)
 
-        elif profile_type == 'doublesersic':
+        prior = PySersicSourcePrior(
+            profile_type=profile_type,
+            sky_type=sky_type,
+            suffix=suffix,
+            sky_guess=self.sky_guess,
+            sky_guess_err=self.sky_guess_err,
+        )
 
-            prior.set_uniform_prior('f_1', 0.,1.)
-
-            prior.set_custom_prior('theta', dist.VonMises(loc = self.theta_guess,concentration=2), reparam= infer.reparam.CircularReparam() )
-
-            r_loc1 = self.r_eff_guess/1.5
-            r_eff_guess_err1 = jnp.sqrt(self.r_eff_guess/1.5)
-            prior.set_truncated_gaussian_prior('r_eff_1', r_loc1,r_eff_guess_err1, low = 0.5)
-
-            r_loc2 = self.r_eff_guess*1.5
-            r_eff_guess_err2 = jnp.sqrt(self.r_eff_guess*1.5)
-            prior.set_truncated_gaussian_prior('r_eff_2', r_loc2,r_eff_guess_err2, low = 0.5)
+        # 3 properties common to all sources
+        prior.set_gaussian_prior("flux", self.flux_guess, self.flux_guess_err)
+        prior.set_gaussian_prior("xc", self.xc_guess, 1.0)
+        prior.set_gaussian_prior("yc", self.yc_guess, 1.0)
+
+        if profile_type in ["exp", "dev", "sersic", "sersic_pointsource"]:
+            prior.set_truncated_gaussian_prior(
+                "r_eff", self.r_eff_guess, self.r_eff_guess_err, low=0.5
+            )
+            prior.set_uniform_prior("ellip", 0, 0.9)
+            # prior.set_custom_prior('theta',
+            #                       dist.VonMises(loc = self.theta_guess,concentration=2),
+            #                       reparam= infer.reparam.CircularReparam() )
+            prior.set_uniform_prior("theta", 0.0, 2.0 * np.pi)
+
+            if "sersic" in profile_type:
+                prior.set_uniform_prior("n", 0.65, 8)
+                if profile_type == "sersic_pointsource":
+                    prior.set_uniform_prior("f_ps", 0.0, 1.0)
+
+        elif profile_type == "doublesersic":
+            prior.set_uniform_prior("f_1", 0.0, 1.0)
+
+            # prior.set_custom_prior('theta',
+            #                       dist.VonMises(loc = self.theta_guess,concentration=2),
+            #                       reparam= infer.reparam.CircularReparam() )
+            prior.set_uniform_prior("theta", 0.0, 2.0 * np.pi)
+
+            r_loc1 = self.r_eff_guess / 1.5
+            r_eff_guess_err1 = jnp.sqrt(self.r_eff_guess / 1.5)
+            prior.set_truncated_gaussian_prior(
+                "r_eff_1", r_loc1, r_eff_guess_err1, low=0.5
+            )
 
+            r_loc2 = self.r_eff_guess * 1.5
+            r_eff_guess_err2 = jnp.sqrt(self.r_eff_guess * 1.5)
+            prior.set_truncated_gaussian_prior(
+                "r_eff_2", r_loc2, r_eff_guess_err2, low=0.5
+            )
 
-            prior.set_uniform_prior('ellip_1', 0,0.9)
-            prior.set_uniform_prior('ellip_2', 0,0.9)
+            prior.set_uniform_prior("ellip_1", 0, 0.9)
+            prior.set_uniform_prior("ellip_2", 0, 0.9)
 
-            prior.set_truncated_gaussian_prior('n_1',4,1, low = 0.65,high = 8)
-            prior.set_truncated_gaussian_prior('n_2',1,1, low = 0.65,high = 8)
+            prior.set_truncated_gaussian_prior("n_1", 4, 1, low=0.65, high=8)
+            prior.set_truncated_gaussian_prior("n_2", 1, 1, low=0.65, high=8)
 
-        
         return prior
-    
-    def visualize(self,figsize: Tuple[float,float]= (6.,6.),cmap:str = 'gray',scale: float = 1.)-> None:
+
+    def visualize(
+        self,
+        figsize: Tuple[float, float] = (6.0, 6.0),
+        cmap: str = "gray",
+        scale: float = 1.0,
+    ) -> None:
         """Display a figure summarizing the current guess for the source properties
 
         Parameters
         ----------
         figsize : Tuple[float,float], optional
             figure, by default (6.,6.)
         cmap : str, optional
             color map, by default 'gray'
         scale : float, optional
             number of +/- std's at which to clip image, by default 1
         """
-        if not hasattr(self,'flux_guess'):
-            self.set_flux_guess() 
-        if not hasattr(self,'r_eff_guess'):
+        if not hasattr(self, "flux_guess"):
+            self.set_flux_guess()
+        if not hasattr(self, "r_eff_guess"):
             self.set_r_eff_guess()
-        if not hasattr(self,'theta_guess'):
-            self.set_theta_guess() 
-        if not hasattr(self,'xc_guess'):
+        if not hasattr(self, "theta_guess"):
+            self.set_theta_guess()
+        if not hasattr(self, "xc_guess"):
             self.set_position_guess()
-        
-        fig, ax = plt.subplots(figsize=figsize,)
+
+        fig, ax = plt.subplots(
+            figsize=figsize,
+        )
         if self.mask is not None:
-            image= np.ma.masked_array(self.image,mask=self.mask)
+            image = np.ma.masked_array(self.image, mask=self.mask)
         else:
             image = self.image
-        vmin = np.mean(image) - scale*np.std(image)
-        vmax = np.mean(image) + scale*np.std(image)
-        ax.imshow(image,cmap=cmap,origin='lower',vmin=vmin,vmax=vmax)
-        ax.plot(self.xc_guess,self.yc_guess,'x',color='r')
-        
-        dx = 10*self.r_eff_guess*np.cos(self.theta_guess+np.pi/2.)
-        dy = 10*self.r_eff_guess*np.sin(self.theta_guess+np.pi/2.)
-        ax.arrow(self.xc_guess,self.yc_guess,dx=dx,dy=dy,width=0.1,head_width=1)
-        arr = np.linspace(0,2*np.pi,100)
-        x = np.cos(arr) * self.r_eff_guess + self.xc_guess 
-        y = np.sin(arr) * self.r_eff_guess + self.yc_guess 
-        ax.plot(x,y,'r',lw=2)
+        vmin = np.mean(image) - scale * np.std(image)
+        vmax = np.mean(image) + scale * np.std(image)
+        ax.imshow(image, cmap=cmap, origin="lower", vmin=vmin, vmax=vmax)
+        ax.plot(self.xc_guess, self.yc_guess, "x", color="r")
+
+        dx = 10 * self.r_eff_guess * np.cos(self.theta_guess)
+        dy = 10 * self.r_eff_guess * np.sin(self.theta_guess)
+        ax.arrow(self.xc_guess, self.yc_guess, dx=dx, dy=dy, width=0.1, head_width=1)
+        arr = np.linspace(0, 2 * np.pi, 100)
+        x = np.cos(arr) * self.r_eff_guess + self.xc_guess
+        y = np.sin(arr) * self.r_eff_guess + self.yc_guess
+        ax.plot(x, y, "r", lw=2)
         plt.show()
 
-def estimate_sky(image: np.array, mask: Optional[np.array] = None, n_pix_sample:int = 5 )-> Tuple[float,float,int]:
+
+def estimate_sky(
+    image: np.array, mask: Optional[np.array] = None, n_pix_sample: int = 5
+) -> Tuple[float, float, int]:
     """Estimate the sky background using the edge of the cutout
 
     Parameters
     ----------
     im : np.array
         image, either an array or masked array
     mask : Optional[np.array], optional
@@ -774,22 +1072,33 @@
         number of pixels around the edge to use, by default 5
 
     Returns
     -------
     Tuple[float,float,int]
         a tuple containing the median, standard deviation and number of pixels used
     """
-    if not np.ma.is_masked(image) and not mask is None:
-        image = np.ma.masked_array(image, mask )
-    edge_pixels = np.concatenate((image[:n_pix_sample,:],image[-n_pix_sample:,:],image[n_pix_sample:-n_pix_sample,:n_pix_sample],image[n_pix_sample:-n_pix_sample,-n_pix_sample:]),axis=None)
+    if not np.ma.is_masked(image) and mask is not None:
+        image = np.ma.masked_array(image, mask)
+    edge_pixels = np.concatenate(
+        (
+            image[:n_pix_sample, :],
+            image[-n_pix_sample:, :],
+            image[n_pix_sample:-n_pix_sample, :n_pix_sample],
+            image[n_pix_sample:-n_pix_sample, -n_pix_sample:],
+        ),
+        axis=None,
+    )
     median_val = np.ma.median(edge_pixels)
     err_on_median = bws(edge_pixels)
     return median_val, err_on_median, np.prod(edge_pixels.shape)
 
-def autoprior(image: np.array, profile_type: 'str', mask:np.array =None, sky_type: str = 'none') -> PySersicSourcePrior:
+
+def autoprior(
+    image: np.array, profile_type: "str", mask: np.array = None, sky_type: str = "none"
+) -> PySersicSourcePrior:
     """Simple wrapper function to generate a prior using the built-in defaults. This can be used as a starting place but may not work for all sources
 
     Parameters
     ----------
     image : np.array
         science image
     profile_type : str
@@ -800,11 +1109,12 @@
         Type of sky to fit, default 'none'
 
     Returns
     -------
     PySersicSourcePrior
         Prior object that can be used in initializing FitSingle
     """
-    props = SourceProperties(image = image, mask = mask)
-    prior = props.generate_prior(profile_type = profile_type, sky_type = sky_type)
-    return prior
 
+    props = SourceProperties(image=image, mask=mask)
+
+    prior = props.generate_prior(profile_type=profile_type, sky_type=sky_type)
+    return prior
```

### Comparing `pysersic-0.1.2/pysersic/pysersic.py` & `pysersic-0.1.4/pysersic/pysersic.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,45 +1,52 @@
 import copy
+import warnings
 from abc import ABC, abstractmethod
 from functools import partial
-from typing import Callable, Optional, Union
+from typing import Callable, Optional
 
 import jax
 import jax.numpy as jnp
 import numpy as np
 import numpyro
 import pandas
 import tqdm
 from jax.random import PRNGKey
+from jax.typing import ArrayLike
 from numpyro import deterministic, infer, optim
 from numpyro.handlers import condition, trace
 from numpyro.infer import SVI, Trace_ELBO
 from numpyro.infer.svi import SVIRunResult
-from pysersic.exceptions import *
-from pysersic.priors import PySersicMultiPrior, PySersicSourcePrior
-from pysersic.rendering import BaseRenderer, HybridRenderer
-from pysersic.results import PySersicResults
 
+from .exceptions import KernelError, ShapeMatchError
 from .loss import gaussian_loss
+from .priors import PySersicMultiPrior, PySersicSourcePrior, base_profile_params
+from .rendering import BaseRenderer, HybridRenderer, base_profile_types
+from .results import PySersicResults
 
-ArrayLike = Union[np.array, jax.numpy.array]
+
+def identity(x: Callable) -> Callable:
+    return x
 
 
 class BaseFitter(ABC):
     """
     Base class for Pysersic Fitters
     """
-    def __init__(self,
+
+    def __init__(
+        self,
         data: ArrayLike,
         rms: ArrayLike,
         psf: ArrayLike,
         mask: Optional[ArrayLike] = None,
         loss_func: Optional[Callable] = gaussian_loss,
-        renderer: Optional[BaseRenderer] =  HybridRenderer, 
-        renderer_kwargs: Optional[dict] = {}) -> None:
+        renderer: Optional[BaseRenderer] = HybridRenderer,
+        renderer_kwargs: Optional[dict] = {},
+    ) -> None:
         """Initialze BaseFitter class
 
         Parameters
         ----------
         data : ArrayLike
             Science image to be fit
         weight_map : ArrayLike
@@ -52,63 +59,64 @@
             One of None, 'flat' or 'tilted-plane' specifying how to model the sky background
         renderer : Optional[BaseRenderer], optional
             The renderer to be used to generate model images, by default HybridRenderer
         renderer_kwargs : Optional[dict], optional
             Any additional arguments to pass to the renderer, by default {}
         """
 
-        
         self.loss_func = loss_func
 
-        
-        self.data = jnp.array(data) 
-        self.rms = jnp.array(rms)
-        self.psf = jnp.array(psf)
-        self.mask = parse_mask(mask,self.data)
-        data_isgood = check_input_data(self.data,rms=self.rms,psf=self.psf,mask=jnp.logical_not(self.mask))
-        self.renderer = renderer(data.shape, psf, **renderer_kwargs)
-    
+        self.data = jnp.array(data.astype(np.float32))
+        self.rms = jnp.array(rms.astype(np.float32))
+        self.psf = jnp.array(psf.astype(np.float32))
+        self.mask = parse_mask(mask, self.data)
+        data_isgood = check_input_data(
+            self.data, rms=self.rms, psf=self.psf, mask=jnp.logical_not(self.mask)
+        )
+        self.renderer = renderer(data.shape, self.psf, **renderer_kwargs)
+        self.prior = None
         self.prior_dict = {}
 
-    
     def set_loss_func(self, loss_func: Callable) -> None:
         """Set loss function to be used for inference
 
         Parameters
         ----------
         loss_func : Callable
             Functions which takes samples the loss function, see utils/loss.py for some examples.
         """
         self.loss_func = loss_func
 
-    def set_prior(self,parameter: str,
-        distribution: numpyro.distributions.Distribution) -> None:
+    def set_prior(
+        self, parameter: str, distribution: numpyro.distributions.Distribution
+    ) -> None:
         """Set the prior for a specific parameter
 
         Parameters
         ----------
         parameter : str
             Parameter to be set
         distribution : numpyro.distributions.Distribution
             Numpyro distribution object corresponding to the prior
         """
         self.prior_dict[parameter] = distribution
 
-
-    def sample(self,
-                num_samples: int = 1000,
-                num_warmup: int = 1000,
-                num_chains: int = 2,
-                init_strategy: Optional[Callable] = infer.init_to_sample,
-                sampler_kwargs: Optional[dict] ={},
-                mcmc_kwargs: Optional[dict] = {},
-                return_model: Optional[bool] = True,
-                rkey: Optional[jax.random.PRNGKey] = jax.random.PRNGKey(3)     
-        ) -> pandas.DataFrame:
-        """ Perform inference using a NUTS sampler
+    def sample(
+        self,
+        rkey: jax.random.PRNGKey,
+        num_samples: int = 1000,
+        num_warmup: int = 1000,
+        num_chains: int = 2,
+        init_strategy: Optional[Callable] = infer.init_to_sample,
+        sampler_kwargs: Optional[dict] = {},
+        mcmc_kwargs: Optional[dict] = {},
+        return_model: Optional[bool] = True,
+        reparam_func: Optional[Callable] = identity,
+    ) -> pandas.DataFrame:
+        """Perform inference using a NUTS sampler
 
         Parameters
         ----------
         num_samples : int, optional
             Number of samples to draw, by default 1000
         num_warmup : int, optional
             Number of warmup samples, by default 1000
@@ -127,36 +135,49 @@
 
         Returns
         -------
         pandas.DataFrame
             ArviZ summary of posterior
         """
 
-        model =  self.build_model(return_model = return_model)
-        self.sampler =infer.MCMC(infer.NUTS(model,init_strategy=init_strategy, **sampler_kwargs),num_chains=num_chains, num_samples=num_samples, num_warmup=num_warmup,  **mcmc_kwargs)
-        self.sampler.run(rkey)
-        self.sampling_results = PySersicResults(data=self.data,rms=self.rms,psf=self.psf,mask=self.mask,loss_func=self.loss_func,renderer=self.renderer)
+        model = self.build_model(return_model=return_model)
+        model = reparam_func(model)
+        sampler = infer.MCMC(
+            infer.NUTS(model, init_strategy=init_strategy, **sampler_kwargs),
+            num_chains=num_chains,
+            num_samples=num_samples,
+            num_warmup=num_warmup,
+            **mcmc_kwargs,
+        )
+        sampler.run(rkey)
+        self.sampling_results = PySersicResults(
+            data=self.data,
+            rms=self.rms,
+            psf=self.psf,
+            mask=self.mask,
+            loss_func=self.loss_func,
+            renderer=self.renderer,
+        )
         self.sampling_results.add_prior(self.prior)
-        self.sampling_results.injest_data(sampler = self.sampler)
-        return self.sampling_results 
-        
-
-
-    def _train_SVI(self,
-            autoguide: numpyro.infer.autoguide.AutoContinuous,
-            method:str,
-            ELBO_loss: Optional[Callable] = infer.Trace_ELBO(1),
-            lr_init: Optional[int] = 1e-2,
-            num_round: Optional[int] = 3,
-            SVI_kwargs: Optional[dict]= {},
-            train_kwargs: Optional[dict] = {},
-            return_model: Optional[bool] = True,
-            num_sample: Optional[int] = 1_000,
-            rkey: Optional[jax.random.PRNGKey] = jax.random.PRNGKey(6),
-            )-> pandas.DataFrame:
+        self.sampling_results.injest_data(sampler=sampler)
+        return self.sampling_results
+
+    def _train_SVI(
+        self,
+        autoguide: numpyro.infer.autoguide.AutoContinuous,
+        method: str,
+        rkey: jax.random.PRNGKey,
+        ELBO_loss: Optional[Callable] = infer.Trace_ELBO(5),
+        lr_init: Optional[int] = 1e-2,
+        num_round: Optional[int] = 3,
+        SVI_kwargs: Optional[dict] = {},
+        train_kwargs: Optional[dict] = {},
+        return_model: Optional[bool] = True,
+        num_sample: Optional[int] = 1_000,
+    ) -> pandas.DataFrame:
         """
         Internal function to perform inference using stochastic variational inference.
 
         Parameters
         ----------
         autoguide : numpyro.infer.autoguide.AutoContinuous
             Function to build guide
@@ -183,30 +204,43 @@
         -------
         pandas.DataFrame
             ArviZ summary of posterior
         """
         model_cur = self.build_model(return_model=return_model)
         guide = autoguide(model_cur)
 
-        svi_kernel = SVI(model_cur,guide, optim.Adam(0.1), loss = ELBO_loss, **SVI_kwargs)
-        numpyro_svi_result = train_numpyro_svi_early_stop(svi_kernel,rkey=rkey,lr_init=lr_init,
-                                                        num_round=num_round, **train_kwargs)
-
-        svi_res_dict =  dict(guide = guide, model = model_cur, svi_result = numpyro_svi_result)
-        self.svi_results = PySersicResults(data=self.data,rms=self.rms,psf=self.psf,mask=self.mask,loss_func=self.loss_func,renderer=self.renderer)
-        self.svi_results.injest_data(svi_res_dict=svi_res_dict,purge_extra=True, num_sample = num_sample)
+        svi_kernel = SVI(
+            model_cur, guide, optim.Adam(0.01), loss=ELBO_loss, **SVI_kwargs
+        )
+        numpyro_svi_result = train_numpyro_svi_early_stop(
+            svi_kernel, rkey=rkey, lr_init=lr_init, num_round=num_round, **train_kwargs
+        )
+
+        svi_res_dict = dict(guide=guide, model=model_cur, svi_result=numpyro_svi_result)
+        self.svi_results = PySersicResults(
+            data=self.data,
+            rms=self.rms,
+            psf=self.psf,
+            mask=self.mask,
+            loss_func=self.loss_func,
+            renderer=self.renderer,
+        )
+        self.svi_results.injest_data(
+            svi_res_dict=svi_res_dict, purge_extra=True, num_sample=num_sample
+        )
         self.svi_results.add_prior(self.prior)
         self.svi_results.add_method_used(method)
         return self.svi_results
 
-
-    
-    def find_MAP(self,
-                return_model: Optional[bool] = True,
-                rkey: Optional[jax.random.PRNGKey] = jax.random.PRNGKey(3),):
+    def find_MAP(
+        self,
+        rkey: jax.random.PRNGKey,
+        return_model: Optional[bool] = True,
+        purge_extra: Optional[bool] = True,
+    ):
         """Find the "best-fit" parameters as the maximum a-posteriori and return a dictionary with values for the parameters.
 
         Parameters
         ----------
         return_model : Optional[bool]
             Whether to return the model images but adds a small memory/time overhead, by default True
         rkey : Optional[jax.random.PRNGKey], optional
@@ -214,42 +248,62 @@
 
         Returns
         -------
         dict
             dictionary with fit parameters and their values.
         """
         model_cur = self.build_model(return_model=return_model)
-        autoguide_map = infer.autoguide.AutoDelta(model_cur, init_loc_fn= infer.init_to_median)
-        train_kwargs = dict(lr_init = 0.01, num_round = 3,frac_lr_decrease  = 0.1, patience = 250, optimizer = optim.Adam, max_train = int(1e4))
-        svi_kernel = SVI(model_cur,autoguide_map, optim.Adam(0.01),loss=Trace_ELBO())
-        
-        res = train_numpyro_svi_early_stop(svi_kernel,rkey=rkey, **train_kwargs)
+        autoguide_map = infer.autoguide.AutoDelta(
+            model_cur, init_loc_fn=infer.init_to_median
+        )
+        train_kwargs = dict(
+            lr_init=0.05,
+            num_round=3,
+            frac_lr_decrease=0.1,
+            patience=250,
+            optimizer=optim.Adam,
+            max_train=int(2e4),
+        )
+        svi_kernel = SVI(model_cur, autoguide_map, optim.Adam(0.01), loss=Trace_ELBO())
+
+        res = train_numpyro_svi_early_stop(svi_kernel, rkey=rkey, **train_kwargs)
 
         use_dict = {}
         for key in res.params.keys():
-            pref = key.split('_auto_loc')[0]
+            pref = key.split("_auto_loc")[0]
             use_dict[pref] = res.params[key]
         trace_out = trace(condition(model_cur, use_dict)).get_trace()
         real_out = {}
-        for key in trace_out:
-            if key == 'Loss':
-                continue
-            elif key == 'model':
-                real_out[key] = np.asarray(trace_out[key]['value'])
-            elif not ('base' in key or 'auto' in key or 'unwrapped' in key or 'factor' in key or 'loss' in key):
-                real_out[key] = float('{:.5e}'.format(trace_out[key]['value']) )
 
+        if purge_extra:
+            for key in trace_out:
+                if "Loss" in key:
+                    continue
+                elif key == "model":
+                    real_out[key] = np.asarray(trace_out[key]["value"])
+                elif not (
+                    "base" in key
+                    or "auto" in key
+                    or "unwrapped" in key
+                    or "factor" in key
+                    or "loss" in key
+                ):
+                    real_out[key] = np.round(trace_out[key]["value"], 5)
+        else:
+            for k, v in trace_out.items():
+                real_out[k] = v["value"]
         return real_out
-    
-    def estimate_posterior(self,
-                        method : str='laplace',
-                        return_model: bool = True,
-                        num_sample: Optional[int] = 1_000,
-                        rkey: Optional[jax.random.PRNGKey] = jax.random.PRNGKey(6),
-                        ) -> pandas.DataFrame:
+
+    def estimate_posterior(
+        self,
+        rkey: jax.random.PRNGKey,
+        method: str = "laplace",
+        return_model: bool = True,
+        num_sample: Optional[int] = 1_000,
+    ) -> pandas.DataFrame:
         """Estimate the posterior using a method other than MCMC sampling. Generally faster than MCMC, but could be less accurate.
         Current Options are:
         - 'laplace'
             - Uses the Laplace approximation, which finds the MAP and then uses a Gaussian approximation to the posterior. The covariance matrix is calculated using the Hessian of the log posterior at the MAP. Generally the fastest method but can lead to numerical problems, especially for fitting several (~> 5) sources since this involves inverting a large matrix.
         - 'svi-mvn'
             - Use variational inference to fit a multivariate normal distribution to the posterior. In practice should give similar results to 'laplace', as both assume the posterior is a multivariate Gaussian but is trained differently and generally less susceptible to the numerical issues discussed above.
         - 'svi-flow'
@@ -262,49 +316,92 @@
         return_model : Optional[bool]
             Whether to return the model images but adds a small memory/time overhead, by default True
                 num_sample: Optional[int]
         Number of samples to draw from trained SVI posterior
             Number of samples to draw from trained SVI posterior
         rkey : Optional[jax.random.PRNGKey], optional
             rng key, by default jax.random.PRNGKey(6)
-        
+
         """
-        assert method in ['laplace','svi-flow','svi-mvn']
-        if method=='laplace':
-            train_kwargs = dict(patience = 250, max_train = 10000)
-            guide_func = partial(infer.autoguide.AutoLaplaceApproximation, init_loc_fn = infer.init_to_median )
-            results = self._train_SVI(guide_func,method=method, train_kwargs=train_kwargs, return_model = return_model, rkey=rkey, num_sample=num_sample)
-        elif method=='svi-flow':
-            train_kwargs = dict(patience = 500, max_train = 20000)
-            guide_func = partial(infer.autoguide.AutoBNAFNormal, num_flows =4,hidden_factors = [5,], init_loc_fn = infer.init_to_median)
-            results = self._train_SVI(guide_func,method='svi-flow',ELBO_loss= infer.Trace_ELBO(8),train_kwargs=train_kwargs,num_round=3,lr_init = 1e-2, rkey=rkey,return_model = return_model,num_sample=num_sample)
-        elif method=='svi-mvn':
-            train_kwargs = dict(patience = 200, max_train = 5000)
-            guide_func = partial(infer.autoguide.AutoLowRankMultivariateNormal, init_scale = 5e-3, init_loc_fn = infer.init_to_median)
-            results = self._train_SVI(guide_func,method='svi-mvn',ELBO_loss= infer.TraceMeanField_ELBO(16),train_kwargs=train_kwargs,num_round=3,lr_init = 1e-1, rkey=rkey,return_model = return_model,num_sample=num_sample)
+        assert method in ["laplace", "svi-flow", "svi-mvn"]
+        if method == "laplace":
+            train_kwargs = dict(patience=250, max_train=20000)
+            guide_func = partial(
+                infer.autoguide.AutoLaplaceApproximation,
+                init_loc_fn=infer.init_to_median,
+            )
+            results = self._train_SVI(
+                guide_func,
+                method=method,
+                lr_init=0.05,
+                train_kwargs=train_kwargs,
+                return_model=return_model,
+                rkey=rkey,
+                num_sample=num_sample,
+            )
+        elif method == "svi-flow":
+            train_kwargs = dict(patience=500, max_train=20000)
+            guide_func = partial(
+                infer.autoguide.AutoBNAFNormal,
+                num_flows=1,
+                hidden_factors=[16, 8],
+                init_loc_fn=infer.init_to_median,
+            )
+            results = self._train_SVI(
+                guide_func,
+                method="svi-flow",
+                ELBO_loss=infer.Trace_ELBO(8),
+                train_kwargs=train_kwargs,
+                num_round=3,
+                lr_init=5e-2,
+                rkey=rkey,
+                return_model=return_model,
+                num_sample=num_sample,
+            )
+        elif method == "svi-mvn":
+            train_kwargs = dict(patience=200, max_train=5000)
+            guide_func = partial(
+                infer.autoguide.AutoLowRankMultivariateNormal,
+                init_scale=5e-3,
+                init_loc_fn=infer.init_to_median,
+            )
+            results = self._train_SVI(
+                guide_func,
+                method="svi-mvn",
+                ELBO_loss=infer.TraceMeanField_ELBO(5),
+                train_kwargs=train_kwargs,
+                num_round=3,
+                lr_init=5e-2,
+                rkey=rkey,
+                return_model=return_model,
+                num_sample=num_sample,
+            )
         return results
 
     @abstractmethod
-    def build_model(self,return_model: bool = True):
+    def build_model(self, return_model: bool = True):
         raise NotImplementedError
 
 
 class FitSingle(BaseFitter):
     """
     Class used to fit a single source
     """
-    def __init__(self,
+
+    def __init__(
+        self,
         data: ArrayLike,
         rms: ArrayLike,
         psf: ArrayLike,
         prior: PySersicSourcePrior,
         mask: Optional[ArrayLike] = None,
         loss_func: Optional[Callable] = gaussian_loss,
-        renderer: Optional[BaseRenderer] =  HybridRenderer, 
-        renderer_kwargs: Optional[dict] = {}) -> None:
+        renderer: Optional[BaseRenderer] = HybridRenderer,
+        renderer_kwargs: Optional[dict] = {},
+    ) -> None:
         """Initialze FitSingle class
 
         Parameters
         ----------
         data : ArrayLike
             Science image to be fit
         weight_map : ArrayLike
@@ -319,63 +416,79 @@
             Must be one of: ['sersic','doublesersic','pointsource','exp','dev'] specifying how to paramaterize the source, default 'sersic'
         renderer : Optional[BaseRenderer], optional
             The renderer to be used to generate model images, by default HybridRenderer
         renderer_kwargs : Optional[dict], optional
             Any additional arguments to pass to the renderer, by default {}
         """
 
-        super().__init__(data,rms,psf,loss_func = loss_func, mask = mask, renderer = renderer, renderer_kwargs = renderer_kwargs)
-
-        if prior.profile_type not in self.renderer.profile_types:
-            raise AssertionError('Profile must be one of:', self.renderer.profile_types)
+        super().__init__(
+            data,
+            rms,
+            psf,
+            loss_func=loss_func,
+            mask=mask,
+            renderer=renderer,
+            renderer_kwargs=renderer_kwargs,
+        )
+
+        if prior.profile_type not in base_profile_types:
+            raise AssertionError("Profile must be one of:", base_profile_types)
+        self.profile_type_number = 0
         self.prior = prior
-        
-
 
     def build_model(self, return_model: bool = True) -> Callable:
-        """ Generate Numpyro model for the specified image, profile and priors
+        """Generate Numpyro model for the specified image, profile and priors
 
         Returns
         -------
         model: Callable
             Function specifying the current model in Numpyro, can be passed to inference algorithms
         """
         # Make sure all variables have priors
         check_prior = self.prior.check_vars
         if not check_prior:
-            raise AssertionError('Not all variables have priors, please run .autogenerate_priors')
+            raise AssertionError(
+                "Not all variables have priors, please run .autogenerate_priors"
+            )
 
-        @numpyro.handlers.reparam(config = self.prior.reparam_dict)
+        @numpyro.handlers.reparam(config=self.prior.reparam_dict)
         def model(return_model: bool = return_model):
             params = self.prior()
-            out = self.renderer.render_source(params, self.prior.profile_type)
+            out = self.renderer.render_source(
+                params, self.prior.profile_type, suffix=self.prior.suffix
+            )
 
             sky = self.prior.sample_sky(self.renderer.X, self.renderer.Y)
 
             obs = out + sky
             if return_model:
-                deterministic('model', obs)
-            self.loss_func(obs, self.data, self.rms, self.mask)
+                deterministic(f"model{self.prior.suffix}", obs)
+            self.loss_func(
+                obs, self.data, self.rms, self.mask, suffix=self.prior.suffix
+            )
+
         return model
 
-    
 
 class FitMulti(BaseFitter):
     """
     Class used to fit multiple sources within a single image
     """
-    def __init__(self,
+
+    def __init__(
+        self,
         data: ArrayLike,
         rms: ArrayLike,
         psf: ArrayLike,
         prior: PySersicMultiPrior,
         mask: Optional[ArrayLike] = None,
         loss_func: Optional[Callable] = gaussian_loss,
-        renderer: Optional[BaseRenderer] =  HybridRenderer, 
-        renderer_kwargs: Optional[dict] = {}) -> None:
+        renderer: Optional[BaseRenderer] = HybridRenderer,
+        renderer_kwargs: Optional[dict] = {},
+    ) -> None:
         """Initialze FitMulti class
 
         Parameters
         ----------
         data : ArrayLike
             Science image to be fit
         weight_map : ArrayLike
@@ -389,82 +502,99 @@
         profile_type : Optional[str], optional
             Must be one of: ['sersic','doublesersic','pointsource','exp','dev'] specifying how to paramaterize the source, default 'sersic'
         renderer : Optional[BaseRenderer], optional
             The renderer to be used to generate model images, by default HybridRenderer
         renderer_kwargs : Optional[dict], optional
             Any additional arguments to pass to the renderer, by default {}
         """
-        super().__init__(data,rms,psf,mask = mask,loss_func = loss_func,renderer = renderer, renderer_kwargs = renderer_kwargs)
+        super().__init__(
+            data,
+            rms,
+            psf,
+            mask=mask,
+            loss_func=loss_func,
+            renderer=renderer,
+            renderer_kwargs=renderer_kwargs,
+        )
         self.prior = prior
-        
+
     def build_model(self, return_model: bool = True) -> Callable:
         """Generate Numpyro model for the specified image, profile and priors
 
         Returns
         -------
         model: Callable
             Function specifying the current model in Numpyro, can be passed to inference algorithms
         """
 
-        @numpyro.handlers.reparam(config = self.prior.reparam_dict)
+        @numpyro.handlers.reparam(config=self.prior.reparam_dict)
         def model(return_model: bool = return_model):
             source_variables = self.prior()
 
-            out = self.renderer.render_multi(self.prior.catalog['type'],source_variables)
+            out = self.renderer.render_for_model(
+                source_variables, self.prior.catalog["type"], suffix=self.prior.suffix
+            )
             sky = self.prior.sample_sky(self.renderer.X, self.renderer.Y)
 
             obs = out + sky
 
             if return_model:
-                obs = deterministic('model', obs)
-            
-            loss = self.loss_func(obs, self.data, self.rms, self.mask)
-            return loss
+                deterministic(f"model{self.prior.suffix}", obs)
+            self.loss_func(
+                obs, self.data, self.rms, self.mask, suffix=self.prior.suffix
+            )
 
         return model
 
-    def find_MAP(self,
-                return_model: Optional[bool] = True,
-                rkey: Optional[jax.random.PRNGKey] = jax.random.PRNGKey(3),):
+    def find_MAP(
+        self,
+        return_model: Optional[bool] = True,
+        rkey: Optional[jax.random.PRNGKey] = jax.random.PRNGKey(3),
+        purge_extra: Optional[bool] = True,
+    ):
         """Find the "best-fit" parameters as the maximum a-posteriori and return a dictionary with values for the parameters.
 
         Parameters
         ----------
         return_model : Optional[bool], optional
             whether to return the model image, adds a small time and memory overhead, by default True
         rkey : Optional[jax.random.PRNGKey], optional
             rng key, by default jax.random.PRNGKey(3)
 
         Returns
         -------
         dict
             dictionary with fit parameters and their values.
         """
-        raw_dict = super().find_MAP(return_model=return_model, rkey=rkey)
-        results_dict = {}
-        for i in range(self.prior.N_sources):
-            results_dict[f'source_{i}'] = {}
-            for pname in self.prior.all_priors[i].param_names:
-                results_dict[f'source_{i}'][pname] = raw_dict.pop(pname + f'_{i:d}')
-        results_dict.update(raw_dict)
+        raw_dict = super().find_MAP(
+            return_model=return_model, rkey=rkey, purge_extra=purge_extra
+        )
+
+        if purge_extra:
+            results_dict = {}
+            for i in range(self.prior.N_sources):
+                results_dict[f"source_{i}"] = {}
+                for pname in base_profile_params[self.prior.catalog["type"][i]]:
+                    results_dict[f"source_{i}"][pname] = raw_dict.pop(pname + f"_{i:d}")
+            results_dict.update(raw_dict)
+        else:
+            results_dict = raw_dict
         return results_dict
 
 
-
-
 def train_numpyro_svi_early_stop(
-        svi_class: SVI,
-        num_round: Optional[int] = 3,
-        max_train: Optional[int] = 5000,
-        lr_init: Optional[float] = 0.01,
-        frac_lr_decrease: Optional[float]  = 0.1,
-        patience: Optional[int] = 100,
-        optimizer: Optional[optim._NumPyroOptim] = optim.Adam,
-        rkey: Optional[PRNGKey] = PRNGKey(10),
-    )-> SVIRunResult:
+    svi_class: SVI,
+    num_round: Optional[int] = 3,
+    max_train: Optional[int] = 5000,
+    lr_init: Optional[float] = 0.01,
+    frac_lr_decrease: Optional[float] = 0.1,
+    patience: Optional[int] = 100,
+    optimizer: Optional[optim._NumPyroOptim] = optim.Adam,
+    rkey: Optional[PRNGKey] = PRNGKey(10),
+) -> SVIRunResult:
     """Optimize a SVI model by training for multiple rounds with a deacreasing learning rate, and early stopping for each round
 
     Parameters
     ----------
     svi_class : SVI
         Initialized numpyo SVI class, note that the optimizer will be overwritten
     num_round : Optional[int], optional
@@ -484,34 +614,34 @@
 
     Returns
     -------
     SVIRunResult
         SVI Result class containing trained model
     """
     optim_init = optimizer(lr_init)
-    svi_class.__setattr__('optim', optim_init)
+    svi_class.__setattr__("optim", optim_init)
 
     init_state = svi_class.init(rkey)
     all_losses = []
 
-    @partial(jax.jit, static_argnums = 1)
-    def update_func(state,svi_class,lr):
-        svi_class.__setattr__('optim', optimizer(lr))
-        state,loss = svi_class.stable_update(state)
-        return state,loss
+    @partial(jax.jit, static_argnums=1)
+    def update_func(state, svi_class, lr):
+        svi_class.__setattr__("optim", optimizer(lr))
+        state, loss = svi_class.stable_update(state)
+        return state, loss
 
     best_state, best_loss = update_func(init_state, svi_class, lr_init)
-    
+
     for r in range(num_round):
         losses = []
         wait_counter = 0
         svi_state = copy.copy(best_state)
 
-        if r>0:
-            lr_cur = lr_init*frac_lr_decrease**r
+        if r > 0:
+            lr_cur = lr_init * frac_lr_decrease**r
             best_loss = jnp.inf
         else:
             lr_cur = lr_init
 
         with tqdm.trange(1, max_train + 1) as t:
             for j in t:
                 svi_state, loss = update_func(svi_state, svi_class, lr_cur)
@@ -519,64 +649,76 @@
                     best_loss = loss
                     best_state = copy.copy(svi_state)
                     wait_counter = 0
                 elif wait_counter >= patience:
                     break
                 else:
                     wait_counter += 1
-                t.set_postfix_str(f'Round = {r:d},step_size = {lr_cur:.1e} loss: {best_loss:.3e}',refresh=False)
+                t.set_postfix_str(
+                    f"Round = {r:d},step_size = {lr_cur:.1e} loss: {best_loss:.3e}",
+                    refresh=False,
+                )
                 losses.append(loss)
-        
+
         all_losses.append(losses)
 
-    return SVIRunResult(svi_class.get_params(best_state), svi_state,losses)
-    
+    return SVIRunResult(svi_class.get_params(best_state), svi_state, losses)
+
 
-def parse_mask(mask:ArrayLike=None,data:ArrayLike=None):
+def parse_mask(mask: ArrayLike = None, data: ArrayLike = None):
     if mask is None:
         return jnp.ones_like(data).astype(jnp.bool_)
     else:
-        return jnp.logical_not(jnp.array(mask)).astype(jnp.bool_)
+        return jnp.logical_not(jnp.array(mask.astype(int))).astype(jnp.bool_)
+
 
-def check_input_data(data:ArrayLike,rms:ArrayLike,psf:ArrayLike,mask:ArrayLike=None):
+def check_input_data(
+    data: ArrayLike, rms: ArrayLike, psf: ArrayLike, mask: ArrayLike = None
+):
     """Check input data for certain conditions and raise warnings or exceptions if needed
 
     Parameters
     ----------
     data : ArrayLike
         input image (galaxy/cutout)
     rms : ArrayLike
-       rms/error map of the data. 
+       rms/error map of the data.
     psf : ArrayLike
         pixelized PSF
     mask :ArrayLike, optional
        mask with True/1 indicating a pixel should be masked, by default None
 
     Raises
     ------
     RMSWarning
         If the rms map is highly discrepant from the rms of the data
     PSFNormalizationWarning
         if the pst normalization is not ~1
     KernelError
         if the provided PSF is larger than the input image (exception)
     MaskWarning
-        If more than 50% of the image is masked. 
+        If more than 70% of the image is masked.
     """
     rms = jnp.array(rms)
     data = jnp.array(data)
     psf = jnp.array(psf)
     if data.shape != rms.shape:
-        raise ShapeMatchError('RMS map ndims must match input data ndims.')
-    if jnp.mean(rms) > 5*jnp.std(data):
-        raise RMSWarning('Input RMS map appears to be highly offset (>5x) in magnitude from the rms of the pixels in the input image.')
-    if not jnp.isclose(jnp.sum(psf),1.0,0.1):
-        raise PSFNormalizationWarning('PSF does not appear to be appropriately normalized; Sum(psf) is more than 0.1 away from 1.')
-    if jnp.all(data.shape<psf.shape):
-        raise KernelError('PSF pixel image size must be smaller than science image.')
+        raise ShapeMatchError("RMS map ndims must match input data ndims.")
+    if jnp.median(rms) > 5 * jnp.std(data):
+        warnings.warn(
+            "Input RMS map appears to be highly offset (>5x) in magnitude from the rms of the pixels in the input image."
+        )
+    if not jnp.isclose(jnp.sum(psf), 1.0, 0.1):
+        warnings.warn(
+            "PSF does not appear to be appropriately normalized; Sum(psf) is more than 0.1 away from 1."
+        )
+    if jnp.all(data.shape < psf.shape):
+        raise KernelError("PSF pixel image size must be smaller than science image.")
     if mask is not None:
-        mask = parse_mask(mask,data)
-        if jnp.sum(mask)/jnp.prod(jnp.array(mask.shape))<0.5:
-            raise MaskWarning('More than 50 percent of input image is masked. Is this correct? (Pysersic treats True/1 as masked; you may need to flip your boolean array.) ')
-        if mask.shape !=data.shape:
-            raise ShapeMatchError('Mask ndims must match input data ndims.')
-    return True
+        mask = parse_mask(mask, data)
+        if jnp.sum(mask) / jnp.prod(jnp.array(mask.shape)) < 0.7:
+            warnings.warn(
+                "More than 70 percent of input image is masked. Is this correct? (Pysersic treats True/1 as masked; you may need to flip your boolean array.) "
+            )
+        if mask.shape != data.shape:
+            raise ShapeMatchError("Mask ndims must match input data ndims.")
+    return True
```

### Comparing `pysersic-0.1.2/pysersic/results.py` & `pysersic-0.1.4/pysersic/results.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 import numpy as np
 import numpyro
 import pandas as pd
 import xarray
 from jax import random
 from mpl_toolkits.axes_grid1.axes_divider import make_axes_locatable
 
-from pysersic.priors import PySersicMultiPrior
-from pysersic.rendering import BaseRenderer
+from .priors import PySersicMultiPrior, base_profile_params
+from .rendering import BaseRenderer
 
 ArrayLike = Union[np.array, jax.numpy.array]
 ListLike = Union[np.array,jax.numpy.array,list]
 
 class PySersicResults():
     def __init__(self,
                 data: ArrayLike,
@@ -147,27 +147,27 @@
         save_model : bool
             Whether to set self.models with model images from posterior
         Returns
         -------
         arviz.InferenceData
             the cleaned up object
         """
-        var_names = list(data.posterior.to_dataframe().columns)
+        var_names = list( data.posterior.data_vars )
         
         for var in var_names:
             if 'theta' in var:
                 new_theta = np.remainder(data['posterior'][var]+np.pi, np.pi)
                 data['posterior'][var] = new_theta
 
         if purge_extra:
             to_drop = []
             for var in var_names:
                 if ('base' in var) or ('auto' in var) or ('unwrapped' in var):
                     to_drop.append(var)
-                elif var == 'model':
+                elif 'model' in var:
                     to_drop.append(var)
                     if save_model:
                         self.models = data['posterior'][var]
             data.posterior = data.posterior.drop_vars(to_drop).drop_dims(['model_dim_0','model_dim_1'], errors = 'ignore')
         return data
 
 
@@ -178,32 +178,18 @@
         -------
         pandas.DataFrame
             data frame containing the arviz summary of the fit.
         """
         return az.summary(self.idata)
     
 
-    def get_median_model(self,)->Tuple[pd.DataFrame ,ArrayLike]:
-        """Selects the best fit model from the posterior draw that is closest to the median. returns the paramaters of the given draw and the model image. For the model images corresponding to every draw use the `.models` attribute of the results class.
-
-        Returns
-        -------
-        ArrayLike
-            model image
-        """
-        post_array = self.idata.posterior.to_dataframe().to_numpy()
-        med_vals =  np.median(post_array, axis = 0)
-        dim_raw = np.argmin( np.sum( np.abs(post_array - med_vals), axis = 1 ) ) # rough way to find closest draw to the median
-
-        draws = self.idata.posterior.dims['draw']
-        chain, draw = dim_raw //draws , dim_raw%draws
-        params = self.idata.posterior.sel(chain = chain, draw = draw).to_pandas()
-        model_im = self.models.sel(chain = chain, draw = draw).values
-        return params, model_im
-    
+    def get_median_model(self,):
+        print('This function has been deprecated as it was buggy and not implemented well. If you require a model we suggest using Fit[x].find_map() of looking at the models from the posterior in PySersicResults.models')
+        print('Please reach out if you have any questions.')
+        return NotImplementedError
 
     def corner(self,quantiles=[.16,.50,.84,],**kwargs):
         """Return a corner plot of the parameter estimation
 
         Parameters
         ----------
         quantiles: ListLike, optional  
@@ -232,15 +218,15 @@
             whether to return dataframe instead of simple dict, by default False
 
         Returns
         -------
         Union[pd.DataFrame,dict]
             dict or dataframe with index/keys as parameters and columns/values as the chosen quantiles.
         """
-        xx = self.idata.posterior.quantile(quantiles).to_dict()
+        xx = self.idata.posterior.quantile(quantiles, dim = ['chain','draw']).to_dict()
         out = {} 
         for i in xx['data_vars'].keys():
             out[i] = xx['data_vars'][i]['data']
         if return_dataframe==False:
             return out
         else:
             df = pd.DataFrame.from_dict(out).T
@@ -248,14 +234,16 @@
             return df 
 
     def retrieve_med_std(self,return_dataframe:bool=False)->Union[pd.DataFrame,dict]:
         out = {}
         q_dict = self.retrieve_param_quantiles()
         for key in q_dict.keys():
             qs = q_dict[key]
+            if isinstance(qs[0], list):
+                qs = np.array(qs)
             med = qs[1]
             std = 0.5*np.abs(qs[2] - qs[0])
             out[key] = np.array([med,std])
         if return_dataframe:
             out = pd.DataFrame.from_dict(out).T.rename(columns= {0:'median',1:'std'})
         return out
 
@@ -345,21 +333,19 @@
         tree = {} 
         tree['input_data'] = {} 
         tree['input_data']['image'] = np.array(self.data)
         tree['input_data']['rms'] = np.array(self.rms)
         tree['input_data']['psf'] = np.array(self.psf)
         tree['input_data']['mask'] = np.array(self.mask)
         tree['loss_func'] = str(self.loss_func)
-        tree['renderer'] = str(self.renderer)
+        tree['rendere_type'] = str( type(self.renderer) )
         tree['method_used'] = self.runtype
         if self.runtype == 'svi':
             tree['svi_method_used'] = self.svi_method_used
         tree['prior_info'] = self.prior.__str__()
-        tree['best_model'] = np.array(self.get_median_model()[1])
-        tree['best_model_params'] = self.get_median_model()[0].to_dict()
         tree['posterior'] = self.idata.to_dict()['posterior']
         for i in tree['posterior']:
             i = np.array(i)
         af = asdf.AsdfFile(tree=tree)
         if not fname.endswith('.asdf'):
             fname+='.asdf'
         af.write_to(fname)
@@ -415,15 +401,16 @@
            print("No need to reset posterior, returning original")
         else:
             idata_all = copy.copy(new_res.idata_all)
             new_res.__setattr__('idata', idata_all)
             new_res.__delattr__('idata_all')
     else:
         #Select variables for source
-        param_names = new_res.prior.all_priors[source_num].param_names
+        prof_type = new_res.prior.catalog['type'][source_num]
+        param_names = base_profile_params[prof_type]
         source_names = [pname + f'_{source_num}' for pname in param_names]
 
         #Search for other meta variables like sky etc.
         meta_names = []
         for k in new_res.idata.posterior.keys():
             if re.search(f"_[0-{new_res.prior.N_sources:d}]", k) is None:
                 meta_names.append(k)
```

### Comparing `pysersic-0.1.2/tests/test_loss.py` & `pysersic-0.1.4/tests/test_loss.py`

 * *Files identical despite different names*

### Comparing `pysersic-0.1.2/tests/test_renderers.py` & `pysersic-0.1.4/tests/test_renderers.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,91 +1,80 @@
-from pysersic.rendering import PixelRenderer,FourierRenderer,HybridRenderer, BaseRenderer
+from pysersic.rendering import PixelRenderer,FourierRenderer,HybridRenderer
 from pysersic.rendering import render_sersic_2d
 from astropy.convolution import Gaussian2DKernel
 import pytest
 import jax.numpy as jnp
-from jax.scipy.special import gammainc
 from scipy.integrate import dblquad
 from functools import partial
- 
+import jax
+
+render_sersic_2d = jax.jit(render_sersic_2d)
 kern = Gaussian2DKernel(x_stddev= 1.5)
-psf = kern.array
+psf = jnp.array(kern.array)
 err_tol = 0.01 # 1% error tolerence for total flux
 
-@pytest.mark.parametrize("renderer", [PixelRenderer,FourierRenderer,HybridRenderer])
-@pytest.mark.parametrize("pos", [(50,50),(50.5,50.5),(50.25,50.25) ,(50.,50.5),(50.5,50.)]) 
-def test_point_source(renderer,pos):
-    flux = 10.
-    renderer_test = renderer((100,100), psf)
-    im = renderer_test.render_pointsource(pos[0],pos[1],flux)
-    assert pytest.approx(im.sum(), rel = err_tol) == flux
+pixel_renderer = PixelRenderer((150,150), psf)
+fourier_renderer = FourierRenderer((150,150), psf)
+hybrid_renderer = HybridRenderer((150,150), psf)
+
+@partial(jax.jit, static_argnums = [1,])
+def get_models(params, profile_type: str):
+    im_px = pixel_renderer.render_source(params, profile_type=profile_type)
+    im_fr = fourier_renderer.render_source(params, profile_type=profile_type)
+    im_hy = hybrid_renderer.render_source(params, profile_type=profile_type)
+    return im_px, im_fr,im_hy
 
+@pytest.mark.parametrize("pos", [(75.,75.),(75.5,75.5),(75.25,75.25) ,(75.,75.5),(75.5,75.)]) 
+def test_point_source(pos):
+    flux = 10.
+    params = dict(flux = flux, xc = pos[0], yc = pos[1] )
+    ims = get_models(params, 'pointsource')
+    assert pytest.approx(ims[0].sum(), rel = err_tol) == flux #pixel
+    assert pytest.approx(ims[1].sum(), rel = err_tol) == flux #fourier
+    assert pytest.approx(ims[2].sum(), rel = err_tol) == flux #hybrid
 
-@pytest.mark.parametrize("renderer", [PixelRenderer,FourierRenderer,HybridRenderer])
 @pytest.mark.parametrize("pos", [(75.,75.),(75.5,75.5),])
 @pytest.mark.parametrize("re", [3.,5.]) 
 @pytest.mark.parametrize("n", [1.5,2.5]) 
 @pytest.mark.parametrize("ellip", [0,0.5])
 @pytest.mark.parametrize("theta", [0,3.14/4.]) 
-def test_sersic(renderer,pos,re,n,ellip,theta):
-    renderer_test = renderer((150,150), psf)
+def test_sersic(pos,re,n,ellip,theta):
     flux = 10
+    params = dict(flux = flux, xc = pos[0], yc = pos[1], n = n, ellip = ellip, theta = theta, r_eff = re )
     #Calculate fraction of flux contained in image
     int_test = partial(render_sersic_2d, xc = pos[0],yc = pos[1], flux = 10, r_eff = re, n = n, ellip = ellip,theta = theta)
     to_int = lambda x,y: float(int_test(x,y))
     lo_fun = lambda x: 0.
     hi_fun = lambda x: 150. 
     flux_int,_ = dblquad(to_int, 0.,150., lo_fun,hi_fun,epsrel=5.e-3)
     
-    im = renderer_test.render_sersic(pos[0],pos[1],flux,re,n,ellip,theta)
-    total = float( jnp.sum(im) )
-    assert pytest.approx(flux_int, rel = err_tol) == total
+    ims = get_models(params, 'sersic')
+    assert pytest.approx(float(ims[0].sum()), rel = err_tol) == flux_int #pixel
+    assert pytest.approx(float(ims[1].sum()), rel = err_tol) == flux_int #fourier
+    assert pytest.approx(float(ims[2].sum()), rel = err_tol) == flux_int #hybrid
 
-@pytest.mark.parametrize("renderer", [PixelRenderer,FourierRenderer,HybridRenderer])
-@pytest.mark.parametrize("prof", ['exp','dev']) 
+@pytest.mark.parametrize("prof", ['exp','dev'])
 @pytest.mark.parametrize("pos", [(75.,75.),(75.5,75.5),])
 @pytest.mark.parametrize("re", [3.,5.]) 
 @pytest.mark.parametrize("ellip", [0,0.5])
 @pytest.mark.parametrize("theta", [0,3.14/4.]) 
-def test_exp_dev(renderer,prof,pos,re,ellip,theta):
+def test_exp_dev(prof,pos,re,ellip,theta):
     flux = 10.
-    renderer_test = renderer((150,150), psf)
+    params = dict(flux = flux, xc = pos[0], yc = pos[1], ellip = ellip, theta = theta, r_eff = re )
+    
     if prof == 'exp':
-        im = renderer_test.render_exp(pos[0],pos[1],flux,re,ellip,theta)
         n=1.
     if prof == 'dev':
-        im = renderer_test.render_dev(pos[0],pos[1],flux,re,ellip,theta)
         n=4.
 
     #Calculate fraction of flux contained in image
     int_test = partial(render_sersic_2d, xc = pos[0],yc = pos[1], flux = 10, r_eff = re, n = n, ellip = ellip,theta = theta)
     to_int = lambda x,y: float(int_test(x,y))
 
     lo_fun = lambda x: 0.
     hi_fun = lambda x: 150. 
     flux_int,_ = dblquad(to_int, 0.,150., lo_fun,hi_fun,epsrel=5.e-3)
 
-    total = float( jnp.sum(im) )
-    assert pytest.approx(flux_int, rel = err_tol) == total
-
-
-def test_sky_rendering():
-    renderer_test = BaseRenderer((100,100), psf)
-
-    assert renderer_test.render_sky(0, None) == 0
-
-    assert renderer_test.render_sky(1., 'flat') == 1
-
-    sky_1 = renderer_test.render_sky([1e-4,0.,0.], 'tilted-plane')
-    assert sky_1.shape == (100,100)
-    sky_sum_1 = float(jnp.sum(sky_1))
-    assert pytest.approx(1e-4*100*100, rel = 1e-6) == sky_sum_1
-
-    sky_2 = renderer_test.render_sky([0.,1e-3,0.], 'tilted-plane')
-    assert sky_2.shape == (100,100)
-    sky_sum_2 = float(jnp.sum(sky_2))
-    assert pytest.approx(0, abs = 1e-4) == sky_sum_2
-
-    sky_3 = renderer_test.render_sky([0.,0.,1e-3,], 'tilted-plane')
-    assert sky_3.shape == (100,100)
-    sky_sum_3 = float(jnp.sum(sky_3))
-    assert pytest.approx(0, abs = 1e-4) == sky_sum_3
+    ims = get_models(params, prof)
+    assert pytest.approx(float(ims[0].sum()), rel = err_tol) == flux_int #pixel
+    assert pytest.approx(float(ims[1].sum()), rel = err_tol) == flux_int #fourier
+    assert pytest.approx(float(ims[2].sum()), rel = err_tol) == flux_int #hybrid
```

