# Comparing `tmp/openst-0.0.8.tar.gz` & `tmp/openst-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openst-0.0.8.tar", max compression
+gzip compressed data, was "openst-0.0.9.tar", max compression
```

## Comparing `openst-0.0.8.tar` & `openst-0.0.9.tar`

### file list

```diff
@@ -1,60 +1,60 @@
--rw-r--r--   0        0        0      896 2024-02-14 16:40:20.599326 openst-0.0.8/LICENSE
--rw-r--r--   0        0        0     4235 2024-04-15 10:07:14.979891 openst-0.0.8/README.md
--rw-r--r--   0        0        0       21 2024-02-14 16:40:22.603322 openst-0.0.8/openst/__init__.py
--rw-r--r--   0        0        0      231 2024-04-11 08:32:57.910641 openst-0.0.8/openst/__main__.py
--rw-r--r--   0        0        0        0 2024-02-14 16:40:22.611322 openst-0.0.8/openst/alignment/__init__.py
--rw-r--r--   0        0        0     5878 2024-04-15 11:40:37.200872 openst-0.0.8/openst/alignment/apply_transform.py
--rw-r--r--   0        0        0    11893 2024-02-14 16:40:22.619322 openst-0.0.8/openst/alignment/feature_matching.py
--rw-r--r--   0        0        0     3628 2024-02-14 16:40:22.623322 openst-0.0.8/openst/alignment/fiducial_detection.py
--rw-r--r--   0        0        0    51224 2024-04-15 10:07:08.227908 openst-0.0.8/openst/alignment/manual_pairwise_aligner.py
--rw-r--r--   0        0        0    25213 2024-04-15 14:18:10.314354 openst-0.0.8/openst/alignment/pairwise_aligner.py
--rw-r--r--   0        0        0     5505 2024-04-15 11:42:56.504675 openst-0.0.8/openst/alignment/transcript_assign.py
--rw-r--r--   0        0        0      798 2024-04-15 10:07:08.231908 openst-0.0.8/openst/alignment/transformation.py
--rw-r--r--   0        0        0    47613 2024-04-15 14:45:02.598230 openst-0.0.8/openst/cli.py
--rw-r--r--   0        0        0        0 2024-02-14 16:40:22.655321 openst-0.0.8/openst/metadata/__init__.py
--rw-r--r--   0        0        0        0 2024-02-14 16:40:22.659321 openst-0.0.8/openst/metadata/classes/__init__.py
--rw-r--r--   0        0        0     2906 2024-02-14 16:40:22.663322 openst-0.0.8/openst/metadata/classes/base.py
--rw-r--r--   0        0        0     3406 2024-04-15 13:57:54.682361 openst-0.0.8/openst/metadata/classes/pairwise_alignment.py
--rw-r--r--   0        0        0     1798 2024-02-14 16:40:22.679321 openst-0.0.8/openst/metadata/classes/segmentation.py
--rw-r--r--   0        0        0     3787 2024-02-14 16:40:22.683321 openst-0.0.8/openst/metadata/example_json.json
--rw-r--r--   0        0        0     1450 2024-04-12 13:55:27.459067 openst-0.0.8/openst/metadata/report.py
--rw-r--r--   0        0        0  1187390 2024-02-14 16:40:22.715321 openst-0.0.8/openst/metadata/templates/pairwise_alignment.html
--rw-r--r--   0        0        0     1745 2024-02-14 16:40:22.723321 openst-0.0.8/openst/preprocessing/CUT/README.md
--rw-r--r--   0        0        0        0 2024-02-14 16:40:22.723321 openst-0.0.8/openst/preprocessing/CUT/__init__.py
--rw-r--r--   0        0        0     3072 2024-02-14 16:40:22.731321 openst-0.0.8/openst/preprocessing/CUT/models/__init__.py
--rw-r--r--   0        0        0    11223 2024-02-14 16:40:22.735321 openst-0.0.8/openst/preprocessing/CUT/models/base_model.py
--rw-r--r--   0        0        0    10228 2024-02-14 16:40:22.739321 openst-0.0.8/openst/preprocessing/CUT/models/cut_model.py
--rw-r--r--   0        0        0    60639 2024-02-14 16:40:22.747321 openst-0.0.8/openst/preprocessing/CUT/models/networks.py
--rw-r--r--   0        0        0     5953 2024-02-14 16:40:22.751321 openst-0.0.8/openst/preprocessing/CUT/models/template_model.py
--rw-r--r--   0        0        0      136 2024-02-14 16:40:22.755321 openst-0.0.8/openst/preprocessing/CUT/options/__init__.py
--rw-r--r--   0        0        0     9720 2024-02-14 16:40:22.763321 openst-0.0.8/openst/preprocessing/CUT/options/base_options.py
--rw-r--r--   0        0        0      975 2024-02-14 16:40:22.767321 openst-0.0.8/openst/preprocessing/CUT/options/test_options.py
--rw-r--r--   0        0        0      102 2024-02-14 16:40:22.775321 openst-0.0.8/openst/preprocessing/CUT/util/__init__.py
--rw-r--r--   0        0        0     2226 2024-02-14 16:40:22.779321 openst-0.0.8/openst/preprocessing/CUT/util/image_pool.py
--rw-r--r--   0        0        0     5135 2024-02-14 16:40:22.783321 openst-0.0.8/openst/preprocessing/CUT/util/util.py
--rw-r--r--   0        0        0        0 2024-02-14 16:40:22.787321 openst-0.0.8/openst/preprocessing/__init__.py
--rw-r--r--   0        0        0     4005 2024-04-12 13:55:27.459067 openst-0.0.8/openst/preprocessing/barcode_preprocessing.py
--rw-r--r--   0        0        0     3027 2024-04-13 10:23:49.385865 openst-0.0.8/openst/preprocessing/image_preprocess.py
--rw-r--r--   0        0        0     4607 2024-04-15 10:07:08.231908 openst-0.0.8/openst/preprocessing/image_stitch.py
--rw-r--r--   0        0        0      690 2024-02-14 16:40:22.811321 openst-0.0.8/openst/preprocessing/imagej_macros/keyence_stitch.ijm
--rw-r--r--   0        0        0      833 2024-04-12 13:55:27.459067 openst-0.0.8/openst/preprocessing/merge_modalities.py
--rw-r--r--   0        0        0     8996 2024-04-15 10:07:08.235908 openst-0.0.8/openst/preprocessing/spatial_stitch.py
--rw-r--r--   0        0        0        0 2024-02-14 16:40:22.819321 openst-0.0.8/openst/segmentation/__init__.py
--rw-r--r--   0        0        0    14684 2024-04-12 13:55:27.463067 openst-0.0.8/openst/segmentation/segment.py
--rw-r--r--   0        0        0     3842 2024-04-15 10:07:08.235908 openst-0.0.8/openst/segmentation/segment_merge.py
--rw-r--r--   0        0        0        0 2024-02-14 16:40:22.827321 openst-0.0.8/openst/threed/__init__.py
--rw-r--r--   0        0        0     9811 2024-04-12 13:55:27.463067 openst-0.0.8/openst/threed/from_3d_registration.py
--rw-r--r--   0        0        0     2500 2024-04-12 13:55:27.467067 openst-0.0.8/openst/threed/to_3d_registration.py
--rw-r--r--   0        0        0        0 2024-02-14 16:40:22.843321 openst-0.0.8/openst/utils/__init__.py
--rw-r--r--   0        0        0     8010 2024-04-15 13:56:11.270437 openst-0.0.8/openst/utils/file.py
--rw-r--r--   0        0        0    13953 2024-04-15 13:46:46.786692 openst-0.0.8/openst/utils/from_spacemake.py
--rw-r--r--   0        0        0     9651 2024-04-15 10:07:08.235908 openst-0.0.8/openst/utils/pimage.py
--rw-r--r--   0        0        0     3018 2024-02-14 16:40:22.859321 openst-0.0.8/openst/utils/points.py
--rw-r--r--   0        0        0     2419 2024-04-15 10:07:08.239908 openst-0.0.8/openst/utils/preview.py
--rw-r--r--   0        0        0    10068 2024-04-15 13:44:23.802687 openst-0.0.8/openst/utils/pseudoimage.py
--rw-r--r--   0        0        0        0 2024-02-14 16:40:22.867321 openst-0.0.8/openst/utils/scanpy/__init__.py
--rw-r--r--   0        0        0       37 2024-02-14 16:40:22.875321 openst-0.0.8/openst/utils/scanpy/pp/__init__.py
--rw-r--r--   0        0        0    10779 2024-02-14 16:40:22.879321 openst-0.0.8/openst/utils/scanpy/pp/_qc.py
--rw-r--r--   0        0        0     3715 2024-02-14 16:40:22.883321 openst-0.0.8/openst/utils/spacemake.py
--rw-r--r--   0        0        0     1985 2024-04-15 13:44:33.982689 openst-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     6373 1970-01-01 00:00:00.000000 openst-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      896 2024-02-14 16:40:20.599326 openst-0.0.9/LICENSE
+-rw-r--r--   0        0        0     4235 2024-04-15 10:07:14.979891 openst-0.0.9/README.md
+-rw-r--r--   0        0        0       21 2024-02-14 16:40:22.603322 openst-0.0.9/openst/__init__.py
+-rw-r--r--   0        0        0      231 2024-04-11 08:32:57.910641 openst-0.0.9/openst/__main__.py
+-rw-r--r--   0        0        0        0 2024-02-14 16:40:22.611322 openst-0.0.9/openst/alignment/__init__.py
+-rw-r--r--   0        0        0     5878 2024-04-15 14:54:16.746512 openst-0.0.9/openst/alignment/apply_transform.py
+-rw-r--r--   0        0        0    11893 2024-02-14 16:40:22.619322 openst-0.0.9/openst/alignment/feature_matching.py
+-rw-r--r--   0        0        0     3628 2024-02-14 16:40:22.623322 openst-0.0.9/openst/alignment/fiducial_detection.py
+-rw-r--r--   0        0        0    51224 2024-04-15 14:54:16.750512 openst-0.0.9/openst/alignment/manual_pairwise_aligner.py
+-rw-r--r--   0        0        0    25638 2024-04-16 05:22:16.053579 openst-0.0.9/openst/alignment/pairwise_aligner.py
+-rw-r--r--   0        0        0     5507 2024-04-16 05:18:17.738134 openst-0.0.9/openst/alignment/transcript_assign.py
+-rw-r--r--   0        0        0      798 2024-04-15 14:54:16.758512 openst-0.0.9/openst/alignment/transformation.py
+-rw-r--r--   0        0        0    47613 2024-04-15 14:54:16.762512 openst-0.0.9/openst/cli.py
+-rw-r--r--   0        0        0        0 2024-02-14 16:40:22.655321 openst-0.0.9/openst/metadata/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-14 16:40:22.659321 openst-0.0.9/openst/metadata/classes/__init__.py
+-rw-r--r--   0        0        0     2906 2024-02-14 16:40:22.663322 openst-0.0.9/openst/metadata/classes/base.py
+-rw-r--r--   0        0        0     3406 2024-04-15 14:54:16.762512 openst-0.0.9/openst/metadata/classes/pairwise_alignment.py
+-rw-r--r--   0        0        0     1798 2024-02-14 16:40:22.679321 openst-0.0.9/openst/metadata/classes/segmentation.py
+-rw-r--r--   0        0        0     3787 2024-02-14 16:40:22.683321 openst-0.0.9/openst/metadata/example_json.json
+-rw-r--r--   0        0        0     1450 2024-04-12 13:55:27.459067 openst-0.0.9/openst/metadata/report.py
+-rw-r--r--   0        0        0  1187390 2024-02-14 16:40:22.715321 openst-0.0.9/openst/metadata/templates/pairwise_alignment.html
+-rw-r--r--   0        0        0     1745 2024-02-14 16:40:22.723321 openst-0.0.9/openst/preprocessing/CUT/README.md
+-rw-r--r--   0        0        0        0 2024-02-14 16:40:22.723321 openst-0.0.9/openst/preprocessing/CUT/__init__.py
+-rw-r--r--   0        0        0     3072 2024-02-14 16:40:22.731321 openst-0.0.9/openst/preprocessing/CUT/models/__init__.py
+-rw-r--r--   0        0        0    11223 2024-02-14 16:40:22.735321 openst-0.0.9/openst/preprocessing/CUT/models/base_model.py
+-rw-r--r--   0        0        0    10228 2024-02-14 16:40:22.739321 openst-0.0.9/openst/preprocessing/CUT/models/cut_model.py
+-rw-r--r--   0        0        0    60639 2024-02-14 16:40:22.747321 openst-0.0.9/openst/preprocessing/CUT/models/networks.py
+-rw-r--r--   0        0        0     5953 2024-02-14 16:40:22.751321 openst-0.0.9/openst/preprocessing/CUT/models/template_model.py
+-rw-r--r--   0        0        0      136 2024-02-14 16:40:22.755321 openst-0.0.9/openst/preprocessing/CUT/options/__init__.py
+-rw-r--r--   0        0        0     9720 2024-02-14 16:40:22.763321 openst-0.0.9/openst/preprocessing/CUT/options/base_options.py
+-rw-r--r--   0        0        0      975 2024-02-14 16:40:22.767321 openst-0.0.9/openst/preprocessing/CUT/options/test_options.py
+-rw-r--r--   0        0        0      102 2024-02-14 16:40:22.775321 openst-0.0.9/openst/preprocessing/CUT/util/__init__.py
+-rw-r--r--   0        0        0     2226 2024-02-14 16:40:22.779321 openst-0.0.9/openst/preprocessing/CUT/util/image_pool.py
+-rw-r--r--   0        0        0     5135 2024-02-14 16:40:22.783321 openst-0.0.9/openst/preprocessing/CUT/util/util.py
+-rw-r--r--   0        0        0        0 2024-02-14 16:40:22.787321 openst-0.0.9/openst/preprocessing/__init__.py
+-rw-r--r--   0        0        0     4005 2024-04-12 13:55:27.459067 openst-0.0.9/openst/preprocessing/barcode_preprocessing.py
+-rw-r--r--   0        0        0     2194 2024-04-15 14:53:45.590507 openst-0.0.9/openst/preprocessing/image_preprocess.py
+-rw-r--r--   0        0        0     4607 2024-04-15 14:54:16.766512 openst-0.0.9/openst/preprocessing/image_stitch.py
+-rw-r--r--   0        0        0      690 2024-02-14 16:40:22.811321 openst-0.0.9/openst/preprocessing/imagej_macros/keyence_stitch.ijm
+-rw-r--r--   0        0        0      833 2024-04-12 13:55:27.459067 openst-0.0.9/openst/preprocessing/merge_modalities.py
+-rw-r--r--   0        0        0     8996 2024-04-15 14:54:16.766512 openst-0.0.9/openst/preprocessing/spatial_stitch.py
+-rw-r--r--   0        0        0        0 2024-02-14 16:40:22.819321 openst-0.0.9/openst/segmentation/__init__.py
+-rw-r--r--   0        0        0    14684 2024-04-12 13:55:27.463067 openst-0.0.9/openst/segmentation/segment.py
+-rw-r--r--   0        0        0     3842 2024-04-15 14:54:16.770512 openst-0.0.9/openst/segmentation/segment_merge.py
+-rw-r--r--   0        0        0        0 2024-02-14 16:40:22.827321 openst-0.0.9/openst/threed/__init__.py
+-rw-r--r--   0        0        0     9811 2024-04-12 13:55:27.463067 openst-0.0.9/openst/threed/from_3d_registration.py
+-rw-r--r--   0        0        0     2500 2024-04-12 13:55:27.467067 openst-0.0.9/openst/threed/to_3d_registration.py
+-rw-r--r--   0        0        0        0 2024-02-14 16:40:22.843321 openst-0.0.9/openst/utils/__init__.py
+-rw-r--r--   0        0        0     8010 2024-04-15 14:54:16.778512 openst-0.0.9/openst/utils/file.py
+-rw-r--r--   0        0        0    13953 2024-04-15 14:54:16.778512 openst-0.0.9/openst/utils/from_spacemake.py
+-rw-r--r--   0        0        0     9651 2024-04-15 14:54:16.782512 openst-0.0.9/openst/utils/pimage.py
+-rw-r--r--   0        0        0     3018 2024-02-14 16:40:22.859321 openst-0.0.9/openst/utils/points.py
+-rw-r--r--   0        0        0     2419 2024-04-15 14:54:16.786512 openst-0.0.9/openst/utils/preview.py
+-rw-r--r--   0        0        0    10068 2024-04-15 14:54:16.786512 openst-0.0.9/openst/utils/pseudoimage.py
+-rw-r--r--   0        0        0        0 2024-02-14 16:40:22.867321 openst-0.0.9/openst/utils/scanpy/__init__.py
+-rw-r--r--   0        0        0       37 2024-02-14 16:40:22.875321 openst-0.0.9/openst/utils/scanpy/pp/__init__.py
+-rw-r--r--   0        0        0    10779 2024-02-14 16:40:22.879321 openst-0.0.9/openst/utils/scanpy/pp/_qc.py
+-rw-r--r--   0        0        0     3737 2024-04-16 05:17:10.030292 openst-0.0.9/openst/utils/spacemake.py
+-rw-r--r--   0        0        0     1985 2024-04-16 05:07:27.559664 openst-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     6373 1970-01-01 00:00:00.000000 openst-0.0.9/PKG-INFO
```

### Comparing `openst-0.0.8/LICENSE` & `openst-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `openst-0.0.8/README.md` & `openst-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `openst-0.0.8/openst/alignment/apply_transform.py` & `openst-0.0.9/openst/alignment/apply_transform.py`

 * *Files identical despite different names*

### Comparing `openst-0.0.8/openst/alignment/feature_matching.py` & `openst-0.0.9/openst/alignment/feature_matching.py`

 * *Files identical despite different names*

### Comparing `openst-0.0.8/openst/alignment/fiducial_detection.py` & `openst-0.0.9/openst/alignment/fiducial_detection.py`

 * *Files identical despite different names*

### Comparing `openst-0.0.8/openst/alignment/manual_pairwise_aligner.py` & `openst-0.0.9/openst/alignment/manual_pairwise_aligner.py`

 * *Files identical despite different names*

### Comparing `openst-0.0.8/openst/alignment/pairwise_aligner.py` & `openst-0.0.9/openst/alignment/pairwise_aligner.py`

 * *Files 1% similar despite different names*

```diff
@@ -171,34 +171,41 @@
 
 
 def prepare_pseudoimage_for_feature_matching(
     image: np.ndarray,
     invert: bool = True,
     gaussian_blur: float = 0,
     flip: list = [1, 1],
+    rotation: float = 0,
 ) -> np.ndarray:
     """
     Prepare an image for feature matching by applying optional transformations.
 
     Args:
         image (np.ndarray): Input image to be prepared.
         invert (bool, options): The image values will be inverted (white/black background).
         gaussian_blur (float, optional): Standard deviation for Gaussian blurring. Default is 0 (no blur).
         flip (list, optional): List indicating whether to flip the image along the x and y axes. Default is [1, 1].
+        rotation (float, optional): float indicating the rotation angle in degrees in counter-clockwise direction.
 
     Returns:
         list: A list containing the prepared image after applying transformations.
             - The list contains a single element, which is the processed image.
 
     Notes:
         - This function applies optional Gaussian blurring and flipping to the input image.
         - The 'gaussian_blur' parameter controls the amount of blurring applied to the image.
         - The 'flip' parameter specifies flipping along the x and y axes using a list of factors [x_flip, y_flip].
     """
