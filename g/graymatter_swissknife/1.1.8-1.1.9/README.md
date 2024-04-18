# Comparing `tmp/graymatter_swissknife-1.1.8.tar.gz` & `tmp/graymatter_swissknife-1.1.9.tar.gz`

## Comparing `graymatter_swissknife-1.1.8.tar` & `graymatter_swissknife-1.1.9.tar`

### file list

```diff
@@ -1,84 +1,84 @@
--rw-r--r--   0        0        0    76578 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/images/GM_models_from_GEM.png
--rw-r--r--   0        0        0   586456 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/images/gm_swissknife_square_low_res.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/src/__init__.py
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/src/graymatter_swissknife/__about__.py
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/src/graymatter_swissknife/__init__.py
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/src/graymatter_swissknife/__main__.py
--rw-r--r--   0        0        0    11346 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/src/graymatter_swissknife/estimate_model.py
--rw-r--r--   0        0        0    10912 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/src/graymatter_swissknife/estimate_model_noiseless.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/__init__.py
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/find_model.py
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/microstructure_models.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/GEM/__init__.py
--rw-r--r--   0        0        0     2604 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/GEM/gem.py
--rw-r--r--   0        0        0     4214 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/GEM/gem_rm.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/GEM/functions/__init__.py
--rw-r--r--   0        0        0    23322 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/GEM/functions/scipy_gem.py
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/NEXI/__init__.py
--rw-r--r--   0        0        0     2877 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/NEXI/nexi.py
--rw-r--r--   0        0        0     2601 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/NEXI/nexi_dot.py
--rw-r--r--   0        0        0     4092 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/NEXI/nexi_dot_rm.py
--rw-r--r--   0        0        0     3973 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/NEXI/nexi_rm.py
--rw-r--r--   0        0        0     2429 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/NEXI/smex.py
--rw-r--r--   0        0        0     3981 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/NEXI/smex_rm.py
--rw-r--r--   0        0        0    36906 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/NEXI/functions/scipy_nexi.py
--rw-r--r--   0        0        0    11231 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/NEXI/functions/scipy_nexi_dot.py
--rw-r--r--   0        0        0    20308 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/NEXI/functions/scipy_smex.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/SANDI/__init__.py
--rw-r--r--   0        0        0     3006 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/SANDI/sandi.py
--rw-r--r--   0        0        0     3544 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/SANDI/sandi_rm.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/SANDI/functions/__init__.py
--rw-r--r--   0        0        0     4206 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/SANDI/functions/scipy_sandi.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/SANDIX/__init__.py
--rw-r--r--   0        0        0     2695 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/SANDIX/sandix.py
--rw-r--r--   0        0        0     3997 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/SANDIX/sandix_rm.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/SANDIX/functions/__init__.py
--rw-r--r--   0        0        0     7372 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/SANDIX/functions/scipy_sandix.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/parameters/__init__.py
--rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/parameters/acq_parameters.py
--rw-r--r--   0        0        0     1956 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/parameters/mist_parameters.py
--rw-r--r--   0        0        0     1808 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/parameters/save_parameters.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/rice_noise/__init__.py
--rw-r--r--   0        0        0     3857 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/rice_noise/rice_mean.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/struct_functions/__init__.py
--rw-r--r--   0        0        0    16385 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/struct_functions/scipy_cylinder.py
--rw-r--r--   0        0        0    21687 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/struct_functions/scipy_sphere.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/src/graymatter_swissknife/nls/__init__.py
--rw-r--r--   0        0        0     6721 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/src/graymatter_swissknife/nls/gridsearch.py
--rw-r--r--   0        0        0     6962 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/src/graymatter_swissknife/nls/nls.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/src/graymatter_swissknife/powderaverage/__init__.py
--rw-r--r--   0        0        0    10247 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/src/graymatter_swissknife/powderaverage/powderaverage.py
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/src/graymatter_swissknife/xgboost/apply_xgboost_model.py
--rw-r--r--   0        0        0     4855 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/src/graymatter_swissknife/xgboost/define_xgboost_model.py
--rw-r--r--   0        0        0     2693 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/src/graymatter_swissknife/xgboost/generate_dataset.py
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/tests/__init__.py
--rw-r--r--   0        0        0     2597 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/tests/graymatter_swissknife/generate_phantom.py
--rw-r--r--   0        0        0     2829 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/tests/graymatter_swissknife/test_estimate_model.py
--rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/tests/graymatter_swissknife/test_estimate_model_noiseless.py
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/tests/graymatter_swissknife/data/lowb_noisemap.nii.gz
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/tests/graymatter_swissknife/data/mask.nii.gz
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/tests/graymatter_swissknife/data/mask_upd_ref.nii.gz
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/tests/graymatter_swissknife/data/normalized_sigma_ref.nii.gz
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/tests/graymatter_swissknife/data/phantom.bval
--rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/tests/graymatter_swissknife/data/phantom.nii.gz
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/tests/graymatter_swissknife/data/phantom.td
--rw-r--r--   0        0        0     1216 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/tests/graymatter_swissknife/data/powderaverage_dwi_ref.nii.gz
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/tests/graymatter_swissknife/data/powderaverage_ref.bval
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/tests/graymatter_swissknife/data/powderaverage_ref.td
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/tests/graymatter_swissknife/data/models_ref/nexi_de_ref.nii.gz
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/tests/graymatter_swissknife/data/models_ref/nexi_di_ref.nii.gz
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/tests/graymatter_swissknife/data/models_ref/nexi_f_ref.nii.gz
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/tests/graymatter_swissknife/data/models_ref/nexi_rice_mean_de_ref.nii.gz
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/tests/graymatter_swissknife/data/models_ref/nexi_rice_mean_di_ref.nii.gz
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/tests/graymatter_swissknife/data/models_ref/nexi_rice_mean_f_ref.nii.gz
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/tests/graymatter_swissknife/data/models_ref/nexi_rice_mean_t_ex_ref.nii.gz
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/tests/graymatter_swissknife/data/models_ref/nexi_t_ex_ref.nii.gz
--rw-r--r--   0        0        0     4077 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/tests/graymatter_swissknife/models/test_nexi_functions.py
--rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/tests/graymatter_swissknife/models/test_rician_mean.py
--rw-r--r--   0        0        0     2209 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/tests/graymatter_swissknife/powderaverage/test_powderaverage.py
--rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/tests/graymatter_swissknife/xgboost/test_generate_dataset.py
--rw-r--r--   0        0        0     3237 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/.gitignore
--rw-r--r--   0        0        0    11542 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/LICENSE
--rw-r--r--   0        0        0    10548 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/README.md
--rw-r--r--   0        0        0     3772 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/pyproject.toml
--rw-r--r--   0        0        0    11577 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/PKG-INFO
+-rw-r--r--   0        0        0    76578 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.9/images/GM_models_from_GEM.png
+-rw-r--r--   0        0        0   586456 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.9/images/gm_swissknife_square_low_res.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.9/src/__init__.py
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.9/src/graymatter_swissknife/__about__.py
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.9/src/graymatter_swissknife/__init__.py
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.9/src/graymatter_swissknife/__main__.py
+-rw-r--r--   0        0        0    11346 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.9/src/graymatter_swissknife/estimate_model.py
+-rw-r--r--   0        0        0    10912 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.9/src/graymatter_swissknife/estimate_model_noiseless.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.9/src/graymatter_swissknife/models/__init__.py
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.9/src/graymatter_swissknife/models/find_model.py
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.9/src/graymatter_swissknife/models/microstructure_models.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.9/src/graymatter_swissknife/models/GEM/__init__.py
+-rw-r--r--   0        0        0     2604 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.9/src/graymatter_swissknife/models/GEM/gem.py
+-rw-r--r--   0        0        0     4214 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.9/src/graymatter_swissknife/models/GEM/gem_rm.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.9/src/graymatter_swissknife/models/GEM/functions/__init__.py
+-rw-r--r--   0        0        0    23322 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.9/src/graymatter_swissknife/models/GEM/functions/scipy_gem.py
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.9/src/graymatter_swissknife/models/NEXI/__init__.py
+-rw-r--r--   0        0        0     2877 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.9/src/graymatter_swissknife/models/NEXI/nexi.py
+-rw-r--r--   0        0        0     2601 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.9/src/graymatter_swissknife/models/NEXI/nexi_dot.py
+-rw-r--r--   0        0        0     4092 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.9/src/graymatter_swissknife/models/NEXI/nexi_dot_rm.py
+-rw-r--r--   0        0        0     3973 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.9/src/graymatter_swissknife/models/NEXI/nexi_rm.py
+-rw-r--r--   0        0        0     2429 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.9/src/graymatter_swissknife/models/NEXI/smex.py
+-rw-r--r--   0        0        0     3981 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.9/src/graymatter_swissknife/models/NEXI/smex_rm.py
+-rw-r--r--   0        0        0    36906 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.9/src/graymatter_swissknife/models/NEXI/functions/scipy_nexi.py
+-rw-r--r--   0        0        0    11231 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.9/src/graymatter_swissknife/models/NEXI/functions/scipy_nexi_dot.py
+-rw-r--r--   0        0        0    20308 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.9/src/graymatter_swissknife/models/NEXI/functions/scipy_smex.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.9/src/graymatter_swissknife/models/SANDI/__init__.py
+-rw-r--r--   0        0        0     3006 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.9/src/graymatter_swissknife/models/SANDI/sandi.py
+-rw-r--r--   0        0        0     3544 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.9/src/graymatter_swissknife/models/SANDI/sandi_rm.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.9/src/graymatter_swissknife/models/SANDI/functions/__init__.py
+-rw-r--r--   0        0        0     4206 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.9/src/graymatter_swissknife/models/SANDI/functions/scipy_sandi.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.9/src/graymatter_swissknife/models/SANDIX/__init__.py
+-rw-r--r--   0        0        0     2695 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.9/src/graymatter_swissknife/models/SANDIX/sandix.py
+-rw-r--r--   0        0        0     3997 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.9/src/graymatter_swissknife/models/SANDIX/sandix_rm.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.9/src/graymatter_swissknife/models/SANDIX/functions/__init__.py
+-rw-r--r--   0        0        0     7372 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.9/src/graymatter_swissknife/models/SANDIX/functions/scipy_sandix.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.9/src/graymatter_swissknife/models/parameters/__init__.py
+-rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.9/src/graymatter_swissknife/models/parameters/acq_parameters.py
+-rw-r--r--   0        0        0     1956 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.9/src/graymatter_swissknife/models/parameters/mist_parameters.py
+-rw-r--r--   0        0        0     1808 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.9/src/graymatter_swissknife/models/parameters/save_parameters.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.9/src/graymatter_swissknife/models/rice_noise/__init__.py
+-rw-r--r--   0        0        0     3857 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.9/src/graymatter_swissknife/models/rice_noise/rice_mean.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.9/src/graymatter_swissknife/models/struct_functions/__init__.py
+-rw-r--r--   0        0        0    16385 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.9/src/graymatter_swissknife/models/struct_functions/scipy_cylinder.py
+-rw-r--r--   0        0        0    21687 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.9/src/graymatter_swissknife/models/struct_functions/scipy_sphere.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.9/src/graymatter_swissknife/nls/__init__.py
+-rw-r--r--   0        0        0     6721 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.9/src/graymatter_swissknife/nls/gridsearch.py
+-rw-r--r--   0        0        0     6962 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.9/src/graymatter_swissknife/nls/nls.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.9/src/graymatter_swissknife/powderaverage/__init__.py
+-rw-r--r--   0        0        0    10247 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.9/src/graymatter_swissknife/powderaverage/powderaverage.py
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.9/src/graymatter_swissknife/xgboost/apply_xgboost_model.py
+-rw-r--r--   0        0        0     5088 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.9/src/graymatter_swissknife/xgboost/define_xgboost_model.py
+-rw-r--r--   0        0        0     2693 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.9/src/graymatter_swissknife/xgboost/generate_dataset.py
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.9/tests/__init__.py
+-rw-r--r--   0        0        0     2597 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.9/tests/graymatter_swissknife/generate_phantom.py
+-rw-r--r--   0        0        0     2829 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.9/tests/graymatter_swissknife/test_estimate_model.py
+-rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.9/tests/graymatter_swissknife/test_estimate_model_noiseless.py
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.9/tests/graymatter_swissknife/data/lowb_noisemap.nii.gz
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.9/tests/graymatter_swissknife/data/mask.nii.gz
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.9/tests/graymatter_swissknife/data/mask_upd_ref.nii.gz
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.9/tests/graymatter_swissknife/data/normalized_sigma_ref.nii.gz
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.9/tests/graymatter_swissknife/data/phantom.bval
+-rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.9/tests/graymatter_swissknife/data/phantom.nii.gz
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.9/tests/graymatter_swissknife/data/phantom.td
+-rw-r--r--   0        0        0     1216 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.9/tests/graymatter_swissknife/data/powderaverage_dwi_ref.nii.gz
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.9/tests/graymatter_swissknife/data/powderaverage_ref.bval
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.9/tests/graymatter_swissknife/data/powderaverage_ref.td
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.9/tests/graymatter_swissknife/data/models_ref/nexi_de_ref.nii.gz
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.9/tests/graymatter_swissknife/data/models_ref/nexi_di_ref.nii.gz
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.9/tests/graymatter_swissknife/data/models_ref/nexi_f_ref.nii.gz
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.9/tests/graymatter_swissknife/data/models_ref/nexi_rice_mean_de_ref.nii.gz
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.9/tests/graymatter_swissknife/data/models_ref/nexi_rice_mean_di_ref.nii.gz
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.9/tests/graymatter_swissknife/data/models_ref/nexi_rice_mean_f_ref.nii.gz
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.9/tests/graymatter_swissknife/data/models_ref/nexi_rice_mean_t_ex_ref.nii.gz
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.9/tests/graymatter_swissknife/data/models_ref/nexi_t_ex_ref.nii.gz
+-rw-r--r--   0        0        0     4077 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.9/tests/graymatter_swissknife/models/test_nexi_functions.py
+-rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.9/tests/graymatter_swissknife/models/test_rician_mean.py
+-rw-r--r--   0        0        0     2209 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.9/tests/graymatter_swissknife/powderaverage/test_powderaverage.py
+-rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.9/tests/graymatter_swissknife/xgboost/test_generate_dataset.py
+-rw-r--r--   0        0        0     3237 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.9/.gitignore
+-rw-r--r--   0        0        0    11542 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.9/LICENSE
+-rw-r--r--   0        0        0    10548 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.9/README.md
+-rw-r--r--   0        0        0     3772 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.9/pyproject.toml
+-rw-r--r--   0        0        0    11577 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.9/PKG-INFO
```

