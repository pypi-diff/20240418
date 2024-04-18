# Comparing `tmp/sergio_rs-0.1.0.tar.gz` & `tmp/sergio_rs-0.2.0.tar.gz`

## Comparing `sergio_rs-0.1.0.tar` & `sergio_rs-0.2.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0      434 1970-01-01 00:00:00.000000 sergio_rs-0.1.0/Cargo.toml
--rw-r--r--   0     1001      127     4062 2024-04-16 11:38:46.000000 sergio_rs-0.1.0/.github/workflows/CI.yml
--rw-r--r--   0     1001      127      686 2024-04-16 11:38:46.000000 sergio_rs-0.1.0/.gitignore
--rw-r--r--   0     1001      127    49080 2024-04-16 11:38:46.000000 sergio_rs-0.1.0/Cargo.lock
--rw-r--r--   0     1001      127    35149 2024-04-16 11:38:46.000000 sergio_rs-0.1.0/LICENSE
--rw-r--r--   0     1001      127     4079 2024-04-16 11:38:46.000000 sergio_rs-0.1.0/README.md
--rw-r--r--   0     1001      127       39 2024-04-16 11:38:46.000000 sergio_rs-0.1.0/sergio_rs/__init__.py
--rw-r--r--   0     1001      127        0 2024-04-16 11:38:46.000000 sergio_rs-0.1.0/sergio_rs/py.typed
--rw-r--r--   0     1001      127     1310 2024-04-16 11:38:46.000000 sergio_rs-0.1.0/sergio_rs/sergio_rs.pyi
--rw-r--r--   0     1001      127     1970 2024-04-16 11:38:46.000000 sergio_rs-0.1.0/src/gene.rs
--rw-r--r--   0     1001      127    13449 2024-04-16 11:38:46.000000 sergio_rs-0.1.0/src/grn.rs
--rw-r--r--   0     1001      127      893 2024-04-16 11:38:46.000000 sergio_rs-0.1.0/src/interaction.rs
--rw-r--r--   0     1001      127      509 2024-04-16 11:38:46.000000 sergio_rs-0.1.0/src/lib.rs
--rw-r--r--   0     1001      127       13 2024-04-16 11:38:46.000000 sergio_rs-0.1.0/src/main.rs
--rw-r--r--   0     1001      127     2375 2024-04-16 11:38:46.000000 sergio_rs-0.1.0/src/mrs.rs
--rw-r--r--   0     1001      127     4886 2024-04-16 11:38:46.000000 sergio_rs-0.1.0/src/noise.rs
--rw-r--r--   0     1001      127     6710 2024-04-16 11:38:46.000000 sergio_rs-0.1.0/src/sim.rs
--rw-r--r--   0     1001      127      620 2024-04-16 11:38:46.000000 sergio_rs-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     4689 1970-01-01 00:00:00.000000 sergio_rs-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      453 1970-01-01 00:00:00.000000 sergio_rs-0.2.0/Cargo.toml
+-rw-r--r--   0     1001      127     4062 2024-04-18 08:14:53.000000 sergio_rs-0.2.0/.github/workflows/CI.yml
+-rw-r--r--   0     1001      127      686 2024-04-18 08:14:53.000000 sergio_rs-0.2.0/.gitignore
+-rw-r--r--   0     1001      127    49318 2024-04-18 08:14:53.000000 sergio_rs-0.2.0/Cargo.lock
+-rw-r--r--   0     1001      127    35149 2024-04-18 08:14:53.000000 sergio_rs-0.2.0/LICENSE
+-rw-r--r--   0     1001      127     4195 2024-04-18 08:14:53.000000 sergio_rs-0.2.0/README.md
+-rw-r--r--   0     1001      127       39 2024-04-18 08:14:53.000000 sergio_rs-0.2.0/sergio_rs/__init__.py
+-rw-r--r--   0     1001      127        0 2024-04-18 08:14:53.000000 sergio_rs-0.2.0/sergio_rs/py.typed
+-rw-r--r--   0     1001      127     1365 2024-04-18 08:14:53.000000 sergio_rs-0.2.0/sergio_rs/sergio_rs.pyi
+-rw-r--r--   0     1001      127     1970 2024-04-18 08:14:53.000000 sergio_rs-0.2.0/src/gene.rs
+-rw-r--r--   0     1001      127    13453 2024-04-18 08:14:53.000000 sergio_rs-0.2.0/src/grn.rs
+-rw-r--r--   0     1001      127      893 2024-04-18 08:14:53.000000 sergio_rs-0.2.0/src/interaction.rs
+-rw-r--r--   0     1001      127      509 2024-04-18 08:14:53.000000 sergio_rs-0.2.0/src/lib.rs
+-rw-r--r--   0     1001      127       13 2024-04-18 08:14:53.000000 sergio_rs-0.2.0/src/main.rs
+-rw-r--r--   0     1001      127     2488 2024-04-18 08:14:53.000000 sergio_rs-0.2.0/src/mrs.rs
+-rw-r--r--   0     1001      127     5403 2024-04-18 08:14:53.000000 sergio_rs-0.2.0/src/noise.rs
+-rw-r--r--   0     1001      127     6853 2024-04-18 08:14:53.000000 sergio_rs-0.2.0/src/sim.rs
+-rw-r--r--   0     1001      127      620 2024-04-18 08:14:53.000000 sergio_rs-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4805 1970-01-01 00:00:00.000000 sergio_rs-0.2.0/PKG-INFO
```

### Comparing `sergio_rs-0.1.0/.github/workflows/CI.yml` & `sergio_rs-0.2.0/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `sergio_rs-0.1.0/.gitignore` & `sergio_rs-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `sergio_rs-0.1.0/Cargo.lock` & `sergio_rs-0.2.0/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -1279,14 +1279,23 @@
 checksum = "32cb0b9bc82b0a0876c2dd994a7e7a2683d3e7390ca40e6886785ef0c7e3ee31"
 dependencies = [
  "num-traits",
  "rand",
 ]
 
 [[package]]
