# Comparing `tmp/astrophot-0.16.2.tar.gz` & `tmp/astrophot-0.16.3.tar.gz`

## Comparing `astrophot-0.16.2.tar` & `astrophot-0.16.3.tar`

### file list

```diff
@@ -1,160 +1,161 @@
--rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 astrophot-0.16.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 astrophot-0.16.2/.readthedocs.yaml
--rw-r--r--   0        0        0     2597 2020-02-02 00:00:00.000000 astrophot-0.16.2/CITATION.cff
--rw-r--r--   0        0        0     5225 2020-02-02 00:00:00.000000 astrophot-0.16.2/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     4651 2020-02-02 00:00:00.000000 astrophot-0.16.2/CONTRIBUTING.md
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 astrophot-0.16.2/MANIFEST.in
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 astrophot-0.16.2/requirements-dev.txt
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 astrophot-0.16.2/requirements.txt
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 astrophot-0.16.2/.github/dependabot.yml
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 astrophot-0.16.2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 astrophot-0.16.2/.github/ISSUE_TEMPLATE/documentation.md
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 astrophot-0.16.2/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 astrophot-0.16.2/.github/ISSUE_TEMPLATE/refactor-request.md
--rw-r--r--   0        0        0     2611 2020-02-02 00:00:00.000000 astrophot-0.16.2/.github/workflows/cd.yaml
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 astrophot-0.16.2/.github/workflows/coverage.yaml
--rw-r--r--   0        0        0     1287 2020-02-02 00:00:00.000000 astrophot-0.16.2/.github/workflows/testing.yaml
--rw-r--r--   0        0        0     3166 2020-02-02 00:00:00.000000 astrophot-0.16.2/astrophot/AP_config.py
--rw-r--r--   0        0        0     6345 2020-02-02 00:00:00.000000 astrophot-0.16.2/astrophot/__init__.py
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 astrophot-0.16.2/astrophot/__main__.py
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 astrophot-0.16.2/astrophot/_version.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 astrophot-0.16.2/astrophot/errors/__init__.py
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 astrophot-0.16.2/astrophot/errors/base.py
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 astrophot-0.16.2/astrophot/errors/fit.py
--rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 astrophot-0.16.2/astrophot/errors/image.py
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 astrophot-0.16.2/astrophot/errors/models.py
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 astrophot-0.16.2/astrophot/errors/param.py
--rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 astrophot-0.16.2/astrophot/fit/__init__.py
--rw-r--r--   0        0        0     6085 2020-02-02 00:00:00.000000 astrophot-0.16.2/astrophot/fit/base.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 astrophot-0.16.2/astrophot/fit/gp.py
--rw-r--r--   0        0        0     6908 2020-02-02 00:00:00.000000 astrophot-0.16.2/astrophot/fit/gradient.py
--rw-r--r--   0        0        0     6862 2020-02-02 00:00:00.000000 astrophot-0.16.2/astrophot/fit/hmc.py
--rw-r--r--   0        0        0    13617 2020-02-02 00:00:00.000000 astrophot-0.16.2/astrophot/fit/iterative.py
--rw-r--r--   0        0        0    22641 2020-02-02 00:00:00.000000 astrophot-0.16.2/astrophot/fit/lm.py
--rw-r--r--   0        0        0     4223 2020-02-02 00:00:00.000000 astrophot-0.16.2/astrophot/fit/mhmcmc.py
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 astrophot-0.16.2/astrophot/fit/minifit.py
--rw-r--r--   0        0        0     7043 2020-02-02 00:00:00.000000 astrophot-0.16.2/astrophot/fit/nuts.py
--rw-r--r--   0        0        0    27868 2020-02-02 00:00:00.000000 astrophot-0.16.2/astrophot/fit/oldlm.py
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 astrophot-0.16.2/astrophot/image/__init__.py
--rw-r--r--   0        0        0    10979 2020-02-02 00:00:00.000000 astrophot-0.16.2/astrophot/image/image_header.py
--rw-r--r--   0        0        0    25543 2020-02-02 00:00:00.000000 astrophot-0.16.2/astrophot/image/image_object.py
--rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 astrophot-0.16.2/astrophot/image/jacobian_image.py
--rw-r--r--   0        0        0     6760 2020-02-02 00:00:00.000000 astrophot-0.16.2/astrophot/image/model_image.py
--rw-r--r--   0        0        0     5516 2020-02-02 00:00:00.000000 astrophot-0.16.2/astrophot/image/psf_image.py
--rw-r--r--   0        0        0    24546 2020-02-02 00:00:00.000000 astrophot-0.16.2/astrophot/image/target_image.py
--rw-r--r--   0        0        0    31910 2020-02-02 00:00:00.000000 astrophot-0.16.2/astrophot/image/wcs.py
--rw-r--r--   0        0        0    25772 2020-02-02 00:00:00.000000 astrophot-0.16.2/astrophot/image/window_object.py
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 astrophot-0.16.2/astrophot/models/__init__.py
--rw-r--r--   0        0        0    17637 2020-02-02 00:00:00.000000 astrophot-0.16.2/astrophot/models/_model_methods.py
--rw-r--r--   0        0        0    22574 2020-02-02 00:00:00.000000 astrophot-0.16.2/astrophot/models/_shared_methods.py
--rw-r--r--   0        0        0     3642 2020-02-02 00:00:00.000000 astrophot-0.16.2/astrophot/models/airy_psf.py
--rw-r--r--   0        0        0    16918 2020-02-02 00:00:00.000000 astrophot-0.16.2/astrophot/models/core_model.py
--rw-r--r--   0        0        0     7102 2020-02-02 00:00:00.000000 astrophot-0.16.2/astrophot/models/edgeon_model.py
--rw-r--r--   0        0        0     6132 2020-02-02 00:00:00.000000 astrophot-0.16.2/astrophot/models/eigen_psf.py
--rw-r--r--   0        0        0    13738 2020-02-02 00:00:00.000000 astrophot-0.16.2/astrophot/models/exponential_model.py
--rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 astrophot-0.16.2/astrophot/models/flatsky_model.py
--rw-r--r--   0        0        0    10789 2020-02-02 00:00:00.000000 astrophot-0.16.2/astrophot/models/foureirellipse_model.py
--rw-r--r--   0        0        0     5601 2020-02-02 00:00:00.000000 astrophot-0.16.2/astrophot/models/galaxy_model_object.py
--rw-r--r--   0        0        0    12853 2020-02-02 00:00:00.000000 astrophot-0.16.2/astrophot/models/gaussian_model.py
--rw-r--r--   0        0        0    13220 2020-02-02 00:00:00.000000 astrophot-0.16.2/astrophot/models/group_model_object.py
--rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 astrophot-0.16.2/astrophot/models/group_psf_model.py
--rw-r--r--   0        0        0    18452 2020-02-02 00:00:00.000000 astrophot-0.16.2/astrophot/models/model_object.py
--rw-r--r--   0        0        0     5595 2020-02-02 00:00:00.000000 astrophot-0.16.2/astrophot/models/moffat_model.py
--rw-r--r--   0        0        0    18634 2020-02-02 00:00:00.000000 astrophot-0.16.2/astrophot/models/nuker_model.py
--rw-r--r--   0        0        0     3702 2020-02-02 00:00:00.000000 astrophot-0.16.2/astrophot/models/pixelated_psf_model.py
--rw-r--r--   0        0        0     2736 2020-02-02 00:00:00.000000 astrophot-0.16.2/astrophot/models/planesky_model.py
--rw-r--r--   0        0        0     7134 2020-02-02 00:00:00.000000 astrophot-0.16.2/astrophot/models/point_source.py
--rw-r--r--   0        0        0    12336 2020-02-02 00:00:00.000000 astrophot-0.16.2/astrophot/models/psf_model_object.py
--rw-r--r--   0        0        0     4698 2020-02-02 00:00:00.000000 astrophot-0.16.2/astrophot/models/ray_model.py
--rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 astrophot-0.16.2/astrophot/models/relspline_model.py
--rw-r--r--   0        0        0    16809 2020-02-02 00:00:00.000000 astrophot-0.16.2/astrophot/models/sersic_model.py
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 astrophot-0.16.2/astrophot/models/sky_model_object.py
--rw-r--r--   0        0        0    10762 2020-02-02 00:00:00.000000 astrophot-0.16.2/astrophot/models/spline_model.py
--rw-r--r--   0        0        0     3157 2020-02-02 00:00:00.000000 astrophot-0.16.2/astrophot/models/superellipse_model.py
--rw-r--r--   0        0        0     5475 2020-02-02 00:00:00.000000 astrophot-0.16.2/astrophot/models/warp_model.py
--rw-r--r--   0        0        0     3703 2020-02-02 00:00:00.000000 astrophot-0.16.2/astrophot/models/wedge_model.py
--rw-r--r--   0        0        0     4527 2020-02-02 00:00:00.000000 astrophot-0.16.2/astrophot/models/zernike_model.py
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 astrophot-0.16.2/astrophot/param/__init__.py
--rw-r--r--   0        0        0     7346 2020-02-02 00:00:00.000000 astrophot-0.16.2/astrophot/param/base.py
--rw-r--r--   0        0        0     3601 2020-02-02 00:00:00.000000 astrophot-0.16.2/astrophot/param/param_context.py
--rw-r--r--   0        0        0    29663 2020-02-02 00:00:00.000000 astrophot-0.16.2/astrophot/param/parameter.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 astrophot-0.16.2/astrophot/parse_config/__init__.py
--rw-r--r--   0        0        0     4119 2020-02-02 00:00:00.000000 astrophot-0.16.2/astrophot/parse_config/basic_config.py
--rw-r--r--   0        0        0     4387 2020-02-02 00:00:00.000000 astrophot-0.16.2/astrophot/parse_config/galfit_config.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astrophot-0.16.2/astrophot/parse_config/shared_methods.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 astrophot-0.16.2/astrophot/plots/__init__.py
--rw-r--r--   0        0        0     3325 2020-02-02 00:00:00.000000 astrophot-0.16.2/astrophot/plots/diagnostic.py
--rw-r--r--   0        0        0    18527 2020-02-02 00:00:00.000000 astrophot-0.16.2/astrophot/plots/image.py
--rw-r--r--   0        0        0     7658 2020-02-02 00:00:00.000000 astrophot-0.16.2/astrophot/plots/profile.py
--rw-r--r--   0        0        0     3035 2020-02-02 00:00:00.000000 astrophot-0.16.2/astrophot/plots/shared_elements.py
--rw-r--r--   0        0        0    20852 2020-02-02 00:00:00.000000 astrophot-0.16.2/astrophot/plots/visuals.py
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 astrophot-0.16.2/astrophot/utils/__init__.py
--rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 astrophot-0.16.2/astrophot/utils/angle_operations.py
--rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 astrophot-0.16.2/astrophot/utils/decorators.py
--rw-r--r--   0        0        0    11474 2020-02-02 00:00:00.000000 astrophot-0.16.2/astrophot/utils/interpolate.py
--rw-r--r--   0        0        0     9067 2020-02-02 00:00:00.000000 astrophot-0.16.2/astrophot/utils/operations.py
--rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 astrophot-0.16.2/astrophot/utils/optimization.py
--rw-r--r--   0        0        0     5694 2020-02-02 00:00:00.000000 astrophot-0.16.2/astrophot/utils/parametric_profiles.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astrophot-0.16.2/astrophot/utils/conversions/__init__.py
--rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 astrophot-0.16.2/astrophot/utils/conversions/coordinates.py
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 astrophot-0.16.2/astrophot/utils/conversions/dict_to_hdf5.py
--rw-r--r--   0        0        0     8078 2020-02-02 00:00:00.000000 astrophot-0.16.2/astrophot/utils/conversions/functions.py
--rw-r--r--   0        0        0     3070 2020-02-02 00:00:00.000000 astrophot-0.16.2/astrophot/utils/conversions/optimization.py
--rw-r--r--   0        0        0     3247 2020-02-02 00:00:00.000000 astrophot-0.16.2/astrophot/utils/conversions/units.py
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 astrophot-0.16.2/astrophot/utils/initialize/__init__.py
--rw-r--r--   0        0        0     2970 2020-02-02 00:00:00.000000 astrophot-0.16.2/astrophot/utils/initialize/center.py
--rw-r--r--   0        0        0     4448 2020-02-02 00:00:00.000000 astrophot-0.16.2/astrophot/utils/initialize/construct_psf.py
--rw-r--r--   0        0        0     3906 2020-02-02 00:00:00.000000 astrophot-0.16.2/astrophot/utils/initialize/initialize.py
--rw-r--r--   0        0        0    11068 2020-02-02 00:00:00.000000 astrophot-0.16.2/astrophot/utils/initialize/segmentation_map.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astrophot-0.16.2/astrophot/utils/isophote/__init__.py
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 astrophot-0.16.2/astrophot/utils/isophote/ellipse.py
--rw-r--r--   0        0        0     8423 2020-02-02 00:00:00.000000 astrophot-0.16.2/astrophot/utils/isophote/extract.py
--rw-r--r--   0        0        0     6928 2020-02-02 00:00:00.000000 astrophot-0.16.2/astrophot/utils/isophote/integrate.py
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 astrophot-0.16.2/docs/Makefile
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 astrophot-0.16.2/docs/requirements.txt
--rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 astrophot-0.16.2/docs/media/AP_logo_favicon.ico
--rw-r--r--   0        0        0     1467 2020-02-02 00:00:00.000000 astrophot-0.16.2/docs/source/_config.yml
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 astrophot-0.16.2/docs/source/_toc.yml
--rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 astrophot-0.16.2/docs/source/citation.rst
--rw-r--r--   0        0        0     2165 2020-02-02 00:00:00.000000 astrophot-0.16.2/docs/source/configfile_interface.rst
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 astrophot-0.16.2/docs/source/contributing.rst
--rw-r--r--   0        0        0    10908 2020-02-02 00:00:00.000000 astrophot-0.16.2/docs/source/coordinates.rst
--rw-r--r--   0        0        0     4326 2020-02-02 00:00:00.000000 astrophot-0.16.2/docs/source/getting_started.rst
--rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 astrophot-0.16.2/docs/source/index.rst
--rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 astrophot-0.16.2/docs/source/install.rst
--rw-r--r--   0        0        0    36085 2020-02-02 00:00:00.000000 astrophot-0.16.2/docs/source/license.rst
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 astrophot-0.16.2/docs/source/modules.rst
--rw-r--r--   0        0        0     1957 2020-02-02 00:00:00.000000 astrophot-0.16.2/docs/source/troubleshooting.rst
--rw-r--r--   0        0        0    19814 2020-02-02 00:00:00.000000 astrophot-0.16.2/docs/source/tutorials/AdvancedPSFModels.ipynb
--rw-r--r--   0        0        0     8317 2020-02-02 00:00:00.000000 astrophot-0.16.2/docs/source/tutorials/BasicPSFModels.ipynb
--rw-r--r--   0        0        0     8727 2020-02-02 00:00:00.000000 astrophot-0.16.2/docs/source/tutorials/ConstrainedModels.ipynb
--rw-r--r--   0        0        0    18299 2020-02-02 00:00:00.000000 astrophot-0.16.2/docs/source/tutorials/CustomModels.ipynb
--rw-r--r--   0        0        0    33534 2020-02-02 00:00:00.000000 astrophot-0.16.2/docs/source/tutorials/FittingMethods.ipynb
--rw-r--r--   0        0        0    27856 2020-02-02 00:00:00.000000 astrophot-0.16.2/docs/source/tutorials/GettingStarted.ipynb
--rw-r--r--   0        0        0     7824 2020-02-02 00:00:00.000000 astrophot-0.16.2/docs/source/tutorials/GroupModels.ipynb
--rw-r--r--   0        0        0    24132 2020-02-02 00:00:00.000000 astrophot-0.16.2/docs/source/tutorials/JointModels.ipynb
--rw-r--r--   0        0        0    53209 2020-02-02 00:00:00.000000 astrophot-0.16.2/docs/source/tutorials/ModelZoo.ipynb
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 astrophot-0.16.2/docs/source/tutorials/index.rst
--rw-r--r--   0        0        0    86041 2020-02-02 00:00:00.000000 astrophot-0.16.2/media/AP_logo.png
--rw-r--r--   0        0        0    90111 2020-02-02 00:00:00.000000 astrophot-0.16.2/media/AP_logo_white.png
--rw-r--r--   0        0        0    89580 2020-02-02 00:00:00.000000 astrophot-0.16.2/media/AstroPhotModelOrgchart.png
--rw-r--r--   0        0        0    67356 2020-02-02 00:00:00.000000 astrophot-0.16.2/media/groupjointmodels.png
--rw-r--r--   0        0        0    16800 2020-02-02 00:00:00.000000 astrophot-0.16.2/tests/test_fit.py
--rw-r--r--   0        0        0     6572 2020-02-02 00:00:00.000000 astrophot-0.16.2/tests/test_group_models.py
--rw-r--r--   0        0        0    22655 2020-02-02 00:00:00.000000 astrophot-0.16.2/tests/test_image.py
--rw-r--r--   0        0        0     4341 2020-02-02 00:00:00.000000 astrophot-0.16.2/tests/test_image_header.py
--rw-r--r--   0        0        0    15586 2020-02-02 00:00:00.000000 astrophot-0.16.2/tests/test_image_list.py
--rw-r--r--   0        0        0     9708 2020-02-02 00:00:00.000000 astrophot-0.16.2/tests/test_model.py
--rw-r--r--   0        0        0    20550 2020-02-02 00:00:00.000000 astrophot-0.16.2/tests/test_parameter.py
--rw-r--r--   0        0        0     3424 2020-02-02 00:00:00.000000 astrophot-0.16.2/tests/test_plots.py
--rw-r--r--   0        0        0     2702 2020-02-02 00:00:00.000000 astrophot-0.16.2/tests/test_psfmodel.py
--rw-r--r--   0        0        0    18920 2020-02-02 00:00:00.000000 astrophot-0.16.2/tests/test_utils.py
--rw-r--r--   0        0        0    18903 2020-02-02 00:00:00.000000 astrophot-0.16.2/tests/test_wcs.py
--rw-r--r--   0        0        0    14405 2020-02-02 00:00:00.000000 astrophot-0.16.2/tests/test_window.py
--rw-r--r--   0        0        0     9018 2020-02-02 00:00:00.000000 astrophot-0.16.2/tests/test_window_list.py
--rw-r--r--   0        0        0     2899 2020-02-02 00:00:00.000000 astrophot-0.16.2/tests/utils.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 astrophot-0.16.2/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 astrophot-0.16.2/LICENSE
--rw-r--r--   0        0        0     3182 2020-02-02 00:00:00.000000 astrophot-0.16.2/README.md
--rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 astrophot-0.16.2/pyproject.toml
--rw-r--r--   0        0        0    45011 2020-02-02 00:00:00.000000 astrophot-0.16.2/PKG-INFO
+-rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 astrophot-0.16.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 astrophot-0.16.3/.readthedocs.yaml
+-rw-r--r--   0        0        0     2597 2020-02-02 00:00:00.000000 astrophot-0.16.3/CITATION.cff
+-rw-r--r--   0        0        0     5225 2020-02-02 00:00:00.000000 astrophot-0.16.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     4651 2020-02-02 00:00:00.000000 astrophot-0.16.3/CONTRIBUTING.md
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 astrophot-0.16.3/MANIFEST.in
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 astrophot-0.16.3/requirements-dev.txt
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 astrophot-0.16.3/requirements.txt
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 astrophot-0.16.3/.github/dependabot.yml
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 astrophot-0.16.3/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 astrophot-0.16.3/.github/ISSUE_TEMPLATE/documentation.md
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 astrophot-0.16.3/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 astrophot-0.16.3/.github/ISSUE_TEMPLATE/refactor-request.md
+-rw-r--r--   0        0        0     2611 2020-02-02 00:00:00.000000 astrophot-0.16.3/.github/workflows/cd.yaml
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 astrophot-0.16.3/.github/workflows/coverage.yaml
+-rw-r--r--   0        0        0     1287 2020-02-02 00:00:00.000000 astrophot-0.16.3/.github/workflows/testing.yaml
+-rw-r--r--   0        0        0     3166 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/AP_config.py
+-rw-r--r--   0        0        0     6345 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/__init__.py
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/__main__.py
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/_version.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/errors/__init__.py
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/errors/base.py
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/errors/fit.py
+-rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/errors/image.py
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/errors/models.py
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/errors/param.py
+-rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/fit/__init__.py
+-rw-r--r--   0        0        0     6085 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/fit/base.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/fit/gp.py
+-rw-r--r--   0        0        0     6908 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/fit/gradient.py
+-rw-r--r--   0        0        0     6862 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/fit/hmc.py
+-rw-r--r--   0        0        0    13617 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/fit/iterative.py
+-rw-r--r--   0        0        0    22641 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/fit/lm.py
+-rw-r--r--   0        0        0     4223 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/fit/mhmcmc.py
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/fit/minifit.py
+-rw-r--r--   0        0        0     7043 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/fit/nuts.py
+-rw-r--r--   0        0        0    27868 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/fit/oldlm.py
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/image/__init__.py
+-rw-r--r--   0        0        0    10979 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/image/image_header.py
+-rw-r--r--   0        0        0    25543 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/image/image_object.py
+-rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/image/jacobian_image.py
+-rw-r--r--   0        0        0     6760 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/image/model_image.py
+-rw-r--r--   0        0        0     5516 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/image/psf_image.py
+-rw-r--r--   0        0        0    24825 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/image/target_image.py
+-rw-r--r--   0        0        0    31910 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/image/wcs.py
+-rw-r--r--   0        0        0    25772 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/image/window_object.py
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/models/__init__.py
+-rw-r--r--   0        0        0    17637 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/models/_model_methods.py
+-rw-r--r--   0        0        0    22574 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/models/_shared_methods.py
+-rw-r--r--   0        0        0     3642 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/models/airy_psf.py
+-rw-r--r--   0        0        0    16918 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/models/core_model.py
+-rw-r--r--   0        0        0     7102 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/models/edgeon_model.py
+-rw-r--r--   0        0        0     6132 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/models/eigen_psf.py
+-rw-r--r--   0        0        0    13738 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/models/exponential_model.py
+-rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/models/flatsky_model.py
+-rw-r--r--   0        0        0    10789 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/models/foureirellipse_model.py
+-rw-r--r--   0        0        0     5601 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/models/galaxy_model_object.py
+-rw-r--r--   0        0        0    12853 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/models/gaussian_model.py
+-rw-r--r--   0        0        0    13220 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/models/group_model_object.py
+-rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/models/group_psf_model.py
+-rw-r--r--   0        0        0    18452 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/models/model_object.py
+-rw-r--r--   0        0        0     5595 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/models/moffat_model.py
+-rw-r--r--   0        0        0    18634 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/models/nuker_model.py
+-rw-r--r--   0        0        0     3702 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/models/pixelated_psf_model.py
+-rw-r--r--   0        0        0     2736 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/models/planesky_model.py
+-rw-r--r--   0        0        0     7134 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/models/point_source.py
+-rw-r--r--   0        0        0    12336 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/models/psf_model_object.py
+-rw-r--r--   0        0        0     4698 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/models/ray_model.py
+-rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/models/relspline_model.py
+-rw-r--r--   0        0        0    16809 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/models/sersic_model.py
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/models/sky_model_object.py
+-rw-r--r--   0        0        0    10762 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/models/spline_model.py
+-rw-r--r--   0        0        0     3157 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/models/superellipse_model.py
+-rw-r--r--   0        0        0     5475 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/models/warp_model.py
+-rw-r--r--   0        0        0     3703 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/models/wedge_model.py
+-rw-r--r--   0        0        0     4527 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/models/zernike_model.py
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/param/__init__.py
+-rw-r--r--   0        0        0     7346 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/param/base.py
+-rw-r--r--   0        0        0     3601 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/param/param_context.py
+-rw-r--r--   0        0        0    29663 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/param/parameter.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/parse_config/__init__.py
+-rw-r--r--   0        0        0     4119 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/parse_config/basic_config.py
+-rw-r--r--   0        0        0     4387 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/parse_config/galfit_config.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/parse_config/shared_methods.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/plots/__init__.py
+-rw-r--r--   0        0        0     3325 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/plots/diagnostic.py
+-rw-r--r--   0        0        0    18527 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/plots/image.py
+-rw-r--r--   0        0        0     7658 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/plots/profile.py
+-rw-r--r--   0        0        0     3035 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/plots/shared_elements.py
+-rw-r--r--   0        0        0    20852 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/plots/visuals.py
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/utils/__init__.py
+-rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/utils/angle_operations.py
+-rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/utils/decorators.py
+-rw-r--r--   0        0        0    11474 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/utils/interpolate.py
+-rw-r--r--   0        0        0     9067 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/utils/operations.py
+-rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/utils/optimization.py
+-rw-r--r--   0        0        0     5694 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/utils/parametric_profiles.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/utils/conversions/__init__.py
+-rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/utils/conversions/coordinates.py
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/utils/conversions/dict_to_hdf5.py
+-rw-r--r--   0        0        0     8078 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/utils/conversions/functions.py
+-rw-r--r--   0        0        0     3070 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/utils/conversions/optimization.py
+-rw-r--r--   0        0        0     3247 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/utils/conversions/units.py
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/utils/initialize/__init__.py
+-rw-r--r--   0        0        0     2970 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/utils/initialize/center.py
+-rw-r--r--   0        0        0     4448 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/utils/initialize/construct_psf.py
+-rw-r--r--   0        0        0     3906 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/utils/initialize/initialize.py
+-rw-r--r--   0        0        0    11068 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/utils/initialize/segmentation_map.py
+-rw-r--r--   0        0        0     1866 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/utils/initialize/variance.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/utils/isophote/__init__.py
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/utils/isophote/ellipse.py
+-rw-r--r--   0        0        0     8423 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/utils/isophote/extract.py
+-rw-r--r--   0        0        0     6928 2020-02-02 00:00:00.000000 astrophot-0.16.3/astrophot/utils/isophote/integrate.py
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 astrophot-0.16.3/docs/Makefile
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 astrophot-0.16.3/docs/requirements.txt
+-rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 astrophot-0.16.3/docs/media/AP_logo_favicon.ico
+-rw-r--r--   0        0        0     1467 2020-02-02 00:00:00.000000 astrophot-0.16.3/docs/source/_config.yml
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 astrophot-0.16.3/docs/source/_toc.yml
+-rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 astrophot-0.16.3/docs/source/citation.rst
+-rw-r--r--   0        0        0     2165 2020-02-02 00:00:00.000000 astrophot-0.16.3/docs/source/configfile_interface.rst
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 astrophot-0.16.3/docs/source/contributing.rst
+-rw-r--r--   0        0        0    10908 2020-02-02 00:00:00.000000 astrophot-0.16.3/docs/source/coordinates.rst
+-rw-r--r--   0        0        0     4326 2020-02-02 00:00:00.000000 astrophot-0.16.3/docs/source/getting_started.rst
+-rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 astrophot-0.16.3/docs/source/index.rst
+-rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 astrophot-0.16.3/docs/source/install.rst
+-rw-r--r--   0        0        0    36085 2020-02-02 00:00:00.000000 astrophot-0.16.3/docs/source/license.rst
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 astrophot-0.16.3/docs/source/modules.rst
+-rw-r--r--   0        0        0     1957 2020-02-02 00:00:00.000000 astrophot-0.16.3/docs/source/troubleshooting.rst
+-rw-r--r--   0        0        0    19814 2020-02-02 00:00:00.000000 astrophot-0.16.3/docs/source/tutorials/AdvancedPSFModels.ipynb
+-rw-r--r--   0        0        0     8317 2020-02-02 00:00:00.000000 astrophot-0.16.3/docs/source/tutorials/BasicPSFModels.ipynb
+-rw-r--r--   0        0        0     8727 2020-02-02 00:00:00.000000 astrophot-0.16.3/docs/source/tutorials/ConstrainedModels.ipynb
+-rw-r--r--   0        0        0    18299 2020-02-02 00:00:00.000000 astrophot-0.16.3/docs/source/tutorials/CustomModels.ipynb
+-rw-r--r--   0        0        0    33534 2020-02-02 00:00:00.000000 astrophot-0.16.3/docs/source/tutorials/FittingMethods.ipynb
+-rw-r--r--   0        0        0    27921 2020-02-02 00:00:00.000000 astrophot-0.16.3/docs/source/tutorials/GettingStarted.ipynb
+-rw-r--r--   0        0        0     7861 2020-02-02 00:00:00.000000 astrophot-0.16.3/docs/source/tutorials/GroupModels.ipynb
+-rw-r--r--   0        0        0    23851 2020-02-02 00:00:00.000000 astrophot-0.16.3/docs/source/tutorials/JointModels.ipynb
+-rw-r--r--   0        0        0    53209 2020-02-02 00:00:00.000000 astrophot-0.16.3/docs/source/tutorials/ModelZoo.ipynb
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 astrophot-0.16.3/docs/source/tutorials/index.rst
+-rw-r--r--   0        0        0    86041 2020-02-02 00:00:00.000000 astrophot-0.16.3/media/AP_logo.png
+-rw-r--r--   0        0        0    90111 2020-02-02 00:00:00.000000 astrophot-0.16.3/media/AP_logo_white.png
+-rw-r--r--   0        0        0    89580 2020-02-02 00:00:00.000000 astrophot-0.16.3/media/AstroPhotModelOrgchart.png
+-rw-r--r--   0        0        0    67356 2020-02-02 00:00:00.000000 astrophot-0.16.3/media/groupjointmodels.png
+-rw-r--r--   0        0        0    16800 2020-02-02 00:00:00.000000 astrophot-0.16.3/tests/test_fit.py
+-rw-r--r--   0        0        0     6572 2020-02-02 00:00:00.000000 astrophot-0.16.3/tests/test_group_models.py
+-rw-r--r--   0        0        0    22789 2020-02-02 00:00:00.000000 astrophot-0.16.3/tests/test_image.py
+-rw-r--r--   0        0        0     4341 2020-02-02 00:00:00.000000 astrophot-0.16.3/tests/test_image_header.py
+-rw-r--r--   0        0        0    15586 2020-02-02 00:00:00.000000 astrophot-0.16.3/tests/test_image_list.py
+-rw-r--r--   0        0        0     9708 2020-02-02 00:00:00.000000 astrophot-0.16.3/tests/test_model.py
+-rw-r--r--   0        0        0    20550 2020-02-02 00:00:00.000000 astrophot-0.16.3/tests/test_parameter.py
+-rw-r--r--   0        0        0     3424 2020-02-02 00:00:00.000000 astrophot-0.16.3/tests/test_plots.py
+-rw-r--r--   0        0        0     2702 2020-02-02 00:00:00.000000 astrophot-0.16.3/tests/test_psfmodel.py
+-rw-r--r--   0        0        0    18920 2020-02-02 00:00:00.000000 astrophot-0.16.3/tests/test_utils.py
+-rw-r--r--   0        0        0    18903 2020-02-02 00:00:00.000000 astrophot-0.16.3/tests/test_wcs.py
+-rw-r--r--   0        0        0    14405 2020-02-02 00:00:00.000000 astrophot-0.16.3/tests/test_window.py
+-rw-r--r--   0        0        0     9018 2020-02-02 00:00:00.000000 astrophot-0.16.3/tests/test_window_list.py
+-rw-r--r--   0        0        0     2899 2020-02-02 00:00:00.000000 astrophot-0.16.3/tests/utils.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 astrophot-0.16.3/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 astrophot-0.16.3/LICENSE
+-rw-r--r--   0        0        0     3353 2020-02-02 00:00:00.000000 astrophot-0.16.3/README.md
+-rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 astrophot-0.16.3/pyproject.toml
+-rw-r--r--   0        0        0    45182 2020-02-02 00:00:00.000000 astrophot-0.16.3/PKG-INFO
```

