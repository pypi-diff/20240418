# Comparing `tmp/graymatter_swissknife-1.1.7.tar.gz` & `tmp/graymatter_swissknife-1.1.8.tar.gz`

## Comparing `graymatter_swissknife-1.1.7.tar` & `graymatter_swissknife-1.1.8.tar`

### file list

```diff
@@ -1,84 +1,84 @@
--rw-r--r--   0        0        0    76578 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/images/GM_models_from_GEM.png
--rw-r--r--   0        0        0   586456 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/images/gm_swissknife_square_low_res.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/src/__init__.py
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/src/graymatter_swissknife/__about__.py
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/src/graymatter_swissknife/__init__.py
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/src/graymatter_swissknife/__main__.py
--rw-r--r--   0        0        0    11346 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/src/graymatter_swissknife/estimate_model.py
--rw-r--r--   0        0        0    10912 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/src/graymatter_swissknife/estimate_model_noiseless.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/__init__.py
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/find_model.py
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/microstructure_models.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/GEM/__init__.py
--rw-r--r--   0        0        0     2604 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/GEM/gem.py
--rw-r--r--   0        0        0     4214 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/GEM/gem_rm.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/GEM/functions/__init__.py
--rw-r--r--   0        0        0    23322 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/GEM/functions/scipy_gem.py
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/NEXI/__init__.py
--rw-r--r--   0        0        0     2877 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/NEXI/nexi.py
--rw-r--r--   0        0        0     2601 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/NEXI/nexi_dot.py
--rw-r--r--   0        0        0     4092 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/NEXI/nexi_dot_rm.py
--rw-r--r--   0        0        0     3973 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/NEXI/nexi_rm.py
--rw-r--r--   0        0        0     2429 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/NEXI/smex.py
--rw-r--r--   0        0        0     3981 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/NEXI/smex_rm.py
--rw-r--r--   0        0        0    36906 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/NEXI/functions/scipy_nexi.py
--rw-r--r--   0        0        0    11231 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/NEXI/functions/scipy_nexi_dot.py
--rw-r--r--   0        0        0    20308 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/NEXI/functions/scipy_smex.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/SANDI/__init__.py
--rw-r--r--   0        0        0     3006 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/SANDI/sandi.py
--rw-r--r--   0        0        0     3544 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/SANDI/sandi_rm.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/SANDI/functions/__init__.py
--rw-r--r--   0        0        0     4206 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/SANDI/functions/scipy_sandi.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/SANDIX/__init__.py
--rw-r--r--   0        0        0     2695 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/SANDIX/sandix.py
--rw-r--r--   0        0        0     3997 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/SANDIX/sandix_rm.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/SANDIX/functions/__init__.py
--rw-r--r--   0        0        0     7372 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/SANDIX/functions/scipy_sandix.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/parameters/__init__.py
--rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/parameters/acq_parameters.py
--rw-r--r--   0        0        0     1956 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/parameters/mist_parameters.py
--rw-r--r--   0        0        0     1808 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/parameters/save_parameters.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/rice_noise/__init__.py
--rw-r--r--   0        0        0     3857 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/rice_noise/rice_mean.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/struct_functions/__init__.py
--rw-r--r--   0        0        0    16385 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/struct_functions/scipy_cylinder.py
--rw-r--r--   0        0        0    21687 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/struct_functions/scipy_sphere.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/src/graymatter_swissknife/nls/__init__.py
--rw-r--r--   0        0        0     6721 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/src/graymatter_swissknife/nls/gridsearch.py
--rw-r--r--   0        0        0     6962 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/src/graymatter_swissknife/nls/nls.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/src/graymatter_swissknife/powderaverage/__init__.py
--rw-r--r--   0        0        0    10247 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/src/graymatter_swissknife/powderaverage/powderaverage.py
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/src/graymatter_swissknife/xgboost/apply_xgboost_model.py
--rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/src/graymatter_swissknife/xgboost/define_xgboost_model.py
--rw-r--r--   0        0        0     2693 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/src/graymatter_swissknife/xgboost/generate_dataset.py
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/tests/__init__.py
--rw-r--r--   0        0        0     2597 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/tests/graymatter_swissknife/generate_phantom.py
--rw-r--r--   0        0        0     2829 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/tests/graymatter_swissknife/test_estimate_model.py
--rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/tests/graymatter_swissknife/test_estimate_model_noiseless.py
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/tests/graymatter_swissknife/data/lowb_noisemap.nii.gz
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/tests/graymatter_swissknife/data/mask.nii.gz
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/tests/graymatter_swissknife/data/mask_upd_ref.nii.gz
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/tests/graymatter_swissknife/data/normalized_sigma_ref.nii.gz
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/tests/graymatter_swissknife/data/phantom.bval
--rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/tests/graymatter_swissknife/data/phantom.nii.gz
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/tests/graymatter_swissknife/data/phantom.td
--rw-r--r--   0        0        0     1216 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/tests/graymatter_swissknife/data/powderaverage_dwi_ref.nii.gz
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/tests/graymatter_swissknife/data/powderaverage_ref.bval
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/tests/graymatter_swissknife/data/powderaverage_ref.td
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/tests/graymatter_swissknife/data/models_ref/nexi_de_ref.nii.gz
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/tests/graymatter_swissknife/data/models_ref/nexi_di_ref.nii.gz
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/tests/graymatter_swissknife/data/models_ref/nexi_f_ref.nii.gz
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/tests/graymatter_swissknife/data/models_ref/nexi_rice_mean_de_ref.nii.gz
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/tests/graymatter_swissknife/data/models_ref/nexi_rice_mean_di_ref.nii.gz
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/tests/graymatter_swissknife/data/models_ref/nexi_rice_mean_f_ref.nii.gz
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/tests/graymatter_swissknife/data/models_ref/nexi_rice_mean_t_ex_ref.nii.gz
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/tests/graymatter_swissknife/data/models_ref/nexi_t_ex_ref.nii.gz
--rw-r--r--   0        0        0     4077 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/tests/graymatter_swissknife/models/test_nexi_functions.py
--rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/tests/graymatter_swissknife/models/test_rician_mean.py
--rw-r--r--   0        0        0     2209 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/tests/graymatter_swissknife/powderaverage/test_powderaverage.py
--rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/tests/graymatter_swissknife/xgboost/test_generate_dataset.py
--rw-r--r--   0        0        0     3237 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/.gitignore
--rw-r--r--   0        0        0    11542 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/LICENSE
--rw-r--r--   0        0        0     9794 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/README.md
--rw-r--r--   0        0        0     3772 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/pyproject.toml
--rw-r--r--   0        0        0    10829 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/PKG-INFO
+-rw-r--r--   0        0        0    76578 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/images/GM_models_from_GEM.png
+-rw-r--r--   0        0        0   586456 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/images/gm_swissknife_square_low_res.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/src/__init__.py
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/src/graymatter_swissknife/__about__.py
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/src/graymatter_swissknife/__init__.py
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/src/graymatter_swissknife/__main__.py
+-rw-r--r--   0        0        0    11346 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/src/graymatter_swissknife/estimate_model.py
+-rw-r--r--   0        0        0    10912 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/src/graymatter_swissknife/estimate_model_noiseless.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/__init__.py
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/find_model.py
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/microstructure_models.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/GEM/__init__.py
+-rw-r--r--   0        0        0     2604 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/GEM/gem.py
+-rw-r--r--   0        0        0     4214 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/GEM/gem_rm.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/GEM/functions/__init__.py
+-rw-r--r--   0        0        0    23322 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/GEM/functions/scipy_gem.py
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/NEXI/__init__.py
+-rw-r--r--   0        0        0     2877 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/NEXI/nexi.py
+-rw-r--r--   0        0        0     2601 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/NEXI/nexi_dot.py
+-rw-r--r--   0        0        0     4092 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/NEXI/nexi_dot_rm.py
+-rw-r--r--   0        0        0     3973 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/NEXI/nexi_rm.py
+-rw-r--r--   0        0        0     2429 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/NEXI/smex.py
+-rw-r--r--   0        0        0     3981 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/NEXI/smex_rm.py
+-rw-r--r--   0        0        0    36906 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/NEXI/functions/scipy_nexi.py
+-rw-r--r--   0        0        0    11231 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/NEXI/functions/scipy_nexi_dot.py
+-rw-r--r--   0        0        0    20308 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/NEXI/functions/scipy_smex.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/SANDI/__init__.py
+-rw-r--r--   0        0        0     3006 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/SANDI/sandi.py
+-rw-r--r--   0        0        0     3544 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/SANDI/sandi_rm.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/SANDI/functions/__init__.py
+-rw-r--r--   0        0        0     4206 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/SANDI/functions/scipy_sandi.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/SANDIX/__init__.py
+-rw-r--r--   0        0        0     2695 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/SANDIX/sandix.py
+-rw-r--r--   0        0        0     3997 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/SANDIX/sandix_rm.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/SANDIX/functions/__init__.py
+-rw-r--r--   0        0        0     7372 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/SANDIX/functions/scipy_sandix.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/parameters/__init__.py
+-rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/parameters/acq_parameters.py
+-rw-r--r--   0        0        0     1956 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/parameters/mist_parameters.py
+-rw-r--r--   0        0        0     1808 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/parameters/save_parameters.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/rice_noise/__init__.py
+-rw-r--r--   0        0        0     3857 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/rice_noise/rice_mean.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/struct_functions/__init__.py
+-rw-r--r--   0        0        0    16385 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/struct_functions/scipy_cylinder.py
+-rw-r--r--   0        0        0    21687 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/struct_functions/scipy_sphere.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/src/graymatter_swissknife/nls/__init__.py
+-rw-r--r--   0        0        0     6721 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/src/graymatter_swissknife/nls/gridsearch.py
+-rw-r--r--   0        0        0     6962 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/src/graymatter_swissknife/nls/nls.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/src/graymatter_swissknife/powderaverage/__init__.py
+-rw-r--r--   0        0        0    10247 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/src/graymatter_swissknife/powderaverage/powderaverage.py
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/src/graymatter_swissknife/xgboost/apply_xgboost_model.py
+-rw-r--r--   0        0        0     4855 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/src/graymatter_swissknife/xgboost/define_xgboost_model.py
+-rw-r--r--   0        0        0     2693 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/src/graymatter_swissknife/xgboost/generate_dataset.py
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/tests/__init__.py
+-rw-r--r--   0        0        0     2597 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/tests/graymatter_swissknife/generate_phantom.py
+-rw-r--r--   0        0        0     2829 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/tests/graymatter_swissknife/test_estimate_model.py
+-rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/tests/graymatter_swissknife/test_estimate_model_noiseless.py
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/tests/graymatter_swissknife/data/lowb_noisemap.nii.gz
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/tests/graymatter_swissknife/data/mask.nii.gz
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/tests/graymatter_swissknife/data/mask_upd_ref.nii.gz
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/tests/graymatter_swissknife/data/normalized_sigma_ref.nii.gz
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/tests/graymatter_swissknife/data/phantom.bval
+-rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/tests/graymatter_swissknife/data/phantom.nii.gz
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/tests/graymatter_swissknife/data/phantom.td
+-rw-r--r--   0        0        0     1216 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/tests/graymatter_swissknife/data/powderaverage_dwi_ref.nii.gz
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/tests/graymatter_swissknife/data/powderaverage_ref.bval
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/tests/graymatter_swissknife/data/powderaverage_ref.td
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/tests/graymatter_swissknife/data/models_ref/nexi_de_ref.nii.gz
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/tests/graymatter_swissknife/data/models_ref/nexi_di_ref.nii.gz
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/tests/graymatter_swissknife/data/models_ref/nexi_f_ref.nii.gz
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/tests/graymatter_swissknife/data/models_ref/nexi_rice_mean_de_ref.nii.gz
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/tests/graymatter_swissknife/data/models_ref/nexi_rice_mean_di_ref.nii.gz
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/tests/graymatter_swissknife/data/models_ref/nexi_rice_mean_f_ref.nii.gz
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/tests/graymatter_swissknife/data/models_ref/nexi_rice_mean_t_ex_ref.nii.gz
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/tests/graymatter_swissknife/data/models_ref/nexi_t_ex_ref.nii.gz
+-rw-r--r--   0        0        0     4077 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/tests/graymatter_swissknife/models/test_nexi_functions.py
+-rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/tests/graymatter_swissknife/models/test_rician_mean.py
+-rw-r--r--   0        0        0     2209 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/tests/graymatter_swissknife/powderaverage/test_powderaverage.py
+-rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/tests/graymatter_swissknife/xgboost/test_generate_dataset.py
+-rw-r--r--   0        0        0     3237 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/.gitignore
+-rw-r--r--   0        0        0    11542 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/LICENSE
+-rw-r--r--   0        0        0    10548 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/README.md
+-rw-r--r--   0        0        0     3772 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/pyproject.toml
+-rw-r--r--   0        0        0    11577 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.8/PKG-INFO
```