### Comparing `graymatter_swissknife-1.1.8/images/GM_models_from_GEM.png` & `graymatter_swissknife-1.1.9/images/GM_models_from_GEM.png`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.8/images/gm_swissknife_square_low_res.png` & `graymatter_swissknife-1.1.9/images/gm_swissknife_square_low_res.png`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.8/src/graymatter_swissknife/estimate_model.py` & `graymatter_swissknife-1.1.9/src/graymatter_swissknife/estimate_model.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.8/src/graymatter_swissknife/estimate_model_noiseless.py` & `graymatter_swissknife-1.1.9/src/graymatter_swissknife/estimate_model_noiseless.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/find_model.py` & `graymatter_swissknife-1.1.9/src/graymatter_swissknife/models/find_model.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/microstructure_models.py` & `graymatter_swissknife-1.1.9/src/graymatter_swissknife/models/microstructure_models.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/GEM/gem.py` & `graymatter_swissknife-1.1.9/src/graymatter_swissknife/models/GEM/gem.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/GEM/gem_rm.py` & `graymatter_swissknife-1.1.9/src/graymatter_swissknife/models/GEM/gem_rm.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/GEM/functions/scipy_gem.py` & `graymatter_swissknife-1.1.9/src/graymatter_swissknife/models/GEM/functions/scipy_gem.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/NEXI/nexi.py` & `graymatter_swissknife-1.1.9/src/graymatter_swissknife/models/NEXI/nexi.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/NEXI/nexi_dot.py` & `graymatter_swissknife-1.1.9/src/graymatter_swissknife/models/NEXI/nexi_dot.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/NEXI/nexi_dot_rm.py` & `graymatter_swissknife-1.1.9/src/graymatter_swissknife/models/NEXI/nexi_dot_rm.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/NEXI/nexi_rm.py` & `graymatter_swissknife-1.1.9/src/graymatter_swissknife/models/NEXI/nexi_rm.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/NEXI/smex.py` & `graymatter_swissknife-1.1.9/src/graymatter_swissknife/models/NEXI/smex.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/NEXI/smex_rm.py` & `graymatter_swissknife-1.1.9/src/graymatter_swissknife/models/NEXI/smex_rm.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/NEXI/functions/scipy_nexi.py` & `graymatter_swissknife-1.1.9/src/graymatter_swissknife/models/NEXI/functions/scipy_nexi.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/NEXI/functions/scipy_nexi_dot.py` & `graymatter_swissknife-1.1.9/src/graymatter_swissknife/models/NEXI/functions/scipy_nexi_dot.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/NEXI/functions/scipy_smex.py` & `graymatter_swissknife-1.1.9/src/graymatter_swissknife/models/NEXI/functions/scipy_smex.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/SANDI/sandi.py` & `graymatter_swissknife-1.1.9/src/graymatter_swissknife/models/SANDI/sandi.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/SANDI/sandi_rm.py` & `graymatter_swissknife-1.1.9/src/graymatter_swissknife/models/SANDI/sandi_rm.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/SANDI/functions/scipy_sandi.py` & `graymatter_swissknife-1.1.9/src/graymatter_swissknife/models/SANDI/functions/scipy_sandi.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/SANDIX/sandix.py` & `graymatter_swissknife-1.1.9/src/graymatter_swissknife/models/SANDIX/sandix.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/SANDIX/sandix_rm.py` & `graymatter_swissknife-1.1.9/src/graymatter_swissknife/models/SANDIX/sandix_rm.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/SANDIX/functions/scipy_sandix.py` & `graymatter_swissknife-1.1.9/src/graymatter_swissknife/models/SANDIX/functions/scipy_sandix.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/parameters/acq_parameters.py` & `graymatter_swissknife-1.1.9/src/graymatter_swissknife/models/parameters/acq_parameters.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/parameters/mist_parameters.py` & `graymatter_swissknife-1.1.9/src/graymatter_swissknife/models/parameters/mist_parameters.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/parameters/save_parameters.py` & `graymatter_swissknife-1.1.9/src/graymatter_swissknife/models/parameters/save_parameters.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/rice_noise/rice_mean.py` & `graymatter_swissknife-1.1.9/src/graymatter_swissknife/models/rice_noise/rice_mean.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/struct_functions/scipy_cylinder.py` & `graymatter_swissknife-1.1.9/src/graymatter_swissknife/models/struct_functions/scipy_cylinder.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/struct_functions/scipy_sphere.py` & `graymatter_swissknife-1.1.9/src/graymatter_swissknife/models/struct_functions/scipy_sphere.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.8/src/graymatter_swissknife/nls/gridsearch.py` & `graymatter_swissknife-1.1.9/src/graymatter_swissknife/nls/gridsearch.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.8/src/graymatter_swissknife/nls/nls.py` & `graymatter_swissknife-1.1.9/src/graymatter_swissknife/nls/nls.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.8/src/graymatter_swissknife/powderaverage/powderaverage.py` & `graymatter_swissknife-1.1.9/src/graymatter_swissknife/powderaverage/powderaverage.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.8/src/graymatter_swissknife/xgboost/apply_xgboost_model.py` & `graymatter_swissknife-1.1.9/src/graymatter_swissknife/xgboost/apply_xgboost_model.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.8/src/graymatter_swissknife/xgboost/define_xgboost_model.py` & `graymatter_swissknife-1.1.9/src/graymatter_swissknife/xgboost/define_xgboost_model.py`

 * *Files 11% similar despite different names*