### Comparing `astrophot-0.16.2/.pre-commit-config.yaml` & `astrophot-0.16.3/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -5,27 +5,27 @@
 
 ci:
   autoupdate_commit_msg: "chore: update pre-commit hooks"
   autofix_commit_msg: "style: pre-commit fixes"
 
 repos:
   - repo: https://github.com/psf/black
-    rev: "24.3.0"
+    rev: "24.4.0"
     hooks:
       - id: black-jupyter
         args: ["--line-length", "100"]
 
   - repo: https://github.com/asottile/blacken-docs
     rev: "1.16.0"
     hooks:
       - id: blacken-docs
         additional_dependencies: [black==23.7.0]
 
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: "v4.5.0"
+    rev: "v4.6.0"
     hooks:
       - id: check-added-large-files
       - id: check-case-conflict
       - id: check-merge-conflict
       - id: check-symlinks
       - id: check-yaml
       - id: debug-statements
```

### Comparing `astrophot-0.16.2/.readthedocs.yaml` & `astrophot-0.16.3/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/CITATION.cff` & `astrophot-0.16.3/CITATION.cff`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/CODE_OF_CONDUCT.md` & `astrophot-0.16.3/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/CONTRIBUTING.md` & `astrophot-0.16.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/.github/dependabot.yml` & `astrophot-0.16.3/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/.github/ISSUE_TEMPLATE/bug_report.md` & `astrophot-0.16.3/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/.github/ISSUE_TEMPLATE/feature_request.md` & `astrophot-0.16.3/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/.github/ISSUE_TEMPLATE/refactor-request.md` & `astrophot-0.16.3/.github/ISSUE_TEMPLATE/refactor-request.md`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/.github/workflows/cd.yaml` & `astrophot-0.16.3/.github/workflows/cd.yaml`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/.github/workflows/coverage.yaml` & `astrophot-0.16.3/.github/workflows/coverage.yaml`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/.github/workflows/testing.yaml` & `astrophot-0.16.3/.github/workflows/testing.yaml`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/astrophot/AP_config.py` & `astrophot-0.16.3/astrophot/AP_config.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/astrophot/__init__.py` & `astrophot-0.16.3/astrophot/__init__.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/astrophot/errors/image.py` & `astrophot-0.16.3/astrophot/errors/image.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/astrophot/fit/__init__.py` & `astrophot-0.16.3/astrophot/fit/__init__.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/astrophot/fit/base.py` & `astrophot-0.16.3/astrophot/fit/base.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/astrophot/fit/gradient.py` & `astrophot-0.16.3/astrophot/fit/gradient.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/astrophot/fit/hmc.py` & `astrophot-0.16.3/astrophot/fit/hmc.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/astrophot/fit/iterative.py` & `astrophot-0.16.3/astrophot/fit/iterative.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/astrophot/fit/lm.py` & `astrophot-0.16.3/astrophot/fit/lm.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/astrophot/fit/mhmcmc.py` & `astrophot-0.16.3/astrophot/fit/mhmcmc.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/astrophot/fit/minifit.py` & `astrophot-0.16.3/astrophot/fit/minifit.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/astrophot/fit/nuts.py` & `astrophot-0.16.3/astrophot/fit/nuts.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/astrophot/fit/oldlm.py` & `astrophot-0.16.3/astrophot/fit/oldlm.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/astrophot/image/image_header.py` & `astrophot-0.16.3/astrophot/image/image_header.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/astrophot/image/image_object.py` & `astrophot-0.16.3/astrophot/image/image_object.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/astrophot/image/jacobian_image.py` & `astrophot-0.16.3/astrophot/image/jacobian_image.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/astrophot/image/model_image.py` & `astrophot-0.16.3/astrophot/image/model_image.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/astrophot/image/psf_image.py` & `astrophot-0.16.3/astrophot/image/psf_image.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/astrophot/image/target_image.py` & `astrophot-0.16.3/astrophot/image/target_image.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import numpy as np
 
 from .image_object import Image, Image_List
 from .jacobian_image import Jacobian_Image, Jacobian_Image_List
 from .model_image import Model_Image, Model_Image_List
 from .psf_image import PSF_Image
 from .. import AP_config
+from ..utils.initialize import auto_variance
 from ..errors import SpecificationConflict, InvalidImage
 
 __all__ = ["Target_Image", "Target_Image_List"]
 
 
 class Target_Image(Image):
     """Image object which represents the data to be fit by a model. It can
@@ -79,20 +80,20 @@
     """
 
     image_count = 0
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
+        if not self.has_mask:
+            self.set_mask(kwargs.get("mask", None))
         if not self.has_weight and "weight" in kwargs:
             self.set_weight(kwargs.get("weight", None))
         elif not self.has_variance and "variance" in kwargs:
             self.set_variance(kwargs.get("variance", None))
-        if not self.has_mask:
-            self.set_mask(kwargs.get("mask", None))
         if not self.has_psf:
             self.set_psf(kwargs.get("psf", None), kwargs.get("psf_upscale", 1))
 
         # Set nan pixels to be masked automatically
         if torch.any(torch.isnan(self.data)).item():
             self.set_mask(torch.logical_or(self.mask, torch.isnan(self.data)))
 
@@ -270,24 +271,29 @@
     def set_variance(self, variance):
         """
         Provide a variance tensor for the image. Variance is equal to :math:`\\sigma^2`. This should have the same shape as the data.
         """
         if variance is None:
             self._weight = None
             return
+        if isinstance(variance, str) and variance == "auto":
+            self.set_weight("auto")
+            return
         self.set_weight(1 / variance)
 
     def set_weight(self, weight):
         """Provide a weight tensor for the image. Weight is equal to :math:`\\frac{1}{\\sigma^2}`. This should have the same
         shape as the data.
 
         """
         if weight is None:
             self._weight = None
             return
+        if isinstance(weight, str) and weight == "auto":
+            weight = 1 / auto_variance(self.data, self.mask)
         if weight.shape != self.data.shape:
             raise SpecificationConflict(
                 f"weight/variance must have same shape as data ({weight.shape} vs {self.data.shape})"
             )
         self._weight = (
             weight.to(dtype=AP_config.ap_dtype, device=AP_config.ap_device)
             if isinstance(weight, torch.Tensor)
```