+name = "rand_pcg"
+version = "0.3.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "59cad018caf63deb318e5a4586d99a24424a364f40f1e5778c29aca23f4fc73e"
+dependencies = [
+ "rand_core",
+]
+
+[[package]]
 name = "raw-cpuid"
 version = "11.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9d86a7c4638d42c44551f4791a20e687dbb4c3de1f33c43dd71e355cd429def1"
 dependencies = [
  "bitflags 2.5.0",
 ]
@@ -1434,24 +1443,25 @@
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
 name = "sergio"
-version = "0.1.0"
+version = "0.2.0"
 dependencies = [
  "ndarray",
  "ndarray-rand",
  "ndarray-stats",
  "noisy_float",
  "numpy",
  "polars",
  "pyo3",
  "pyo3-polars",
+ "rand_pcg",
 ]
 
 [[package]]
 name = "simdutf8"
 version = "0.1.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f27f6278552951f1f2b8cf9da965d10969b2efdea95a6ec47987ab46edfe263a"
```

### Comparing `sergio_rs-0.1.0/LICENSE` & `sergio_rs-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sergio_rs-0.1.0/README.md` & `sergio_rs-0.2.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -57,52 +57,59 @@
 
 **_NOTE_**: Currently, only random MR profile generation is supported.
 
 ```py
 NUM_CELL_TYPES = 10
 LOW_RANGE = (0, 2)
 HIGH_RANGE = (2, 4)
+SEED = 42
 
 mr_profile = sergio_rs.MrProfile.from_random(
     grn,
     num_cell_types=NUM_CELL_TYPES,
     low_range=LOW_RANGE,
     high_range=HIGH_RANGE,
+    seed=SEED
 )
 ```
 
 ### Step 3: Simulate
 
 **_NOTE_**: Resulting gene expression data are in a Polars DataFrame rather than a Pandas one. This is mostly the same as SERGIO output, with the only difference being that Polars has no "index", so the "index" with gene names is just another column in the DataFrame called "Genes".
 
 ```py
 NUM_CELLS = 200
 NOISE_S = 1
 SAFETY_ITER = 150
 SCALE_ITER = 10
 DT = 0.01
+SEED = 42
 
 sim = sergio_rs.Sim(
     grn,
     num_cells=NUM_CELLS,
     noise_s=NOISE_S,
     safety_iter=SAFETY_ITER,
     scale_iter=SCALE_ITER,
     dt=DT,
+    seed=SEED,
 )
 data = sim.simulate(mr_profile)
 
 # Convert to 2D NumPy array
 data_np = data.drop("Genes").to_numpy()
 ```
 
 ### Step 4: Add technical noise
 
 ```py
-noisy_data = sergio_rs.add_technical_noise(data_np, sergio_rs.NoiseSetting.DS6)
+SEED = 42
+NOISE_PROFILE = sergio_rs.NoiseSetting.DS6
+
+noisy_data = sergio_rs.add_technical_noise(data_np, NOISE_PROFILE, seed=SEED)
 ```
 
 ### Step 5: Perturb
 
 ```py
 GENE_TO_PERTURB = "GENE0001"
 perturbed_grn, perturbed_mr_profile = grn.ko_perturbation(gene_name=GENE_TO_PERTURB, mr_profile=mr_profile)
@@ -110,10 +117,11 @@
 perturbed_sim = sergio_rs.Sim(
     perturbed_grn,
     num_cells=NUM_CELLS,
     noise_s=NOISE_S,
     safety_iter=SAFETY_ITER,
     scale_iter=SCALE_ITER,
     dt=DT,
+    seed=SEED,
 )
 perturbed_data = sim.simulate(perturbed_mr_profile)
 ```