### Comparing `graymatter_swissknife-1.1.7/images/GM_models_from_GEM.png` & `graymatter_swissknife-1.1.8/images/GM_models_from_GEM.png`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.7/images/gm_swissknife_square_low_res.png` & `graymatter_swissknife-1.1.8/images/gm_swissknife_square_low_res.png`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.7/src/graymatter_swissknife/estimate_model.py` & `graymatter_swissknife-1.1.8/src/graymatter_swissknife/estimate_model.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.7/src/graymatter_swissknife/estimate_model_noiseless.py` & `graymatter_swissknife-1.1.8/src/graymatter_swissknife/estimate_model_noiseless.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/find_model.py` & `graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/find_model.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/microstructure_models.py` & `graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/microstructure_models.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/GEM/gem.py` & `graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/GEM/gem.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/GEM/gem_rm.py` & `graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/GEM/gem_rm.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/GEM/functions/scipy_gem.py` & `graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/GEM/functions/scipy_gem.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/NEXI/nexi.py` & `graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/NEXI/nexi.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/NEXI/nexi_dot.py` & `graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/NEXI/nexi_dot.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/NEXI/nexi_dot_rm.py` & `graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/NEXI/nexi_dot_rm.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/NEXI/nexi_rm.py` & `graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/NEXI/nexi_rm.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/NEXI/smex.py` & `graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/NEXI/smex.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/NEXI/smex_rm.py` & `graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/NEXI/smex_rm.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/NEXI/functions/scipy_nexi.py` & `graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/NEXI/functions/scipy_nexi.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/NEXI/functions/scipy_nexi_dot.py` & `graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/NEXI/functions/scipy_nexi_dot.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/NEXI/functions/scipy_smex.py` & `graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/NEXI/functions/scipy_smex.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/SANDI/sandi.py` & `graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/SANDI/sandi.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/SANDI/sandi_rm.py` & `graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/SANDI/sandi_rm.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/SANDI/functions/scipy_sandi.py` & `graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/SANDI/functions/scipy_sandi.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/SANDIX/sandix.py` & `graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/SANDIX/sandix.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/SANDIX/sandix_rm.py` & `graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/SANDIX/sandix_rm.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/SANDIX/functions/scipy_sandix.py` & `graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/SANDIX/functions/scipy_sandix.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/parameters/acq_parameters.py` & `graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/parameters/acq_parameters.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/parameters/mist_parameters.py` & `graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/parameters/mist_parameters.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/parameters/save_parameters.py` & `graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/parameters/save_parameters.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/rice_noise/rice_mean.py` & `graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/rice_noise/rice_mean.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/struct_functions/scipy_cylinder.py` & `graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/struct_functions/scipy_cylinder.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/struct_functions/scipy_sphere.py` & `graymatter_swissknife-1.1.8/src/graymatter_swissknife/models/struct_functions/scipy_sphere.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.7/src/graymatter_swissknife/nls/gridsearch.py` & `graymatter_swissknife-1.1.8/src/graymatter_swissknife/nls/gridsearch.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.7/src/graymatter_swissknife/nls/nls.py` & `graymatter_swissknife-1.1.8/src/graymatter_swissknife/nls/nls.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.7/src/graymatter_swissknife/powderaverage/powderaverage.py` & `graymatter_swissknife-1.1.8/src/graymatter_swissknife/powderaverage/powderaverage.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.7/src/graymatter_swissknife/xgboost/apply_xgboost_model.py` & `graymatter_swissknife-1.1.8/src/graymatter_swissknife/xgboost/apply_xgboost_model.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.7/src/graymatter_swissknife/xgboost/generate_dataset.py` & `graymatter_swissknife-1.1.8/src/graymatter_swissknife/xgboost/generate_dataset.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.7/tests/graymatter_swissknife/generate_phantom.py` & `graymatter_swissknife-1.1.8/tests/graymatter_swissknife/generate_phantom.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.7/tests/graymatter_swissknife/test_estimate_model.py` & `graymatter_swissknife-1.1.8/tests/graymatter_swissknife/test_estimate_model.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.7/tests/graymatter_swissknife/test_estimate_model_noiseless.py` & `graymatter_swissknife-1.1.8/tests/graymatter_swissknife/test_estimate_model_noiseless.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.7/tests/graymatter_swissknife/data/phantom.nii.gz` & `graymatter_swissknife-1.1.8/tests/graymatter_swissknife/data/phantom.nii.gz`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.7/tests/graymatter_swissknife/data/powderaverage_dwi_ref.nii.gz` & `graymatter_swissknife-1.1.8/tests/graymatter_swissknife/data/powderaverage_dwi_ref.nii.gz`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.7/tests/graymatter_swissknife/models/test_nexi_functions.py` & `graymatter_swissknife-1.1.8/tests/graymatter_swissknife/models/test_nexi_functions.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.7/tests/graymatter_swissknife/models/test_rician_mean.py` & `graymatter_swissknife-1.1.8/tests/graymatter_swissknife/models/test_rician_mean.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.7/tests/graymatter_swissknife/powderaverage/test_powderaverage.py` & `graymatter_swissknife-1.1.8/tests/graymatter_swissknife/powderaverage/test_powderaverage.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.7/tests/graymatter_swissknife/xgboost/test_generate_dataset.py` & `graymatter_swissknife-1.1.8/tests/graymatter_swissknife/xgboost/test_generate_dataset.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.7/.gitignore` & `graymatter_swissknife-1.1.8/.gitignore`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.7/LICENSE` & `graymatter_swissknife-1.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.7/README.md` & `graymatter_swissknife-1.1.8/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 - [Citation](#citation)
 - [License](#license)
 
 
 ## Installation
 
 ```console
-pip install numpy nibabel tqdm joblib scipy xgboost scikit-learn
+pip install numpy nibabel tqdm joblib scipy xgboost scikit-learn matplotlib
 pip install graymatter_swissknife
 ```
 
 ## Usage
 
 ### Estimate Gray Matter microstructure model parameters
 
@@ -101,23 +101,29 @@
 
 To compute a grey matter mask, one common approach involves using a T1 image, [FastSurfer](https://deep-mi.org/research/fastsurfer/), and performing registration to the diffusion (b = 0 ms/µm²) space. However, you can choose any other method to compute a grey matter mask.
 
 ## Citation
 
 If you use this package in your research, please consider citing the following papers:
 
-## Original gray matter model papers
+### Development of this package
+Quentin Uhl, Tommaso Pavan, Thorsten Feiweier, Gian Franco Piredda, Sune N. Jespersen and Ileana Jelescu, [NEXI for the quantification of human gray matter microstructure on a clinical MRI scanner](https://www.ismrm.org/24m/), Proc. Intl. Soc. Mag. Reson. Med. 2024. 
+Presented at the Annual Meeting of the ISMRM, Singapore, Singapore, p. 0937.
 
 ### Generalized Exchange Model ($GEM$) / Development of this package
 Quentin Uhl, Tommaso Pavan, Inès de Riedmatten, Jasmine Nguyen-Duc, and Ileana Jelescu, [GEM: a unifying model for Gray Matter microstructure](https://www.ismrm.org/24m/), Proc. Intl. Soc. Mag. Reson. Med. 2024. 
 Presented at the Annual Meeting of the ISMRM, Singapore, Singapore, p. 7970.
 
+## Other original gray matter model papers
+
 ### Neurite Exchange Imaging ($NEXI$, or $NEXI_{Narrow Pulse Approximation}$)
 Ileana O. Jelescu, Alexandre de Skowronski, Françoise Geffroy, Marco Palombo, Dmitry S. Novikov, [Neurite Exchange Imaging (NEXI): A minimal model of diffusion in gray matter with inter-compartment water exchange](https://www.sciencedirect.com/science/article/pii/S1053811922003986), NeuroImage, 2022.
 
+Quentin Uhl, Tommaso Pavan, Malwina Molendowska, Derek K. Jones, Marco Palombo, Ileana Jelescu, [Quantifying human gray matter microstructure using Neurite Exchange Imaging (NEXI) and 300 mT/m gradients](https://direct.mit.edu/imag/article/doi/10.1162/imag_a_00104/119673/Quantifying-human-gray-matter-microstructure-using), Imaging Neuroscience, 2024
+
 ### Standard Model with Exchange ($SMEX$, or $NEXI_{Wide Pulses}$)
 Jonas L. Olesen, Leif Østergaard, Noam Shemesh, Sune N. Jespersen, [Diffusion time dependence, power-law scaling, and exchange in gray matter](https://doi.org/10.1016/j.neuroimage.2022.118976), NeuroImage, 2022.
 
 ###  Soma And Neurite Density Imaging ($SANDI$)
 Marco Palombo, Andrada Ianus, Michele Guerreri, Daniel Nunes, Daniel C. Alexander, Noam Shemesh, Hui Zhang, [SANDI: A compartment-based model for non-invasive apparent soma and neurite imaging by diffusion MRI](https://doi.org/10.1016/j.neuroimage.2020.116835), NeuroImage, 2020.
 
 ###  Soma And Neurite Density Imaging with eXchange ($SANDIX$)
```

### Comparing `graymatter_swissknife-1.1.7/pyproject.toml` & `graymatter_swissknife-1.1.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.7/PKG-INFO` & `graymatter_swissknife-1.1.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: graymatter_swissknife
-Version: 1.1.7
+Version: 1.1.8
 Summary: Gray Matter Swiss Knife : Generalized Exchange Model estimators for diffusion MRI
 Project-URL: Documentation, https://github.com/QuentinUhl/graymatter_swissknife#readme
 Project-URL: Issues, https://github.com/QuentinUhl/graymatter_swissknife/issues
 Project-URL: Source, https://github.com/QuentinUhl/graymatter_swissknife
 Author-email: Quentin Uhl <quentin.uhl@gmail.com>, "Ileana O. Jelescu" <ileana.jelescu@chuv.ch>
 License-Expression: Apache-2.0
 License-File: LICENSE
@@ -45,15 +45,15 @@
 - [Citation](#citation)
 - [License](#license)
 
 
 ## Installation
 
 ```console
-pip install numpy nibabel tqdm joblib scipy xgboost scikit-learn
+pip install numpy nibabel tqdm joblib scipy xgboost scikit-learn matplotlib
 pip install graymatter_swissknife
 ```
 
 ## Usage
 
 ### Estimate Gray Matter microstructure model parameters
 
@@ -124,23 +124,29 @@
 
 To compute a grey matter mask, one common approach involves using a T1 image, [FastSurfer](https://deep-mi.org/research/fastsurfer/), and performing registration to the diffusion (b = 0 ms/µm²) space. However, you can choose any other method to compute a grey matter mask.
 
 ## Citation
 
 If you use this package in your research, please consider citing the following papers:
 
-## Original gray matter model papers
+### Development of this package
+Quentin Uhl, Tommaso Pavan, Thorsten Feiweier, Gian Franco Piredda, Sune N. Jespersen and Ileana Jelescu, [NEXI for the quantification of human gray matter microstructure on a clinical MRI scanner](https://www.ismrm.org/24m/), Proc. Intl. Soc. Mag. Reson. Med. 2024. 
+Presented at the Annual Meeting of the ISMRM, Singapore, Singapore, p. 0937.
 
 ### Generalized Exchange Model ($GEM$) / Development of this package
 Quentin Uhl, Tommaso Pavan, Inès de Riedmatten, Jasmine Nguyen-Duc, and Ileana Jelescu, [GEM: a unifying model for Gray Matter microstructure](https://www.ismrm.org/24m/), Proc. Intl. Soc. Mag. Reson. Med. 2024. 
 Presented at the Annual Meeting of the ISMRM, Singapore, Singapore, p. 7970.
 
+## Other original gray matter model papers
+
 ### Neurite Exchange Imaging ($NEXI$, or $NEXI_{Narrow Pulse Approximation}$)
 Ileana O. Jelescu, Alexandre de Skowronski, Françoise Geffroy, Marco Palombo, Dmitry S. Novikov, [Neurite Exchange Imaging (NEXI): A minimal model of diffusion in gray matter with inter-compartment water exchange](https://www.sciencedirect.com/science/article/pii/S1053811922003986), NeuroImage, 2022.
 
+Quentin Uhl, Tommaso Pavan, Malwina Molendowska, Derek K. Jones, Marco Palombo, Ileana Jelescu, [Quantifying human gray matter microstructure using Neurite Exchange Imaging (NEXI) and 300 mT/m gradients](https://direct.mit.edu/imag/article/doi/10.1162/imag_a_00104/119673/Quantifying-human-gray-matter-microstructure-using), Imaging Neuroscience, 2024
+
 ### Standard Model with Exchange ($SMEX$, or $NEXI_{Wide Pulses}$)
 Jonas L. Olesen, Leif Østergaard, Noam Shemesh, Sune N. Jespersen, [Diffusion time dependence, power-law scaling, and exchange in gray matter](https://doi.org/10.1016/j.neuroimage.2022.118976), NeuroImage, 2022.
 
 ###  Soma And Neurite Density Imaging ($SANDI$)
 Marco Palombo, Andrada Ianus, Michele Guerreri, Daniel Nunes, Daniel C. Alexander, Noam Shemesh, Hui Zhang, [SANDI: A compartment-based model for non-invasive apparent soma and neurite imaging by diffusion MRI](https://doi.org/10.1016/j.neuroimage.2020.116835), NeuroImage, 2020.
 
 ###  Soma And Neurite Density Imaging with eXchange ($SANDIX$)
```