```diff
@@ -82,15 +82,17 @@
         if n_params % 2 == 0:
             n_cols = n_params // n_rows
         else:
             n_cols = n_params // n_rows + 1
         for param_index in range(n_params):
             plt.subplot(n_rows, n_cols, param_index + 1)
             plt.scatter(y_test[:, param_index], y_hat[:, param_index], s=1)
-            plt.plot([0, 1], [0, 1], color="black", linestyle="--")
-            plt.xlabel(f"GT {microstruct_model.params[param_index]}")
-            plt.ylabel(f"Predicted {microstruct_model.params[param_index]}")
-            plt.title(f"{microstruct_model.params[param_index]}")
+            plt.plot([microstruct_model.param_lim[param_index][0], microstruct_model.param_lim[param_index][1]], 
+                     [microstruct_model.param_lim[param_index][0], microstruct_model.param_lim[param_index][1]], 
+                     color="black", linestyle="--")
+            plt.xlabel(f"Target {microstruct_model.param_names[param_index]}")
+            plt.ylabel(f"Predicted {microstruct_model.param_names[param_index]}")
+            plt.title(f"{microstruct_model.param_names[param_index]}")
         plt.tight_layout()
         plt.savefig(xgboost_test_plot_path)
 
     return xgboost_model
```

### Comparing `graymatter_swissknife-1.1.8/src/graymatter_swissknife/xgboost/generate_dataset.py` & `graymatter_swissknife-1.1.9/src/graymatter_swissknife/xgboost/generate_dataset.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.8/tests/graymatter_swissknife/generate_phantom.py` & `graymatter_swissknife-1.1.9/tests/graymatter_swissknife/generate_phantom.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.8/tests/graymatter_swissknife/test_estimate_model.py` & `graymatter_swissknife-1.1.9/tests/graymatter_swissknife/test_estimate_model.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.8/tests/graymatter_swissknife/test_estimate_model_noiseless.py` & `graymatter_swissknife-1.1.9/tests/graymatter_swissknife/test_estimate_model_noiseless.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.8/tests/graymatter_swissknife/data/phantom.nii.gz` & `graymatter_swissknife-1.1.9/tests/graymatter_swissknife/data/phantom.nii.gz`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.8/tests/graymatter_swissknife/data/powderaverage_dwi_ref.nii.gz` & `graymatter_swissknife-1.1.9/tests/graymatter_swissknife/data/powderaverage_dwi_ref.nii.gz`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.8/tests/graymatter_swissknife/models/test_nexi_functions.py` & `graymatter_swissknife-1.1.9/tests/graymatter_swissknife/models/test_nexi_functions.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.8/tests/graymatter_swissknife/models/test_rician_mean.py` & `graymatter_swissknife-1.1.9/tests/graymatter_swissknife/models/test_rician_mean.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.8/tests/graymatter_swissknife/powderaverage/test_powderaverage.py` & `graymatter_swissknife-1.1.9/tests/graymatter_swissknife/powderaverage/test_powderaverage.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.8/tests/graymatter_swissknife/xgboost/test_generate_dataset.py` & `graymatter_swissknife-1.1.9/tests/graymatter_swissknife/xgboost/test_generate_dataset.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.8/.gitignore` & `graymatter_swissknife-1.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.8/LICENSE` & `graymatter_swissknife-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.8/README.md` & `graymatter_swissknife-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.8/pyproject.toml` & `graymatter_swissknife-1.1.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.8/PKG-INFO` & `graymatter_swissknife-1.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: graymatter_swissknife
-Version: 1.1.8
+Version: 1.1.9
 Summary: Gray Matter Swiss Knife : Generalized Exchange Model estimators for diffusion MRI
 Project-URL: Documentation, https://github.com/QuentinUhl/graymatter_swissknife#readme
 Project-URL: Issues, https://github.com/QuentinUhl/graymatter_swissknife/issues
 Project-URL: Source, https://github.com/QuentinUhl/graymatter_swissknife
 Author-email: Quentin Uhl <quentin.uhl@gmail.com>, "Ileana O. Jelescu" <ileana.jelescu@chuv.ch>
 License-Expression: Apache-2.0
 License-File: LICENSE
```