+    # Check if flip argument is a list with two elements
+    if not isinstance(flip, list) or len(flip) != 2:
+        raise ValueError("The 'flip' argument should be a list with two elements [x_flip, y_flip].")
+
     _image = image.copy() if not invert else ((-image) - ((-image).min()))
+    _image = transform_image(_image, flip, crop=None, rotation=rotation)
     return [gaussian(equalize_adapthist(_image), gaussian_blur)[:: flip[0], :: flip[1]]]
 
 
 def run_registration(
     in_coords: np.ndarray,
     total_counts: np.ndarray,
     tile_id: np.ndarray,
```

### Comparing `openst-0.0.8/openst/alignment/transcript_assign.py` & `openst-0.0.9/openst/alignment/transcript_assign.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
     return adata_by_cell
 
 
 def subset_adata_to_mask(mask, adata, spatial_key: str = 'spatial'):
     # Subset adata to the valid coordinates from the mask
     adata = adata[(adata.obsm[spatial_key][:, 0] >= 0) & 
-                  (adata.obsm[spatial_key][:, 1] <= 0)
+                  (adata.obsm[spatial_key][:, 1] >= 0) &
                   (adata.obsm[spatial_key][:, 0] <= mask.shape[0]) & 
                   (adata.obsm[spatial_key][:, 1] <= mask.shape[1])].copy()
 
     # Subset the labels to those in the mask
     labels = mask[adata.obsm[spatial_key][:, 0].astype(int), adata.obsm[spatial_key][:, 1].astype(int)]
 
     # Assign label as cell_ID
```

### Comparing `openst-0.0.8/openst/alignment/transformation.py` & `openst-0.0.9/openst/alignment/transformation.py`

 * *Files identical despite different names*

### Comparing `openst-0.0.8/openst/cli.py` & `openst-0.0.9/openst/cli.py`

 * *Files identical despite different names*

### Comparing `openst-0.0.8/openst/metadata/classes/base.py` & `openst-0.0.9/openst/metadata/classes/base.py`

 * *Files identical despite different names*

### Comparing `openst-0.0.8/openst/metadata/classes/pairwise_alignment.py` & `openst-0.0.9/openst/metadata/classes/pairwise_alignment.py`

 * *Files identical despite different names*

### Comparing `openst-0.0.8/openst/metadata/classes/segmentation.py` & `openst-0.0.9/openst/metadata/classes/segmentation.py`

 * *Files identical despite different names*

### Comparing `openst-0.0.8/openst/metadata/example_json.json` & `openst-0.0.9/openst/metadata/example_json.json`

 * *Files identical despite different names*

### Comparing `openst-0.0.8/openst/metadata/report.py` & `openst-0.0.9/openst/metadata/report.py`

 * *Files identical despite different names*

### Comparing `openst-0.0.8/openst/metadata/templates/pairwise_alignment.html` & `openst-0.0.9/openst/metadata/templates/pairwise_alignment.html`

 * *Files identical despite different names*

### Comparing `openst-0.0.8/openst/preprocessing/CUT/README.md` & `openst-0.0.9/openst/preprocessing/CUT/README.md`

 * *Files identical despite different names*

### Comparing `openst-0.0.8/openst/preprocessing/CUT/models/__init__.py` & `openst-0.0.9/openst/preprocessing/CUT/models/__init__.py`

 * *Files identical despite different names*

### Comparing `openst-0.0.8/openst/preprocessing/CUT/models/base_model.py` & `openst-0.0.9/openst/preprocessing/CUT/models/base_model.py`

 * *Files identical despite different names*

### Comparing `openst-0.0.8/openst/preprocessing/CUT/models/cut_model.py` & `openst-0.0.9/openst/preprocessing/CUT/models/cut_model.py`

 * *Files identical despite different names*

### Comparing `openst-0.0.8/openst/preprocessing/CUT/models/networks.py` & `openst-0.0.9/openst/preprocessing/CUT/models/networks.py`

 * *Files identical despite different names*

### Comparing `openst-0.0.8/openst/preprocessing/CUT/models/template_model.py` & `openst-0.0.9/openst/preprocessing/CUT/models/template_model.py`

 * *Files identical despite different names*

### Comparing `openst-0.0.8/openst/preprocessing/CUT/options/base_options.py` & `openst-0.0.9/openst/preprocessing/CUT/options/base_options.py`

 * *Files identical despite different names*

### Comparing `openst-0.0.8/openst/preprocessing/CUT/options/test_options.py` & `openst-0.0.9/openst/preprocessing/CUT/options/test_options.py`

 * *Files identical despite different names*

### Comparing `openst-0.0.8/openst/preprocessing/CUT/util/image_pool.py` & `openst-0.0.9/openst/preprocessing/CUT/util/image_pool.py`

 * *Files identical despite different names*

### Comparing `openst-0.0.8/openst/preprocessing/CUT/util/util.py` & `openst-0.0.9/openst/preprocessing/CUT/util/util.py`

 * *Files identical despite different names*

### Comparing `openst-0.0.8/openst/preprocessing/barcode_preprocessing.py` & `openst-0.0.9/openst/preprocessing/barcode_preprocessing.py`

 * *Files identical despite different names*

### Comparing `openst-0.0.8/openst/preprocessing/image_preprocess.py` & `openst-0.0.9/openst/preprocessing/image_preprocess.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,46 +1,14 @@
 import numpy as np
+import os
 
 from PIL import Image
 from tqdm import tqdm
 
-from torch.utils.data import DataLoader
-
-from openst.preprocessing.CUT.models import create_model
-from openst.preprocessing.CUT.options.test_options import TestOptions
-
-def create_dataset(opt):
-    data_loader = OpenSTDatasetDataLoader(opt)
-    dataset = data_loader.load_data()
-    return dataset
-
-class OpenSTDatasetDataLoader():
-    """Wrapper class of Dataset class that performs multi-threaded data loading"""
-
-    def __init__(self, image_tiles):
-        self.image_tiles = image_tiles
-        self.dataloader = DataLoader(
-            self.image_tiles,
-            batch_size=1,
-            shuffle=False,
-            num_workers=1,
-            drop_last=False,
-        )
-
-    def load_data(self):
-        return self
-
-    def __len__(self):
-        """Return the number of data in the dataset"""
-        return len(self.image_tiles)
-
-    def __iter__(self):
-        """Return a batch of data"""
-        for i, data in enumerate(self.dataloader):
-            yield data
+# from openst.preprocessing.CUT.models import create_model
 
 def _images_to_tiles(img):
     _img_shape = img.shape
     tiles = []
     for x in range(0, _img_shape[0]-args.tile_size_px, args.tile_size_px):
         for y in range(0, _img_shape[1]-args.tile_size_px, args.tile_size_px):
             tiles.append([x, y])
@@ -54,51 +22,49 @@
 
 def _tiles_to_images(tiles, imgs, dest_shape):
     img_restitch = np.zeros(dest_shape)
     for i, coord in tqdm(enumerate(tiles)):
         img_restitch[coord[0]:(coord[0]+args.tile_size_px), coord[1]:(coord[1]+args.tile_size_px)] = imgs[i] 
 
 
-def _image_preprocess(model, dataset):
-    model.data_dependent_initialize(dataset[0])
-    model.eval()
-    
-    output = []
-    for data in dataset:
+def _image_preprocess(imgs_tiles, model):
+    for i, data in enumerate(dataset):
+        if i == 0:
+            model.data_dependent_initialize(data)
+            model.setup(opt)
+            model.parallelize()
+            if args.eval:
+                model.eval()
         data = {'A': None, 'B': None, 'A_paths': None, 'B_paths': None}
-        model.set_input(data)
-        model.test()
-        output += [model.get_current_visuals()]
-    
-    return output
+        model.set_input(data)  # unpack data from data loader
+        model.test()           # run inference
+        visuals = model.get_current_visuals()  # get image results
 
 
-def _run_image_preprocess(args):
+def _run_image_preprocess():
+    # loading arguments
+    args = parser.parse_args()
+
     Image.MAX_IMAGE_PIXELS = 933120000
 
     # Load image and get shape
-    # TODO: load from h5 file, or load from lazy object
     img = np.array(Image.open(args.input_img))
     _img_shape = img.shape
 
     tiles, imgs_tiles = _images_to_tiles(img)
 
     opt = TestOptions().parse()
     opt.num_threads = 1
     opt.batch_size = 1
     opt.serial_batches = True
     opt.no_flip = True
     opt.load_size = args.tile_size_px
 
     model = create_model(opt)
-    model.setup(opt)
-    model.parallelize()
-
-    dataset = create_dataset(imgs_tiles)
-    imgs_tiles_processed = _image_preprocess(model, dataset)
+    imgs_tiles_processed = _image_preprocess(imgs_tiles)
 
     img_restitch = _tiles_to_images(tiles, imgs_tiles_processed, _img_shape)
     Image.fromarray(img_restitch.astype(np.uint8)).save(args.output_img)
 
 if __name__ == "__main__":
     from openst.cli import get_image_preprocess_parser
     args = get_image_preprocess_parser().parse_args()
```

### Comparing `openst-0.0.8/openst/preprocessing/image_stitch.py` & `openst-0.0.9/openst/preprocessing/image_stitch.py`

 * *Files identical despite different names*

### Comparing `openst-0.0.8/openst/preprocessing/imagej_macros/keyence_stitch.ijm` & `openst-0.0.9/openst/preprocessing/imagej_macros/keyence_stitch.ijm`

 * *Files identical despite different names*

### Comparing `openst-0.0.8/openst/preprocessing/merge_modalities.py` & `openst-0.0.9/openst/preprocessing/merge_modalities.py`

 * *Files identical despite different names*

### Comparing `openst-0.0.8/openst/preprocessing/spatial_stitch.py` & `openst-0.0.9/openst/preprocessing/spatial_stitch.py`

 * *Files identical despite different names*

### Comparing `openst-0.0.8/openst/segmentation/segment.py` & `openst-0.0.9/openst/segmentation/segment.py`

 * *Files identical despite different names*

### Comparing `openst-0.0.8/openst/segmentation/segment_merge.py` & `openst-0.0.9/openst/segmentation/segment_merge.py`

 * *Files identical despite different names*

### Comparing `openst-0.0.8/openst/threed/from_3d_registration.py` & `openst-0.0.9/openst/threed/from_3d_registration.py`

 * *Files identical despite different names*

### Comparing `openst-0.0.8/openst/threed/to_3d_registration.py` & `openst-0.0.9/openst/threed/to_3d_registration.py`

 * *Files identical despite different names*

### Comparing `openst-0.0.8/openst/utils/file.py` & `openst-0.0.9/openst/utils/file.py`

 * *Files identical despite different names*

### Comparing `openst-0.0.8/openst/utils/from_spacemake.py` & `openst-0.0.9/openst/utils/from_spacemake.py`

 * *Files identical despite different names*

### Comparing `openst-0.0.8/openst/utils/pimage.py` & `openst-0.0.9/openst/utils/pimage.py`

 * *Files identical despite different names*

### Comparing `openst-0.0.8/openst/utils/points.py` & `openst-0.0.9/openst/utils/points.py`

 * *Files identical despite different names*

### Comparing `openst-0.0.8/openst/utils/preview.py` & `openst-0.0.9/openst/utils/preview.py`

 * *Files identical despite different names*

### Comparing `openst-0.0.8/openst/utils/pseudoimage.py` & `openst-0.0.9/openst/utils/pseudoimage.py`

 * *Files identical despite different names*

### Comparing `openst-0.0.8/openst/utils/scanpy/pp/_qc.py` & `openst-0.0.9/openst/utils/scanpy/pp/_qc.py`

 * *Files identical despite different names*

### Comparing `openst-0.0.8/openst/utils/spacemake.py` & `openst-0.0.9/openst/utils/spacemake.py`

 * *Files 6% similar despite different names*

```diff
@@ -83,15 +83,15 @@
         n_reads=summarise_adata_obs_column(adata, "n_reads"),
     )
 
     adata_out.obs["n_joined"] = [len(x) for x in ix_array]
 
     mesh_bc_ilocs = np.arange(len(original_ilocs))[original_ilocs]
 