```

### Comparing `sergio_rs-0.1.0/sergio_rs/sergio_rs.pyi` & `sergio_rs-0.2.0/sergio_rs/sergio_rs.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -20,33 +20,37 @@
         self,
         grn: GRN,
         num_cells: int,
         safety_iter: int,
         scale_iter: int,
         dt: float,
         noise_s: int,
+        seed: int,
     ) -> None: ...
     def simulate(self, mr_profile: MrProfile) -> polars.DataFrame: ...
 
 class MrProfile:
     @classmethod
     def from_random(
         cls,
         grn: GRN,
         num_cell_types: int,
         low_range: tuple[SupportsFloat, SupportsFloat],
         high_range: tuple[SupportsFloat, SupportsFloat],
+        seed: int,
     ) -> MrProfile: ...
 
 class NoiseSetting(enum.Enum):
     DS1 = enum.auto()
     DS2 = enum.auto()
     DS3 = enum.auto()
     DS4 = enum.auto()
     DS5 = enum.auto()
     DS6 = enum.auto()
     DS7 = enum.auto()
     DS8 = enum.auto()
     DS13 = enum.auto()
     DS14 = enum.auto()
 
-def add_technical_noise(expr: npt.NDArray, setting: NoiseSetting) -> npt.NDArray: ...
+def add_technical_noise(
+    expr: npt.NDArray, setting: NoiseSetting, seed: int
+) -> npt.NDArray: ...
```

### Comparing `sergio_rs-0.1.0/src/gene.rs` & `sergio_rs-0.2.0/src/gene.rs`

 * *Files identical despite different names*

### Comparing `sergio_rs-0.1.0/src/grn.rs` & `sergio_rs-0.2.0/src/grn.rs`

 * *Files 1% similar despite different names*

```diff
@@ -370,15 +370,15 @@
         grn.add_interaction(&g2, &g3, 3.0, None, 2);
         grn.add_interaction(&g5, &g6, 3.0, None, 2);
         grn.add_interaction(&g3, &g5, 3.0, None, 2);
 
         grn.set_mrs();
 
         let num_cell_types = 10;