### Comparing `astrophot-0.16.2/astrophot/image/wcs.py` & `astrophot-0.16.3/astrophot/image/wcs.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/astrophot/image/window_object.py` & `astrophot-0.16.3/astrophot/image/window_object.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/astrophot/models/__init__.py` & `astrophot-0.16.3/astrophot/models/__init__.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/astrophot/models/_model_methods.py` & `astrophot-0.16.3/astrophot/models/_model_methods.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/astrophot/models/_shared_methods.py` & `astrophot-0.16.3/astrophot/models/_shared_methods.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/astrophot/models/airy_psf.py` & `astrophot-0.16.3/astrophot/models/airy_psf.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/astrophot/models/core_model.py` & `astrophot-0.16.3/astrophot/models/core_model.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/astrophot/models/edgeon_model.py` & `astrophot-0.16.3/astrophot/models/edgeon_model.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/astrophot/models/eigen_psf.py` & `astrophot-0.16.3/astrophot/models/eigen_psf.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/astrophot/models/exponential_model.py` & `astrophot-0.16.3/astrophot/models/exponential_model.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/astrophot/models/flatsky_model.py` & `astrophot-0.16.3/astrophot/models/flatsky_model.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/astrophot/models/foureirellipse_model.py` & `astrophot-0.16.3/astrophot/models/foureirellipse_model.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/astrophot/models/galaxy_model_object.py` & `astrophot-0.16.3/astrophot/models/galaxy_model_object.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/astrophot/models/gaussian_model.py` & `astrophot-0.16.3/astrophot/models/gaussian_model.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/astrophot/models/group_model_object.py` & `astrophot-0.16.3/astrophot/models/group_model_object.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/astrophot/models/group_psf_model.py` & `astrophot-0.16.3/astrophot/models/group_psf_model.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/astrophot/models/model_object.py` & `astrophot-0.16.3/astrophot/models/model_object.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/astrophot/models/moffat_model.py` & `astrophot-0.16.3/astrophot/models/moffat_model.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/astrophot/models/nuker_model.py` & `astrophot-0.16.3/astrophot/models/nuker_model.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/astrophot/models/pixelated_psf_model.py` & `astrophot-0.16.3/astrophot/models/pixelated_psf_model.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/astrophot/models/planesky_model.py` & `astrophot-0.16.3/astrophot/models/planesky_model.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/astrophot/models/point_source.py` & `astrophot-0.16.3/astrophot/models/point_source.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/astrophot/models/psf_model_object.py` & `astrophot-0.16.3/astrophot/models/psf_model_object.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/astrophot/models/ray_model.py` & `astrophot-0.16.3/astrophot/models/ray_model.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/astrophot/models/relspline_model.py` & `astrophot-0.16.3/astrophot/models/relspline_model.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/astrophot/models/sersic_model.py` & `astrophot-0.16.3/astrophot/models/sersic_model.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/astrophot/models/sky_model_object.py` & `astrophot-0.16.3/astrophot/models/sky_model_object.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/astrophot/models/spline_model.py` & `astrophot-0.16.3/astrophot/models/spline_model.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/astrophot/models/superellipse_model.py` & `astrophot-0.16.3/astrophot/models/superellipse_model.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/astrophot/models/warp_model.py` & `astrophot-0.16.3/astrophot/models/warp_model.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/astrophot/models/wedge_model.py` & `astrophot-0.16.3/astrophot/models/wedge_model.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/astrophot/models/zernike_model.py` & `astrophot-0.16.3/astrophot/models/zernike_model.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/astrophot/param/base.py` & `astrophot-0.16.3/astrophot/param/base.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/astrophot/param/param_context.py` & `astrophot-0.16.3/astrophot/param/param_context.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/astrophot/param/parameter.py` & `astrophot-0.16.3/astrophot/param/parameter.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/astrophot/parse_config/basic_config.py` & `astrophot-0.16.3/astrophot/parse_config/basic_config.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/astrophot/parse_config/galfit_config.py` & `astrophot-0.16.3/astrophot/parse_config/galfit_config.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/astrophot/plots/diagnostic.py` & `astrophot-0.16.3/astrophot/plots/diagnostic.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/astrophot/plots/image.py` & `astrophot-0.16.3/astrophot/plots/image.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/astrophot/plots/profile.py` & `astrophot-0.16.3/astrophot/plots/profile.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/astrophot/plots/shared_elements.py` & `astrophot-0.16.3/astrophot/plots/shared_elements.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/astrophot/plots/visuals.py` & `astrophot-0.16.3/astrophot/plots/visuals.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/astrophot/utils/angle_operations.py` & `astrophot-0.16.3/astrophot/utils/angle_operations.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/astrophot/utils/decorators.py` & `astrophot-0.16.3/astrophot/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/astrophot/utils/interpolate.py` & `astrophot-0.16.3/astrophot/utils/interpolate.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/astrophot/utils/operations.py` & `astrophot-0.16.3/astrophot/utils/operations.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/astrophot/utils/optimization.py` & `astrophot-0.16.3/astrophot/utils/optimization.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/astrophot/utils/parametric_profiles.py` & `astrophot-0.16.3/astrophot/utils/parametric_profiles.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/astrophot/utils/conversions/coordinates.py` & `astrophot-0.16.3/astrophot/utils/conversions/coordinates.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/astrophot/utils/conversions/dict_to_hdf5.py` & `astrophot-0.16.3/astrophot/utils/conversions/dict_to_hdf5.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/astrophot/utils/conversions/functions.py` & `astrophot-0.16.3/astrophot/utils/conversions/functions.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/astrophot/utils/conversions/optimization.py` & `astrophot-0.16.3/astrophot/utils/conversions/optimization.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/astrophot/utils/conversions/units.py` & `astrophot-0.16.3/astrophot/utils/conversions/units.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/astrophot/utils/initialize/__init__.py` & `astrophot-0.16.3/astrophot/utils/initialize/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from .segmentation_map import *
 from .initialize import isophotes
 from .center import center_of_mass, GaussianDensity_Peak, Lanczos_peak
 from .construct_psf import gaussian_psf, moffat_psf, construct_psf