-    joined_dict = {i: mesh_bc_ilocs[x] for i, x in enumerate(ix_array)}
+    joined_dict = {i: mesh_bc_ilocs[ix_array[i].astype(int)] for i, x in enumerate(ix_array)}
 
     indices_joined_spatial_units = dok_matrix((len(joined_dict), len(adata.obs_names)), dtype=np.int8)
 
     for obs_name_aggregate, obs_name_to_aggregate in joined_dict.items():
         indices_joined_spatial_units[obs_name_aggregate, obs_name_to_aggregate] = 1
 
     indices_joined_spatial_units = indices_joined_spatial_units.tocsr()
```

### Comparing `openst-0.0.8/pyproject.toml` & `openst-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "openst"
-version = "0.0.8"
+version = "0.0.9"
 description = "The computational pipeline for the Open-ST method."
 license = "GPL-2.0"
 authors = [
     "Daniel León-Periñán <daniel.leonperinan@mdc-berlin.de>",
     "Nikolaos Karaiskos <nikolaos.karaiskos@mdc-berlin.de>",
 ]
 maintainers = [
```

### Comparing `openst-0.0.8/PKG-INFO` & `openst-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openst
-Version: 0.0.8
+Version: 0.0.9
 Summary: The computational pipeline for the Open-ST method.
 License: GPL-2.0
 Author: Daniel León-Periñán
 Author-email: daniel.leonperinan@mdc-berlin.de
 Maintainer: Daniel León-Periñán
 Maintainer-email: daniel.leonperinan@mdc-berlin.de
 Requires-Python: >=3.8,<4.0
```