-        let mr_profile = MrProfile::from_random(&grn, num_cell_types, 1.0..2.5, 3.5..5.0);
+        let mr_profile = MrProfile::from_random(&grn, num_cell_types, 1.0..2.5, 3.5..5.0, 42);
         let max_iter = 2000;
         grn.init(&mr_profile, max_iter);
         for gene in grn.genes.iter() {
             let gene_binding = gene.read().unwrap();
             for inter in gene_binding.in_interactions.iter() {
                 assert!(inter.h.is_some());
             }
```

### Comparing `sergio_rs-0.1.0/src/interaction.rs` & `sergio_rs-0.2.0/src/interaction.rs`

 * *Files identical despite different names*

### Comparing `sergio_rs-0.1.0/src/mrs.rs` & `sergio_rs-0.2.0/src/mrs.rs`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 use std::collections::HashMap;
 use std::ops::Range;
 
 use ndarray::{Array, Array1};
-use ndarray_rand::rand::thread_rng;
+use ndarray_rand::rand::SeedableRng;
 use ndarray_rand::rand_distr::{Bernoulli, Distribution, Uniform};
 use pyo3::exceptions::PyValueError;
 use pyo3::types::PyType;
 use pyo3::{pyclass, pymethods, Bound, PyResult};
+use rand_pcg::Lcg128Xsl64;
 
 use crate::grn::GRN;
 
 #[pyclass]
 #[derive(Clone)]
 pub struct MrProfile {
     pub num_cell_types: usize,
@@ -23,14 +24,15 @@
     #[pyo3(name = "from_random")]
     pub fn py_from_random(
         _cls: &Bound<'_, PyType>,
         grn: &GRN,
         num_cell_types: usize,
         low_range: (f64, f64),
         high_range: (f64, f64),
+        seed: u64,
     ) -> PyResult<Self> {
         if low_range.0 > low_range.1 {
             return Err(PyValueError::new_err("low_range is invalid."));
         } else if high_range.0 > high_range.1 {
             return Err(PyValueError::new_err("high_range is invalid."));
         } else if high_range.0 < low_range.1 {
             return Err(PyValueError::new_err(
@@ -39,37 +41,40 @@
         }
 
         Ok(MrProfile::from_random(
             &grn,
             num_cell_types,
             low_range.0..low_range.1,
             high_range.0..high_range.1,
+            seed,
         ))
     }
 }
 
 impl MrProfile {
     pub fn from_random(
         grn: &GRN,
         num_cell_types: usize,
         low_range: Range<f64>,
         high_range: Range<f64>,
+        seed: u64,
     ) -> Self {
         assert!(grn.mrs.len() > 0, "the GRN must have MRs.");
+        let mut rng = Lcg128Xsl64::seed_from_u64(seed);
 
         let mut mr_prod_rates: HashMap<String, Array1<f64>> = HashMap::new();
         let low_high_dist = Bernoulli::new(0.5).unwrap();
         let low_dist = Uniform::new(low_range.start, low_range.end);
         let high_dist = Uniform::new(high_range.start, high_range.end);
         for mr in grn.mrs.iter() {
             let cts: Array1<f64> = Array::zeros((num_cell_types,)).map(|x: &f64| {
-                if low_high_dist.sample(&mut thread_rng()) {
-                    x + high_dist.sample(&mut thread_rng())
+                if low_high_dist.sample(&mut rng) {
+                    x + high_dist.sample(&mut rng)
                 } else {
-                    x + low_dist.sample(&mut thread_rng())
+                    x + low_dist.sample(&mut rng)
                 }
             });
             mr_prod_rates.insert(mr.read().unwrap().name.clone(), cts);
         }
         Self {
             num_cell_types,
             mr_prod_rates,
```

### Comparing `sergio_rs-0.1.0/src/noise.rs` & `sergio_rs-0.2.0/src/noise.rs`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 use ndarray::{s, Array, Array1, Array2, ArrayView2, Axis, NewAxis};
 use ndarray_rand::{
-    rand::thread_rng,
+    rand::{Rng, SeedableRng},
     rand_distr::{Bernoulli, Distribution, LogNormal, Poisson},
     RandomExt,
 };
 use ndarray_stats::{interpolate::Linear, QuantileExt};
 use noisy_float::types::N64;
 use numpy::{PyArray2, PyReadonlyArray2, ToPyArray};
 use pyo3::{pyclass, pyfunction, Bound, Python};
+use rand_pcg::Lcg128Xsl64;
 
 #[pyclass]
 pub enum NoiseSetting {
     DS1,
     DS2,
     DS3,
     DS4,
@@ -19,47 +20,50 @@
     DS6,
     DS7,
     DS8,
     DS13,
     DS14,
 }
 
-pub fn add_outlier_effect(expr: &mut Array2<f64>, p: f64, mu: f64, sigma: f64) {
-    let outlier_indicator = Array::random_using(
-        expr.len_of(Axis(0)),
-        Bernoulli::new(p).unwrap(),
-        &mut thread_rng(),
-    );
+pub fn add_outlier_effect<T: Rng>(
+    expr: &mut Array2<f64>,
+    p: f64,
+    mu: f64,
+    sigma: f64,
+    rng: &mut T,
+) {
+    let outlier_indicator =
+        Array::random_using(expr.len_of(Axis(0)), Bernoulli::new(p).unwrap(), rng);
     let outlier_factors = Array::random_using(
         expr.len_of(Axis(0)),
         LogNormal::new(mu, sigma).unwrap(),
-        &mut thread_rng(),
+        rng,
     );
     expr.axis_iter_mut(Axis(0))
         .zip(outlier_factors)
         .enumerate()
         .for_each(|(i, (mut gene_expr, outlier_factor))| {
             if outlier_indicator[i] {
                 gene_expr.map_inplace(|x| *x *= outlier_factor)
             }
         });
 }
 
-pub fn add_lib_size_effect(expr: &mut Array2<f64>, mu: f64, sigma: f64) {
+pub fn add_lib_size_effect<T: Rng>(expr: &mut Array2<f64>, mu: f64, sigma: f64, rng: &mut T) {
     let lib_factors = Array::random_using(
         expr.len_of(Axis(1)),
         LogNormal::new(mu, sigma).unwrap(),
-        &mut thread_rng(),
+        rng,
     );
     let norm_constant = expr.sum_axis(Axis(0));
     let cell_factors = &lib_factors / &norm_constant;
     expr.zip_mut_with(&cell_factors.slice(s![NewAxis, ..]), |x, c| *x *= c);
 }
 
-pub fn add_dropout(expr: &mut Array2<f64>, k: f64, q: N64) {
+pub fn add_dropout<T: Rng>(expr: &mut Array2<f64>, k: f64, q: N64, rng: &mut T) {
     let log_expr = expr.map(|x| (x + 1.0).ln());
     // Percentile calculation
     // Have to first flatten the array to get similar behaviour to NumPy
     let mut log_expr_flat: Array1<f64> = Array::from_iter(log_expr.iter().cloned());
     let log_mid_point = log_expr_flat
         .quantile_axis_skipnan_mut(Axis(0), q / 100.0, &Linear)
         .unwrap()
@@ -70,79 +74,106 @@
     // Bernoulli prob matrix calculation
     let mut p = Array::zeros(expr.shape());
     p.zip_mut_with(&log_expr, |p, x| {
         *p = 1.0 / (1.0 + (-1.0 * k * (*x - log_mid_point)).exp());
     });
 
     expr.zip_mut_with(&p, |x, p| {
-        if Bernoulli::new(1.0 - *p).unwrap().sample(&mut thread_rng()) {
+        if Bernoulli::new(1.0 - *p).unwrap().sample(rng) {
             *x = 0.0;
         }
     });
 }
 
-pub fn to_umi_counts(expr: &mut Array2<f64>) {
+pub fn to_umi_counts<T: Rng>(expr: &mut Array2<f64>, rng: &mut T) {
     expr.map_inplace(|x| {
         *x = if *x > 0.0 {
-            Poisson::new(*x).unwrap().sample(&mut thread_rng())
+            Poisson::new(*x).unwrap().sample(rng)
         } else {
             0.0
         }
     });
 }
 
 pub fn add_technical_noise_custom(
     expr: &ArrayView2<f64>,
     outlier_mu: f64,
     library_mu: f64,
     library_sigma: f64,
     dropout_k: f64,
     dropout_q: N64,
+    seed: u64,
 ) -> Array2<f64> {
+    let mut rng = Lcg128Xsl64::seed_from_u64(seed);
     let mut data_copy = expr.to_owned();
-    add_outlier_effect(&mut data_copy, 0.01, outlier_mu, 1.0);
-    add_lib_size_effect(&mut data_copy, library_mu, library_sigma);
-    add_dropout(&mut data_copy, dropout_k, dropout_q);
-    to_umi_counts(&mut data_copy);
+    add_outlier_effect(&mut data_copy, 0.01, outlier_mu, 1.0, &mut rng);
+    add_lib_size_effect(&mut data_copy, library_mu, library_sigma, &mut rng);
+    add_dropout(&mut data_copy, dropout_k, dropout_q, &mut rng);
+    to_umi_counts(&mut data_copy, &mut rng);
     data_copy
 }
 
-pub fn add_technical_noise(expr: &ArrayView2<f64>, setting: &NoiseSetting) -> Array2<f64> {
+pub fn add_technical_noise(
+    expr: &ArrayView2<f64>,
+    setting: &NoiseSetting,
+    seed: u64,
+) -> Array2<f64> {
     match setting {
-        NoiseSetting::DS1 => add_technical_noise_custom(expr, 0.8, 4.8, 0.3, 20.0, N64::new(82.0)),
-        NoiseSetting::DS2 => add_technical_noise_custom(expr, 0.8, 6.0, 0.4, 12.0, N64::new(80.0)),
-        NoiseSetting::DS3 => add_technical_noise_custom(expr, 0.8, 7.0, 0.4, 8.0, N64::new(80.0)),
-        NoiseSetting::DS4 => add_technical_noise_custom(expr, 3.0, 6.0, 0.3, 8.0, N64::new(74.0)),
-        NoiseSetting::DS5 => add_technical_noise_custom(expr, 3.0, 6.0, 0.4, 8.0, N64::new(82.0)),
-        NoiseSetting::DS6 => add_technical_noise_custom(expr, 5.0, 4.5, 0.7, 8.0, N64::new(45.0)),
-        NoiseSetting::DS7 => add_technical_noise_custom(expr, 3.0, 4.4, 0.8, 8.0, N64::new(85.0)),
-        NoiseSetting::DS8 => add_technical_noise_custom(expr, 4.5, 10.8, 0.55, 2.0, N64::new(92.0)),
-        NoiseSetting::DS13 => add_technical_noise_custom(expr, 0.8, 3.6, 0.4, 8.0, N64::new(70.0)),
-        NoiseSetting::DS14 => add_technical_noise_custom(expr, 0.8, 5.0, 0.4, 4.0, N64::new(80.0)),
+        NoiseSetting::DS1 => {
+            add_technical_noise_custom(expr, 0.8, 4.8, 0.3, 20.0, N64::new(82.0), seed)
+        }
+        NoiseSetting::DS2 => {
+            add_technical_noise_custom(expr, 0.8, 6.0, 0.4, 12.0, N64::new(80.0), seed)
+        }
+        NoiseSetting::DS3 => {
+            add_technical_noise_custom(expr, 0.8, 7.0, 0.4, 8.0, N64::new(80.0), seed)
+        }
+        NoiseSetting::DS4 => {
+            add_technical_noise_custom(expr, 3.0, 6.0, 0.3, 8.0, N64::new(74.0), seed)
+        }
+        NoiseSetting::DS5 => {
+            add_technical_noise_custom(expr, 3.0, 6.0, 0.4, 8.0, N64::new(82.0), seed)
+        }
+        NoiseSetting::DS6 => {
+            add_technical_noise_custom(expr, 5.0, 4.5, 0.7, 8.0, N64::new(45.0), seed)
+        }
+        NoiseSetting::DS7 => {
+            add_technical_noise_custom(expr, 3.0, 4.4, 0.8, 8.0, N64::new(85.0), seed)
+        }
+        NoiseSetting::DS8 => {
+            add_technical_noise_custom(expr, 4.5, 10.8, 0.55, 2.0, N64::new(92.0), seed)
+        }
+        NoiseSetting::DS13 => {
+            add_technical_noise_custom(expr, 0.8, 3.6, 0.4, 8.0, N64::new(70.0), seed)
+        }
+        NoiseSetting::DS14 => {
+            add_technical_noise_custom(expr, 0.8, 5.0, 0.4, 4.0, N64::new(80.0), seed)
+        }
     }
 }
 
 #[pyfunction]
 #[pyo3(name = "add_technical_noise")]
 pub fn py_add_technical_noise<'py>(
     py: Python<'py>,
     expr: PyReadonlyArray2<f64>,
     setting: &NoiseSetting,
+    seed: u64,
 ) -> Bound<'py, PyArray2<f64>> {
     let rust_array = expr.as_array();
-    let noisy_data = add_technical_noise(&rust_array, setting);
+    let noisy_data = add_technical_noise(&rust_array, setting, seed);
     noisy_data.to_pyarray_bound(py)
 }
 
 #[cfg(test)]
 mod tests {
-    use ndarray_rand::rand_distr::Uniform;
+    use ndarray_rand::{rand::thread_rng, rand_distr::Uniform};
 
     use super::*;
 
     #[test]
     fn test_noise() {
         let arr1 = Array::random_using((10, 10), Uniform::new(0.0, 150.0), &mut thread_rng());
-        let noisy_data = add_technical_noise(&arr1.view(), &NoiseSetting::DS6);
+        let noisy_data = add_technical_noise(&arr1.view(), &NoiseSetting::DS6, 42);
         assert_ne!(arr1, noisy_data);
     }
 }
```

### Comparing `sergio_rs-0.1.0/src/sim.rs` & `sergio_rs-0.2.0/src/sim.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,72 +1,78 @@
 use ndarray::{s, Array, Array1, Array2, ArrayView2, Axis, NewAxis};
 use ndarray_rand::{
+    rand::{Rng, SeedableRng},
     rand_distr::{Distribution, Normal, Uniform},
     RandomExt,
 };
 use polars::{frame::DataFrame, prelude::NamedFrom, series::Series};
 use pyo3::{pyclass, pymethods};
 use pyo3_polars::PyDataFrame;
+use rand_pcg::Lcg128Xsl64;
 
 use crate::{gene::ConcType, grn::GRN, mrs::MrProfile};
-use ndarray_rand::rand::thread_rng;
 
 #[pyclass]
 pub struct Sim {
     grn: GRN,
     num_cells: usize,
     safety_iter: usize,
     scale_iter: usize,
     dt: f64,
     noise_s: f64,
+    seed: u64,
 }
 
 #[pymethods]
 impl Sim {
     #[new]
     pub fn new(
         grn: GRN,
         num_cells: usize,
         safety_iter: usize,
         scale_iter: usize,
         dt: f64,
         noise_s: f64,
+        seed: u64,
     ) -> Self {
         Self {
             grn,
             num_cells,
             safety_iter,
             scale_iter,
             dt,
             noise_s,
+            seed,
         }
     }
 
     pub fn simulate(&mut self, mr_profile: &MrProfile) -> PyDataFrame {
+        let mut rng = Lcg128Xsl64::seed_from_u64(self.seed);
         let max_iter = self.num_cells * self.scale_iter + self.safety_iter;
         self.grn.init(mr_profile, max_iter);
         let lambda = Array1::from_iter(self.grn.genes.iter().map(|x| x.read().unwrap().decay));
         let lambda_col = lambda.slice(s![.., NewAxis]);
         let rand_dist = Normal::new(0.0, 1.0).unwrap();
         let computation_shape = (self.grn.genes.len(), self.grn.num_cell_types);
 
         for _ in 0..max_iter {
-            self.iter_ss(&lambda_col, &rand_dist, &computation_shape);
+            self.iter_ss(&lambda_col, &rand_dist, &computation_shape, &mut rng);
         }
 
-        PyDataFrame(self.get_expr_df(mr_profile))
+        PyDataFrame(self.get_expr_df(mr_profile, &mut rng))
     }
 }
 
 impl Sim {
-    fn iter_ss<T: Distribution<f64>>(
+    fn iter_ss<T: Distribution<f64>, R: Rng>(
         &self,
         lambda: &ArrayView2<f64>,
         rand_dist: &T,
         computation_shape: &(usize, usize),
+        rng: &mut R,
     ) {
         let x_vec: Vec<f64> = self
             .grn
             .genes
             .iter()
             .map(|x| x.read().unwrap().get_last_conc().to_owned())
             .flatten()
@@ -84,34 +90,31 @@
                 .unwrap()
                 .map(|x| x.max(0.0));
         let sqrt_p = p.map(|x| x.sqrt());
 
         let d = lambda * &x;
         let sqrt_d = d.map(|x| x.sqrt());
         let sqrt_dt = self.dt.sqrt();
-        let rnd_p = Array::random_using(*computation_shape, rand_dist, &mut thread_rng());
-        let rnd_d = Array::random_using(*computation_shape, rand_dist, &mut thread_rng());
+        let rnd_p = Array::random_using(*computation_shape, rand_dist, rng);
+        let rnd_d = Array::random_using(*computation_shape, rand_dist, rng);
         // Eq 3 in the paper
         let new_x = &x
             + (&p - &d).mapv_into(|x| x * self.dt)
             + (&sqrt_p * &rnd_p + &sqrt_d * &rnd_d).mapv_into(|x| x * self.noise_s * sqrt_dt);
         for (gene, row) in self.grn.genes.iter().zip(new_x.axis_iter(Axis(0))) {
             gene.write().unwrap().append_sim_conc(&row);
         }
     }
 
-    fn get_expr_df(&self, mr_profile: &MrProfile) -> DataFrame {
+    fn get_expr_df<T: Rng>(&self, mr_profile: &MrProfile, rng: &mut T) -> DataFrame {
         // Sample random timesteps after safety_iter
         let rnd_dist = Uniform::new(0, self.num_cells * self.scale_iter);
-        let rnd_inds: Array2<usize> = Array::random_using(
-            (mr_profile.num_cell_types, self.num_cells),
-            rnd_dist,
-            &mut thread_rng(),
-        )
-        .map(|x| x + self.safety_iter);
+        let rnd_inds: Array2<usize> =
+            Array::random_using((mr_profile.num_cell_types, self.num_cells), rnd_dist, rng)
+                .map(|x| x + self.safety_iter);
         // DF Data
         let mut gene_names: Vec<String> = self
             .grn
             .genes
             .iter()
             .map(|x| x.read().unwrap().name.clone())
             .collect();
@@ -191,14 +194,14 @@
         grn.add_interaction(&g5, &g6, 3.0, None, 2);
         grn.add_interaction(&g3, &g5, 3.0, None, 2);
 
         grn.set_mrs();
 
         let num_cell_types = 10;
         let num_cells = 200;
-        let mr_profile = MrProfile::from_random(&grn, num_cell_types, 1.0..2.5, 3.5..5.0);
-        let mut sim = Sim::new(grn, num_cells, 150, 10, 0.01, 1.0);
+        let mr_profile = MrProfile::from_random(&grn, num_cell_types, 1.0..2.5, 3.5..5.0, 42);
+        let mut sim = Sim::new(grn, num_cells, 150, 10, 0.01, 1.0, 42);
         let df = sim.simulate(&mr_profile);
         assert!(df.0.get_columns().len() == num_cell_types * num_cells + 1);
         assert!(df.0.get_column_names()[0] == "Genes");
     }
 }
```

### Comparing `sergio_rs-0.1.0/pyproject.toml` & `sergio_rs-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sergio_rs-0.1.0/PKG-INFO` & `sergio_rs-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: sergio_rs
-Version: 0.1.0
+Version: 0.2.0
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Programming Language :: Rust
@@ -73,52 +73,59 @@
 
 **_NOTE_**: Currently, only random MR profile generation is supported.
 
 ```py
 NUM_CELL_TYPES = 10
 LOW_RANGE = (0, 2)
 HIGH_RANGE = (2, 4)
+SEED = 42
 
 mr_profile = sergio_rs.MrProfile.from_random(
     grn,
     num_cell_types=NUM_CELL_TYPES,
     low_range=LOW_RANGE,
     high_range=HIGH_RANGE,
+    seed=SEED
 )
 ```
 
 ### Step 3: Simulate
 
 **_NOTE_**: Resulting gene expression data are in a Polars DataFrame rather than a Pandas one. This is mostly the same as SERGIO output, with the only difference being that Polars has no "index", so the "index" with gene names is just another column in the DataFrame called "Genes".
 
 ```py
 NUM_CELLS = 200
 NOISE_S = 1
 SAFETY_ITER = 150
 SCALE_ITER = 10
 DT = 0.01
+SEED = 42
 
 sim = sergio_rs.Sim(
     grn,
     num_cells=NUM_CELLS,
     noise_s=NOISE_S,
     safety_iter=SAFETY_ITER,
     scale_iter=SCALE_ITER,
     dt=DT,
+    seed=SEED,
 )
 data = sim.simulate(mr_profile)
 
 # Convert to 2D NumPy array
 data_np = data.drop("Genes").to_numpy()
 ```
 
 ### Step 4: Add technical noise
 
 ```py
-noisy_data = sergio_rs.add_technical_noise(data_np, sergio_rs.NoiseSetting.DS6)
+SEED = 42
+NOISE_PROFILE = sergio_rs.NoiseSetting.DS6
+
+noisy_data = sergio_rs.add_technical_noise(data_np, NOISE_PROFILE, seed=SEED)
 ```
 
 ### Step 5: Perturb
 
 ```py
 GENE_TO_PERTURB = "GENE0001"
 perturbed_grn, perturbed_mr_profile = grn.ko_perturbation(gene_name=GENE_TO_PERTURB, mr_profile=mr_profile)
@@ -126,11 +133,12 @@
 perturbed_sim = sergio_rs.Sim(
     perturbed_grn,
     num_cells=NUM_CELLS,
     noise_s=NOISE_S,
     safety_iter=SAFETY_ITER,
     scale_iter=SCALE_ITER,
     dt=DT,
+    seed=SEED,
 )
 perturbed_data = sim.simulate(perturbed_mr_profile)
 ```
```