+from .variance import auto_variance
 
 __all__ = (
     "isophotes",
     "center_of_mass",
     "GaussianDensity_Peak",
     "Lanczos_peak",
     "gaussian_psf",
@@ -14,8 +15,9 @@
     "centroids_from_segmentation_map",
     "PA_from_segmentation_map",
     "q_from_segmentation_map",
     "windows_from_segmentation_map",
     "scale_windows",
     "filter_windows",
     "transfer_windows",
+    "auto_variance",
 )
```

### Comparing `astrophot-0.16.2/astrophot/utils/initialize/center.py` & `astrophot-0.16.3/astrophot/utils/initialize/center.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/astrophot/utils/initialize/construct_psf.py` & `astrophot-0.16.3/astrophot/utils/initialize/construct_psf.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/astrophot/utils/initialize/initialize.py` & `astrophot-0.16.3/astrophot/utils/initialize/initialize.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/astrophot/utils/initialize/segmentation_map.py` & `astrophot-0.16.3/astrophot/utils/initialize/segmentation_map.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/astrophot/utils/isophote/ellipse.py` & `astrophot-0.16.3/astrophot/utils/isophote/ellipse.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/astrophot/utils/isophote/extract.py` & `astrophot-0.16.3/astrophot/utils/isophote/extract.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/astrophot/utils/isophote/integrate.py` & `astrophot-0.16.3/astrophot/utils/isophote/integrate.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/docs/Makefile` & `astrophot-0.16.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/docs/media/AP_logo_favicon.ico` & `astrophot-0.16.3/docs/media/AP_logo_favicon.ico`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/docs/source/_config.yml` & `astrophot-0.16.3/docs/source/_config.yml`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/docs/source/citation.rst` & `astrophot-0.16.3/docs/source/citation.rst`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/docs/source/configfile_interface.rst` & `astrophot-0.16.3/docs/source/configfile_interface.rst`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/docs/source/coordinates.rst` & `astrophot-0.16.3/docs/source/coordinates.rst`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/docs/source/getting_started.rst` & `astrophot-0.16.3/docs/source/getting_started.rst`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/docs/source/index.rst` & `astrophot-0.16.3/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/docs/source/install.rst` & `astrophot-0.16.3/docs/source/install.rst`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/docs/source/license.rst` & `astrophot-0.16.3/docs/source/license.rst`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/docs/source/troubleshooting.rst` & `astrophot-0.16.3/docs/source/troubleshooting.rst`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/docs/source/tutorials/AdvancedPSFModels.ipynb` & `astrophot-0.16.3/docs/source/tutorials/AdvancedPSFModels.ipynb`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/docs/source/tutorials/BasicPSFModels.ipynb` & `astrophot-0.16.3/docs/source/tutorials/BasicPSFModels.ipynb`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/docs/source/tutorials/ConstrainedModels.ipynb` & `astrophot-0.16.3/docs/source/tutorials/ConstrainedModels.ipynb`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/docs/source/tutorials/CustomModels.ipynb` & `astrophot-0.16.3/docs/source/tutorials/CustomModels.ipynb`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/docs/source/tutorials/FittingMethods.ipynb` & `astrophot-0.16.3/docs/source/tutorials/FittingMethods.ipynb`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/docs/source/tutorials/GettingStarted.ipynb` & `astrophot-0.16.3/docs/source/tutorials/GettingStarted.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999778079710145%*

 * *Differences: {"'cells'": '{6: {\'source\': {insert: [(11, \'    variance="auto",  # Automatic variance estimate '*

 * *            'for testing and demo purposes, in real analysis use weight maps, counts, gain, etc to '*

 * *            "compute variance!\\n')], delete: [12, 11]}}, 9: {'source': {insert: [(3, "*

 * *            "'ap.plots.residual_image(fig5, ax5[1], model2, normalize_residuals=True)\\n')], "*

 * *            "delete: [3]}}, 18: {'source': {insert: [(3, 'ap.plots.residual_image(fig7, ax7[1], "*

 * *            "model3, normaliz […]*

```diff
@@ -103,16 +103,15 @@
                 "target_data = np.array(hdu[0].data, dtype=np.float64)\n",
                 "\n",
                 "# Create a target object with specified pixelscale and zeropoint\n",
                 "target = ap.image.Target_Image(\n",
                 "    data=target_data,\n",
                 "    pixelscale=0.262,  # Every target image needs to know it's pixelscale in arcsec/pixel\n",
                 "    zeropoint=22.5,  # optionally, you can give a zeropoint to tell AstroPhot what the pixel flux units are\n",
-                "    variance=np.ones(target_data.shape)\n",
-                "    / 1e3,  # set the variance for this image (in general it should be more accurate than this)\n",
+                "    variance=\"auto\",  # Automatic variance estimate for testing and demo purposes, in real analysis use weight maps, counts, gain, etc to compute variance!\n",
                 ")\n",
                 "\n",
                 "# The default AstroPhot target plotting method uses log scaling in bright areas and histogram scaling in faint areas\n",
                 "fig3, ax3 = plt.subplots(figsize=(8, 8))\n",
                 "ap.plots.target_image(fig3, ax3, target)\n",
                 "plt.show()"
             ]
@@ -164,15 +163,15 @@
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# we now plot the fitted model and the image residuals\n",
                 "fig5, ax5 = plt.subplots(1, 2, figsize=(16, 6))\n",
                 "ap.plots.model_image(fig5, ax5[0], model2)\n",
-                "ap.plots.residual_image(fig5, ax5[1], model2)\n",
+                "ap.plots.residual_image(fig5, ax5[1], model2, normalize_residuals=True)\n",
                 "plt.show()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
@@ -285,15 +284,15 @@
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# Note that when only a window is fit, the default plotting methods will only show that window\n",
                 "fig7, ax7 = plt.subplots(1, 2, figsize=(16, 6))\n",
                 "ap.plots.model_image(fig7, ax7[0], model3)\n",
-                "ap.plots.residual_image(fig7, ax7[1], model3)\n",
+                "ap.plots.residual_image(fig7, ax7[1], model3, normalize_residuals=True)\n",
                 "plt.show()"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
```

### Comparing `astrophot-0.16.2/docs/source/tutorials/GroupModels.ipynb` & `astrophot-0.16.3/docs/source/tutorials/GroupModels.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.99927398989899%*

 * *Differences: {"'cells'": '{4: {\'source\': {insert: [(5, \'    variance="auto",  # np.ones_like(target_data) * '*

 * *            "np.std(target_data[segmap == 0]) ** 2,\\n')], delete: [5]}}, 6: {'source': {insert: "*

 * *            "[(4, '    windows, image_shape=target_data.shape, expand_scale=2, "*

 * *            "expand_border=10\\n')], delete: [4]}}, 10: {'source': {insert: [(3, "*

 * *            "'ap.plots.residual_image(fig10, ax10[1], groupmodel, normalize_residuals=True)\\n')], "*

 * *            'delete: [3]}}}'}*

```diff
@@ -74,15 +74,15 @@
             "outputs": [],
             "source": [
                 "pixelscale = 0.262\n",
                 "target = ap.image.Target_Image(\n",
                 "    data=target_data,\n",
                 "    pixelscale=pixelscale,\n",
                 "    zeropoint=22.5,\n",
-                "    variance=np.ones_like(target_data) * np.std(target_data[segmap == 0]) ** 2,\n",
+                "    variance=\"auto\",  # np.ones_like(target_data) * np.std(target_data[segmap == 0]) ** 2,\n",
                 ")\n",
                 "fig2, ax2 = plt.subplots(figsize=(8, 8))\n",
                 "ap.plots.target_image(fig2, ax2, target)\n",
                 "plt.show()"
             ]
         },
         {
@@ -102,15 +102,15 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "# This will convert the segmentation map into boxes that enclose the identified pixels\n",
                 "windows = ap.utils.initialize.windows_from_segmentation_map(segmap)\n",
                 "# Next we scale up the windows so that AstroPhot can fit the faint parts of each object as well\n",
                 "windows = ap.utils.initialize.scale_windows(\n",
-                "    windows, image_shape=target_data.shape, expand_scale=1.5, expand_border=10\n",
+                "    windows, image_shape=target_data.shape, expand_scale=2, expand_border=10\n",
                 ")\n",
                 "# Here we get some basic starting parameters for the galaxies (center, position angle, axis ratio)\n",
                 "centers = ap.utils.initialize.centroids_from_segmentation_map(segmap, target_data)\n",
                 "PAs = ap.utils.initialize.PA_from_segmentation_map(segmap, target_data, centers)\n",
                 "qs = ap.utils.initialize.q_from_segmentation_map(segmap, target_data, centers, PAs)"
             ]
         },
@@ -187,15 +187,15 @@
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# Now we can see what the fitting has produced\n",
                 "fig10, ax10 = plt.subplots(1, 2, figsize=(16, 7))\n",
                 "ap.plots.model_image(fig10, ax10[0], groupmodel)\n",
-                "ap.plots.residual_image(fig10, ax10[1], groupmodel)\n",
+                "ap.plots.residual_image(fig10, ax10[1], groupmodel, normalize_residuals=True)\n",
                 "plt.show()"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
```

### Comparing `astrophot-0.16.2/docs/source/tutorials/JointModels.ipynb` & `astrophot-0.16.3/docs/source/tutorials/JointModels.ipynb`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9995654063864352%*

 * *Differences: {"'cells'": '{2: {\'source\': {insert: [(17, \'    variance="auto",  # auto variance gets it '*

 * *            "roughly right, use better estimate for science!\\n'), (32, '    "*

 * *            'variance="auto",\\n\'), (45, \'    variance="auto",\\n\')], delete: [47, 34, 19, 18, '*

 * *            "17]}}, 8: {'source': {insert: [(4, 'ap.plots.residual_image(fig1, ax1, model_full, "*

 * *            "flipx=True, normalize_residuals=True)\\n')], delete: [4]}}, 10: {'source': {insert: "*

 * *            '[(20, \'    variance="auto", […]*

```diff
@@ -47,45 +47,43 @@
                 "# Our first image is from the DESI Legacy-Survey r-band. This image has a pixelscale of 0.262 arcsec/pixel and is 500 pixels across\n",
                 "lrimg = fits.open(\n",
                 "    \"https://www.legacysurvey.org/viewer/fits-cutout?ra=187.3119&dec=12.9783&size=500&layer=ls-dr9&pixscale=0.262&bands=r\"\n",
                 ")\n",
                 "target_r = ap.image.Target_Image(\n",
                 "    data=np.array(lrimg[0].data, dtype=np.float64),\n",
                 "    zeropoint=22.5,\n",
-                "    variance=np.ones((500, 500))\n",
-                "    * 0.008\n",
-                "    ** 2,  # Here we just use the IQR^2 of the pixel values as the variance, for science data one would use a more accurate variance value\n",
+                "    variance=\"auto\",  # auto variance gets it roughly right, use better estimate for science!\n",
                 "    psf=ap.utils.initialize.gaussian_psf(\n",
                 "        1.12 / 2.355, 51, 0.262\n",
                 "    ),  # we construct a basic gaussian psf for each image by giving the simga (arcsec), image width (pixels), and pixelscale (arcsec/pixel)\n",
                 "    wcs=WCS(lrimg[0].header),  # note pixelscale and origin not needed when we have a WCS object!\n",
                 ")\n",
                 "\n",
                 "\n",
                 "# The second image is a unWISE W1 band image. This image has a pixelscale of 2.75 arcsec/pixel and is 52 pixels across\n",
                 "lw1img = fits.open(\n",
                 "    \"https://www.legacysurvey.org/viewer/fits-cutout?ra=187.3119&dec=12.9783&size=52&layer=unwise-neo7&pixscale=2.75&bands=1\"\n",
                 ")\n",
                 "target_W1 = ap.image.Target_Image(\n",
                 "    data=np.array(lw1img[0].data, dtype=np.float64),\n",
                 "    zeropoint=25.199,\n",
-                "    variance=np.ones((52, 52)) * 4.9**2,\n",
+                "    variance=\"auto\",\n",
                 "    psf=ap.utils.initialize.gaussian_psf(6.1 / 2.355, 21, 2.75),\n",
                 "    wcs=WCS(lw1img[0].header),\n",
                 "    reference_radec=target_r.window.reference_radec,\n",
                 ")\n",
                 "\n",
                 "# The third image is a GALEX NUV band image. This image has a pixelscale of 1.5 arcsec/pixel and is 90 pixels across\n",
                 "lnuvimg = fits.open(\n",
                 "    \"https://www.legacysurvey.org/viewer/fits-cutout?ra=187.3119&dec=12.9783&size=90&layer=galex&pixscale=1.5&bands=n\"\n",
                 ")\n",
                 "target_NUV = ap.image.Target_Image(\n",
                 "    data=np.array(lnuvimg[0].data, dtype=np.float64),\n",
                 "    zeropoint=20.08,\n",
-                "    variance=np.ones((90, 90)) * 0.0007**2,\n",
+                "    variance=\"auto\",\n",
                 "    psf=ap.utils.initialize.gaussian_psf(5.4 / 2.355, 21, 1.5),\n",
                 "    wcs=WCS(lnuvimg[0].header),\n",
                 "    reference_radec=target_r.window.reference_radec,\n",
                 ")\n",
                 "\n",
                 "fig1, ax1 = plt.subplots(1, 3, figsize=(18, 6))\n",
                 "ap.plots.target_image(fig1, ax1[0], target_r, flipx=True)\n",
@@ -198,15 +196,15 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "# We can also plot the residual images. As can be seen, the galaxy is fit in all three bands simultaneously\n",
                 "# with the majority of the light removed in all bands. A residual can be seen in the r band. This is likely\n",
                 "# due to there being more structure in the r-band than just a sersic. The W1 and NUV bands look excellent though\n",
                 "fig1, ax1 = plt.subplots(1, 3, figsize=(18, 6))\n",
-                "ap.plots.residual_image(fig1, ax1, model_full, flipx=True)\n",
+                "ap.plots.residual_image(fig1, ax1, model_full, flipx=True, normalize_residuals=True)\n",
                 "ax1[0].set_title(\"r-band residual image\")\n",
                 "ax1[1].set_title(\"W1-band residual image\")\n",
                 "ax1[2].set_title(\"NUV-band residual image\")\n",
                 "plt.show()"
             ]
         },
         {
@@ -244,46 +242,44 @@
                 "ref_loc = rwcs.pixel_to_world(0, 0)\n",
                 "target_r.header.reference_radec = (ref_loc.ra.deg, ref_loc.dec.deg)\n",
                 "\n",
                 "# Now we make our targets\n",
                 "target_r = ap.image.Target_Image(\n",
                 "    data=rimg_data,\n",
                 "    zeropoint=22.5,\n",
-                "    variance=np.ones((rsize, rsize))\n",
-                "    * 0.008\n",
-                "    ** 2,  # note that the variance is important to ensure all images are compared with proper statistical weight. Here we just use the IQR^2 of the pixel values as the variance, for science data one would use a more accurate variance value\n",
+                "    variance=\"auto\",  # Note that the variance is important to ensure all images are compared with proper statistical weight. Use better estimate than auto for science!\n",
                 "    psf=ap.utils.initialize.gaussian_psf(\n",
                 "        1.12 / 2.355, 51, 0.262\n",
                 "    ),  # we construct a basic gaussian psf for each image by giving the simga (arcsec), image width (pixels), and pixelscale (arcsec/pixel)\n",
                 "    wcs=rwcs,\n",
                 ")\n",
                 "\n",
                 "# The second image is a unWISE W1 band image. This image has a pixelscale of 2.75 arcsec/pixel\n",
                 "wsize = int(rsize * 0.262 / 2.75)\n",
                 "w1img = fits.open(\n",
                 "    f\"https://www.legacysurvey.org/viewer/fits-cutout?ra={RA}&dec={DEC}&size={wsize}&layer=unwise-neo7&pixscale=2.75&bands=1\"\n",
                 ")\n",
                 "target_W1 = ap.image.Target_Image(\n",
                 "    data=np.array(w1img[0].data, dtype=np.float64),\n",
                 "    zeropoint=25.199,\n",
-                "    variance=np.ones((wsize, wsize)) * 4.9**2,\n",
+                "    variance=\"auto\",\n",
                 "    psf=ap.utils.initialize.gaussian_psf(6.1 / 2.355, 21, 2.75),\n",
                 "    wcs=WCS(w1img[0].header),\n",
                 "    reference_radec=target_r.window.reference_radec,\n",
                 ")\n",
                 "\n",
                 "# The third image is a GALEX NUV band image. This image has a pixelscale of 1.5 arcsec/pixel\n",
                 "gsize = int(rsize * 0.262 / 1.5)\n",
                 "nuvimg = fits.open(\n",
                 "    f\"https://www.legacysurvey.org/viewer/fits-cutout?ra={RA}&dec={DEC}&size={gsize}&layer=galex&pixscale=1.5&bands=n\"\n",
                 ")\n",
                 "target_NUV = ap.image.Target_Image(\n",
                 "    data=np.array(nuvimg[0].data, dtype=np.float64),\n",
                 "    zeropoint=20.08,\n",
-                "    variance=np.ones((gsize, gsize)) * 0.0007**2,\n",
+                "    variance=\"auto\",\n",
                 "    psf=ap.utils.initialize.gaussian_psf(5.4 / 2.355, 21, 1.5),\n",
                 "    wcs=WCS(nuvimg[0].header),\n",
                 "    reference_radec=target_r.window.reference_radec,\n",
                 ")\n",
                 "target_full = ap.image.Target_Image_List((target_r, target_W1, target_NUV))\n",
                 "\n",
                 "fig1, ax1 = plt.subplots(1, 3, figsize=(18, 6))\n",
@@ -447,15 +443,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "fig, ax = plt.subplots(1, 3, figsize=(18, 6))\n",
-                "ap.plots.residual_image(fig, ax, MODEL, flipx=True)\n",
+                "ap.plots.residual_image(fig, ax, MODEL, flipx=True, normalize_residuals=True)\n",
                 "ax[0].set_title(\"r-band residual image\")\n",
                 "ax[1].set_title(\"W1-band residual image\")\n",
                 "ax[2].set_title(\"NUV-band residual image\")\n",
                 "plt.show()"
             ]
         },
         {
```

### Comparing `astrophot-0.16.2/docs/source/tutorials/ModelZoo.ipynb` & `astrophot-0.16.3/docs/source/tutorials/ModelZoo.ipynb`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/media/AP_logo.png` & `astrophot-0.16.3/media/AP_logo.png`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/media/AP_logo_white.png` & `astrophot-0.16.3/media/AP_logo_white.png`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/media/AstroPhotModelOrgchart.png` & `astrophot-0.16.3/media/AstroPhotModelOrgchart.png`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/media/groupjointmodels.png` & `astrophot-0.16.3/media/groupjointmodels.png`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/tests/test_fit.py` & `astrophot-0.16.3/tests/test_fit.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/tests/test_group_models.py` & `astrophot-0.16.3/tests/test_group_models.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/tests/test_image.py` & `astrophot-0.16.3/tests/test_image.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import unittest
 from astrophot import image
 import astrophot as ap
 import torch
 import numpy as np
 
-from utils import get_astropy_wcs
+from utils import get_astropy_wcs, make_basic_sersic
 
 ######################################################################
 # Image Objects
 ######################################################################
 
 
 class TestImage(unittest.TestCase):
@@ -435,14 +435,15 @@
         new_image.psf = None
         self.assertFalse(new_image.has_psf, "target image update to no variance")
 
     def test_reduce(self):
         new_image = image.Target_Image(
             data=torch.ones((30, 36)),
             psf=torch.ones((9, 9)),
+            variance="auto",
             pixelscale=1.0,
             zeropoint=1.0,
             origin=torch.zeros(2) + 0.1,
         )
         smaller_image = new_image.reduce(3)
         self.assertEqual(smaller_image.data[0][0], 9, "reduction should sum flux")
         self.assertEqual(
@@ -456,15 +457,15 @@
             (3, 3),
             "reduction should decrease psf image size",
         )
 
     def test_target_save_load(self):
         new_image = image.Target_Image(
             data=torch.ones((16, 32)),
-            variance=torch.ones((16, 32)),
+            variance="auto",
             mask=torch.zeros((16, 32)),
             psf=torch.ones((9, 9)),
             pixelscale=1.0,
             zeropoint=1.0,
             origin=torch.zeros(2) + 0.1,
         )
 
@@ -477,14 +478,18 @@
             "Loaded image should have same variance",
         )
         self.assertTrue(
             torch.all(new_image.psf.data == loaded_image.psf.data),
             "Loaded image should have same psf",
         )
 
+    def test_auto_var(self):
+        target = make_basic_sersic()
+        target.variance = "auto"
+
     def test_target_errors(self):
         new_image = image.Target_Image(
             data=torch.ones((16, 32)),
             pixelscale=1.0,
             zeropoint=1.0,
             origin=torch.zeros(2) + 0.1,
         )
```

### Comparing `astrophot-0.16.2/tests/test_image_header.py` & `astrophot-0.16.3/tests/test_image_header.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/tests/test_image_list.py` & `astrophot-0.16.3/tests/test_image_list.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/tests/test_model.py` & `astrophot-0.16.3/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/tests/test_parameter.py` & `astrophot-0.16.3/tests/test_parameter.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/tests/test_plots.py` & `astrophot-0.16.3/tests/test_plots.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/tests/test_psfmodel.py` & `astrophot-0.16.3/tests/test_psfmodel.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/tests/test_utils.py` & `astrophot-0.16.3/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/tests/test_wcs.py` & `astrophot-0.16.3/tests/test_wcs.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/tests/test_window.py` & `astrophot-0.16.3/tests/test_window.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/tests/test_window_list.py` & `astrophot-0.16.3/tests/test_window_list.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/tests/utils.py` & `astrophot-0.16.3/tests/utils.py`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/LICENSE` & `astrophot-0.16.3/LICENSE`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/README.md` & `astrophot-0.16.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -48,7 +48,11 @@
 author, [Connor Stone](https://connorjstone.com/), for any questions not
 answered by the documentation or tutorials.
 
 ## Credit / Citation
 
 If you use AstroPhot in your research, please follow the
 [citation instructions here](https://autostronomy.github.io/AstroPhot/citation.html).
+
+## Thanks to our contributors!
+
+[![Contributors](https://contrib.rocks/image?repo=Autostronomy/AstroPhot)](https://github.com/Autostronomy/AstroPhot/graphs/contributors)
```

### Comparing `astrophot-0.16.2/pyproject.toml` & `astrophot-0.16.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `astrophot-0.16.2/PKG-INFO` & `astrophot-0.16.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: astrophot
-Version: 0.16.2
+Version: 0.16.3
 Summary: A fast, flexible, automated, and differentiable astronomical image 2D forward modelling tool for precise parallel multi-wavelength photometry.
 Project-URL: Homepage, https://autostronomy.github.io/AstroPhot/
 Project-URL: Documentation, https://autostronomy.github.io/AstroPhot/
 Project-URL: Repository, https://github.com/Autostronomy/AstroPhot
 Project-URL: Issues, https://github.com/Autostronomy/AstroPhot/issues
 Author-email: Connor Stone <connorstone628@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
@@ -751,7 +751,11 @@
 author, [Connor Stone](https://connorjstone.com/), for any questions not
 answered by the documentation or tutorials.
 
 ## Credit / Citation
 
 If you use AstroPhot in your research, please follow the
 [citation instructions here](https://autostronomy.github.io/AstroPhot/citation.html).
+
+## Thanks to our contributors!
+
+[![Contributors](https://contrib.rocks/image?repo=Autostronomy/AstroPhot)](https://github.com/Autostronomy/AstroPhot/graphs/contributors)
```

