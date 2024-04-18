# Comparing `tmp/lezargus-0.0.4.dev44.tar.gz` & `tmp/lezargus-0.0.4.dev51.tar.gz`

## Comparing `lezargus-0.0.4.dev44.tar` & `lezargus-0.0.4.dev51.tar`

### file list

```diff
@@ -1,396 +1,399 @@
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/.gitattributes
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/CONTRIBUTING.md
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/SECURITY.md
--rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/rebuild.ps1
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/workspace.code-workspace
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/.github/workflows/format.yaml
--rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/.github/workflows/lint.yaml
--rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/.github/workflows/publish.yaml
--rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/.github/workflows/tests.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/.nojekyll
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/Makefile
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/index.html
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/make.bat
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/.buildinfo
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/.nojekyll
--rw-r--r--   0        0        0    65247 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/genindex.html
--rw-r--r--   0        0        0    21185 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/index.html
--rw-r--r--   0        0        0     3174 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/objects.inv
--rw-r--r--   0        0        0    23530 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/py-modindex.html
--rw-r--r--   0        0        0    16490 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/search.html
--rw-r--r--   0        0        0    87688 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/searchindex.js
--rw-r--r--   0        0        0 11410022 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/.doctrees/environment.pickle
--rw-r--r--   0        0        0    11389 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/.doctrees/index.doctree
--rw-r--r--   0        0        0     3612 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/.doctrees/code/lezargus.__main__.doctree
--rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/.doctrees/code/lezargus.__version__.doctree
--rw-r--r--   0        0        0    34027 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/.doctrees/code/lezargus.container.broadcast.doctree
--rw-r--r--   0        0        0    73977 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/.doctrees/code/lezargus.container.cube.doctree
--rw-r--r--   0        0        0     4779 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/.doctrees/code/lezargus.container.doctree
--rw-r--r--   0        0        0    65366 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/.doctrees/code/lezargus.container.image.doctree
--rw-r--r--   0        0        0     8619 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/.doctrees/code/lezargus.container.mosaic.doctree
--rw-r--r--   0        0        0   116995 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/.doctrees/code/lezargus.container.parent.doctree
--rw-r--r--   0        0        0   102654 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/.doctrees/code/lezargus.container.spectra.doctree
--rw-r--r--   0        0        0     4619 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/.doctrees/code/lezargus.doctree
--rw-r--r--   0        0        0    62610 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/.doctrees/code/lezargus.initialize.doctree
--rw-r--r--   0        0        0    59785 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/.doctrees/code/lezargus.library.array.doctree
--rw-r--r--   0        0        0    62157 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/.doctrees/code/lezargus.library.atmosphere.doctree
--rw-r--r--   0        0        0    65773 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/.doctrees/code/lezargus.library.config.doctree
--rw-r--r--   0        0        0    31206 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/.doctrees/code/lezargus.library.conversion.doctree
--rw-r--r--   0        0        0    74908 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/.doctrees/code/lezargus.library.convolution.doctree
--rw-r--r--   0        0        0    27404 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/.doctrees/code/lezargus.library.data.doctree
--rw-r--r--   0        0        0     4765 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/.doctrees/code/lezargus.library.doctree
--rw-r--r--   0        0        0    69686 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/.doctrees/code/lezargus.library.fits.doctree
--rw-r--r--   0        0        0    19684 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/.doctrees/code/lezargus.library.flags.doctree
--rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/.doctrees/code/lezargus.library.hint.doctree
--rw-r--r--   0        0        0    90023 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/.doctrees/code/lezargus.library.interpolate.doctree
--rw-r--r--   0        0        0   166375 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/.doctrees/code/lezargus.library.logging.doctree
--rw-r--r--   0        0        0   132980 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/.doctrees/code/lezargus.library.math.doctree
--rw-r--r--   0        0        0    62638 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/.doctrees/code/lezargus.library.path.doctree
--rw-r--r--   0        0        0    51051 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/.doctrees/code/lezargus.library.photometry.doctree
--rw-r--r--   0        0        0   106204 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/.doctrees/code/lezargus.library.stitch.doctree
--rw-r--r--   0        0        0    29533 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/.doctrees/code/lezargus.library.temporary.doctree
--rw-r--r--   0        0        0     2617 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/.doctrees/code/lezargus.library.uncertainty.doctree
--rw-r--r--   0        0        0    24266 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/.doctrees/code/lezargus.library.wrapper.doctree
--rw-r--r--   0        0        0     4204 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/.doctrees/code/lezargus.simulation.doctree
--rw-r--r--   0        0        0   134886 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/.doctrees/code/lezargus.simulation.spectre.doctree
--rw-r--r--   0        0        0     2827 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/.doctrees/code/modules.doctree
--rw-r--r--   0        0        0    69224 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/.doctrees/technical/contributing.doctree
--rw-r--r--   0        0        0     9342 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/.doctrees/technical/convention.doctree
--rw-r--r--   0        0        0     3590 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/.doctrees/technical/index.doctree
--rw-r--r--   0        0        0     2621 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/.doctrees/technical/photometry.doctree
--rw-r--r--   0        0        0     2233 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/.doctrees/technical/synthetic_photometry.doctree
--rw-r--r--   0        0        0    16371 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/.doctrees/technical/uncertainty.doctree
--rw-r--r--   0        0        0     3416 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/.doctrees/user/index.doctree
--rw-r--r--   0        0        0    17787 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_modules/index.html
--rw-r--r--   0        0        0   116653 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_modules/lezargus/initialize.html
--rw-r--r--   0        0        0    62090 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_modules/lezargus/container/broadcast.html
--rw-r--r--   0        0        0    46530 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_modules/lezargus/container/cube.html
--rw-r--r--   0        0        0    32238 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_modules/lezargus/container/image.html
--rw-r--r--   0        0        0    18272 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_modules/lezargus/container/mosaic.html
--rw-r--r--   0        0        0   103676 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_modules/lezargus/container/parent.html
--rw-r--r--   0        0        0    68856 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_modules/lezargus/container/spectra.html
--rw-r--r--   0        0        0    56786 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_modules/lezargus/library/array.html
--rw-r--r--   0        0        0    47740 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_modules/lezargus/library/atmosphere.html
--rw-r--r--   0        0        0    75804 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_modules/lezargus/library/config.html
--rw-r--r--   0        0        0    36996 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_modules/lezargus/library/conversion.html
--rw-r--r--   0        0        0    81383 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_modules/lezargus/library/convolution.html
--rw-r--r--   0        0        0    33409 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_modules/lezargus/library/data.html
--rw-r--r--   0        0        0   103320 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_modules/lezargus/library/fits.html
--rw-r--r--   0        0        0    24806 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_modules/lezargus/library/flags.html
--rw-r--r--   0        0        0    65339 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_modules/lezargus/library/interpolate.html
--rw-r--r--   0        0        0    90693 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_modules/lezargus/library/logging.html
--rw-r--r--   0        0        0    72946 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_modules/lezargus/library/math.html
--rw-r--r--   0        0        0    43502 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_modules/lezargus/library/path.html
--rw-r--r--   0        0        0    58231 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_modules/lezargus/library/photometry.html
--rw-r--r--   0        0        0   110146 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_modules/lezargus/library/stitch.html
--rw-r--r--   0        0        0    36261 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_modules/lezargus/library/temporary.html
--rw-r--r--   0        0        0    63595 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_modules/lezargus/library/uncertainty.html
--rw-r--r--   0        0        0    36520 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_modules/lezargus/library/wrapper.html
--rw-r--r--   0        0        0   115174 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_modules/lezargus/simulation/spectre.html
--rw-r--r--   0        0        0     1987 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_sources/index.rst
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_sources/code/lezargus.__main__.rst
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_sources/code/lezargus.__version__.rst
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_sources/code/lezargus.container.broadcast.rst
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_sources/code/lezargus.container.cube.rst
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_sources/code/lezargus.container.image.rst
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_sources/code/lezargus.container.mosaic.rst
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_sources/code/lezargus.container.parent.rst
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_sources/code/lezargus.container.rst
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_sources/code/lezargus.container.spectra.rst
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_sources/code/lezargus.initialize.rst
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_sources/code/lezargus.library.array.rst
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_sources/code/lezargus.library.atmosphere.rst
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_sources/code/lezargus.library.config.rst
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_sources/code/lezargus.library.conversion.rst
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_sources/code/lezargus.library.convolution.rst
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_sources/code/lezargus.library.data.rst
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_sources/code/lezargus.library.fits.rst
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_sources/code/lezargus.library.flags.rst
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_sources/code/lezargus.library.hint.rst
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_sources/code/lezargus.library.interpolate.rst
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_sources/code/lezargus.library.logging.rst
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_sources/code/lezargus.library.math.rst
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_sources/code/lezargus.library.path.rst
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_sources/code/lezargus.library.photometry.rst
--rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_sources/code/lezargus.library.rst
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_sources/code/lezargus.library.stitch.rst
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_sources/code/lezargus.library.temporary.rst
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_sources/code/lezargus.library.uncertainty.rst
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_sources/code/lezargus.library.wrapper.rst
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_sources/code/lezargus.rst
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_sources/code/lezargus.simulation.rst
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_sources/code/lezargus.simulation.spectre.rst
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_sources/code/modules.rst
--rw-r--r--   0        0        0    13856 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_sources/technical/contributing.rst
--rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_sources/technical/convention.rst
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_sources/technical/index.rst
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_sources/technical/photometry.rst
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_sources/technical/synthetic_photometry.rst
--rw-r--r--   0        0        0     3485 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_sources/technical/uncertainty.rst
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_sources/user/index.rst
--rw-r--r--   0        0        0    15094 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_static/basic.css
--rw-r--r--   0        0        0     4472 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_static/doctools.js
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_static/documentation_options.js
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_static/file.png
--rw-r--r--   0        0        0     4758 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_static/language_data.js
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_static/minus.png
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_static/plus.png
--rw-r--r--   0        0        0    12757 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_static/pygments.css
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_static/sbt-webpack-macros.html
--rw-r--r--   0        0        0    18732 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_static/searchtools.js
--rw-r--r--   0        0        0     5123 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_static/sphinx_highlight.js
--rw-r--r--   0        0        0     1983 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_static/webpack-macros.html
--rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_static/images/logo_binder.svg
--rw-r--r--   0        0        0     7601 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_static/images/logo_colab.png
--rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_static/images/logo_deepnote.svg
--rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_static/images/logo_jupyterhub.svg
--rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_static/locales/ar/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_static/locales/bg/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_static/locales/bn/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_static/locales/ca/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_static/locales/cs/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_static/locales/da/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_static/locales/de/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_static/locales/el/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_static/locales/eo/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_static/locales/es/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_static/locales/et/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_static/locales/fi/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_static/locales/fr/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_static/locales/hr/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_static/locales/id/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_static/locales/it/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_static/locales/iw/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_static/locales/ja/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_static/locales/ko/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_static/locales/lt/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_static/locales/lv/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_static/locales/ml/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_static/locales/mr/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_static/locales/ms/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_static/locales/nl/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_static/locales/no/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_static/locales/pl/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_static/locales/pt/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_static/locales/ro/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_static/locales/ru/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_static/locales/sk/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_static/locales/sl/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_static/locales/sr/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1283 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_static/locales/sv/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_static/locales/ta/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_static/locales/te/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_static/locales/tg/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_static/locales/th/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_static/locales/tl/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_static/locales/tr/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_static/locales/uk/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_static/locales/ur/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1349 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_static/locales/vi/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_static/locales/zh_CN/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_static/locales/zh_TW/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0    81380 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_static/scripts/bootstrap.js
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_static/scripts/bootstrap.js.LICENSE.txt
--rw-r--r--   0        0        0   332823 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_static/scripts/bootstrap.js.map
--rw-r--r--   0        0        0     9206 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_static/scripts/pydata-sphinx-theme.js
--rw-r--r--   0        0        0    43768 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_static/scripts/pydata-sphinx-theme.js.map
--rw-r--r--   0        0        0     3075 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_static/scripts/sphinx-book-theme.js
--rw-r--r--   0        0        0    13066 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_static/scripts/sphinx-book-theme.js.map
--rw-r--r--   0        0        0   208854 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_static/styles/bootstrap.css
--rw-r--r--   0        0        0   555088 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_static/styles/bootstrap.css.map
--rw-r--r--   0        0        0    72384 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_static/styles/pydata-sphinx-theme.css
--rw-r--r--   0        0        0   294320 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_static/styles/pydata-sphinx-theme.css.map
--rw-r--r--   0        0        0    14558 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_static/styles/sphinx-book-theme.css
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_static/styles/theme.css
--rw-r--r--   0        0        0     7427 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_static/vendor/fontawesome/6.1.2/LICENSE.txt
--rw-r--r--   0        0        0   101691 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_static/vendor/fontawesome/6.1.2/css/all.min.css
--rw-r--r--   0        0        0  1731490 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_static/vendor/fontawesome/6.1.2/js/all.min.js
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_static/vendor/fontawesome/6.1.2/js/all.min.js.LICENSE.txt
--rw-r--r--   0        0        0   181264 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.ttf
--rw-r--r--   0        0        0   105112 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.woff2
--rw-r--r--   0        0        0    60236 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.ttf
--rw-r--r--   0        0        0    24028 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.woff2
--rw-r--r--   0        0        0   389948 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.ttf
--rw-r--r--   0        0        0   154840 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.woff2
--rw-r--r--   0        0        0    10084 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.ttf
--rw-r--r--   0        0        0     4776 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.woff2
--rw-r--r--   0        0        0     7427 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_static/vendor/fontawesome/6.5.1/LICENSE.txt
--rw-r--r--   0        0        0   102621 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_static/vendor/fontawesome/6.5.1/css/all.min.css
--rw-r--r--   0        0        0  1485766 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_static/vendor/fontawesome/6.5.1/js/all.min.js
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_static/vendor/fontawesome/6.5.1/js/all.min.js.LICENSE.txt
--rw-r--r--   0        0        0   207972 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-brands-400.ttf
--rw-r--r--   0        0        0   117372 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-brands-400.woff2
--rw-r--r--   0        0        0    68004 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-regular-400.ttf
--rw-r--r--   0        0        0    25452 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-regular-400.woff2
--rw-r--r--   0        0        0   419720 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-solid-900.ttf
--rw-r--r--   0        0        0   156496 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-solid-900.woff2
--rw-r--r--   0        0        0    10832 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-v4compatibility.ttf
--rw-r--r--   0        0        0     4792 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-v4compatibility.woff2
--rw-r--r--   0        0        0    18025 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/code/lezargus.__main__.html
--rw-r--r--   0        0        0    17977 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/code/lezargus.__version__.html
--rw-r--r--   0        0        0    30706 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/code/lezargus.container.broadcast.html
--rw-r--r--   0        0        0    45422 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/code/lezargus.container.cube.html
--rw-r--r--   0        0        0    31839 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/code/lezargus.container.html
--rw-r--r--   0        0        0    40973 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/code/lezargus.container.image.html
--rw-r--r--   0        0        0    21651 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/code/lezargus.container.mosaic.html
--rw-r--r--   0        0        0    68876 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/code/lezargus.container.parent.html
--rw-r--r--   0        0        0    54793 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/code/lezargus.container.spectra.html
--rw-r--r--   0        0        0    57992 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/code/lezargus.html
--rw-r--r--   0        0        0    42180 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/code/lezargus.initialize.html
--rw-r--r--   0        0        0    40101 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/code/lezargus.library.array.html
--rw-r--r--   0        0        0    41852 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/code/lezargus.library.atmosphere.html
--rw-r--r--   0        0        0    43332 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/code/lezargus.library.config.html
--rw-r--r--   0        0        0    29421 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/code/lezargus.library.conversion.html
--rw-r--r--   0        0        0    45866 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/code/lezargus.library.convolution.html
--rw-r--r--   0        0        0    28409 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/code/lezargus.library.data.html
--rw-r--r--   0        0        0    43928 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/code/lezargus.library.fits.html
--rw-r--r--   0        0        0    26308 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/code/lezargus.library.flags.html
--rw-r--r--   0        0        0    18523 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/code/lezargus.library.hint.html
--rw-r--r--   0        0        0    52704 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/code/lezargus.library.html
--rw-r--r--   0        0        0    56777 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/code/lezargus.library.interpolate.html
--rw-r--r--   0        0        0    96075 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/code/lezargus.library.logging.html
--rw-r--r--   0        0        0    66988 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/code/lezargus.library.math.html
--rw-r--r--   0        0        0    39831 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/code/lezargus.library.path.html
--rw-r--r--   0        0        0    35916 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/code/lezargus.library.photometry.html
--rw-r--r--   0        0        0    56680 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/code/lezargus.library.stitch.html
--rw-r--r--   0        0        0    28407 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/code/lezargus.library.temporary.html
--rw-r--r--   0        0        0    16859 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/code/lezargus.library.uncertainty.html
--rw-r--r--   0        0        0    27890 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/code/lezargus.library.wrapper.html
--rw-r--r--   0        0        0    25940 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/code/lezargus.simulation.html
--rw-r--r--   0        0        0    82522 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/code/lezargus.simulation.spectre.html
--rw-r--r--   0        0        0    21820 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/code/modules.html
--rw-r--r--   0        0        0    43301 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/technical/contributing.html
--rw-r--r--   0        0        0    21407 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/technical/convention.html
--rw-r--r--   0        0        0    17881 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/technical/index.html
--rw-r--r--   0        0        0    17811 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/technical/photometry.html
--rw-r--r--   0        0        0    17634 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/technical/synthetic_photometry.html
--rw-r--r--   0        0        0    25514 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/technical/uncertainty.html
--rw-r--r--   0        0        0    17930 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/build/html/user/index.html
--rw-r--r--   0        0        0     2749 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/source/conf.py
--rw-r--r--   0        0        0     1987 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/source/index.rst
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/source/code/lezargus.__main__.rst
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/source/code/lezargus.__version__.rst
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/source/code/lezargus.container.broadcast.rst
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/source/code/lezargus.container.cube.rst
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/source/code/lezargus.container.image.rst
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/source/code/lezargus.container.mosaic.rst
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/source/code/lezargus.container.parent.rst
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/source/code/lezargus.container.rst
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/source/code/lezargus.container.spectra.rst
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/source/code/lezargus.initialize.rst
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/source/code/lezargus.library.array.rst
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/source/code/lezargus.library.atmosphere.rst
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/source/code/lezargus.library.config.rst
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/source/code/lezargus.library.conversion.rst
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/source/code/lezargus.library.convolution.rst
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/source/code/lezargus.library.data.rst
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/source/code/lezargus.library.fits.rst
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/source/code/lezargus.library.flags.rst
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/source/code/lezargus.library.hint.rst
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/source/code/lezargus.library.interpolate.rst
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/source/code/lezargus.library.logging.rst
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/source/code/lezargus.library.math.rst
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/source/code/lezargus.library.path.rst
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/source/code/lezargus.library.photometry.rst
--rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/source/code/lezargus.library.rst
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/source/code/lezargus.library.stitch.rst
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/source/code/lezargus.library.temporary.rst
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/source/code/lezargus.library.wrapper.rst
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/source/code/lezargus.rst
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/source/code/lezargus.simulation.rst
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/source/code/lezargus.simulation.spectre.rst
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/source/code/modules.rst
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/source/technical/atmosphere.rst
--rw-r--r--   0        0        0    13857 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/source/technical/contributing.rst
--rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/source/technical/convention.rst
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/source/technical/index.rst
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/source/technical/photometry.rst
--rw-r--r--   0        0        0     3485 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/source/technical/uncertainty.rst
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/docs/source/user/index.rst
--rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/src/lezargus/__init__.py
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/src/lezargus/__main__.py
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/src/lezargus/__version__.py
--rw-r--r--   0        0        0     4937 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/src/lezargus/configuration.yaml
--rw-r--r--   0        0        0    30353 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/src/lezargus/initialize.py
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/src/lezargus/container/__init__.py
--rw-r--r--   0        0        0    17058 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/src/lezargus/container/broadcast.py
--rw-r--r--   0        0        0    10234 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/src/lezargus/container/cube.py
--rw-r--r--   0        0        0     5834 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/src/lezargus/container/image.py
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/src/lezargus/container/mosaic.py
--rw-r--r--   0        0        0    29943 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/src/lezargus/container/parent.py
--rw-r--r--   0        0        0    18729 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/src/lezargus/container/spectra.py
--rw-r--r--   0        0        0   144000 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/src/lezargus/data/atm_rad_za0.fits
--rw-r--r--   0        0        0   144000 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/src/lezargus/data/atm_rad_za30.fits
--rw-r--r--   0        0        0   144000 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/src/lezargus/data/atm_rad_za45.fits
--rw-r--r--   0        0        0   144000 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/src/lezargus/data/atm_rad_za60.fits
--rw-r--r--   0        0        0   144000 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/src/lezargus/data/atm_trans_za0.fits
--rw-r--r--   0        0        0   144000 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/src/lezargus/data/atm_trans_za30.fits
--rw-r--r--   0        0        0   144000 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/src/lezargus/data/atm_trans_za45.fits
--rw-r--r--   0        0        0   144000 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/src/lezargus/data/atm_trans_za60.fits
--rw-r--r--   0        0        0    31680 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/src/lezargus/data/filter_2MASS_H_energy.fits
--rw-r--r--   0        0        0    31680 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/src/lezargus/data/filter_2MASS_H_photon.fits
--rw-r--r--   0        0        0    31680 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/src/lezargus/data/filter_2MASS_J_energy.fits
--rw-r--r--   0        0        0    31680 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/src/lezargus/data/filter_2MASS_J_photon.fits
--rw-r--r--   0        0        0    31680 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/src/lezargus/data/filter_2MASS_Ks_energy.fits
--rw-r--r--   0        0        0    31680 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/src/lezargus/data/filter_2MASS_Ks_photon.fits
--rw-r--r--   0        0        0    40320 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/src/lezargus/data/filter_Gaia_GB_energy.fits
--rw-r--r--   0        0        0    40320 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/src/lezargus/data/filter_Gaia_GB_photon.fits
--rw-r--r--   0        0        0    51840 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/src/lezargus/data/filter_Gaia_GG_energy.fits
--rw-r--r--   0        0        0    51840 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/src/lezargus/data/filter_Gaia_GG_photon.fits
--rw-r--r--   0        0        0    40320 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/src/lezargus/data/filter_Gaia_GR_energy.fits
--rw-r--r--   0        0        0    40320 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/src/lezargus/data/filter_Gaia_GR_photon.fits
--rw-r--r--   0        0        0    31680 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/src/lezargus/data/filter_Johnson_B_energy.fits
--rw-r--r--   0        0        0    31680 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/src/lezargus/data/filter_Johnson_B_photon.fits
--rw-r--r--   0        0        0    31680 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/src/lezargus/data/filter_Johnson_U_energy.fits
--rw-r--r--   0        0        0    31680 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/src/lezargus/data/filter_Johnson_U_photon.fits
--rw-r--r--   0        0        0    31680 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/src/lezargus/data/filter_Johnson_V_energy.fits
--rw-r--r--   0        0        0    31680 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/src/lezargus/data/filter_Johnson_V_photon.fits
--rw-r--r--   0        0        0  6837120 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/src/lezargus/data/gem_atm_ir_rad.fits
--rw-r--r--   0        0        0    92160 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/src/lezargus/data/gem_atm_opt_rad.fits
--rw-r--r--   0        0        0   144000 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/src/lezargus/data/psg_atm_rad_za0.fits
--rw-r--r--   0        0        0   144000 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/src/lezargus/data/psg_atm_rad_za30.fits
--rw-r--r--   0        0        0   144000 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/src/lezargus/data/psg_atm_rad_za45.fits
--rw-r--r--   0        0        0   144000 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/src/lezargus/data/psg_atm_rad_za60.fits
--rw-r--r--   0        0        0   144000 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/src/lezargus/data/psg_atm_trans_za0.fits
--rw-r--r--   0        0        0   144000 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/src/lezargus/data/psg_atm_trans_za30.fits
--rw-r--r--   0        0        0   144000 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/src/lezargus/data/psg_atm_trans_za45.fits
--rw-r--r--   0        0        0   144000 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/src/lezargus/data/psg_atm_trans_za60.fits
--rw-r--r--   0        0        0   126720 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/src/lezargus/data/star_spectra_109Vir.fits
--rw-r--r--   0        0        0   126720 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/src/lezargus/data/star_spectra_16CygB.fits
--rw-r--r--   0        0        0   103680 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/src/lezargus/data/star_spectra_A0V.fits
--rw-r--r--   0        0        0    54720 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/src/lezargus/data/star_spectra_Sun.fits
--rw-r--r--   0        0        0   120960 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/src/lezargus/data/star_spectra_Vega.fits
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/src/lezargus/library/__init__.py
--rw-r--r--   0        0        0    12292 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/src/lezargus/library/array.py
--rw-r--r--   0        0        0    12861 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/src/lezargus/library/atmosphere.py
--rw-r--r--   0        0        0    20520 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/src/lezargus/library/config.py
--rw-r--r--   0        0        0     7929 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/src/lezargus/library/conversion.py
--rw-r--r--   0        0        0    21789 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/src/lezargus/library/convolution.py
--rw-r--r--   0        0        0     5687 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/src/lezargus/library/data.py
--rw-r--r--   0        0        0    25173 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/src/lezargus/library/fits.py
--rw-r--r--   0        0        0     2741 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/src/lezargus/library/flags.py
--rw-r--r--   0        0        0     1953 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/src/lezargus/library/hint.py
--rw-r--r--   0        0        0    43769 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/src/lezargus/library/interpolate.py
--rw-r--r--   0        0        0    25032 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/src/lezargus/library/logging.py
--rw-r--r--   0        0        0    21379 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/src/lezargus/library/math.py
--rw-r--r--   0        0        0     8789 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/src/lezargus/library/path.py
--rw-r--r--   0        0        0    14161 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/src/lezargus/library/photometry.py
--rw-r--r--   0        0        0    31979 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/src/lezargus/library/stitch.py
--rw-r--r--   0        0        0     7659 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/src/lezargus/library/temporary.py
--rw-r--r--   0        0        0     7706 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/src/lezargus/library/wrapper.py
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/src/lezargus/simulation/__init__.py
--rw-r--r--   0        0        0    37984 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/src/lezargus/simulation/spectre.py
--rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/tests/conftest.py
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/tests/test_configuration_overrides.yaml
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/tests/test_init.py
--rw-r--r--   0        0        0     3549 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/tests/test_library_config.py
--rw-r--r--   0        0        0     4053 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/tests/test_library_logging.py
--rw-r--r--   0        0        0    12376 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/tests/test_library_path.py
--rw-r--r--   0        0        0     3583 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/tests/test_library_wrapper.py
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/tests/test_files/config_filename_not_flat_configuration.yaml
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/tests/test_files/config_filename_with_lowercase_keys.yaml
--rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/LICENSE.txt
--rw-r--r--   0        0        0     3026 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/README.md
--rw-r--r--   0        0        0     5779 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/pyproject.toml
--rw-r--r--   0        0        0     4057 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev44/PKG-INFO
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/.gitattributes
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/CONTRIBUTING.md
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/SECURITY.md
+-rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/rebuild.ps1
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/workspace.code-workspace
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/.github/workflows/format.yaml
+-rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/.github/workflows/lint.yaml
+-rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/.github/workflows/tests.yaml
+-rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/.vscode/settings.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/.nojekyll
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/Makefile
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/index.html
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/make.bat
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/.buildinfo
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/.nojekyll
+-rw-r--r--   0        0        0    65247 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/genindex.html
+-rw-r--r--   0        0        0    21185 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/index.html
+-rw-r--r--   0        0        0     3174 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/objects.inv
+-rw-r--r--   0        0        0    23530 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/py-modindex.html
+-rw-r--r--   0        0        0    16490 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/search.html
+-rw-r--r--   0        0        0    87688 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/searchindex.js
+-rw-r--r--   0        0        0 11410022 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/.doctrees/environment.pickle
+-rw-r--r--   0        0        0    11389 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/.doctrees/index.doctree
+-rw-r--r--   0        0        0     3612 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/.doctrees/code/lezargus.__main__.doctree
+-rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/.doctrees/code/lezargus.__version__.doctree
+-rw-r--r--   0        0        0    34027 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/.doctrees/code/lezargus.container.broadcast.doctree
+-rw-r--r--   0        0        0    73977 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/.doctrees/code/lezargus.container.cube.doctree
+-rw-r--r--   0        0        0     4779 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/.doctrees/code/lezargus.container.doctree
+-rw-r--r--   0        0        0    65366 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/.doctrees/code/lezargus.container.image.doctree
+-rw-r--r--   0        0        0     8619 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/.doctrees/code/lezargus.container.mosaic.doctree
+-rw-r--r--   0        0        0   116995 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/.doctrees/code/lezargus.container.parent.doctree
+-rw-r--r--   0        0        0   102654 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/.doctrees/code/lezargus.container.spectra.doctree
+-rw-r--r--   0        0        0     4619 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/.doctrees/code/lezargus.doctree
+-rw-r--r--   0        0        0    62610 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/.doctrees/code/lezargus.initialize.doctree
+-rw-r--r--   0        0        0    59785 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/.doctrees/code/lezargus.library.array.doctree
+-rw-r--r--   0        0        0    62157 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/.doctrees/code/lezargus.library.atmosphere.doctree
+-rw-r--r--   0        0        0    65773 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/.doctrees/code/lezargus.library.config.doctree
+-rw-r--r--   0        0        0    31206 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/.doctrees/code/lezargus.library.conversion.doctree
+-rw-r--r--   0        0        0    74908 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/.doctrees/code/lezargus.library.convolution.doctree
+-rw-r--r--   0        0        0    27404 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/.doctrees/code/lezargus.library.data.doctree
+-rw-r--r--   0        0        0     4765 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/.doctrees/code/lezargus.library.doctree
+-rw-r--r--   0        0        0    69686 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/.doctrees/code/lezargus.library.fits.doctree
+-rw-r--r--   0        0        0    19684 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/.doctrees/code/lezargus.library.flags.doctree
+-rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/.doctrees/code/lezargus.library.hint.doctree
+-rw-r--r--   0        0        0    90023 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/.doctrees/code/lezargus.library.interpolate.doctree
+-rw-r--r--   0        0        0   166375 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/.doctrees/code/lezargus.library.logging.doctree
+-rw-r--r--   0        0        0   132980 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/.doctrees/code/lezargus.library.math.doctree
+-rw-r--r--   0        0        0    62638 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/.doctrees/code/lezargus.library.path.doctree
+-rw-r--r--   0        0        0    51051 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/.doctrees/code/lezargus.library.photometry.doctree
+-rw-r--r--   0        0        0   106204 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/.doctrees/code/lezargus.library.stitch.doctree
+-rw-r--r--   0        0        0    29533 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/.doctrees/code/lezargus.library.temporary.doctree
+-rw-r--r--   0        0        0     2617 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/.doctrees/code/lezargus.library.uncertainty.doctree
+-rw-r--r--   0        0        0    24266 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/.doctrees/code/lezargus.library.wrapper.doctree
+-rw-r--r--   0        0        0     4204 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/.doctrees/code/lezargus.simulation.doctree
+-rw-r--r--   0        0        0   134886 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/.doctrees/code/lezargus.simulation.spectre.doctree
+-rw-r--r--   0        0        0     2827 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/.doctrees/code/modules.doctree
+-rw-r--r--   0        0        0    69224 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/.doctrees/technical/contributing.doctree
+-rw-r--r--   0        0        0     9342 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/.doctrees/technical/convention.doctree
+-rw-r--r--   0        0        0     3590 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/.doctrees/technical/index.doctree
+-rw-r--r--   0        0        0     2621 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/.doctrees/technical/photometry.doctree
+-rw-r--r--   0        0        0     2233 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/.doctrees/technical/synthetic_photometry.doctree
+-rw-r--r--   0        0        0    16371 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/.doctrees/technical/uncertainty.doctree
+-rw-r--r--   0        0        0     3416 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/.doctrees/user/index.doctree
+-rw-r--r--   0        0        0    17787 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_modules/index.html
+-rw-r--r--   0        0        0   116653 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_modules/lezargus/initialize.html
+-rw-r--r--   0        0        0    62090 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_modules/lezargus/container/broadcast.html
+-rw-r--r--   0        0        0    46530 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_modules/lezargus/container/cube.html
+-rw-r--r--   0        0        0    32238 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_modules/lezargus/container/image.html
+-rw-r--r--   0        0        0    18272 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_modules/lezargus/container/mosaic.html
+-rw-r--r--   0        0        0   103676 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_modules/lezargus/container/parent.html
+-rw-r--r--   0        0        0    68856 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_modules/lezargus/container/spectra.html
+-rw-r--r--   0        0        0    56786 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_modules/lezargus/library/array.html
+-rw-r--r--   0        0        0    47740 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_modules/lezargus/library/atmosphere.html
+-rw-r--r--   0        0        0    75804 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_modules/lezargus/library/config.html
+-rw-r--r--   0        0        0    36996 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_modules/lezargus/library/conversion.html
+-rw-r--r--   0        0        0    81383 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_modules/lezargus/library/convolution.html
+-rw-r--r--   0        0        0    33409 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_modules/lezargus/library/data.html
+-rw-r--r--   0        0        0   103320 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_modules/lezargus/library/fits.html
+-rw-r--r--   0        0        0    24806 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_modules/lezargus/library/flags.html
+-rw-r--r--   0        0        0    65339 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_modules/lezargus/library/interpolate.html
+-rw-r--r--   0        0        0    90693 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_modules/lezargus/library/logging.html
+-rw-r--r--   0        0        0    72946 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_modules/lezargus/library/math.html
+-rw-r--r--   0        0        0    43502 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_modules/lezargus/library/path.html
+-rw-r--r--   0        0        0    58231 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_modules/lezargus/library/photometry.html
+-rw-r--r--   0        0        0   110146 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_modules/lezargus/library/stitch.html
+-rw-r--r--   0        0        0    36261 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_modules/lezargus/library/temporary.html
+-rw-r--r--   0        0        0    63595 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_modules/lezargus/library/uncertainty.html
+-rw-r--r--   0        0        0    36520 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_modules/lezargus/library/wrapper.html
+-rw-r--r--   0        0        0   115174 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_modules/lezargus/simulation/spectre.html
+-rw-r--r--   0        0        0     1987 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_sources/index.rst
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_sources/code/lezargus.__main__.rst
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_sources/code/lezargus.__version__.rst
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_sources/code/lezargus.container.broadcast.rst
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_sources/code/lezargus.container.cube.rst
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_sources/code/lezargus.container.image.rst
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_sources/code/lezargus.container.mosaic.rst
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_sources/code/lezargus.container.parent.rst
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_sources/code/lezargus.container.rst
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_sources/code/lezargus.container.spectra.rst
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_sources/code/lezargus.initialize.rst
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_sources/code/lezargus.library.array.rst
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_sources/code/lezargus.library.atmosphere.rst
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_sources/code/lezargus.library.config.rst
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_sources/code/lezargus.library.conversion.rst
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_sources/code/lezargus.library.convolution.rst
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_sources/code/lezargus.library.data.rst
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_sources/code/lezargus.library.fits.rst
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_sources/code/lezargus.library.flags.rst
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_sources/code/lezargus.library.hint.rst
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_sources/code/lezargus.library.interpolate.rst
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_sources/code/lezargus.library.logging.rst
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_sources/code/lezargus.library.math.rst
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_sources/code/lezargus.library.path.rst
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_sources/code/lezargus.library.photometry.rst
+-rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_sources/code/lezargus.library.rst
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_sources/code/lezargus.library.stitch.rst
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_sources/code/lezargus.library.temporary.rst
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_sources/code/lezargus.library.uncertainty.rst
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_sources/code/lezargus.library.wrapper.rst
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_sources/code/lezargus.rst
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_sources/code/lezargus.simulation.rst
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_sources/code/lezargus.simulation.spectre.rst
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_sources/code/modules.rst
+-rw-r--r--   0        0        0    13856 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_sources/technical/contributing.rst
+-rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_sources/technical/convention.rst
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_sources/technical/index.rst
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_sources/technical/photometry.rst
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_sources/technical/synthetic_photometry.rst
+-rw-r--r--   0        0        0     3485 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_sources/technical/uncertainty.rst
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_sources/user/index.rst
+-rw-r--r--   0        0        0    15094 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_static/basic.css
+-rw-r--r--   0        0        0     4472 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_static/doctools.js
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_static/documentation_options.js
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_static/file.png
+-rw-r--r--   0        0        0     4758 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_static/language_data.js
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_static/minus.png
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_static/plus.png
+-rw-r--r--   0        0        0    12757 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_static/pygments.css
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_static/sbt-webpack-macros.html
+-rw-r--r--   0        0        0    18732 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_static/searchtools.js
+-rw-r--r--   0        0        0     5123 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_static/sphinx_highlight.js
+-rw-r--r--   0        0        0     1983 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_static/webpack-macros.html
+-rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_static/images/logo_binder.svg
+-rw-r--r--   0        0        0     7601 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_static/images/logo_colab.png
+-rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_static/images/logo_deepnote.svg
+-rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_static/images/logo_jupyterhub.svg
+-rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_static/locales/ar/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_static/locales/bg/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_static/locales/bn/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_static/locales/ca/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_static/locales/cs/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_static/locales/da/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_static/locales/de/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_static/locales/el/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_static/locales/eo/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_static/locales/es/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_static/locales/et/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_static/locales/fi/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_static/locales/fr/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_static/locales/hr/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_static/locales/id/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_static/locales/it/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_static/locales/iw/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_static/locales/ja/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_static/locales/ko/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_static/locales/lt/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_static/locales/lv/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_static/locales/ml/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_static/locales/mr/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_static/locales/ms/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_static/locales/nl/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_static/locales/no/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_static/locales/pl/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_static/locales/pt/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_static/locales/ro/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_static/locales/ru/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_static/locales/sk/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_static/locales/sl/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_static/locales/sr/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1283 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_static/locales/sv/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_static/locales/ta/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_static/locales/te/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_static/locales/tg/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_static/locales/th/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_static/locales/tl/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_static/locales/tr/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_static/locales/uk/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_static/locales/ur/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1349 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_static/locales/vi/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_static/locales/zh_CN/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_static/locales/zh_TW/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0    81380 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_static/scripts/bootstrap.js
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_static/scripts/bootstrap.js.LICENSE.txt
+-rw-r--r--   0        0        0   332823 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_static/scripts/bootstrap.js.map
+-rw-r--r--   0        0        0     9206 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_static/scripts/pydata-sphinx-theme.js
+-rw-r--r--   0        0        0    43768 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_static/scripts/pydata-sphinx-theme.js.map
+-rw-r--r--   0        0        0     3075 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_static/scripts/sphinx-book-theme.js
+-rw-r--r--   0        0        0    13066 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_static/scripts/sphinx-book-theme.js.map
+-rw-r--r--   0        0        0   208854 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_static/styles/bootstrap.css
+-rw-r--r--   0        0        0   555088 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_static/styles/bootstrap.css.map
+-rw-r--r--   0        0        0    72384 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_static/styles/pydata-sphinx-theme.css
+-rw-r--r--   0        0        0   294320 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_static/styles/pydata-sphinx-theme.css.map
+-rw-r--r--   0        0        0    14558 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_static/styles/sphinx-book-theme.css
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_static/styles/theme.css
+-rw-r--r--   0        0        0     7427 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_static/vendor/fontawesome/6.1.2/LICENSE.txt
+-rw-r--r--   0        0        0   101691 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_static/vendor/fontawesome/6.1.2/css/all.min.css
+-rw-r--r--   0        0        0  1731490 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_static/vendor/fontawesome/6.1.2/js/all.min.js
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_static/vendor/fontawesome/6.1.2/js/all.min.js.LICENSE.txt
+-rw-r--r--   0        0        0   181264 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.ttf
+-rw-r--r--   0        0        0   105112 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.woff2
+-rw-r--r--   0        0        0    60236 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.ttf
+-rw-r--r--   0        0        0    24028 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.woff2
+-rw-r--r--   0        0        0   389948 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.ttf
+-rw-r--r--   0        0        0   154840 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.woff2
+-rw-r--r--   0        0        0    10084 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.ttf
+-rw-r--r--   0        0        0     4776 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.woff2
+-rw-r--r--   0        0        0     7427 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_static/vendor/fontawesome/6.5.1/LICENSE.txt
+-rw-r--r--   0        0        0   102621 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_static/vendor/fontawesome/6.5.1/css/all.min.css
+-rw-r--r--   0        0        0  1485766 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_static/vendor/fontawesome/6.5.1/js/all.min.js
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_static/vendor/fontawesome/6.5.1/js/all.min.js.LICENSE.txt
+-rw-r--r--   0        0        0   207972 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-brands-400.ttf
+-rw-r--r--   0        0        0   117372 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-brands-400.woff2
+-rw-r--r--   0        0        0    68004 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-regular-400.ttf
+-rw-r--r--   0        0        0    25452 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-regular-400.woff2
+-rw-r--r--   0        0        0   419720 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-solid-900.ttf
+-rw-r--r--   0        0        0   156496 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-solid-900.woff2
+-rw-r--r--   0        0        0    10832 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-v4compatibility.ttf
+-rw-r--r--   0        0        0     4792 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-v4compatibility.woff2
+-rw-r--r--   0        0        0    18025 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/code/lezargus.__main__.html
+-rw-r--r--   0        0        0    17977 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/code/lezargus.__version__.html
+-rw-r--r--   0        0        0    30706 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/code/lezargus.container.broadcast.html
+-rw-r--r--   0        0        0    45422 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/code/lezargus.container.cube.html
+-rw-r--r--   0        0        0    31839 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/code/lezargus.container.html
+-rw-r--r--   0        0        0    40973 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/code/lezargus.container.image.html
+-rw-r--r--   0        0        0    21651 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/code/lezargus.container.mosaic.html
+-rw-r--r--   0        0        0    68876 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/code/lezargus.container.parent.html
+-rw-r--r--   0        0        0    54793 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/code/lezargus.container.spectra.html
+-rw-r--r--   0        0        0    57992 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/code/lezargus.html
+-rw-r--r--   0        0        0    42180 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/code/lezargus.initialize.html
+-rw-r--r--   0        0        0    40101 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/code/lezargus.library.array.html
+-rw-r--r--   0        0        0    41852 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/code/lezargus.library.atmosphere.html
+-rw-r--r--   0        0        0    43332 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/code/lezargus.library.config.html
+-rw-r--r--   0        0        0    29421 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/code/lezargus.library.conversion.html
+-rw-r--r--   0        0        0    45866 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/code/lezargus.library.convolution.html
+-rw-r--r--   0        0        0    28409 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/code/lezargus.library.data.html
+-rw-r--r--   0        0        0    43928 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/code/lezargus.library.fits.html
+-rw-r--r--   0        0        0    26308 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/code/lezargus.library.flags.html
+-rw-r--r--   0        0        0    18523 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/code/lezargus.library.hint.html
+-rw-r--r--   0        0        0    52704 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/code/lezargus.library.html
+-rw-r--r--   0        0        0    56777 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/code/lezargus.library.interpolate.html
+-rw-r--r--   0        0        0    96075 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/code/lezargus.library.logging.html
+-rw-r--r--   0        0        0    66988 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/code/lezargus.library.math.html
+-rw-r--r--   0        0        0    39831 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/code/lezargus.library.path.html
+-rw-r--r--   0        0        0    35916 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/code/lezargus.library.photometry.html
+-rw-r--r--   0        0        0    56680 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/code/lezargus.library.stitch.html
+-rw-r--r--   0        0        0    28407 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/code/lezargus.library.temporary.html
+-rw-r--r--   0        0        0    16859 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/code/lezargus.library.uncertainty.html
+-rw-r--r--   0        0        0    27890 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/code/lezargus.library.wrapper.html
+-rw-r--r--   0        0        0    25940 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/code/lezargus.simulation.html
+-rw-r--r--   0        0        0    82522 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/code/lezargus.simulation.spectre.html
+-rw-r--r--   0        0        0    21820 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/code/modules.html
+-rw-r--r--   0        0        0    43301 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/technical/contributing.html
+-rw-r--r--   0        0        0    21407 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/technical/convention.html
+-rw-r--r--   0        0        0    17881 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/technical/index.html
+-rw-r--r--   0        0        0    17811 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/technical/photometry.html
+-rw-r--r--   0        0        0    17634 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/technical/synthetic_photometry.html
+-rw-r--r--   0        0        0    25514 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/technical/uncertainty.html
+-rw-r--r--   0        0        0    17930 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/build/html/user/index.html
+-rw-r--r--   0        0        0     2724 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/source/conf.py
+-rw-r--r--   0        0        0     1987 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/source/index.rst
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/source/code/lezargus.__main__.rst
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/source/code/lezargus.__version__.rst
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/source/code/lezargus.container.broadcast.rst
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/source/code/lezargus.container.cube.rst
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/source/code/lezargus.container.image.rst
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/source/code/lezargus.container.mosaic.rst
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/source/code/lezargus.container.parent.rst
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/source/code/lezargus.container.rst
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/source/code/lezargus.container.spectra.rst
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/source/code/lezargus.initialize.rst
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/source/code/lezargus.library.array.rst
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/source/code/lezargus.library.atmosphere.rst
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/source/code/lezargus.library.config.rst
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/source/code/lezargus.library.conversion.rst
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/source/code/lezargus.library.convolution.rst
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/source/code/lezargus.library.data.rst
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/source/code/lezargus.library.fits.rst
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/source/code/lezargus.library.flags.rst
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/source/code/lezargus.library.hint.rst
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/source/code/lezargus.library.interpolate.rst
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/source/code/lezargus.library.logging.rst
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/source/code/lezargus.library.math.rst
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/source/code/lezargus.library.path.rst
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/source/code/lezargus.library.photometry.rst
+-rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/source/code/lezargus.library.rst
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/source/code/lezargus.library.stitch.rst
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/source/code/lezargus.library.temporary.rst
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/source/code/lezargus.library.wrapper.rst
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/source/code/lezargus.rst
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/source/code/lezargus.simulation.rst
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/source/code/lezargus.simulation.spectre.rst
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/source/code/modules.rst
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/source/technical/atmosphere.rst
+-rw-r--r--   0        0        0    13857 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/source/technical/contributing.rst
+-rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/source/technical/convention.rst
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/source/technical/index.rst
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/source/technical/photometry.rst
+-rw-r--r--   0        0        0     3485 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/source/technical/uncertainty.rst
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/docs/source/user/index.rst
+-rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/src/lezargus/__init__.py
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/src/lezargus/__main__.py
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/src/lezargus/__version__.py
+-rw-r--r--   0        0        0     4937 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/src/lezargus/configuration.yaml
+-rw-r--r--   0        0        0    26180 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/src/lezargus/initialize.py
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/src/lezargus/container/__init__.py
+-rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/src/lezargus/container/atmosphere.py
+-rw-r--r--   0        0        0    17250 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/src/lezargus/container/broadcast.py
+-rw-r--r--   0        0        0    10234 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/src/lezargus/container/cube.py
+-rw-r--r--   0        0        0     5834 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/src/lezargus/container/image.py
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/src/lezargus/container/mosaic.py
+-rw-r--r--   0        0        0    29824 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/src/lezargus/container/parent.py
+-rw-r--r--   0        0        0    19693 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/src/lezargus/container/spectrum.py
+-rw-r--r--   0        0        0   144000 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/src/lezargus/data/atm_rad_za0.fits
+-rw-r--r--   0        0        0   144000 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/src/lezargus/data/atm_rad_za30.fits
+-rw-r--r--   0        0        0   144000 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/src/lezargus/data/atm_rad_za45.fits
+-rw-r--r--   0        0        0   144000 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/src/lezargus/data/atm_rad_za60.fits
+-rw-r--r--   0        0        0   144000 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/src/lezargus/data/atm_trans_za0.fits
+-rw-r--r--   0        0        0   144000 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/src/lezargus/data/atm_trans_za30.fits
+-rw-r--r--   0        0        0   144000 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/src/lezargus/data/atm_trans_za45.fits
+-rw-r--r--   0        0        0   144000 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/src/lezargus/data/atm_trans_za60.fits
+-rw-r--r--   0        0        0    31680 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/src/lezargus/data/filter_2MASS_H_energy.fits
+-rw-r--r--   0        0        0    31680 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/src/lezargus/data/filter_2MASS_H_photon.fits
+-rw-r--r--   0        0        0    31680 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/src/lezargus/data/filter_2MASS_J_energy.fits
+-rw-r--r--   0        0        0    31680 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/src/lezargus/data/filter_2MASS_J_photon.fits
+-rw-r--r--   0        0        0    31680 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/src/lezargus/data/filter_2MASS_Ks_energy.fits
+-rw-r--r--   0        0        0    31680 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/src/lezargus/data/filter_2MASS_Ks_photon.fits
+-rw-r--r--   0        0        0    40320 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/src/lezargus/data/filter_Gaia_GB_energy.fits
+-rw-r--r--   0        0        0    40320 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/src/lezargus/data/filter_Gaia_GB_photon.fits
+-rw-r--r--   0        0        0    51840 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/src/lezargus/data/filter_Gaia_GG_energy.fits
+-rw-r--r--   0        0        0    51840 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/src/lezargus/data/filter_Gaia_GG_photon.fits
+-rw-r--r--   0        0        0    40320 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/src/lezargus/data/filter_Gaia_GR_energy.fits
+-rw-r--r--   0        0        0    40320 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/src/lezargus/data/filter_Gaia_GR_photon.fits
+-rw-r--r--   0        0        0    31680 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/src/lezargus/data/filter_Johnson_B_energy.fits
+-rw-r--r--   0        0        0    31680 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/src/lezargus/data/filter_Johnson_B_photon.fits
+-rw-r--r--   0        0        0    31680 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/src/lezargus/data/filter_Johnson_U_energy.fits
+-rw-r--r--   0        0        0    31680 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/src/lezargus/data/filter_Johnson_U_photon.fits
+-rw-r--r--   0        0        0    31680 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/src/lezargus/data/filter_Johnson_V_energy.fits
+-rw-r--r--   0        0        0    31680 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/src/lezargus/data/filter_Johnson_V_photon.fits
+-rw-r--r--   0        0        0  6837120 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/src/lezargus/data/gem_atm_ir_rad.fits
+-rw-r--r--   0        0        0    92160 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/src/lezargus/data/gem_atm_opt_rad.fits
+-rw-r--r--   0        0        0   144000 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/src/lezargus/data/psg_atm_rad_za0.fits
+-rw-r--r--   0        0        0   144000 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/src/lezargus/data/psg_atm_rad_za30.fits
+-rw-r--r--   0        0        0   144000 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/src/lezargus/data/psg_atm_rad_za45.fits
+-rw-r--r--   0        0        0   144000 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/src/lezargus/data/psg_atm_rad_za60.fits
+-rw-r--r--   0        0        0   144000 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/src/lezargus/data/psg_atm_trans_za0.fits
+-rw-r--r--   0        0        0   144000 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/src/lezargus/data/psg_atm_trans_za30.fits
+-rw-r--r--   0        0        0   144000 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/src/lezargus/data/psg_atm_trans_za45.fits
+-rw-r--r--   0        0        0   144000 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/src/lezargus/data/psg_atm_trans_za60.fits
+-rw-r--r--   0        0        0   126720 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/src/lezargus/data/star_spectra_109Vir.fits
+-rw-r--r--   0        0        0   126720 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/src/lezargus/data/star_spectra_16CygB.fits
+-rw-r--r--   0        0        0   103680 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/src/lezargus/data/star_spectra_A0V.fits
+-rw-r--r--   0        0        0    54720 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/src/lezargus/data/star_spectra_Sun.fits
+-rw-r--r--   0        0        0   120960 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/src/lezargus/data/star_spectra_Vega.fits
+-rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/src/lezargus/library/__init__.py
+-rw-r--r--   0        0        0     8353 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/src/lezargus/library/array.py
+-rw-r--r--   0        0        0    12850 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/src/lezargus/library/atmosphere.py
+-rw-r--r--   0        0        0    20520 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/src/lezargus/library/config.py
+-rw-r--r--   0        0        0     3983 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/src/lezargus/library/conversion.py
+-rw-r--r--   0        0        0    21789 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/src/lezargus/library/convolution.py
+-rw-r--r--   0        0        0     5690 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/src/lezargus/library/data.py
+-rw-r--r--   0        0        0    25156 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/src/lezargus/library/fits.py
+-rw-r--r--   0        0        0     2741 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/src/lezargus/library/flags.py
+-rw-r--r--   0        0        0     1954 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/src/lezargus/library/hint.py
+-rw-r--r--   0        0        0    50311 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/src/lezargus/library/interpolate.py
+-rw-r--r--   0        0        0    25383 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/src/lezargus/library/logging.py
+-rw-r--r--   0        0        0    22739 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/src/lezargus/library/math.py
+-rw-r--r--   0        0        0     8796 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/src/lezargus/library/path.py
+-rw-r--r--   0        0        0    14173 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/src/lezargus/library/photometry.py
+-rw-r--r--   0        0        0     8496 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/src/lezargus/library/sanitize.py
+-rw-r--r--   0        0        0    32549 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/src/lezargus/library/stitch.py
+-rw-r--r--   0        0        0     7659 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/src/lezargus/library/temporary.py
+-rw-r--r--   0        0        0     7706 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/src/lezargus/library/wrapper.py
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/src/lezargus/simulation/__init__.py
+-rw-r--r--   0        0        0    38027 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/src/lezargus/simulation/spectre.py
+-rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/tests/conftest.py
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/tests/test_configuration_overrides.yaml
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/tests/test_init.py
+-rw-r--r--   0        0        0     3588 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/tests/test_library_config.py
+-rw-r--r--   0        0        0     4044 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/tests/test_library_logging.py
+-rw-r--r--   0        0        0    12328 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/tests/test_library_path.py
+-rw-r--r--   0        0        0     3539 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/tests/test_library_wrapper.py
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/tests/test_files/config_filename_not_flat_configuration.yaml
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/tests/test_files/config_filename_with_lowercase_keys.yaml
+-rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/LICENSE.txt
+-rw-r--r--   0        0        0     3026 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/README.md
+-rw-r--r--   0        0        0     5853 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/pyproject.toml
+-rw-r--r--   0        0        0     4057 2020-02-02 00:00:00.000000 lezargus-0.0.4.dev51/PKG-INFO
```

### Comparing `lezargus-0.0.4.dev44/.gitattributes` & `lezargus-0.0.4.dev51/.gitattributes`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/SECURITY.md` & `lezargus-0.0.4.dev51/SECURITY.md`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/rebuild.ps1` & `lezargus-0.0.4.dev51/rebuild.ps1`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/.github/workflows/format.yaml` & `lezargus-0.0.4.dev51/.github/workflows/format.yaml`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/.github/workflows/lint.yaml` & `lezargus-0.0.4.dev51/.github/workflows/lint.yaml`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/.github/workflows/publish.yaml` & `lezargus-0.0.4.dev51/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/.github/workflows/tests.yaml` & `lezargus-0.0.4.dev51/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/Makefile` & `lezargus-0.0.4.dev51/docs/Makefile`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/make.bat` & `lezargus-0.0.4.dev51/docs/make.bat`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/genindex.html` & `lezargus-0.0.4.dev51/docs/build/html/genindex.html`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/index.html` & `lezargus-0.0.4.dev51/docs/build/html/index.html`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/objects.inv` & `lezargus-0.0.4.dev51/docs/build/html/objects.inv`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/py-modindex.html` & `lezargus-0.0.4.dev51/docs/build/html/py-modindex.html`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/search.html` & `lezargus-0.0.4.dev51/docs/build/html/search.html`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/searchindex.js` & `lezargus-0.0.4.dev51/docs/build/html/searchindex.js`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/.doctrees/environment.pickle` & `lezargus-0.0.4.dev51/docs/build/html/.doctrees/environment.pickle`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/.doctrees/index.doctree` & `lezargus-0.0.4.dev51/docs/build/html/.doctrees/index.doctree`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/.doctrees/code/lezargus.__main__.doctree` & `lezargus-0.0.4.dev51/docs/build/html/.doctrees/code/lezargus.__main__.doctree`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/.doctrees/code/lezargus.__version__.doctree` & `lezargus-0.0.4.dev51/docs/build/html/.doctrees/code/lezargus.__version__.doctree`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/.doctrees/code/lezargus.container.broadcast.doctree` & `lezargus-0.0.4.dev51/docs/build/html/.doctrees/code/lezargus.container.broadcast.doctree`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/.doctrees/code/lezargus.container.cube.doctree` & `lezargus-0.0.4.dev51/docs/build/html/.doctrees/code/lezargus.container.cube.doctree`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/.doctrees/code/lezargus.container.doctree` & `lezargus-0.0.4.dev51/docs/build/html/.doctrees/code/lezargus.container.doctree`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/.doctrees/code/lezargus.container.image.doctree` & `lezargus-0.0.4.dev51/docs/build/html/.doctrees/code/lezargus.container.image.doctree`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/.doctrees/code/lezargus.container.mosaic.doctree` & `lezargus-0.0.4.dev51/docs/build/html/.doctrees/code/lezargus.container.mosaic.doctree`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/.doctrees/code/lezargus.container.parent.doctree` & `lezargus-0.0.4.dev51/docs/build/html/.doctrees/code/lezargus.container.parent.doctree`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/.doctrees/code/lezargus.container.spectra.doctree` & `lezargus-0.0.4.dev51/docs/build/html/.doctrees/code/lezargus.container.spectra.doctree`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/.doctrees/code/lezargus.doctree` & `lezargus-0.0.4.dev51/docs/build/html/.doctrees/code/lezargus.doctree`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/.doctrees/code/lezargus.initialize.doctree` & `lezargus-0.0.4.dev51/docs/build/html/.doctrees/code/lezargus.initialize.doctree`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/.doctrees/code/lezargus.library.array.doctree` & `lezargus-0.0.4.dev51/docs/build/html/.doctrees/code/lezargus.library.array.doctree`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/.doctrees/code/lezargus.library.atmosphere.doctree` & `lezargus-0.0.4.dev51/docs/build/html/.doctrees/code/lezargus.library.atmosphere.doctree`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/.doctrees/code/lezargus.library.config.doctree` & `lezargus-0.0.4.dev51/docs/build/html/.doctrees/code/lezargus.library.config.doctree`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/.doctrees/code/lezargus.library.conversion.doctree` & `lezargus-0.0.4.dev51/docs/build/html/.doctrees/code/lezargus.library.conversion.doctree`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/.doctrees/code/lezargus.library.convolution.doctree` & `lezargus-0.0.4.dev51/docs/build/html/.doctrees/code/lezargus.library.convolution.doctree`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/.doctrees/code/lezargus.library.data.doctree` & `lezargus-0.0.4.dev51/docs/build/html/.doctrees/code/lezargus.library.data.doctree`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/.doctrees/code/lezargus.library.doctree` & `lezargus-0.0.4.dev51/docs/build/html/.doctrees/code/lezargus.library.doctree`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/.doctrees/code/lezargus.library.fits.doctree` & `lezargus-0.0.4.dev51/docs/build/html/.doctrees/code/lezargus.library.fits.doctree`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/.doctrees/code/lezargus.library.flags.doctree` & `lezargus-0.0.4.dev51/docs/build/html/.doctrees/code/lezargus.library.flags.doctree`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/.doctrees/code/lezargus.library.hint.doctree` & `lezargus-0.0.4.dev51/docs/build/html/.doctrees/code/lezargus.library.hint.doctree`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/.doctrees/code/lezargus.library.interpolate.doctree` & `lezargus-0.0.4.dev51/docs/build/html/.doctrees/code/lezargus.library.interpolate.doctree`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/.doctrees/code/lezargus.library.logging.doctree` & `lezargus-0.0.4.dev51/docs/build/html/.doctrees/code/lezargus.library.logging.doctree`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/.doctrees/code/lezargus.library.math.doctree` & `lezargus-0.0.4.dev51/docs/build/html/.doctrees/code/lezargus.library.math.doctree`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/.doctrees/code/lezargus.library.path.doctree` & `lezargus-0.0.4.dev51/docs/build/html/.doctrees/code/lezargus.library.path.doctree`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/.doctrees/code/lezargus.library.photometry.doctree` & `lezargus-0.0.4.dev51/docs/build/html/.doctrees/code/lezargus.library.photometry.doctree`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/.doctrees/code/lezargus.library.stitch.doctree` & `lezargus-0.0.4.dev51/docs/build/html/.doctrees/code/lezargus.library.stitch.doctree`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/.doctrees/code/lezargus.library.temporary.doctree` & `lezargus-0.0.4.dev51/docs/build/html/.doctrees/code/lezargus.library.temporary.doctree`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/.doctrees/code/lezargus.library.uncertainty.doctree` & `lezargus-0.0.4.dev51/docs/build/html/.doctrees/code/lezargus.library.uncertainty.doctree`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/.doctrees/code/lezargus.library.wrapper.doctree` & `lezargus-0.0.4.dev51/docs/build/html/.doctrees/code/lezargus.library.wrapper.doctree`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/.doctrees/code/lezargus.simulation.doctree` & `lezargus-0.0.4.dev51/docs/build/html/.doctrees/code/lezargus.simulation.doctree`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/.doctrees/code/lezargus.simulation.spectre.doctree` & `lezargus-0.0.4.dev51/docs/build/html/.doctrees/code/lezargus.simulation.spectre.doctree`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/.doctrees/code/modules.doctree` & `lezargus-0.0.4.dev51/docs/build/html/.doctrees/code/modules.doctree`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/.doctrees/technical/contributing.doctree` & `lezargus-0.0.4.dev51/docs/build/html/.doctrees/technical/contributing.doctree`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/.doctrees/technical/convention.doctree` & `lezargus-0.0.4.dev51/docs/build/html/.doctrees/technical/convention.doctree`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/.doctrees/technical/index.doctree` & `lezargus-0.0.4.dev51/docs/build/html/.doctrees/technical/index.doctree`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/.doctrees/technical/photometry.doctree` & `lezargus-0.0.4.dev51/docs/build/html/.doctrees/technical/photometry.doctree`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/.doctrees/technical/synthetic_photometry.doctree` & `lezargus-0.0.4.dev51/docs/build/html/.doctrees/technical/synthetic_photometry.doctree`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/.doctrees/technical/uncertainty.doctree` & `lezargus-0.0.4.dev51/docs/build/html/.doctrees/technical/uncertainty.doctree`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/.doctrees/user/index.doctree` & `lezargus-0.0.4.dev51/docs/build/html/.doctrees/user/index.doctree`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/_modules/index.html` & `lezargus-0.0.4.dev51/docs/build/html/_modules/index.html`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/_modules/lezargus/initialize.html` & `lezargus-0.0.4.dev51/docs/build/html/_modules/lezargus/initialize.html`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/_modules/lezargus/container/broadcast.html` & `lezargus-0.0.4.dev51/docs/build/html/_modules/lezargus/container/broadcast.html`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/_modules/lezargus/container/cube.html` & `lezargus-0.0.4.dev51/docs/build/html/_modules/lezargus/container/cube.html`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/_modules/lezargus/container/image.html` & `lezargus-0.0.4.dev51/docs/build/html/_modules/lezargus/container/image.html`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/_modules/lezargus/container/mosaic.html` & `lezargus-0.0.4.dev51/docs/build/html/_modules/lezargus/container/mosaic.html`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/_modules/lezargus/container/parent.html` & `lezargus-0.0.4.dev51/docs/build/html/_modules/lezargus/container/parent.html`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/_modules/lezargus/container/spectra.html` & `lezargus-0.0.4.dev51/docs/build/html/_modules/lezargus/container/spectra.html`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/_modules/lezargus/library/array.html` & `lezargus-0.0.4.dev51/docs/build/html/_modules/lezargus/library/array.html`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/_modules/lezargus/library/atmosphere.html` & `lezargus-0.0.4.dev51/docs/build/html/_modules/lezargus/library/atmosphere.html`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/_modules/lezargus/library/config.html` & `lezargus-0.0.4.dev51/docs/build/html/_modules/lezargus/library/config.html`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/_modules/lezargus/library/conversion.html` & `lezargus-0.0.4.dev51/docs/build/html/_modules/lezargus/library/conversion.html`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/_modules/lezargus/library/convolution.html` & `lezargus-0.0.4.dev51/docs/build/html/_modules/lezargus/library/convolution.html`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/_modules/lezargus/library/data.html` & `lezargus-0.0.4.dev51/docs/build/html/_modules/lezargus/library/data.html`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/_modules/lezargus/library/fits.html` & `lezargus-0.0.4.dev51/docs/build/html/_modules/lezargus/library/fits.html`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/_modules/lezargus/library/flags.html` & `lezargus-0.0.4.dev51/docs/build/html/_modules/lezargus/library/flags.html`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/_modules/lezargus/library/interpolate.html` & `lezargus-0.0.4.dev51/docs/build/html/_modules/lezargus/library/interpolate.html`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/_modules/lezargus/library/logging.html` & `lezargus-0.0.4.dev51/docs/build/html/_modules/lezargus/library/logging.html`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/_modules/lezargus/library/math.html` & `lezargus-0.0.4.dev51/docs/build/html/_modules/lezargus/library/math.html`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/_modules/lezargus/library/path.html` & `lezargus-0.0.4.dev51/docs/build/html/_modules/lezargus/library/path.html`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/_modules/lezargus/library/photometry.html` & `lezargus-0.0.4.dev51/docs/build/html/_modules/lezargus/library/photometry.html`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/_modules/lezargus/library/stitch.html` & `lezargus-0.0.4.dev51/docs/build/html/_modules/lezargus/library/stitch.html`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/_modules/lezargus/library/temporary.html` & `lezargus-0.0.4.dev51/docs/build/html/_modules/lezargus/library/temporary.html`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/_modules/lezargus/library/uncertainty.html` & `lezargus-0.0.4.dev51/docs/build/html/_modules/lezargus/library/uncertainty.html`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/_modules/lezargus/library/wrapper.html` & `lezargus-0.0.4.dev51/docs/build/html/_modules/lezargus/library/wrapper.html`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/_modules/lezargus/simulation/spectre.html` & `lezargus-0.0.4.dev51/docs/build/html/_modules/lezargus/simulation/spectre.html`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/_sources/index.rst` & `lezargus-0.0.4.dev51/docs/build/html/_sources/index.rst`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/_sources/code/lezargus.library.rst` & `lezargus-0.0.4.dev51/docs/build/html/_sources/code/lezargus.library.rst`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/_sources/technical/contributing.rst` & `lezargus-0.0.4.dev51/docs/build/html/_sources/technical/contributing.rst`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/_sources/technical/convention.rst` & `lezargus-0.0.4.dev51/docs/build/html/_sources/technical/convention.rst`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/_sources/technical/uncertainty.rst` & `lezargus-0.0.4.dev51/docs/build/html/_sources/technical/uncertainty.rst`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/_static/basic.css` & `lezargus-0.0.4.dev51/docs/build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/_static/doctools.js` & `lezargus-0.0.4.dev51/docs/build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/_static/language_data.js` & `lezargus-0.0.4.dev51/docs/build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/_static/pygments.css` & `lezargus-0.0.4.dev51/docs/build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/_static/searchtools.js` & `lezargus-0.0.4.dev51/docs/build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/_static/sphinx_highlight.js` & `lezargus-0.0.4.dev51/docs/build/html/_static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/_static/webpack-macros.html` & `lezargus-0.0.4.dev51/docs/build/html/_static/webpack-macros.html`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/_static/images/logo_binder.svg` & `lezargus-0.0.4.dev51/docs/build/html/_static/images/logo_binder.svg`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/_static/images/logo_colab.png` & `lezargus-0.0.4.dev51/docs/build/html/_static/images/logo_colab.png`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/_static/images/logo_deepnote.svg` & `lezargus-0.0.4.dev51/docs/build/html/_static/images/logo_deepnote.svg`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/_static/images/logo_jupyterhub.svg` & `lezargus-0.0.4.dev51/docs/build/html/_static/images/logo_jupyterhub.svg`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/_static/locales/ar/LC_MESSAGES/booktheme.po` & `lezargus-0.0.4.dev51/docs/build/html/_static/locales/ar/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/_static/locales/bg/LC_MESSAGES/booktheme.po` & `lezargus-0.0.4.dev51/docs/build/html/_static/locales/bg/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/_static/locales/bn/LC_MESSAGES/booktheme.po` & `lezargus-0.0.4.dev51/docs/build/html/_static/locales/bn/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/_static/locales/ca/LC_MESSAGES/booktheme.po` & `lezargus-0.0.4.dev51/docs/build/html/_static/locales/ca/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/_static/locales/cs/LC_MESSAGES/booktheme.po` & `lezargus-0.0.4.dev51/docs/build/html/_static/locales/cs/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/_static/locales/da/LC_MESSAGES/booktheme.po` & `lezargus-0.0.4.dev51/docs/build/html/_static/locales/da/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/_static/locales/de/LC_MESSAGES/booktheme.po` & `lezargus-0.0.4.dev51/docs/build/html/_static/locales/de/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/_static/locales/el/LC_MESSAGES/booktheme.po` & `lezargus-0.0.4.dev51/docs/build/html/_static/locales/el/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/_static/locales/eo/LC_MESSAGES/booktheme.po` & `lezargus-0.0.4.dev51/docs/build/html/_static/locales/eo/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/_static/locales/es/LC_MESSAGES/booktheme.po` & `lezargus-0.0.4.dev51/docs/build/html/_static/locales/es/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/_static/locales/et/LC_MESSAGES/booktheme.po` & `lezargus-0.0.4.dev51/docs/build/html/_static/locales/et/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/_static/locales/fi/LC_MESSAGES/booktheme.po` & `lezargus-0.0.4.dev51/docs/build/html/_static/locales/fi/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/_static/locales/fr/LC_MESSAGES/booktheme.po` & `lezargus-0.0.4.dev51/docs/build/html/_static/locales/fr/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/_static/locales/hr/LC_MESSAGES/booktheme.po` & `lezargus-0.0.4.dev51/docs/build/html/_static/locales/hr/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/_static/locales/id/LC_MESSAGES/booktheme.po` & `lezargus-0.0.4.dev51/docs/build/html/_static/locales/id/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/_static/locales/it/LC_MESSAGES/booktheme.po` & `lezargus-0.0.4.dev51/docs/build/html/_static/locales/it/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/_static/locales/iw/LC_MESSAGES/booktheme.po` & `lezargus-0.0.4.dev51/docs/build/html/_static/locales/iw/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/_static/locales/ja/LC_MESSAGES/booktheme.po` & `lezargus-0.0.4.dev51/docs/build/html/_static/locales/ja/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/_static/locales/ko/LC_MESSAGES/booktheme.po` & `lezargus-0.0.4.dev51/docs/build/html/_static/locales/ko/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/_static/locales/lt/LC_MESSAGES/booktheme.po` & `lezargus-0.0.4.dev51/docs/build/html/_static/locales/lt/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/_static/locales/lv/LC_MESSAGES/booktheme.po` & `lezargus-0.0.4.dev51/docs/build/html/_static/locales/lv/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/_static/locales/ml/LC_MESSAGES/booktheme.po` & `lezargus-0.0.4.dev51/docs/build/html/_static/locales/ml/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/_static/locales/mr/LC_MESSAGES/booktheme.po` & `lezargus-0.0.4.dev51/docs/build/html/_static/locales/mr/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/_static/locales/ms/LC_MESSAGES/booktheme.po` & `lezargus-0.0.4.dev51/docs/build/html/_static/locales/ms/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/_static/locales/nl/LC_MESSAGES/booktheme.po` & `lezargus-0.0.4.dev51/docs/build/html/_static/locales/nl/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/_static/locales/no/LC_MESSAGES/booktheme.po` & `lezargus-0.0.4.dev51/docs/build/html/_static/locales/no/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/_static/locales/pl/LC_MESSAGES/booktheme.po` & `lezargus-0.0.4.dev51/docs/build/html/_static/locales/pl/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/_static/locales/pt/LC_MESSAGES/booktheme.po` & `lezargus-0.0.4.dev51/docs/build/html/_static/locales/pt/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/_static/locales/ro/LC_MESSAGES/booktheme.po` & `lezargus-0.0.4.dev51/docs/build/html/_static/locales/ro/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/_static/locales/ru/LC_MESSAGES/booktheme.po` & `lezargus-0.0.4.dev51/docs/build/html/_static/locales/ru/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/_static/locales/sk/LC_MESSAGES/booktheme.po` & `lezargus-0.0.4.dev51/docs/build/html/_static/locales/sk/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/_static/locales/sl/LC_MESSAGES/booktheme.po` & `lezargus-0.0.4.dev51/docs/build/html/_static/locales/sl/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/_static/locales/sr/LC_MESSAGES/booktheme.po` & `lezargus-0.0.4.dev51/docs/build/html/_static/locales/sr/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/_static/locales/sv/LC_MESSAGES/booktheme.po` & `lezargus-0.0.4.dev51/docs/build/html/_static/locales/sv/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/_static/locales/ta/LC_MESSAGES/booktheme.po` & `lezargus-0.0.4.dev51/docs/build/html/_static/locales/ta/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/_static/locales/te/LC_MESSAGES/booktheme.po` & `lezargus-0.0.4.dev51/docs/build/html/_static/locales/te/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/_static/locales/tg/LC_MESSAGES/booktheme.po` & `lezargus-0.0.4.dev51/docs/build/html/_static/locales/tg/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/_static/locales/th/LC_MESSAGES/booktheme.po` & `lezargus-0.0.4.dev51/docs/build/html/_static/locales/th/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/_static/locales/tl/LC_MESSAGES/booktheme.po` & `lezargus-0.0.4.dev51/docs/build/html/_static/locales/tl/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/_static/locales/tr/LC_MESSAGES/booktheme.po` & `lezargus-0.0.4.dev51/docs/build/html/_static/locales/tr/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/_static/locales/uk/LC_MESSAGES/booktheme.po` & `lezargus-0.0.4.dev51/docs/build/html/_static/locales/uk/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/_static/locales/ur/LC_MESSAGES/booktheme.po` & `lezargus-0.0.4.dev51/docs/build/html/_static/locales/ur/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/_static/locales/vi/LC_MESSAGES/booktheme.po` & `lezargus-0.0.4.dev51/docs/build/html/_static/locales/vi/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/_static/locales/zh_CN/LC_MESSAGES/booktheme.po` & `lezargus-0.0.4.dev51/docs/build/html/_static/locales/zh_CN/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/_static/locales/zh_TW/LC_MESSAGES/booktheme.po` & `lezargus-0.0.4.dev51/docs/build/html/_static/locales/zh_TW/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/_static/scripts/bootstrap.js` & `lezargus-0.0.4.dev51/docs/build/html/_static/scripts/bootstrap.js`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/_static/scripts/bootstrap.js.map` & `lezargus-0.0.4.dev51/docs/build/html/_static/scripts/bootstrap.js.map`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/_static/scripts/pydata-sphinx-theme.js` & `lezargus-0.0.4.dev51/docs/build/html/_static/scripts/pydata-sphinx-theme.js`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/_static/scripts/pydata-sphinx-theme.js.map` & `lezargus-0.0.4.dev51/docs/build/html/_static/scripts/pydata-sphinx-theme.js.map`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/_static/scripts/sphinx-book-theme.js` & `lezargus-0.0.4.dev51/docs/build/html/_static/scripts/sphinx-book-theme.js`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/_static/scripts/sphinx-book-theme.js.map` & `lezargus-0.0.4.dev51/docs/build/html/_static/scripts/sphinx-book-theme.js.map`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/_static/styles/bootstrap.css` & `lezargus-0.0.4.dev51/docs/build/html/_static/styles/bootstrap.css`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/_static/styles/bootstrap.css.map` & `lezargus-0.0.4.dev51/docs/build/html/_static/styles/bootstrap.css.map`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/_static/styles/pydata-sphinx-theme.css` & `lezargus-0.0.4.dev51/docs/build/html/_static/styles/pydata-sphinx-theme.css`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/_static/styles/pydata-sphinx-theme.css.map` & `lezargus-0.0.4.dev51/docs/build/html/_static/styles/pydata-sphinx-theme.css.map`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/_static/styles/sphinx-book-theme.css` & `lezargus-0.0.4.dev51/docs/build/html/_static/styles/sphinx-book-theme.css`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/_static/vendor/fontawesome/6.1.2/LICENSE.txt` & `lezargus-0.0.4.dev51/docs/build/html/_static/vendor/fontawesome/6.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/_static/vendor/fontawesome/6.1.2/css/all.min.css` & `lezargus-0.0.4.dev51/docs/build/html/_static/vendor/fontawesome/6.1.2/css/all.min.css`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/_static/vendor/fontawesome/6.1.2/js/all.min.js` & `lezargus-0.0.4.dev51/docs/build/html/_static/vendor/fontawesome/6.1.2/js/all.min.js`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.ttf` & `lezargus-0.0.4.dev51/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.woff2` & `lezargus-0.0.4.dev51/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.ttf` & `lezargus-0.0.4.dev51/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.woff2` & `lezargus-0.0.4.dev51/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.ttf` & `lezargus-0.0.4.dev51/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.woff2` & `lezargus-0.0.4.dev51/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.ttf` & `lezargus-0.0.4.dev51/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.ttf`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.woff2` & `lezargus-0.0.4.dev51/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.woff2`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/_static/vendor/fontawesome/6.5.1/LICENSE.txt` & `lezargus-0.0.4.dev51/docs/build/html/_static/vendor/fontawesome/6.5.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/_static/vendor/fontawesome/6.5.1/css/all.min.css` & `lezargus-0.0.4.dev51/docs/build/html/_static/vendor/fontawesome/6.5.1/css/all.min.css`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/_static/vendor/fontawesome/6.5.1/js/all.min.js` & `lezargus-0.0.4.dev51/docs/build/html/_static/vendor/fontawesome/6.5.1/js/all.min.js`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-brands-400.ttf` & `lezargus-0.0.4.dev51/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-brands-400.woff2` & `lezargus-0.0.4.dev51/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-regular-400.ttf` & `lezargus-0.0.4.dev51/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-regular-400.woff2` & `lezargus-0.0.4.dev51/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-solid-900.ttf` & `lezargus-0.0.4.dev51/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-solid-900.woff2` & `lezargus-0.0.4.dev51/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-v4compatibility.ttf` & `lezargus-0.0.4.dev51/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-v4compatibility.ttf`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-v4compatibility.woff2` & `lezargus-0.0.4.dev51/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-v4compatibility.woff2`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/code/lezargus.__main__.html` & `lezargus-0.0.4.dev51/docs/build/html/code/lezargus.__main__.html`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/code/lezargus.__version__.html` & `lezargus-0.0.4.dev51/docs/build/html/code/lezargus.__version__.html`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/code/lezargus.container.broadcast.html` & `lezargus-0.0.4.dev51/docs/build/html/code/lezargus.container.broadcast.html`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/code/lezargus.container.cube.html` & `lezargus-0.0.4.dev51/docs/build/html/code/lezargus.container.cube.html`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/code/lezargus.container.html` & `lezargus-0.0.4.dev51/docs/build/html/code/lezargus.container.html`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/code/lezargus.container.image.html` & `lezargus-0.0.4.dev51/docs/build/html/code/lezargus.container.image.html`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/code/lezargus.container.mosaic.html` & `lezargus-0.0.4.dev51/docs/build/html/code/lezargus.container.mosaic.html`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/code/lezargus.container.parent.html` & `lezargus-0.0.4.dev51/docs/build/html/code/lezargus.container.parent.html`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/code/lezargus.container.spectra.html` & `lezargus-0.0.4.dev51/docs/build/html/code/lezargus.container.spectra.html`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/code/lezargus.html` & `lezargus-0.0.4.dev51/docs/build/html/code/lezargus.html`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/code/lezargus.initialize.html` & `lezargus-0.0.4.dev51/docs/build/html/code/lezargus.initialize.html`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/code/lezargus.library.array.html` & `lezargus-0.0.4.dev51/docs/build/html/code/lezargus.library.array.html`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/code/lezargus.library.atmosphere.html` & `lezargus-0.0.4.dev51/docs/build/html/code/lezargus.library.atmosphere.html`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/code/lezargus.library.config.html` & `lezargus-0.0.4.dev51/docs/build/html/code/lezargus.library.config.html`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/code/lezargus.library.conversion.html` & `lezargus-0.0.4.dev51/docs/build/html/code/lezargus.library.conversion.html`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/code/lezargus.library.convolution.html` & `lezargus-0.0.4.dev51/docs/build/html/code/lezargus.library.convolution.html`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/code/lezargus.library.data.html` & `lezargus-0.0.4.dev51/docs/build/html/code/lezargus.library.data.html`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/code/lezargus.library.fits.html` & `lezargus-0.0.4.dev51/docs/build/html/code/lezargus.library.fits.html`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/code/lezargus.library.flags.html` & `lezargus-0.0.4.dev51/docs/build/html/code/lezargus.library.flags.html`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/code/lezargus.library.hint.html` & `lezargus-0.0.4.dev51/docs/build/html/code/lezargus.library.hint.html`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/code/lezargus.library.html` & `lezargus-0.0.4.dev51/docs/build/html/code/lezargus.library.html`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/code/lezargus.library.interpolate.html` & `lezargus-0.0.4.dev51/docs/build/html/code/lezargus.library.interpolate.html`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/code/lezargus.library.logging.html` & `lezargus-0.0.4.dev51/docs/build/html/code/lezargus.library.logging.html`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/code/lezargus.library.math.html` & `lezargus-0.0.4.dev51/docs/build/html/code/lezargus.library.math.html`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/code/lezargus.library.path.html` & `lezargus-0.0.4.dev51/docs/build/html/code/lezargus.library.path.html`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/code/lezargus.library.photometry.html` & `lezargus-0.0.4.dev51/docs/build/html/code/lezargus.library.photometry.html`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/code/lezargus.library.stitch.html` & `lezargus-0.0.4.dev51/docs/build/html/code/lezargus.library.stitch.html`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/code/lezargus.library.temporary.html` & `lezargus-0.0.4.dev51/docs/build/html/code/lezargus.library.temporary.html`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/code/lezargus.library.uncertainty.html` & `lezargus-0.0.4.dev51/docs/build/html/code/lezargus.library.uncertainty.html`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/code/lezargus.library.wrapper.html` & `lezargus-0.0.4.dev51/docs/build/html/code/lezargus.library.wrapper.html`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/code/lezargus.simulation.html` & `lezargus-0.0.4.dev51/docs/build/html/code/lezargus.simulation.html`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/code/lezargus.simulation.spectre.html` & `lezargus-0.0.4.dev51/docs/build/html/code/lezargus.simulation.spectre.html`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/code/modules.html` & `lezargus-0.0.4.dev51/docs/build/html/code/modules.html`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/technical/contributing.html` & `lezargus-0.0.4.dev51/docs/build/html/technical/contributing.html`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/technical/convention.html` & `lezargus-0.0.4.dev51/docs/build/html/technical/convention.html`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/technical/index.html` & `lezargus-0.0.4.dev51/docs/build/html/technical/index.html`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/technical/photometry.html` & `lezargus-0.0.4.dev51/docs/build/html/technical/photometry.html`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/technical/synthetic_photometry.html` & `lezargus-0.0.4.dev51/docs/build/html/technical/synthetic_photometry.html`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/technical/uncertainty.html` & `lezargus-0.0.4.dev51/docs/build/html/technical/uncertainty.html`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/build/html/user/index.html` & `lezargus-0.0.4.dev51/docs/build/html/user/index.html`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/source/conf.py` & `lezargus-0.0.4.dev51/docs/source/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # Configuration file for the Sphinx documentation builder.
 #
 # For the full list of built-in configuration values, see the documentation:
 # https://www.sphinx-doc.org/en/master/usage/configuration.html
 
 import os
 import sys
-import sphinx_book_theme
 
 # For the Python code itself.
 sys.path.insert(0, os.path.abspath(os.path.join("..", "..", "src")))
 
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
```

### Comparing `lezargus-0.0.4.dev44/docs/source/index.rst` & `lezargus-0.0.4.dev51/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/source/code/lezargus.library.rst` & `lezargus-0.0.4.dev51/docs/source/code/lezargus.library.rst`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/source/technical/contributing.rst` & `lezargus-0.0.4.dev51/docs/source/technical/contributing.rst`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/source/technical/convention.rst` & `lezargus-0.0.4.dev51/docs/source/technical/convention.rst`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/docs/source/technical/uncertainty.rst` & `lezargus-0.0.4.dev51/docs/source/technical/uncertainty.rst`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/src/lezargus/__init__.py` & `lezargus-0.0.4.dev51/src/lezargus/__init__.py`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/src/lezargus/configuration.yaml` & `lezargus-0.0.4.dev51/src/lezargus/configuration.yaml`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/src/lezargus/initialize.py` & `lezargus-0.0.4.dev51/src/lezargus/initialize.py`

 * *Files 26% similar despite different names*

```diff
@@ -47,20 +47,15 @@
             critical_type=logging.InputError,
             message=(
                 "Initialization cannot have positional arguments, use keyword"
                 " arguments."
             ),
         )
     # This is to "use" the kwarg parameter, nothing much else.
-    if len(kwargs) != 0:
-        logging.debug(
-            message=(
-                "Overriding keyword parameters to full initialization present."
-            ),
-        )
+    lezargus.library.wrapper.do_nothing(**kwargs)
 
     # Load in the default configuration file.
     initialize_configuration(**kwargs)
 
     # Load the logging outputs.
     initialize_logging_outputs(**kwargs)
 
@@ -103,21 +98,15 @@
             critical_type=logging.InputError,
             message=(
                 "Initialization cannot have positional arguments, use keyword"
                 " arguments."
             ),
         )
     # This is to "use" the kwarg parameter, nothing much else.
-    if len(kwargs) != 0:
-        logging.debug(
-            message=(
-                "Overriding keyword parameters to configuration initialization"
-                " present."
-            ),
-        )
+    lezargus.library.wrapper.do_nothing(**kwargs)
 
     # Load the default configuration parameters. The user's configurations
     # should overwrite these when supplied.
     lezargus.library.config.load_configuration_file(
         filename=lezargus.library.path.merge_pathname(
             directory=lezargus.library.config.INTERNAL_MODULE_INSTALLATION_PATH,
             filename="configuration",
@@ -154,21 +143,15 @@
             critical_type=logging.InputError,
             message=(
                 "Initialization cannot have positional arguments, use keyword"
                 " arguments."
             ),
         )
     # This is to "use" the kwarg parameter, nothing much else.
-    if len(kwargs) != 0:
-        logging.debug(
-            message=(
-                "Overriding keyword parameters to logging initialization"
-                " present."
-            ),
-        )
+    lezargus.library.wrapper.do_nothing(**kwargs)
 
     # Construct the default console and file-based logging functions. The file
     # is saved in the package directory.
     lezargus.library.logging.add_console_logging_handler(
         console=sys.stderr,
         log_level=lezargus.library.logging.LOGGING_INFO_LEVEL,
         use_color=lezargus.library.config.LOGGING_STREAM_USE_COLOR,
@@ -245,21 +228,15 @@
             critical_type=logging.InputError,
             message=(
                 "Initialization cannot have positional arguments, use keyword"
                 " arguments."
             ),
         )
     # This is to "use" the kwarg parameter, nothing much else.
-    if len(kwargs) != 0:
-        logging.debug(
-            message=(
-                "Overriding keyword parameters to data file initialization"
-                " present."
-            ),
-        )
+    lezargus.library.wrapper.do_nothing(**kwargs)
 
     # We need to get the temporary directory path, if the configurations were
     # not loaded, we inform the user.
     try:
         temporary_directory = (
             lezargus.library.config.LEZARGUS_TEMPORARY_DIRECTORY
         )
@@ -317,37 +294,31 @@
             critical_type=logging.InputError,
             message=(
                 "Initialization cannot have positional arguments, use keyword"
                 " arguments."
             ),
         )
     # This is to "use" the kwarg parameter, nothing much else.
-    if len(kwargs) != 0:
-        logging.debug(
-            message=(
-                "Overriding keyword parameters to data file initialization"
-                " present."
-            ),
-        )
+    lezargus.library.wrapper.do_nothing(**kwargs)
 
     # Loading all of the data files.
     initialize_data_star_files(**kwargs)
     initialize_data_filter_files(**kwargs)
     initialize_data_atmosphere_files(**kwargs)
 
     # Computing the other data values.
     initialize_data_filter_zero_point_values(**kwargs)
 
     # All done.
 
 
 def initialize_data_star_files(*args: tuple, **kwargs: object) -> None:
-    """Initialize the stellar spectra data files.
+    """Initialize the stellar spectrum data files.
 
-    Load all of stellar spectra and other data files into the library data
+    Load all of stellar spectrum and other data files into the library data
     module.
 
     Parameters
     ----------
     *args : tuple
         Positional arguments. There should be no positional arguments. This
         serves to catch them.
@@ -368,66 +339,60 @@
             critical_type=logging.InputError,
             message=(
                 "Initialization cannot have positional arguments, use keyword"
                 " arguments."
             ),
         )
     # This is to "use" the kwarg parameter, nothing much else.
-    if len(kwargs) != 0:
-        logging.debug(
-            message=(
-                "Overriding keyword parameters to data star file initialization"
-                " present."
-            ),
-        )
+    lezargus.library.wrapper.do_nothing(**kwargs)
 
     # Loading the stars.
     lezargus.library.data.add_data_object(
         name="STAR_16CYGB",
-        data=lezargus.container.LezargusSpectra.read_fits_file(
+        data=lezargus.container.LezargusSpectrum.read_fits_file(
             filename=lezargus.library.path.merge_pathname(
                 directory=lezargus.library.config.INTERNAL_MODULE_DATA_DIRECTORY,
                 filename="star_spectra_16CygB",
                 extension="fits",
             ),
         ),
     )
     lezargus.library.data.add_data_object(
         name="STAR_109VIR",
-        data=lezargus.container.LezargusSpectra.read_fits_file(
+        data=lezargus.container.LezargusSpectrum.read_fits_file(
             filename=lezargus.library.path.merge_pathname(
                 directory=lezargus.library.config.INTERNAL_MODULE_DATA_DIRECTORY,
                 filename="star_spectra_109Vir",
                 extension="fits",
             ),
         ),
     )
     lezargus.library.data.add_data_object(
         name="STAR_SUN",
-        data=lezargus.container.LezargusSpectra.read_fits_file(
+        data=lezargus.container.LezargusSpectrum.read_fits_file(
             filename=lezargus.library.path.merge_pathname(
                 directory=lezargus.library.config.INTERNAL_MODULE_DATA_DIRECTORY,
                 filename="star_spectra_Sun",
                 extension="fits",
             ),
         ),
     )
     lezargus.library.data.add_data_object(
         name="STAR_VEGA",
-        data=lezargus.container.LezargusSpectra.read_fits_file(
+        data=lezargus.container.LezargusSpectrum.read_fits_file(
             filename=lezargus.library.path.merge_pathname(
                 directory=lezargus.library.config.INTERNAL_MODULE_DATA_DIRECTORY,
                 filename="star_spectra_Vega",
                 extension="fits",
             ),
         ),
     )
     lezargus.library.data.add_data_object(
         name="STAR_A0V",
-        data=lezargus.container.LezargusSpectra.read_fits_file(
+        data=lezargus.container.LezargusSpectrum.read_fits_file(
             filename=lezargus.library.path.merge_pathname(
                 directory=lezargus.library.config.INTERNAL_MODULE_DATA_DIRECTORY,
                 filename="star_spectra_A0V",
                 extension="fits",
             ),
         ),
     )
@@ -460,112 +425,106 @@
             critical_type=logging.InputError,
             message=(
                 "Initialization cannot have positional arguments, use keyword"
                 " arguments."
             ),
         )
     # This is to "use" the kwarg parameter, nothing much else.
-    if len(kwargs) != 0:
-        logging.debug(
-            message=(
-                "Overriding keyword parameters to data photometric filter file"
-                " initialization present."
-            ),
-        )
+    lezargus.library.wrapper.do_nothing(**kwargs)
 
     # Loading the photometric filter files.
 
     # Loading Johnson filters.
     lezargus.library.data.add_data_object(
         name="FILTER_JOHNSON_U_PHOTON",
-        data=lezargus.container.LezargusSpectra.read_fits_file(
+        data=lezargus.container.LezargusSpectrum.read_fits_file(
             filename=lezargus.library.path.merge_pathname(
                 directory=lezargus.library.config.INTERNAL_MODULE_DATA_DIRECTORY,
                 filename="filter_Johnson_U_photon",
                 extension="fits",
             ),
         ),
     )
     lezargus.library.data.add_data_object(
         name="FILTER_JOHNSON_B_PHOTON",
-        data=lezargus.container.LezargusSpectra.read_fits_file(
+        data=lezargus.container.LezargusSpectrum.read_fits_file(
             filename=lezargus.library.path.merge_pathname(
                 directory=lezargus.library.config.INTERNAL_MODULE_DATA_DIRECTORY,
                 filename="filter_Johnson_B_photon",
                 extension="fits",
             ),
         ),
     )
     lezargus.library.data.add_data_object(
         name="FILTER_JOHNSON_V_PHOTON",
-        data=lezargus.container.LezargusSpectra.read_fits_file(
+        data=lezargus.container.LezargusSpectrum.read_fits_file(
             filename=lezargus.library.path.merge_pathname(
                 directory=lezargus.library.config.INTERNAL_MODULE_DATA_DIRECTORY,
                 filename="filter_Johnson_V_photon",
                 extension="fits",
             ),
         ),
     )
 
     # Loading GAIA filters.
     lezargus.library.data.add_data_object(
         name="FILTER_GAIA_GG_PHOTON",
-        data=lezargus.container.LezargusSpectra.read_fits_file(
+        data=lezargus.container.LezargusSpectrum.read_fits_file(
             filename=lezargus.library.path.merge_pathname(
                 directory=lezargus.library.config.INTERNAL_MODULE_DATA_DIRECTORY,
                 filename="filter_Gaia_GG_photon",
                 extension="fits",
             ),
         ),
     )
     lezargus.library.data.add_data_object(
         name="FILTER_GAIA_GB_PHOTON",
-        data=lezargus.container.LezargusSpectra.read_fits_file(
+        data=lezargus.container.LezargusSpectrum.read_fits_file(
             filename=lezargus.library.path.merge_pathname(
                 directory=lezargus.library.config.INTERNAL_MODULE_DATA_DIRECTORY,
                 filename="filter_Gaia_GB_photon",
                 extension="fits",
             ),
         ),
     )
     lezargus.library.data.add_data_object(
         name="FILTER_GAIA_GR_PHOTON",
-        data=lezargus.container.LezargusSpectra.read_fits_file(
+        data=lezargus.container.LezargusSpectrum.read_fits_file(
             filename=lezargus.library.path.merge_pathname(
                 directory=lezargus.library.config.INTERNAL_MODULE_DATA_DIRECTORY,
                 filename="filter_Gaia_GR_photon",
                 extension="fits",
             ),
         ),
     )
 
     # Loading 2MASS filters.
     lezargus.library.data.add_data_object(
         name="FILTER_2MASS_J_PHOTON",
-        data=lezargus.container.LezargusSpectra.read_fits_file(
+        data=lezargus.container.LezargusSpectrum.read_fits_file(
             filename=lezargus.library.path.merge_pathname(
                 directory=lezargus.library.config.INTERNAL_MODULE_DATA_DIRECTORY,
                 filename="filter_2MASS_J_photon",
                 extension="fits",
             ),
         ),
     )
     lezargus.library.data.add_data_object(
         name="FILTER_2MASS_H_PHOTON",
-        data=lezargus.container.LezargusSpectra.read_fits_file(
+        data=lezargus.container.LezargusSpectrum.read_fits_file(
             filename=lezargus.library.path.merge_pathname(
                 directory=lezargus.library.config.INTERNAL_MODULE_DATA_DIRECTORY,
                 filename="filter_2MASS_H_photon",
                 extension="fits",
             ),
         ),
     )
     lezargus.library.data.add_data_object(
         name="FILTER_2MASS_KS_PHOTON",
-        data=lezargus.container.LezargusSpectra.read_fits_file(
+        data=lezargus.container.LezargusSpectrum.read_fits_file(
             filename=lezargus.library.path.merge_pathname(
                 directory=lezargus.library.config.INTERNAL_MODULE_DATA_DIRECTORY,
                 filename="filter_2MASS_Ks_photon",
                 extension="fits",
             ),
         ),
     )
@@ -599,105 +558,24 @@
             critical_type=logging.InputError,
             message=(
                 "Initialization cannot have positional arguments, use keyword"
                 " arguments."
             ),
         )
     # This is to "use" the kwarg parameter, nothing much else.
-    if len(kwargs) != 0:
-        logging.debug(
-            message=(
-                "Overriding keyword parameters to data atmospheric file"
-                " initialization present."
-            ),
-        )
+    lezargus.library.wrapper.do_nothing(**kwargs)
 
-    # We first load all of the atmospheric transmission files.
-    lezargus.library.data.add_data_object(
-        name="PSG_ATM_TRANS_ZA0",
-        data=lezargus.container.LezargusSpectra.read_fits_file(
-            filename=lezargus.library.path.merge_pathname(
-                directory=lezargus.library.config.INTERNAL_MODULE_DATA_DIRECTORY,
-                filename="psg_atm_trans_za0",
-                extension="fits",
-            ),
-        ),
-    )
-    lezargus.library.data.add_data_object(
-        name="PSG_ATM_TRANS_ZA30",
-        data=lezargus.container.LezargusSpectra.read_fits_file(
-            filename=lezargus.library.path.merge_pathname(
-                directory=lezargus.library.config.INTERNAL_MODULE_DATA_DIRECTORY,
-                filename="psg_atm_trans_za30",
-                extension="fits",
-            ),
-        ),
-    )
-    lezargus.library.data.add_data_object(
-        name="PSG_ATM_TRANS_ZA45",
-        data=lezargus.container.LezargusSpectra.read_fits_file(
-            filename=lezargus.library.path.merge_pathname(
-                directory=lezargus.library.config.INTERNAL_MODULE_DATA_DIRECTORY,
-                filename="psg_atm_trans_za45",
-                extension="fits",
-            ),
-        ),
-    )
-    lezargus.library.data.add_data_object(
-        name="PSG_ATM_TRANS_ZA60",
-        data=lezargus.container.LezargusSpectra.read_fits_file(
-            filename=lezargus.library.path.merge_pathname(
-                directory=lezargus.library.config.INTERNAL_MODULE_DATA_DIRECTORY,
-                filename="psg_atm_trans_za60",
-                extension="fits",
-            ),
-        ),
-    )
+    # The PSG atmospheric files are generated outside of this package and so
+    # the defined zenith angles and precipitable water vapor values are known
+    # before hand. The units here are defined based on the filenames.
+    zenith_angles = [0, 30, 45, 60]
+    pwv_values = [0.5, 1.0, 2.0, 3.0]
 
-    # We next load all of the atmospheric radiance files.
-    lezargus.library.data.add_data_object(
-        name="PSG_ATM_RAD_ZA0",
-        data=lezargus.container.LezargusSpectra.read_fits_file(
-            filename=lezargus.library.path.merge_pathname(
-                directory=lezargus.library.config.INTERNAL_MODULE_DATA_DIRECTORY,
-                filename="psg_atm_rad_za0",
-                extension="fits",
-            ),
-        ),
-    )
-    lezargus.library.data.add_data_object(
-        name="PSG_ATM_RAD_ZA30",
-        data=lezargus.container.LezargusSpectra.read_fits_file(
-            filename=lezargus.library.path.merge_pathname(
-                directory=lezargus.library.config.INTERNAL_MODULE_DATA_DIRECTORY,
-                filename="psg_atm_rad_za30",
-                extension="fits",
-            ),
-        ),
-    )
-    lezargus.library.data.add_data_object(
-        name="PSG_ATM_RAD_ZA45",
-        data=lezargus.container.LezargusSpectra.read_fits_file(
-            filename=lezargus.library.path.merge_pathname(
-                directory=lezargus.library.config.INTERNAL_MODULE_DATA_DIRECTORY,
-                filename="psg_atm_rad_za45",
-                extension="fits",
-            ),
-        ),
-    )
-    lezargus.library.data.add_data_object(
-        name="PSG_ATM_RAD_ZA60",
-        data=lezargus.container.LezargusSpectra.read_fits_file(
-            filename=lezargus.library.path.merge_pathname(
-                directory=lezargus.library.config.INTERNAL_MODULE_DATA_DIRECTORY,
-                filename="psg_atm_rad_za60",
-                extension="fits",
-            ),
-        ),
-    )
+    lezargus.library.wrapper.do_nothing(zenith_angles, pwv_values)
+    logging.error(error_type=logging.ToDoError, message="Data atmosphere files")
 
 
 def initialize_data_filter_zero_point_values(
     *args: tuple,
     **kwargs: object,
 ) -> None:
     """Initialize the PSG atmospheric data files.
@@ -727,21 +605,15 @@
             critical_type=logging.InputError,
             message=(
                 "Initialization cannot have positional arguments, use keyword"
                 " arguments."
             ),
         )
     # This is to "use" the kwarg parameter, nothing much else.
-    if len(kwargs) != 0:
-        logging.debug(
-            message=(
-                "Overriding keyword parameters to data zero point value"
-                " initialization present."
-            ),
-        )
+    lezargus.library.wrapper.do_nothing(**kwargs)
 
     # Calculating Johnson filters zero point values.
     # Johnson U band.
     (
         johnson_u_zp,
         johnson_u_zpu,
     ) = lezargus.library.photometry.calculate_filter_zero_point_vega(
```

### Comparing `lezargus-0.0.4.dev44/src/lezargus/container/broadcast.py` & `lezargus-0.0.4.dev51/src/lezargus/container/broadcast.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,152 +3,159 @@
 Sometimes operations are needed to be performed between two dimensions of
 data structures. We have functions here which serve to convert from one
 structure to another based on some broadcasting pattern. We properly handle
 the internal conversions (such as the flags, mask, wavelength, etc) as well
 based on the input template structure broadcasting to.
 """
 
-# This is a last resort solution to fixing the recursive import of the
-# type hints here.
+# isort: split
+# Import required to remove circular dependencies from type checking.
 from __future__ import annotations
 
+from typing import TYPE_CHECKING
+
+if TYPE_CHECKING:
+    from lezargus.library import hint
+# isort: split
+
+
 import numpy as np
 
 import lezargus
-from lezargus.library import hint
 from lezargus.library import logging
 
 
-def broadcast_spectra_to_cube_uniform(
-    input_spectra: hint.LezargusSpectra,
+def broadcast_spectrum_to_cube_uniform(
+    input_spectrum: hint.LezargusSpectrum,
     template_cube: hint.LezargusCube,
     wavelength_mode: str = "error",
 ) -> hint.LezargusCube:
-    """Make a LezargusCube from a LezargusSpectra via uniform broadcasting.
+    """Make a LezargusCube from a LezargusSpectrum via uniform broadcasting.
 
     We make a LezargusCube, from a provided template, using uniform
     broadcasting. Uniform broadcasting is where all spectral slices, within
     the cube, are all the same for a uniform spatial distribution of the
-    spectra, which is in this case the provided input spectra.
+    spectrum, which is in this case the provided input spectrum.
 
-    In the case of both the input spectra and provided template cube having
+    In the case of both the input spectrum and provided template cube having
     different wavelength arrays, we follow the provided mode to handle the
     different cases. The input template cube only provides the array shapes and
     the wavelength axis (dependant on the mode); the rest comes from the
-    input spectra.
+    input spectrum.
 
     Parameters
     ----------
-    input_spectra : LezargusSpectra
-        The input spectra which will be broadcasted to fit the input template
+    input_spectrum : LezargusSpectrum
+        The input spectrum which will be broadcasted to fit the input template
         cube.
     template_cube : LezargusCube
         The template cube which will serve as a template to determine the
         dimensional properties of the resulting broadcasting cube.
     wavelength_mode : str, default = "error"
         The mode to handle possible wavelength array conflicts between the
-        spectra and the cube. The available options are:
+        spectrum and the cube. The available options are:
 
-            - "spectra" : Prefer the spectra's wavelength array; the cube's
+            - "spectrum" : Prefer the spectrum's wavelength array; the cube's
               wavelength is ignored.
-            - "cube" : Prefer the cube's wavelength array; the spectra is
+            - "cube" : Prefer the cube's wavelength array; the spectrum is
               interpolated to align to the new wavelength.
             - "error" : We log an error. We still attempt to figure it out,
-              defaulting to the spectra's wavelength array.
+              defaulting to the spectrum's wavelength array.
 
     Returns
     -------
     broadcast_cube : LezargusCube
-        The LezargusCube after the spectra was uniformly broadcast spatially.
-        Any header information came from first the spectra then the cube.
+        The LezargusCube after the spectrum was uniformly broadcast spatially.
+        Any header information came from first the spectrum then the cube.
 
     """
     # First thing is first, type check the input.
     if not (
-        isinstance(input_spectra, lezargus.container.LezargusSpectra)
+        isinstance(input_spectrum, lezargus.container.LezargusSpectrum)
         and isinstance(template_cube, lezargus.container.LezargusCube)
     ):
         # The objects are not the proper type so broadcasting them might go
         # really wrong.
         logging.error(
             error_type=logging.InputError,
             message=(
-                f"The input spectra type {type(input_spectra)} and template"
+                f"The input spectrum type {type(input_spectrum)} and template"
                 f" cube type {type(template_cube)} are not instances of the"
-                " expected LezargusSpectra and LezargusCube types"
+                " expected LezargusSpectrum and LezargusCube types"
                 " respectively. Broadcasting may fail."
             ),
         )
 
     # Now, we need to determine the definitive wavelength array based on the
     # provided wavelength mode. However, the two wavelength units might be
     # different, this is problem that we ought to warn.
-    if input_spectra.wavelength_unit != template_cube.wavelength_unit:
+    if input_spectrum.wavelength_unit != template_cube.wavelength_unit:
         logging.warning(
             warning_type=logging.AccuracyWarning,
             message=(
-                "The input spectra wavelength unit is"
-                f" {input_spectra.wavelength_unit}, different from the template"
-                f" cube wavelength unit {template_cube.wavelength_unit}"
+                "The input spectrum wavelength unit is"
+                f" {input_spectrum.wavelength_unit}, different from the "
+                " template cube wavelength unit "
+                f" {template_cube.wavelength_unit}"
             ),
         )
     # Regardless of the unit situation, we try our best to determine the
     # the preferred wavelength.
     wavelength_mode = wavelength_mode.casefold()
-    if wavelength_mode == "spectra":
-        # We rely on the spectra's wavelength.
-        broadcast_wavelength = input_spectra.wavelength
-        broadcast_wavelength_unit = input_spectra.wavelength_unit
+    if wavelength_mode == "spectrum":
+        # We rely on the spectrum's wavelength.
+        broadcast_wavelength = input_spectrum.wavelength
+        broadcast_wavelength_unit = input_spectrum.wavelength_unit
     elif wavelength_mode == "cube":
         # We rely on the cube's wavelength.
         broadcast_wavelength = template_cube.wavelength
         broadcast_wavelength_unit = template_cube.wavelength_unit
     elif wavelength_mode == "error":
         # If the wavelengths differ, we raise an error on their mismatch.
         if not np.all(
-            np.isclose(input_spectra.wavelength, template_cube.wavelength),
+            np.isclose(input_spectrum.wavelength, template_cube.wavelength),
         ):
             logging.error(
                 error_type=logging.InputError,
                 message=(
-                    "Input spectra and template cube wavelength arrays do not"
+                    "Input spectrum and template cube wavelength arrays do not"
                     " match; wavelength mode is `error`; returning None."
                 ),
             )
-        # Regardless if the error was logged or not, we use the input spectra
+        # Regardless if the error was logged or not, we use the input spectrum
         # as the broadcast.
-        broadcast_wavelength = input_spectra.wavelength
-        broadcast_wavelength_unit = input_spectra.wavelength_unit
+        broadcast_wavelength = input_spectrum.wavelength
+        broadcast_wavelength_unit = input_spectrum.wavelength_unit
     else:
         # The input parameter is not a given parameter.
         logging.critical(
             critical_type=logging.InputError,
             message=(
                 f"The input wavelength mode {wavelength_mode} is not a"
                 " supported option."
             ),
         )
 
-    # Finally, we determine the appropriate data based on the spectra and
+    # Finally, we determine the appropriate data based on the spectrum and
     # the preferred wavelength array.
     (
         interpolated_data,
         interpolated_uncertainty,
         interpolated_mask,
         interpolated_flags,
-    ) = input_spectra.interpolate(
+    ) = input_spectrum.interpolate(
         wavelength=broadcast_wavelength,
         skip_mask=False,
         skip_flags=False,
     )
     # The data unit for the data and the like.
-    broadcast_data_unit = input_spectra.data_unit
+    broadcast_data_unit = input_spectrum.data_unit
 
     # Now, we assemble the cube. We only need the spatial coverage of the cube
-    # and broadcast our 1D spectra to the spatial dimensions. We do not
+    # and broadcast our 1D spectrum to the spatial dimensions. We do not
     # really care for the wavelength shape of the cube.
     x_dim, y_dim, __ = template_cube.data.shape
     wave_dim = broadcast_wavelength.shape[0]
     # Building the cubes.
     broadcast_data = np.broadcast_to(
         interpolated_data,
         shape=(x_dim, y_dim, wave_dim),
@@ -169,17 +176,17 @@
     # The pixel and slice scale of the broadcasted cube is based on the
     # template cube as that is where the shape is derived from.
     pixel_scale = template_cube.pixel_scale
     slice_scale = template_cube.slice_scale
 
     # Finally, we reconstruct the cube. We work on copies of the headers
     # just in case.
-    spectra_header = input_spectra.header.copy()
+    spectrum_header = input_spectrum.header.copy()
     cube_header = template_cube.header.copy()
-    broadcast_header = cube_header.update(spectra_header)
+    broadcast_header = cube_header.update(spectrum_header)
 
     # Building the new broadcasted cube. We use the template's cube's class
     # just in case it has been subclassed or something.
     template_cube_class = type(template_cube)
     broadcast_cube = template_cube_class(
         wavelength=broadcast_wavelength,
         data=broadcast_data,
@@ -192,150 +199,151 @@
         flags=broadcast_flags,
         header=broadcast_header,
     )
     # All done.
     return broadcast_cube
 
 
-def broadcast_spectra_to_cube_center(
-    input_spectra: hint.LezargusSpectra,
+def broadcast_spectrum_to_cube_center(
+    input_spectrum: hint.LezargusSpectrum,
     template_cube: hint.LezargusCube,
     wavelength_mode: str = "error",
     allow_even_center: bool = True,
 ) -> hint.LezargusCube:
-    """Make a LezargusCube from a LezargusSpectra via center broadcasting.
+    """Make a LezargusCube from a LezargusSpectrum via center broadcasting.
 
     We make a LezargusCube, from a provided template, using center
     broadcasting. Center broadcasting is the provided spectral slice is
     centered in the cube; all other values are zero (or the blank equivalent
     for masks and flags). If any side of an image slice of the template cube
     is even, we can still try to place the image in the center, biasing it
     towards the lower value corner.
 
-    In the case of both the input spectra and provided template cube having
+    In the case of both the input spectrum and provided template cube having
     different wavelength arrays, we follow the provided mode to handle the
     different cases. The input template cube only provides the array shapes and
     the wavelength axis (dependant on the mode); the rest comes from the
-    input spectra.
+    input spectrum.
 
     Parameters
     ----------
-    input_spectra : LezargusSpectra
-        The input spectra which will be broadcasted to fit the input template
+    input_spectrum : LezargusSpectrum
+        The input spectrum which will be broadcasted to fit the input template
         cube.
     template_cube : LezargusCube
         The template cube which will serve as a template to determine the
         dimensional properties of the resulting broadcasting cube.
     wavelength_mode : str, default = "error"
         The mode to handle possible wavelength array conflicts between the
-        spectra and the cube. The available options are:
+        spectrum and the cube. The available options are:
 
-            - "spectra" : Prefer the spectra's wavelength array; the cube's
+            - "spectrum" : Prefer the spectrum's wavelength array; the cube's
               wavelength is ignored.
-            - "cube" : Prefer the cube's wavelength array; the spectra is
+            - "cube" : Prefer the cube's wavelength array; the spectrum is
               interpolated to align to the new wavelength.
             - "error" : We log an error and return None.
 
     allow_even_center : bool, default = True
         If True, and if any axis of an image slice is even, a warning is
-        logged and the spectra is put it as close to the center as possible.
+        logged and the spectrum is put it as close to the center as possible.
         If False, instead, an exception is raised.
 
     Returns
     -------
     broadcast_cube : LezargusCube
-        The LezargusCube after the spectra was center broadcast spatially.
-        Any header information came from first the spectra then the cube.
+        The LezargusCube after the spectrum was center broadcast spatially.
+        Any header information came from first the spectrum then the cube.
 
     """
     # First thing is first, type check the input.
     if not (
-        isinstance(input_spectra, lezargus.container.LezargusSpectra)
+        isinstance(input_spectrum, lezargus.container.LezargusSpectrum)
         and isinstance(template_cube, lezargus.container.LezargusCube)
     ):
         # The objects are not the proper type so broadcasting them might go
         # really wrong.
         logging.error(
             error_type=logging.InputError,
             message=(
-                f"The input spectra type {type(input_spectra)} and template"
+                f"The input spectrum type {type(input_spectrum)} and template"
                 f" cube type {type(template_cube)} are not instances of the"
-                " expected LezargusSpectra and LezargusCube types"
+                " expected LezargusSpectrum and LezargusCube types"
                 " respectively. Broadcasting may fail."
             ),
         )
 
     # Now, we need to determine the definitive wavelength array based on the
     # provided wavelength mode. However, the two wavelength units might be
     # different, this is problem that we ought to warn.
-    if input_spectra.wavelength_unit != template_cube.wavelength_unit:
+    if input_spectrum.wavelength_unit != template_cube.wavelength_unit:
         logging.warning(
             warning_type=logging.AccuracyWarning,
             message=(
-                "The input spectra wavelength unit is"
-                f" {input_spectra.wavelength_unit}, different from the template"
-                f" cube wavelength unit {template_cube.wavelength_unit}"
+                "The input spectrum wavelength unit is"
+                f" {input_spectrum.wavelength_unit}, different from the "
+                " template cube wavelength unit "
+                f" {template_cube.wavelength_unit}"
             ),
         )
     # Regardless of the unit situation, we try our best to determine the
     # the preferred wavelength.
     wavelength_mode = wavelength_mode.casefold()
-    if wavelength_mode == "spectra":
-        # We rely on the spectra's wavelength.
-        broadcast_wavelength = input_spectra.wavelength
-        broadcast_wavelength_unit = input_spectra.wavelength_unit
+    if wavelength_mode == "spectrum":
+        # We rely on the spectrum's wavelength.
+        broadcast_wavelength = input_spectrum.wavelength
+        broadcast_wavelength_unit = input_spectrum.wavelength_unit
     elif wavelength_mode == "cube":
         # We rely on the cube's wavelength.
         broadcast_wavelength = template_cube.wavelength
         broadcast_wavelength_unit = template_cube.wavelength_unit
     elif wavelength_mode == "error":
         # If the wavelengths differ, we raise an error on their mismatch.
         if not np.all(
-            np.isclose(input_spectra.wavelength, template_cube.wavelength),
+            np.isclose(input_spectrum.wavelength, template_cube.wavelength),
         ):
             logging.error(
                 error_type=logging.InputError,
                 message=(
-                    "Input spectra and template cube wavelength arrays do not"
+                    "Input spectrum and template cube wavelength arrays do not"
                     " match; wavelength mode is `error`; returning None."
                 ),
             )
             broadcast_wavelength = None
             broadcast_wavelength_unit = None
             return None
         # Otherwise, if they do match, we can continue with the broadcasting.
-        broadcast_wavelength = input_spectra.wavelength
-        broadcast_wavelength_unit = input_spectra.wavelength_unit
+        broadcast_wavelength = input_spectrum.wavelength
+        broadcast_wavelength_unit = input_spectrum.wavelength_unit
     else:
         # The input parameter is not a given parameter.
         logging.critical(
             critical_type=logging.InputError,
             message=(
                 f"The input wavelength mode {wavelength_mode} is not a"
                 " supported option."
             ),
         )
 
-    # Finally, we determine the appropriate data based on the spectra and
+    # Finally, we determine the appropriate data based on the spectrum and
     # the preferred wavelength array.
     (
         interpolated_data,
         interpolated_uncertainty,
         interpolated_mask,
         interpolated_flags,
-    ) = input_spectra.interpolate(
+    ) = input_spectrum.interpolate(
         wavelength=broadcast_wavelength,
         skip_mask=False,
         skip_flags=False,
     )
     # The data unit for the data and the like.
-    broadcast_data_unit = input_spectra.data_unit
+    broadcast_data_unit = input_spectrum.data_unit
 
     # Now, we assemble the cube. We only need the spatial coverage of the cube
-    # and broadcast our 1D spectra to the spatial dimensions. We do not
+    # and broadcast our 1D spectrum to the spatial dimensions. We do not
     # really care for the wavelength shape of the cube.
     x_dim, y_dim, __ = template_cube.data.shape
     wave_dim = broadcast_wavelength.shape[0]
 
     # If either the x or y dimension size is even, the center pixel is not
     # defined. Although we still attempt to put it in the center.
     if x_dim % 2 == 0 or y_dim % 2 == 0:
@@ -343,15 +351,15 @@
         # flag.
         if allow_even_center:
             # We attempt to find the center.
             logging.warning(
                 warning_type=logging.AccuracyWarning,
                 message=(
                     f"The image slice of the template cube is even: ({x_dim},"
-                    f" {y_dim}). A best attempt at putting the spectra in the"
+                    f" {y_dim}). A best attempt at putting the spectrum in the"
                     " center is attempted."
                 ),
             )
         else:
             # We do not allow an even center, and so we raise.
             logging.critical(
                 critical_type=logging.InputError,
@@ -384,17 +392,17 @@
     # The pixel and slice scale of the broadcasted cube is based on the
     # template cube as that is where the shape is derived from.
     pixel_scale = template_cube.pixel_scale
     slice_scale = template_cube.slice_scale
 
     # Finally, we reconstruct the cube. We work on copies of the headers
     # just in case.
-    spectra_header = input_spectra.header.copy()
+    spectrum_header = input_spectrum.header.copy()
     cube_header = template_cube.header.copy()
-    cube_header.update(spectra_header)
+    cube_header.update(spectrum_header)
     broadcast_header = cube_header
 
     # Building the new broadcasted cube. We use the template's cube's class
     # just in case it has been subclassed or something.
     template_cube_class = type(template_cube)
     broadcast_cube = template_cube_class(
         wavelength=broadcast_wavelength,
```

### Comparing `lezargus-0.0.4.dev44/src/lezargus/container/cube.py` & `lezargus-0.0.4.dev51/src/lezargus/container/cube.py`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/src/lezargus/container/image.py` & `lezargus-0.0.4.dev51/src/lezargus/container/image.py`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/src/lezargus/container/mosaic.py` & `lezargus-0.0.4.dev51/src/lezargus/container/mosaic.py`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/src/lezargus/container/parent.py` & `lezargus-0.0.4.dev51/src/lezargus/container/parent.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,20 +15,18 @@
 
 import lezargus
 from lezargus.library import hint
 from lezargus.library import logging
 
 
 class LezargusContainerArithmetic:
-    """Lezargus wavelength-aware arithmetic.
+    """Lezargus wavelength-aware arithmetic for the major containers.
 
     This is the class which allows for the arithmetic behind the scenes to
-    work with wavelength knowledge. All we do is overwrite the NDDataArray
-    arithmetic functions to perform wavelength checks and pass it through
-    without wavelength issues.
+    work with wavelength knowledge.
 
     Attributes
     ----------
     wavelength : ndarray
         The wavelength of the spectra. The unit of wavelength is typically
         in meters; but, check the :py:attr:`wavelength_unit` value.
     data : ndarray
```

### Comparing `lezargus-0.0.4.dev44/src/lezargus/container/spectra.py` & `lezargus-0.0.4.dev51/src/lezargus/container/spectrum.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,57 +1,66 @@
-"""Spectra data container.
+"""Spectrum data container, holding spectral data.
 
 This module and class primarily deals with spectral data.
 """
 
+# isort: split
+# Import required to remove circular dependencies from type checking.
+from __future__ import annotations
+
+from typing import TYPE_CHECKING
+
+if TYPE_CHECKING:
+    from lezargus.library import hint
+# isort: split
+
 import copy
 
 import numpy as np
 
 import lezargus
 from lezargus.container import LezargusContainerArithmetic
-from lezargus.library import hint
 from lezargus.library import logging
 
 
-class LezargusSpectra(LezargusContainerArithmetic):
+class LezargusSpectrum(LezargusContainerArithmetic):
     """Container to hold spectral data and perform operations on it.
 
     Attributes
     ----------
     For all available attributes, see :py:class:`LezargusContainerArithmetic`.
 
     """
 
     def __init__(
-        self: "LezargusSpectra",
+        self: LezargusSpectrum,
         wavelength: hint.ndarray,
         data: hint.ndarray,
         uncertainty: hint.ndarray | None = None,
         wavelength_unit: str | hint.Unit | None = None,
         data_unit: str | hint.Unit | None = None,
         pixel_scale: float | None = None,
         slice_scale: float | None = None,
         mask: hint.ndarray | None = None,
         flags: hint.ndarray | None = None,
         header: hint.Header | None = None,
     ) -> None:
-        """Instantiate the spectra class.
+        """Instantiate the spectrum class.
 
         Parameters
         ----------
         wavelength : ndarray
             The wavelength axis of the spectral component of the data, if any.
             The unit of wavelength is typically in meters; but, check the
             :py:attr:`wavelength_unit` value.
         data : ndarray
             The data stored in this container. The unit of the flux is typically
             in W m^-2 m^-1; but, check the :py:attr:`data_unit` value.
         uncertainty : ndarray
-            The uncertainty in the data of the spectra. The unit of the
+            The uncertainty in the data of the spectrum. The unit of the
             uncertainty is the same as the data value; per
             :py:attr:`uncertainty_unit`.
         wavelength_unit : Astropy Unit
             The unit of the wavelength array. If None, we assume unit-less.
         data_unit : Astropy Unit
             The unit of the data array. If None, we assume unit-less.
         pixel_scale : float, default = None
@@ -83,15 +92,15 @@
         """
         # The data must be one dimensional.
         container_dimensions = 1
         if len(data.shape) != container_dimensions:
             logging.error(
                 error_type=logging.InputError,
                 message=(
-                    "The input data for a LezargusSpectra instantiation has a"
+                    "The input data for a LezargusSpectrum instantiation has a"
                     f" shape {data.shape}, which is not the expected one"
                     " dimension."
                 ),
             )
         # The wavelength and the data must be parallel, and thus the same
         # shape.
         wavelength = np.array(wavelength, dtype=float)
@@ -123,43 +132,182 @@
         )
 
     @classmethod
     def read_fits_file(
         cls: hint.Type[hint.Self],
         filename: str,
     ) -> hint.Self:
-        """Read a Lezargus spectra FITS file.
+        """Read a Lezargus spectrum FITS file.
 
         We load a Lezargus FITS file from disk. Note that this should only
-        be used for 1-D spectra files.
+        be used for a 1-D spectrum file.
 
         Parameters
         ----------
         filename : str
             The filename to load.
 
         Returns
         -------
-        spectra : Self-like
-            The LezargusSpectra class instance.
+        spectrum : Self-like
+            The LezargusSpectrum class instance.
 
         """
         # Any pre-processing is done here.
         # Loading the file.
-        spectra = cls._read_fits_file(filename=filename)
+        spectrum = cls._read_fits_file(filename=filename)
         # Any post-processing is done here.
         # All done.
-        return spectra
+        return spectrum
+
+    @classmethod
+    def stitch(
+        cls: hint.Type[hint.Self],
+        *spectra: hint.LezargusSpectrum,
+        weights: list[hint.ndarray] | str = "uniform",
+        average_routine: hint.Callable[
+            [hint.ndarray, hint.ndarray, hint.ndarray],
+            tuple[float, float],
+        ] = None,
+    ) -> hint.Self:
+        """Stitch spectra together to make a single spectrum.
+
+        We stitch all of the input spectra. If the spectrum are not already
+        to the same scale however, this will result in wildly incorrect
+        results. The header information is preserved, though we take what we
+        can from the other objects.
+
+        Parameters
+        ----------
+        *spectra : LezargusSpectrum
+            The set of Lezargus spectra which we will stitch together.
+        weights : list[ndarray] or str, default = None
+            A list of the weights in the data for stitching. Each entry in
+            the list must have a corresponding entry in the wavelength and
+            data list, or None. For convenience, we provide short-cut inputs
+            for the following:
+
+                - `uniform` : Uniform weights.
+                - `invar` : Inverse variance weights.
+        average_routine : Callable, str, default = None
+            The function used to average all of the spectra together.
+            It must also be able to accept weights and propagate uncertainties.
+            If None, we default to the weighted mean. Namely, it must be of the
+            form f(val, uncert, weight) = avg, uncert.
+
+        Returns
+        -------
+        stitch_spectrum : LezargusSpectrum
+            The spectrum after stitching.
+
+        """
+        # If there are no spectra to stitch, then we do nothing.
+        if len(spectra) == 0:
+            # We still warn just in case.
+            logging.warning(
+                warning_type=logging.InputWarning,
+                message=("No spectra supplied to stitch."),
+            )
+            return spectra
+
+        # We need to make sure these are all Lezargus spectrum.
+        lz_spectra = []
+        for spectrumdex in spectra:
+            if not isinstance(spectrumdex, LezargusSpectrum):
+                logging.critical(
+                    critical_type=logging.InputError,
+                    message=(
+                        f"Input type {type(spectrumdex)} is not a"
+                        " LezargusSpectrum, we cannot use it to stitch."
+                    ),
+                )
+            lz_spectra.append(spectrumdex)
+
+        # We need to translate the weight input.
+        if isinstance(weights, str):
+            weights = weights.casefold()
+            if weights == "uniform":
+                # We compute uniform weights.
+                using_weights = [
+                    np.ones_like(spectrumdex.wavelength)
+                    for spectrumdex in lz_spectra
+                ]
+            elif weights == "invar":
+                # We compute weights which are the inverse of the variance
+                # in the data.
+                using_weights = [
+                    1 / spectrumdex.uncertainty**2 for spectrumdex in lz_spectra
+                ]
+            else:
+                # A valid shortcut string has not been provided.
+                accepted_options = ["uniform", "invar"]
+                logging.critical(
+                    critical_type=logging.InputError,
+                    message=(
+                        f"The weight shortcut option {weights} is not valid; it"
+                        f" must be one of: {accepted_options}"
+                    ),
+                )
+        else:
+            using_weights = weights
+
+        # Next, we stitch together the data for the spectrum.
+        (
+            stitch_wavelength,
+            stitch_data,
+            stitch_uncertainty,
+        ) = lezargus.library.stitch.stitch_spectra_discrete(
+            wavelength_arrays=[
+                spectrumdex.wavelength for spectrumdex in lz_spectra
+            ],
+            data_arrays=[spectrumdex.data for spectrumdex in lz_spectra],
+            uncertainty_arrays=[
+                spectrumdex.uncertainty for spectrumdex in lz_spectra
+            ],
+            weight_arrays=using_weights,
+            average_routine=average_routine,
+            interpolate_routine=None,
+        )
+        # We also stitch together the flags and the mask. They are handled
+        # with a different function.
+        logging.error(
+            error_type=logging.ToDoError,
+            message="Flag and mask stitching not yet supported.",
+        )
+        stitch_mask = None
+        stitch_flags = None
+
+        # We merge the header.
+        logging.error(
+            error_type=logging.ToDoError,
+            message="Header stitching not yet supported.",
+        )
+        stitch_header = None
+
+        # We compile the new spectrum. We do not expect a subclass but we
+        # try and allow it.
+        stitch_spectrum = cls(
+            wavelength=stitch_wavelength,
+            data=stitch_data,
+            uncertainty=stitch_uncertainty,
+            wavelength_unit=lz_spectra[0].wavelength_unit,
+            data_unit=lz_spectra[0].data_unit,
+            mask=stitch_mask,
+            flags=stitch_flags,
+            header=stitch_header,
+        )
+        # All done.
+        return stitch_spectrum
 
     def write_fits_file(
         self: hint.Self,
         filename: str,
         overwrite: bool = False,
     ) -> hint.Self:
-        """Write a Lezargus spectra FITS file.
+        """Write a Lezargus spectrum FITS file.
 
         We write a Lezargus FITS file to disk.
 
         Parameters
         ----------
         filename : str
             The filename to write to.
@@ -174,31 +322,31 @@
         # Any pre-processing is done here.
         # Saving the file.
         self._write_fits_file(filename=filename, overwrite=overwrite)
         # Any post-processing is done here.
         # All done.
 
     def convolve(self: hint.Self, kernel: hint.ndarray) -> hint.Self:
-        """Convolve the spectra with a custom kernel.
+        """Convolve the spectrum with a custom kernel.
 
-        We compute the convolution and return a near copy of the spectra after
+        We compute the convolution and return a near copy of the spectrum after
         convolution. The wavelength is not affected.
 
         Parameters
         ----------
         kernel : ndarray
             The kernel which we are using to convolve.
 
         Returns
         -------
-        convolved_spectra : ndarray
-            A near copy of the spectra after convolution.
+        convolved_spectrum : ndarray
+            A near copy of the spectrum after convolution.
 
         """
-        # Using this kernel, we convolve the spectra. We assume that the
+        # Using this kernel, we convolve the spectrum. We assume that the
         # uncertainties add in quadrature.
         convolved_data = (
             lezargus.library.convolution.convolve_1d_array_by_1d_kernel(
                 array=self.data,
                 kernel=kernel,
             )
         )
@@ -216,43 +364,43 @@
             message=(
                 "Propagation of mask and flags via convolution is not done."
             ),
         )
         convolved_mask = self.mask
         convolved_flags = self.flags
 
-        # From the above information, we construct the new spectra.
-        spectra_class = type(self)
-        convolved_spectra = spectra_class(
+        # From the above information, we construct the new spectrum.
+        spectrum_class = type(self)
+        convolved_spectrum = spectrum_class(
             wavelength=self.wavelength,
             data=convolved_data,
             uncertainty=convolved_uncertainty,
             wavelength_unit=self.wavelength_unit,
             data_unit=self.data_unit,
             mask=convolved_mask,
             flags=convolved_flags,
             header=self.header,
         )
 
         # All done.
-        return convolved_spectra
+        return convolved_spectrum
 
     def interpolate(
         self: hint.Self,
         wavelength: hint.ndarray,
         extrapolate: bool = False,
         skip_mask: bool = True,
         skip_flags: bool = True,
     ) -> tuple[
         hint.ndarray,
         hint.ndarray,
         hint.ndarray | None,
         hint.ndarray | None,
     ]:
-        """Interpolation calling function for spectra.
+        """Interpolation calling function for spectrum.
 
         Each entry is considered a single point to interpolate over.
 
         Parameters
         ----------
         wavelength : ndarray
             The wavelength values which we are going to interpolate to. The
@@ -287,15 +435,15 @@
         """
         # Interpolation cannot deal with NaNs, so we exclude any set of data
         # which includes them.
         (
             clean_wavelength,
             clean_data,
             clean_uncertainty,
-        ) = lezargus.library.array.clean_finite_arrays(
+        ) = lezargus.library.sanitize.clean_finite_arrays(
             self.wavelength,
             self.data,
             self.uncertainty,
         )
 
         # If the wavelengths we are using to interpolate to are not all
         # numbers, it is a good idea to warn. It is not a good idea to change
@@ -349,170 +497,54 @@
         if skip_mask:
             interp_mask = None
         else:
             interp_mask = np.full_like(interp_data, False)
             logging.error(
                 error_type=logging.ToDoError,
                 message=(
-                    "The interpolation of a mask for spectra is not yet"
+                    "The interpolation of a mask for a spectrum is not yet"
                     " implemented."
                 ),
             )
         # Checking if we need to compute the interpolation of flag array.
         if skip_flags:
             interp_flags = None
         else:
             interp_flags = np.full_like(interp_data, 1)
             logging.error(
                 error_type=logging.ToDoError,
                 message=(
-                    "The interpolation of flags for spectra is not yet"
+                    "The interpolation of flags for a spectrum is not yet"
                     " implemented."
                 ),
             )
 
         # All done.
         return interp_data, interp_uncertainty, interp_mask, interp_flags
 
-    def stitch(
-        self: "LezargusSpectra",
-        *spectra: "LezargusSpectra",
-        weight: list[hint.ndarray] | str = "uniform",
-        average_routine: hint.Callable[
-            [hint.ndarray, hint.ndarray, hint.ndarray],
-            tuple[float, float],
-        ] = None,
+    def stitch_on(
+        self: hint.Self,
+        *spectra: hint.LezargusSpectrum,
+        **kwargs: object,
     ) -> hint.Self:
-        """Stitch together different spectra; we do not scaling.
+        """Stitch this spectrum with other input spectra.
 
-        We stitch this spectra with input spectra. If the spectra are not
-        already to the same scale however, this will result in wildly incorrect
-        results. The header information is preserved, though we take what we
-        can from the other objects.
+        We stitch spectra onto this spectra. This function is basically
+        a compatibility wrapper around the class method :py:meth:`stitch`.
 
         Parameters
         ----------
-        *spectra : LezargusSpectra
+        *spectra : LezargusSpectrum
             A set of Lezargus spectra which we will stitch to this one.
-        weight : list[ndarray] or str, default = None
-            A list of the weights in the data for stitching. Each entry in
-            the list must have a corresponding entry in the wavelength and
-            data list, or None. For convenience, we provide short-cut inputs
-            for the following:
-
-                - `uniform` : Uniform weights.
-                - `invar` : Inverse variance weights.
-        average_routine : Callable, str, default = None
-            The function used to average all of the spectra together.
-            It must also be able to accept weights and propagate uncertainties.
-            If None, we default to the weighted mean. Namely, it must be of the
-            form f(val, uncert, weight) = avg, uncert.
+        **kwargs : object
+            Arguments passed to :py:meth:`stitch`.
 
         Returns
         -------
-        stitch_spectra : LezargusSpectra
-            The spectra after stitching.
+        stitch_spectrum : LezargusSpectrum
+            The spectrum after stitching.
 
         """
-        # If there are no spectra to stitch, then we do nothing.
-        if len(spectra) == 0:
-            # We still warn just in case.
-            logging.warning(
-                warning_type=logging.InputWarning,
-                message=(
-                    "No additional spectra objects were submitted to stitch, no"
-                    " stitching applied."
-                ),
-            )
-            return self
-
-        # We need to make sure these are all Lezargus spectra.
-        lz_spectra = []
-        for spectradex in spectra:
-            if not isinstance(spectradex, LezargusSpectra):
-                logging.critical(
-                    critical_type=logging.InputError,
-                    message=(
-                        f"Input type {type(spectradex)} is not a"
-                        " LezargusSpectra, we cannot use it to stitch."
-                    ),
-                )
-            lz_spectra.append(spectradex)
-        # We finally append ourselves. Working on a copy is probably for the
-        # best.
-        lz_spectra.append(copy.deepcopy(self))
-
-        # We need to translate the weight input.
-        if isinstance(weight, str):
-            weight = weight.casefold()
-            if weight == "uniform":
-                # We compute uniform weights.
-                using_weights = [
-                    np.ones_like(spectradex.wavelength)
-                    for spectradex in lz_spectra
-                ]
-            elif weight == "invar":
-                # We compute weights which are the inverse of the variance
-                # in the data.
-                using_weights = [
-                    1 / spectradex.uncertainty**2 for spectradex in lz_spectra
-                ]
-            else:
-                # A valid shortcut string has not been provided.
-                accepted_options = ["uniform", "invar"]
-                logging.critical(
-                    critical_type=logging.InputError,
-                    message=(
-                        f"The weight shortcut option {weight} is not valid; it"
-                        f" must be one of: {accepted_options}"
-                    ),
-                )
-        else:
-            using_weights = weight
-
-        # Next, we stitch together the data for the spectra.
-        (
-            stitch_wavelength,
-            stitch_data,
-            stitch_uncertainty,
-        ) = lezargus.library.stitch.stitch_spectra_discrete(
-            wavelength_arrays=[
-                spectradex.wavelength for spectradex in lz_spectra
-            ],
-            data_arrays=[spectradex.data for spectradex in lz_spectra],
-            uncertainty_arrays=[
-                spectradex.uncertainty for spectradex in lz_spectra
-            ],
-            weight_arrays=using_weights,
-            average_routine=average_routine,
-            interpolate_routine=None,
-        )
-        # We also stitch together the flags and the mask. They are handled
-        # with a different function.
-        logging.error(
-            error_type=logging.ToDoError,
-            message="Flag and mask stitching not yet supported.",
-        )
-        stitch_mask = None
-        stitch_flags = None
-
-        # We merge the header.
-        logging.error(
-            error_type=logging.ToDoError,
-            message="Header stitching not yet supported.",
-        )
-        stitch_header = None
-
-        # We compile the new Spectra. We do not expect a subclass but we
-        # try and allow it.
-        stitch_spectra = self.__class__(
-            wavelength=stitch_wavelength,
-            data=stitch_data,
-            uncertainty=stitch_uncertainty,
-            wavelength_unit=self.wavelength_unit,
-            data_unit=self.data_unit,
-            mask=stitch_mask,
-            flags=stitch_flags,
-            header=stitch_header,
-        )
-        # All done.
-        return stitch_spectra
+        # We just add ourselves to the rest of the spectra to stitch together.
+        self_copy = copy.deepcopy(self)
+        all_spectra = [self_copy, *spectra]
+        return self.stitch(*all_spectra, **kwargs)
```

### Comparing `lezargus-0.0.4.dev44/src/lezargus/data/atm_rad_za0.fits` & `lezargus-0.0.4.dev51/src/lezargus/data/atm_rad_za0.fits`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/src/lezargus/data/atm_rad_za30.fits` & `lezargus-0.0.4.dev51/src/lezargus/data/atm_rad_za30.fits`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/src/lezargus/data/atm_rad_za45.fits` & `lezargus-0.0.4.dev51/src/lezargus/data/atm_rad_za45.fits`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/src/lezargus/data/atm_rad_za60.fits` & `lezargus-0.0.4.dev51/src/lezargus/data/atm_rad_za60.fits`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/src/lezargus/data/atm_trans_za0.fits` & `lezargus-0.0.4.dev51/src/lezargus/data/atm_trans_za0.fits`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/src/lezargus/data/atm_trans_za30.fits` & `lezargus-0.0.4.dev51/src/lezargus/data/atm_trans_za30.fits`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/src/lezargus/data/atm_trans_za45.fits` & `lezargus-0.0.4.dev51/src/lezargus/data/atm_trans_za45.fits`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/src/lezargus/data/atm_trans_za60.fits` & `lezargus-0.0.4.dev51/src/lezargus/data/atm_trans_za60.fits`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/src/lezargus/data/filter_2MASS_H_energy.fits` & `lezargus-0.0.4.dev51/src/lezargus/data/filter_2MASS_H_energy.fits`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/src/lezargus/data/filter_2MASS_H_photon.fits` & `lezargus-0.0.4.dev51/src/lezargus/data/filter_2MASS_H_photon.fits`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/src/lezargus/data/filter_2MASS_J_energy.fits` & `lezargus-0.0.4.dev51/src/lezargus/data/filter_2MASS_J_energy.fits`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/src/lezargus/data/filter_2MASS_J_photon.fits` & `lezargus-0.0.4.dev51/src/lezargus/data/filter_2MASS_J_photon.fits`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/src/lezargus/data/filter_2MASS_Ks_energy.fits` & `lezargus-0.0.4.dev51/src/lezargus/data/filter_2MASS_Ks_energy.fits`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/src/lezargus/data/filter_2MASS_Ks_photon.fits` & `lezargus-0.0.4.dev51/src/lezargus/data/filter_2MASS_Ks_photon.fits`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/src/lezargus/data/filter_Gaia_GB_energy.fits` & `lezargus-0.0.4.dev51/src/lezargus/data/filter_Gaia_GB_energy.fits`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/src/lezargus/data/filter_Gaia_GB_photon.fits` & `lezargus-0.0.4.dev51/src/lezargus/data/filter_Gaia_GB_photon.fits`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/src/lezargus/data/filter_Gaia_GG_energy.fits` & `lezargus-0.0.4.dev51/src/lezargus/data/filter_Gaia_GG_energy.fits`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/src/lezargus/data/filter_Gaia_GG_photon.fits` & `lezargus-0.0.4.dev51/src/lezargus/data/filter_Gaia_GG_photon.fits`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/src/lezargus/data/filter_Gaia_GR_energy.fits` & `lezargus-0.0.4.dev51/src/lezargus/data/filter_Gaia_GR_energy.fits`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/src/lezargus/data/filter_Gaia_GR_photon.fits` & `lezargus-0.0.4.dev51/src/lezargus/data/filter_Gaia_GR_photon.fits`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/src/lezargus/data/filter_Johnson_B_energy.fits` & `lezargus-0.0.4.dev51/src/lezargus/data/filter_Johnson_B_energy.fits`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/src/lezargus/data/filter_Johnson_B_photon.fits` & `lezargus-0.0.4.dev51/src/lezargus/data/filter_Johnson_B_photon.fits`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/src/lezargus/data/filter_Johnson_U_energy.fits` & `lezargus-0.0.4.dev51/src/lezargus/data/filter_Johnson_U_energy.fits`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/src/lezargus/data/filter_Johnson_U_photon.fits` & `lezargus-0.0.4.dev51/src/lezargus/data/filter_Johnson_U_photon.fits`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/src/lezargus/data/filter_Johnson_V_energy.fits` & `lezargus-0.0.4.dev51/src/lezargus/data/filter_Johnson_V_energy.fits`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/src/lezargus/data/filter_Johnson_V_photon.fits` & `lezargus-0.0.4.dev51/src/lezargus/data/filter_Johnson_V_photon.fits`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/src/lezargus/data/gem_atm_ir_rad.fits` & `lezargus-0.0.4.dev51/src/lezargus/data/gem_atm_ir_rad.fits`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/src/lezargus/data/gem_atm_opt_rad.fits` & `lezargus-0.0.4.dev51/src/lezargus/data/gem_atm_opt_rad.fits`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/src/lezargus/data/psg_atm_rad_za0.fits` & `lezargus-0.0.4.dev51/src/lezargus/data/psg_atm_rad_za0.fits`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/src/lezargus/data/psg_atm_rad_za30.fits` & `lezargus-0.0.4.dev51/src/lezargus/data/psg_atm_rad_za30.fits`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/src/lezargus/data/psg_atm_rad_za45.fits` & `lezargus-0.0.4.dev51/src/lezargus/data/psg_atm_rad_za45.fits`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/src/lezargus/data/psg_atm_rad_za60.fits` & `lezargus-0.0.4.dev51/src/lezargus/data/psg_atm_rad_za60.fits`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/src/lezargus/data/psg_atm_trans_za0.fits` & `lezargus-0.0.4.dev51/src/lezargus/data/psg_atm_trans_za0.fits`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/src/lezargus/data/psg_atm_trans_za30.fits` & `lezargus-0.0.4.dev51/src/lezargus/data/psg_atm_trans_za30.fits`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/src/lezargus/data/psg_atm_trans_za45.fits` & `lezargus-0.0.4.dev51/src/lezargus/data/psg_atm_trans_za45.fits`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/src/lezargus/data/psg_atm_trans_za60.fits` & `lezargus-0.0.4.dev51/src/lezargus/data/psg_atm_trans_za60.fits`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/src/lezargus/data/star_spectra_109Vir.fits` & `lezargus-0.0.4.dev51/src/lezargus/data/star_spectra_109Vir.fits`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/src/lezargus/data/star_spectra_16CygB.fits` & `lezargus-0.0.4.dev51/src/lezargus/data/star_spectra_16CygB.fits`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/src/lezargus/data/star_spectra_A0V.fits` & `lezargus-0.0.4.dev51/src/lezargus/data/star_spectra_A0V.fits`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/src/lezargus/data/star_spectra_Sun.fits` & `lezargus-0.0.4.dev51/src/lezargus/data/star_spectra_Sun.fits`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/src/lezargus/data/star_spectra_Vega.fits` & `lezargus-0.0.4.dev51/src/lezargus/data/star_spectra_Vega.fits`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/src/lezargus/library/__init__.py` & `lezargus-0.0.4.dev51/src/lezargus/library/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,10 +10,11 @@
 from lezargus.library import flags
 from lezargus.library import hint
 from lezargus.library import interpolate
 from lezargus.library import logging
 from lezargus.library import math
 from lezargus.library import path
 from lezargus.library import photometry
+from lezargus.library import sanitize
 from lezargus.library import stitch
 from lezargus.library import temporary
 from lezargus.library import wrapper
```

### Comparing `lezargus-0.0.4.dev44/src/lezargus/library/atmosphere.py` & `lezargus-0.0.4.dev51/src/lezargus/library/atmosphere.py`

 * *Files 1% similar despite different names*

```diff
@@ -255,20 +255,20 @@
 
     # The constant of refraction.
     const_of_refr = (ior_moist_air**2 - 1) / (2 * ior_moist_air**2)
     # Incorporating the zenith angle.
     abs_atm_refr = const_of_refr * np.tan(zenith_angle)
 
     # Creating the function itself.
-    abs_atm_refr_func = (
-        lezargus.library.interpolate.spline_1d_interpolate_factory(
-            x=wavelength,
-            y=abs_atm_refr,
-        )
+    abs_atm_refr_func = lezargus.library.interpolate.Spline1DInterpolate(
+        x=wavelength,
+        v=abs_atm_refr,
+        extrapolate=True,
     )
+
     return abs_atm_refr_func
 
 
 def relative_atmospheric_refraction_function(
     wavelength: hint.ndarray,
     reference_wavelength: float,
     zenith_angle: float,
```

### Comparing `lezargus-0.0.4.dev44/src/lezargus/library/config.py` & `lezargus-0.0.4.dev51/src/lezargus/library/config.py`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/src/lezargus/library/convolution.py` & `lezargus-0.0.4.dev51/src/lezargus/library/convolution.py`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/src/lezargus/library/data.py` & `lezargus-0.0.4.dev51/src/lezargus/library/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,29 +118,29 @@
     # All done.
     return zero_wavelength, zero_transmission
 
 
 def custom_rectangular_filter(
     lower_limit: float,
     upper_limit: float,
-) -> hint.LezargusSpectra:
+) -> hint.LezargusSpectrum:
     """Make a custom rectangular filter profile.
 
     Parameters
     ----------
     lower_limit : float
         The lower limit of the rectangular filter. This value is typically
         a wavelength, in meters.
     upper_limit : float
         The upper limit of the rectangular filter. This value is typically
         a wavelength, in meters.
 
     Returns
     -------
-    rectangular_filter : LezargusSpectra
+    rectangular_filter : LezargusSpectrum
         The filter, as defined.
 
     """
     # Wavelength and data. The 100 data points are arbitrary but we think it
     # is enough.
     n_data_points = 100
     filter_wave = np.linspace(lower_limit, upper_limit, n_data_points)
@@ -149,15 +149,15 @@
     # Customarily, filters have a little bit of data outside their band pass
     # for zeros.
     buffer_filter_wave, buffer_filter_trans = _zero_buffer_custom_filters(
         wavelength=filter_wave,
         transmission=filter_trans,
     )
     # Now we construct the filter object.
-    rectangular_filter = lezargus.container.LezargusSpectra(
+    rectangular_filter = lezargus.container.LezargusSpectrum(
         wavelength=buffer_filter_wave,
         data=buffer_filter_trans,
         uncertainty=None,
         wavelength_unit="m",
         data_unit="",
         header={"LZO_NAME": "Custom_rect_photon"},
     )
```

### Comparing `lezargus-0.0.4.dev44/src/lezargus/library/fits.py` & `lezargus-0.0.4.dev51/src/lezargus/library/fits.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     "LZO_NAME": (None, "LZ: Object name."),
     "LZOPK__X": (None, "LZ: PSF peak X index."),
     "LZOPK__Y": (None, "LZ: PSF peak Y index."),
     "LZOPK_RA": (None, "LZ: PSF peak RA value, deg."),
     "LZOPKDEC": (None, "LZ: PSF peak DEC value, deg."),
     "LZO_ROTA": (None, "LZ: Rotation angle, deg."),
     "LZO_AIRM": (None, "LZ: Airmass."),
-    # Synthetic photometric magnitudes derived from the spectra. This is a
+    # Synthetic photometric magnitudes derived from the spectrum. This is a
     # helpful place to put photometry measurements.
     "LZPM_J_U": (None, "LZ: Johnson U magnitude."),
     "LZPU_J_U": (None, "LZ: Johnson U uncertainty."),
     "LZPM_J_B": (None, "LZ: Johnson B magnitude."),
     "LZPU_J_B": (None, "LZ: Johnson B uncertainty."),
     "LZPM_J_V": (None, "LZ: Johnson V magnitude."),
     "LZPU_J_V": (None, "LZ: Johnson V uncertainty."),
@@ -435,15 +435,15 @@
 
     # We sort through every record and fix the issues with the dictionary.
     corrected_cards = []
     for keydex, valuedex in input_dict.items():
         # The header keys are usually capitalized.
         key = str(keydex).upper()
 
-        value = lezargus.library.conversion.convert_to_fits_header_types(
+        value = lezargus.library.sanitize.fix_fits_header_value(
             input_data=valuedex,
         )
 
         # Saving the corrected record.
         carddex = astropy.io.fits.Card(key, value)
         corrected_cards.append(carddex)
 
@@ -504,15 +504,15 @@
             valuedex = header_copy[keydex]
         else:
             # Otherwise, we just use the default.
             valuedex = defaultdex
 
         # We type check as FITS header files are picky about the object types
         # they get FITS headers really only support some specific basic types.
-        valuedex = lezargus.library.conversion.convert_to_fits_header_types(
+        valuedex = lezargus.library.sanitize.fix_fits_header_value(
             input_data=valuedex,
         )
         lezargus_header[keydex] = (valuedex, commentdex)
 
     # We construct the WCS header from the Lezargus header if one does not
     # already exist. We insert it in the WCS section of the header.
     if header.get("LZWBEGIN", False):
```

### Comparing `lezargus-0.0.4.dev44/src/lezargus/library/flags.py` & `lezargus-0.0.4.dev51/src/lezargus/library/flags.py`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/src/lezargus/library/hint.py` & `lezargus-0.0.4.dev51/src/lezargus/library/hint.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 from PySide6.QtWidgets import QWidget
 
 # Containers...
 from lezargus.container import LezargusContainerArithmetic
 from lezargus.container import LezargusCube
 from lezargus.container import LezargusImage
 from lezargus.container import LezargusMosaic
-from lezargus.container import LezargusSpectra
+from lezargus.container import LezargusSpectrum
 
 # Lezargus aliases.
 # Library things.
 from lezargus.library.interpolate import Generic1DInterpolate
 
 # Simulators...
 from lezargus.simulation import SimulatorSpectre
```

### Comparing `lezargus-0.0.4.dev44/src/lezargus/library/interpolate.py` & `lezargus-0.0.4.dev51/src/lezargus/library/interpolate.py`

 * *Files 10% similar despite different names*

```diff
@@ -120,15 +120,15 @@
         -------
         None
 
         """
         # We first sanitize the raw data so that the used interpolations
         # do not really complain. We also sort the arrays, interpolation on
         # unsorted arrays don't make any sense.
-        clean_x, clean_v = lezargus.library.array.clean_finite_arrays(x, v)
+        clean_x, clean_v = lezargus.library.sanitize.clean_finite_arrays(x, v)
         sort_index = np.argsort(clean_x)
         self.x = clean_x[sort_index]
         self.v = clean_v[sort_index]
 
         # We generate the interpolator itself.
         self.raw_interpolator = self._interpolator_generator(x=self.x, v=self.v)
 
@@ -561,21 +561,20 @@
         interpolator : Callable
             The modified Akima interpolator.
 
         """
         # The Akima1D interpolator. The modified version is the better one to
         # use considering its advantages. Namely the higher dimensionality and
         # better handling of flat data.
-        if False:
-            interpolator = scipy.interpolate.Akima1DInterpolator(
-                x,
-                v,
-                method="makima",
-                extrapolate=True,
-            )
+        # Akima  interpolator = scipy.interpolate.Akima1DInterpolator(
+        # Akima      x,
+        # Akima      v,
+        # Akima      method="makima",
+        # Akima      extrapolate=True,
+        # Akima  )
 
         # Super temporary; REMOVE when makima is proper.
         interpolator = scipy.interpolate.PchipInterpolator(
             x,
             v,
             extrapolate=True,
         )
@@ -594,21 +593,22 @@
 
     We do suggest using the repeat interpolators which actually define their
     axes; such are built for 2D :py:class:`Repeat2DInterpolate` and
     3D :py:class:`Repeat3DInterpolate` interpolators. For single dimensions,
     see :py:class:`Generic1DInterpolate` and its subclasses.
     For higher dimensions,  we suggest using this class.
 
-    Parameters
+    Attributes
     ----------
     domain : list
         A list of the domain axes values which define the multidimensional
         data.
     v : ndarray
-        The multi-dimensional data who's axes are defined.
+        The multi-dimensional data who's axes are defined. This data is the
+        data interpolated.
     interpolator_template : Callable
         The template function for the 1D interpolations.
 
     """
 
     def __init__(
         self: "RepeatNDInterpolate",
@@ -632,22 +632,23 @@
 
         Returns
         -------
         None
 
         """
         # We check that the shape provided by the domain matches the data
-        # shape.
+        # shape. The domain order provided above is actually the reverse of
+        # the Numpy convention.
         domain_shape = tuple(domaindex.size for domaindex in domain)
-        if domain_shape != v.shape:
+        if reversed(domain_shape) != v.shape:
             logging.error(
                 error_type=logging.InputError,
                 message=(
-                    f"The shape of the data is {v.shape} which does not match"
-                    " the expected shape from the provided domain"
+                    f"The shape of the data is {v.shape} which does not "
+                    " match the expected shape from the provided domain"
                     f" {domain_shape}."
                 ),
             )
 
         # We test the template function here with dummy data, just to make
         # sure it is a template function.
         temp_linear_data = np.linspace(0, 10, 10)
@@ -774,28 +775,28 @@
         This function is hidden so this class can be subclassed easily. Please
         call the public interface class to interpolate:
         :py:meth:`interpolate`.
 
         Parameters
         ----------
         *domain : ndarray
-            The domain axes which we are interpolating at, given in order as
-            the axes domain of this class.
+            The domain value axes which we are interpolating at, given in
+            order as the axes domain of this class.
 
         Returns
         -------
         v : ndarray
             The interpolated values.
 
         """
         # We only want to work with arrays.
         domain = [np.asarray(domaindex) for domaindex in domain]
 
         # The shape of all the the input must be the same shape. Defaulting
-        # to have the first element be the primo.
+        # to have the first element be the primary.
         input_shape = domain[0].shape
         for domaindex in domain:
             if domaindex.shape != input_shape:
                 logging.error(
                     logging.InputError,
                     message="Not all input domain axes have the same shape.",
                 )
@@ -973,20 +974,23 @@
         template : Callable
             The 1D interpolator template function which will be used to build
             the needed 1D interpolators. A template function can be constructed
             from the helper function :py:func:`generate_template`.
 
         """
         # We make sure that the axes provided properly match the array.
-        if v.shape != (x.size, y.size):
+        # The domain order provided above is actually the reverse of
+        # the Numpy convention.
+        domain_shape = (x.size, y.size)
+        if v.shape != reversed(domain_shape):
             logging.error(
                 error_type=logging.InputError,
                 message=(
-                    f"The shape of the data is {v.shape} which does not match"
-                    f" the provided axes (x, y): {(x.size, y.size)}."
+                    f"The shape of the data is {v.shape} which does not"
+                    f" match the provided axes (x, y): {domain_shape}."
                 ),
             )
 
         # Finally, assigning everything.
         self.x = x
         self.y = y
         self.v = v
@@ -1143,20 +1147,24 @@
         template : Callable
             The 1D interpolator template function which will be used to build
             the needed 1D interpolators. A template function can be constructed
             from the helper function :py:func:`generate_template`.
 
         """
         # We make sure that the axes provided properly match the array.
-        if v.shape != (x.size, y.size, z.size):
+        # The domain order provided above is actually the reverse of
+        # the Numpy convention.
+        domain_shape = (x.size, y.size, z.size)
+        if v.shape != reversed(domain_shape):
             logging.error(
                 error_type=logging.InputError,
                 message=(
-                    f"The shape of the data is {v.shape} which does not match"
-                    f" the provided axes (x, y, z): {(x.size, y.size, z.size)}."
+                    f"The shape of the data is {v.shape} which does not "
+                    " match the provided axes (x, y, z):"
+                    f" {domain_shape}."
                 ),
             )
 
         # Finally, assigning everything.
         self.x = x
         self.y = y
         self.z = z
@@ -1277,7 +1285,190 @@
         """
         return self._interpolate_slice(x, y, z)
 
     # A quick alias so that we can compute the interpolation as a simple call.
     __call__ = interpolate
 
 
+class RegularNDInterpolate(scipy.interpolate.RegularGridInterpolator):
+    """Wrapper for Scipy's regular grid interpolator.
+
+    This interpolator is more reliable than the :py:class:`RepeatNDInterpolate`
+    for cases where the regular grid is strictly preserved and no extrapolation
+    is needed. This interpolation is strictly cubic interpolation.
+
+    Note, we do not document attributes for the parent class. See
+    :py:class:`scipy.interpolate.RegularGridInterpolator` for more information.
+
+    Attributes
+    ----------
+    domain : list
+        A list of the domain axes values which define the multidimensional
+        data.
+    v : ndarray
+        The multi-dimensional data who's axes are defined. This data is the
+        data interpolated.
+
+    """
+
+    def __init__(
+        self: "RegularNDInterpolate",
+        domain: list[hint.ndarray],
+        v: hint.ndarray,
+    ) -> None:
+        """Create the interpolator, using the Scipy interpolator as a base.
+
+        Parameters
+        ----------
+        domain : list
+            The list of domain axis values of the multi-dimensional data.
+        v : ndarray
+            The data itself, the dimensions must match the provided axes.
+
+        Returns
+        -------
+        None
+
+        """
+        # We check that the shape provided by the domain matches the data
+        # shape. The domain order provided above is actually the reverse of
+        # the Numpy convention.
+        domain_shape = tuple(domaindex.size for domaindex in domain)
+        if reversed(domain_shape) != v.shape:
+            logging.error(
+                error_type=logging.InputError,
+                message=(
+                    f"The shape of the data is {v.shape} which does not "
+                    " match the expected shape from the provided domain"
+                    f" {domain_shape}."
+                ),
+            )
+
+        # Assigning the class attributes; we do not document any of the
+        # parent class attributes.
+        self.domain = domain
+        self.v = v
+
+        # Calling the parent class for the implementation.
+        super().__init__(
+            points=self.domain,
+            values=self.v,
+            method="cubic",
+            bounds_error=False,
+            fill_value=None,
+        )
+
+    def interpolate(self: hint.Self, *domain: hint.ndarray) -> hint.ndarray:
+        """Interpolate the data points provided their axis values.
+
+        Parameters
+        ----------
+        *domain : ndarray
+            The domain value axes which we are interpolating at, given in
+            order as the axes domain of this class.
+
+        Returns
+        -------
+        v : ndarray
+            The interpolated values.
+
+        """
+        # We only want to work with arrays.
+        domain = [np.asarray(domaindex) for domaindex in domain]
+
+        # The shape of all the the input must be the same shape. Defaulting
+        # to have the first element be the primary.
+        input_shape = domain[0].shape
+        for domaindex in domain:
+            if domaindex.shape != input_shape:
+                logging.error(
+                    logging.InputError,
+                    message="Not all input domain axes have the same shape.",
+                )
+
+        # We work with flat arrays, evaluating the interpolation points then
+        # repackage them back into the proper shape later.
+        flat_domain = [np.ravel(domaindex) for domaindex in domain]
+        # The points to interpolate at. Scipy can handle input of multiple
+        # points.
+        points = list(zip(*flat_domain, strict=True))
+        flat_result = self(points)
+
+        # Repackaging.
+        v = np.reshape(flat_result, input_shape)
+        # All done.
+        return v
+
+    def interpolate_point(self: hint.Self, *point: float) -> float:
+        """Interpolate a single point.
+
+        Parameters
+        ----------
+        *point : float
+            The point that we are interpolating to. The order of the float
+            values in this point should match the interpolation order of the
+            axes; similar to a Cartesian grid point.
+
+        Returns
+        -------
+        v : float
+            The interpolated output value.
+
+        """
+        # Need to make sure there is enough data points.
+        if len(point) != len(self.domain):
+            logging.error(
+                error_type=logging.InputError,
+                message=(
+                    f"Defined point has {len(point)} values, incompatible with"
+                    f" {len(self.domain)} dimensions."
+                ),
+            )
+
+        # We continuously reduce the dimensions, evaluating based on the
+        # input point.
+        v = self(point)
+        return v
+
+    def interpolate_slice(
+        self: hint.Self,
+        *slice_: float | None,
+    ) -> hint.ndarray:
+        """Interpolate a single slice of the data.
+
+        A "slice" is provided by specifying the values of specific points
+        to interpolate the given axis at. Specifying None keeps that dimension
+        part of the slice.
+
+        Parameters
+        ----------
+        slice_ : float | None
+            The slice specification to interpolate at. The order of the
+            parameters corresponds to the axis order. Specifying None
+            means the axis is part of the slice and is not interpolated.
+
+        Returns
+        -------
+        v : float
+            The interpolated output value.
+
+        """
+        # Need to make sure there is enough data points.
+        if len(slice_) != len(self.domain):
+            logging.error(
+                error_type=logging.InputError,
+                message=(
+                    f"Point has {len(slice_)} values, incompatible with"
+                    f" {len(self.domain)} dimensions."
+                ),
+            )
+
+        logging.critical(
+            critical_type=logging.ToDoError,
+            message=(
+                "Slice not figured out for Scipy regular grid interpolation."
+            ),
+        )
+
+        # All done.
+        v = None
+        return v
```

### Comparing `lezargus-0.0.4.dev44/src/lezargus/library/logging.py` & `lezargus-0.0.4.dev51/src/lezargus/library/logging.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,14 +113,23 @@
 
     This error is to be used when the configuration file or parameters are
     wrong. There is a specific expectation for how configuration files and
     configuration parameters are structures are defined.
     """
 
 
+class DeprecationError(LezargusError):
+    """An error used to note that something is deprecated with a replacement.
+
+    This error should be used to note that is a function is deprecated and to
+    use the documented replacement. There must always be a replacement for
+    the deprecated functionality except for extraneous circumstances.
+    """
+
+
 class DirectoryError(LezargusError):
     """An error used for directory issues.
 
     If there are issues with directories, use this error.
     """
```

### Comparing `lezargus-0.0.4.dev44/src/lezargus/library/math.py` & `lezargus-0.0.4.dev51/src/lezargus/library/math.py`

 * *Files 3% similar despite different names*

```diff
@@ -382,14 +382,56 @@
     )
     integrand_uncertainty = 0
     uncertainty = integrand_uncertainty
 
     return result, uncertainty
 
 
+def normalize_weights(weights: hint.ndarray) -> hint.ndarray:
+    """Normalize weights, handling NaNs so they don't screw things up.
+
+    We do not include NaNs in the normalization of the weights, however we
+    still keep them as weights to allow for its proper propagation when needed.
+
+    Parameters
+    ----------
+    weights : ndarray
+        The weights to normalize.
+
+    Returns
+    -------
+    normalized : ndarray
+        The weights normalized.
+
+    """
+    # It is easiest to deal with arrays.
+    weights = np.asarray(weights, dtype=float)
+
+    # Weights only make sense if they are real and finite. We clean up the
+    # weights to get a finite subset to calculate the normalization factor.
+    real_weights = lezargus.library.sanitize.clean_finite_arrays(weights)
+
+    # If there is no left over data to calculate the normalization factor,
+    # we use uniform weights...
+    if len(real_weights) == 0 or np.count_nonzero(real_weights) == 0:
+        using_weights = np.ones_like(real_weights)
+    # ...otherwise, we just use the real weights.
+    else:
+        using_weights = real_weights
+
+    # Computing the normalization summation.
+    weight_sum = np.nansum(using_weights)
+
+    # Normalizing the weights. We just ignore the parts with NaN and pass them
+    # on.
+    normalized = weights / weight_sum
+
+    return normalized
+
+
 def weighted_mean(
     values: hint.ndarray,
     uncertainties: hint.ndarray = None,
     weights: hint.ndarray = None,
 ) -> tuple[float, float]:
     """Calculate a weighted mean, propagating uncertainties where needed.
 
@@ -422,15 +464,15 @@
     # We determine the defaults for the uncertainty and the weights.
     uncertainties = (
         np.zeros_like(values) if uncertainties is None else uncertainties
     )
     weights = np.ones_like(values) if weights is None else weights
 
     # Normalize the weights.
-    norm_weights = weights / np.nansum(weights)
+    norm_weights = normalize_weights(weights=weights)
 
     # Finally, calculating the mean.
     mean_value = np.average(values, weights=norm_weights)
     # The error propagation, done as prescribed. We assume next to no
     # covariance and in general we calculate it via variance propagation of
     # the definition of the weighted mean.
     mean_uncertainty = np.sqrt(np.sum((uncertainties * norm_weights) ** 2))
@@ -475,15 +517,15 @@
     weights = np.ones_like(values) if weights is None else weights
 
     # We also do not include any values which are not actual numbers.
     (
         clean_values,
         clean_uncertainty,
         clean_weights,
-    ) = lezargus.library.array.clean_finite_arrays(
+    ) = lezargus.library.sanitize.clean_finite_arrays(
         values,
         uncertainties,
         weights,
     )
 
     # And we just send it to the original function to compute it.
     mean_value, mean_uncertainty = weighted_mean(
@@ -654,15 +696,15 @@
     weights = np.ones_like(values) if weights is None else weights
 
     # We also do not include any values which are not actual numbers.
     (
         clean_values,
         clean_uncertainty,
         clean_weights,
-    ) = lezargus.library.array.clean_finite_arrays(
+    ) = lezargus.library.sanitize.clean_finite_arrays(
         values,
         uncertainties,
         weights,
     )
 
     # And we just send it to the original function to compute it.
     median_value, median_uncertainty = median(
```

### Comparing `lezargus-0.0.4.dev44/src/lezargus/library/path.py` & `lezargus-0.0.4.dev51/src/lezargus/library/path.py`

 * *Files 2% similar despite different names*

```diff
@@ -190,15 +190,15 @@
 
     """
     extension = os.path.basename(pathname).split(".")[-1]
     return extension
 
 
 def merge_pathname(
-    directory: hint.Union[str, list] = None,
+    directory: hint.Union[str, list] | None = None,
     filename: str | None = None,
     extension: str | None = None,
 ) -> str:
     """Join the directories, filenames, and file extensions into one pathname.
 
     Parameters
     ----------
```

### Comparing `lezargus-0.0.4.dev44/src/lezargus/library/photometry.py` & `lezargus-0.0.4.dev51/src/lezargus/library/photometry.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,35 +2,35 @@
 
 import lezargus
 from lezargus.library import hint
 from lezargus.library import logging
 
 
 def calculate_filter_zero_point_vega(
-    filter_spectra: hint.LezargusSpectra,
-    standard_spectra: hint.LezargusSpectra,
+    filter_spectra: hint.LezargusSpectrum,
+    standard_spectra: hint.LezargusSpectrum,
     standard_filter_magnitude: float,
     standard_filter_uncertainty: float | None = None,
 ) -> tuple[float, float | None]:
     """Calculate the magnitude zero point of a filter in the Vega system.
 
     This function computes Vega zero points by integrating it over the
     filter band pass. To better facilitate this as a library function, the
     standard spectra and its magnitude may be input. However, for most cases,
     the Vega spectra in the data collection is good enough.
 
     Parameters
     ----------
-    filter_spectra : LezargusSpectra
+    filter_spectra : LezargusSpectrum
         The filter transmission, saved as a spectra container instance. The
         filter provided must be in the photon counting form. We assume that
         the wavelength term has already been multiplied through. The
         variable name is chosen to prevent a name clash with the Python
         built-in.
-    standard_spectra : LezargusSpectra
+    standard_spectra : LezargusSpectrum
         The standard star, as saved by a spectra container instance.
     standard_filter_magnitude : float
         The magnitude of the standard star in that filter.
     standard_filter_uncertainty : float, default = None
         The uncertainty in the magnitude of the standard star in that filter.
         Often this is not needed because the magnitude value of standard
         defines the filter system anyways and so, by definition, there is no
@@ -123,31 +123,31 @@
     )
 
     # All done.
     return zero_point, zero_point_uncertainty
 
 
 def calculate_filter_magnitude_vega(
-    star_spectra: hint.LezargusSpectra,
-    filter_spectra: hint.LezargusSpectra,
+    star_spectra: hint.LezargusSpectrum,
+    filter_spectra: hint.LezargusSpectrum,
     filter_zero_point: float,
     filter_zero_point_uncertainty: float | None = None,
 ) -> tuple[float, float]:
     """Calculate the Vega-based synthetic magnitude of a star in a filter.
 
     We compute the synthetic magnitude of a star using its spectra, provided
     the filter transmission. This function is the manual method, where the
     filters and its properties must be defined manually. An automatic mode
     is also available, see `auto_calculate_filter_magnitude_vega`.
 
     Parameters
     ----------
-    star_spectra : LezargusSpectra
+    star_spectra : LezargusSpectrum
         The target star that we will compute the synthetic filter magnitude of.
-    filter_spectra : LezargusSpectra
+    filter_spectra : LezargusSpectrum
         The filter transmission, saved as a spectra container instance. The
         filter provided must be in the photon counting form. We assume that
         the wavelength term has already been multiplied through. The
         variable name is chosen to prevent a name clash with the Python
         built-in.
     filter_zero_point : float
         The zero point value for the provided filter.
@@ -240,16 +240,16 @@
     )
 
     # All done.
     return magnitude, uncertainty
 
 
 def calculate_photometric_correction_factor_vega(
-    star_spectra: hint.LezargusSpectra,
-    filter_spectra: hint.LezargusSpectra,
+    star_spectra: hint.LezargusSpectrum,
+    filter_spectra: hint.LezargusSpectrum,
     star_magnitude: float,
     filter_zero_point: float,
     star_magnitude_uncertainty: float | None = None,
     filter_zero_point_uncertainty: float | None = None,
 ) -> tuple[float, float]:
     """Compute photometric correction factors for Vega-based filters.
 
@@ -257,17 +257,17 @@
     the scaling factor to scale the spectra so that it is
     spectro-photometrically calibrated.
 
     See [[TODO]] for more information.
 
     Parameters
     ----------
-    star_spectra : LezargusSpectra
+    star_spectra : LezargusSpectrum
         The target star that we will compute the synthetic filter magnitude of.
-    filter_spectra : LezargusSpectra
+    filter_spectra : LezargusSpectrum
         The filter transmission, saved as a spectra container instance. The
         filter provided must be in the photon counting form. We assume that
         the wavelength term has already been multiplied through. The
         variable name is chosen to prevent a name clash with the Python
         built-in.
     star_magnitude : float
         The magnitude of the star in the given filter. We use this value to
```

### Comparing `lezargus-0.0.4.dev44/src/lezargus/library/stitch.py` & `lezargus-0.0.4.dev51/src/lezargus/library/stitch.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,31 +17,31 @@
     base_data: hint.ndarray,
     input_wavelength: hint.ndarray,
     input_data: hint.ndarray,
     base_uncertainty: hint.ndarray = None,
     input_uncertainty: hint.ndarray = None,
     bounds: tuple[float, float] = (-np.inf, +np.inf),
 ) -> tuple[float, float]:
-    """Find the scale factor to scale one overlapping spectra to another.
+    """Find the scale factor to scale one overlapping spectrum to another.
 
-    We determine what scale factor would properly match some input spectra
+    We determine what scale factor would properly match some input spectrum
     data to some base data, provided that they have some wavelength overlap.
     An additional bounds may be set in addition to the wavelength overlap.
     The method provided is described in [[TODO]].
 
     Parameter
     ---------
     base_wavelength : ndarray
-        The wavelength array of the base spectra data. Must be the same unit
+        The wavelength array of the base spectrum data. Must be the same unit
         as the input wavelength.
     base_data : ndarray
         The spectral data of the base, which the scale factor would scale the
         input to.
     input_wavelength : ndarray
-        The wavelength array of the input spectra data. Must be the same unit
+        The wavelength array of the input spectrum data. Must be the same unit
         as the base wavelength.
     input_data : ndarray
         The spectral data of the input, what the scale factor is for.
     base_uncertainty : ndarray, default = None
         The uncertainty on the base data. If None, we default to no
         uncertainty.
     input_uncertainty : ndarray, default = None
@@ -120,15 +120,15 @@
     # We do not want to include any NaNs or non-numbers.
     (
         __,
         clean_base_data,
         clean_base_uncertainty,
         clean_input_data,
         clean_input_uncertainty,
-    ) = lezargus.library.array.clean_finite_arrays(
+    ) = lezargus.library.sanitize.clean_finite_arrays(
         overlap_wavelength,
         overlap_base_data,
         overlap_base_uncertainty,
         overlap_input_data,
         overlap_input_uncertainty,
     )
 
@@ -160,16 +160,25 @@
         lezargus.library.math.divide(
             numerator=clean_base_data,
             denominator=guess_input_data,
             numerator_uncertainty=clean_base_uncertainty,
             denominator_uncertainty=guess_input_uncertainty,
         )
     )
+    # Using inverse squared weights. We NaN out any zero uncertainty values
+    # as they are likely not real.
+    using_uncertainty = np.where(
+        base_input_ratio_uncertainty == 0,
+        np.nan,
+        base_input_ratio_uncertainty,
+    )
+    weights = 1 / using_uncertainty**2
+    weights = lezargus.library.math.normalize_weights(weights=weights)
+
     # Finding the average ratio.
-    weights = 1 / base_input_ratio_uncertainty**2
     quantile_cut_ratio = 0.05
     adjust_scale_factor, adjust_scale_uncertainty = (
         lezargus.library.math.weighted_quantile_mean(
             values=base_input_ratio,
             uncertainties=base_input_ratio_uncertainty,
             weights=weights,
             quantile=quantile_cut_ratio,
@@ -217,23 +226,25 @@
     # We need to determine the sampling mode for combining the wavelengths.
     sample_mode = sample_mode.casefold()
     stitched_wavelength_points = []
     if sample_mode == "merge":
         # We are sampling based on total interlacing, without care. We just
         # merge the arrays.
         # Cleaning the arrays first.
-        wavelengths = lezargus.library.array.clean_finite_arrays(*wavelengths)
+        wavelengths = lezargus.library.sanitize.clean_finite_arrays(
+            *wavelengths,
+        )
         # And just combining them.
         for wavedex in wavelengths:
             stitched_wavelength_points = (
                 stitched_wavelength_points + wavedex.tolist()
             )
     elif sample_mode == "hierarchy":
         # We combine the spectra hierarchically, taking into account the
-        # minimum and maximum bounds of the higher level spectra. We first
+        # minimum and maximum bounds of the higher level spectrum. We first
         # start with a case that is always true.
         min_hist = [+np.inf]
         max_hist = [-np.inf]
         for wavedex in wavelengths:
             # We only add points in wave bands that have not already been
             # covered, we use this by checking the history.
             valid_points = np.full_like(wavedex, True, dtype=bool)
@@ -244,15 +255,15 @@
                     (mindex <= wavedex) & (wavedex <= maxdex)
                 )
             # We add only the valid points to the combined wavelength.
             stitched_wavelength_points = (
                 stitched_wavelength_points + wavedex[valid_points].tolist()
             )
             # And we also update the minimum and maximum history to establish
-            # this spectra for the provided region.
+            # this spectrum for the provided region.
             min_hist.append(np.nanmin(wavedex))
             max_hist.append(np.nanmax(wavedex))
     else:
         # The provided mode is not one of the supported ones.
         logging.critical(
             critical_type=logging.InputError,
             message=(
@@ -286,15 +297,15 @@
     hint.Callable[[hint.ndarray], hint.ndarray],
     hint.Callable[[hint.ndarray], hint.ndarray],
     hint.Callable[[hint.ndarray], hint.ndarray],
 ]:
     R"""Stitch spectra functions together.
 
     We take functional forms of the wavelength, data, uncertainty, and weight
-    (in the form of f(wave) = result), and determine the average spectra.
+    (in the form of f(wave) = result), and determine the average spectrum.
     We assume that the all of the functional forms properly handle any bounds,
     gaps, and interpolative limits. The input lists of functions should be
     parallel and all of them should be of the same (unit) scale.
 
     For more information, the formal method is described in [[TODO]].
 
     Parameters
@@ -382,15 +393,17 @@
                 "Stitch functional default bounds should be configuration"
                 " filed."
             ),
         )
         reference_wavelength = np.linspace(0.30, 5.50, 1000000)
     else:
         reference_wavelength = np.sort(
-            *lezargus.library.array.clean_finite_arrays(reference_wavelength),
+            *lezargus.library.sanitize.clean_finite_arrays(
+                reference_wavelength,
+            ),
         )
 
     # Now, we need to have the lists all be parallel, a quick and dirty check
     # is to make sure they are all the same length. We assume the user did not
     # make any mistakes when pairing them up.
     if (
         not len(wavelength_functions)
@@ -458,15 +471,15 @@
         uncertainty_value : float
             The uncertainty on the average as propagated.
 
         """
         # We clean out the data, this is the primary way to determine if there
         # is usable data or not.
         clean_values, clean_uncertainties, clean_weights = (
-            lezargus.library.array.clean_finite_arrays(
+            lezargus.library.sanitize.clean_finite_arrays(
                 _values,
                 _uncertainty,
                 _weights,
             )
         )
         # If any of the arrays are blank, there are no clean values to use.
         if (
@@ -567,45 +580,45 @@
     interpolate_routine: hint.Generic1DInterpolate | None = None,
     reference_wavelength: hint.ndarray = None,
 ) -> tuple[hint.ndarray, hint.ndarray, hint.ndarray]:
     R"""Stitch spectra data arrays together.
 
     We take the discrete point data of spectra (wavelength, data, and
     uncertainty), along with weights, to stitch together and determine the
-    average spectra. The scale of the data and uncertainty should be of the
+    average spectrum. The scale of the data and uncertainty should be of the
     same scale, as should the wavelength and reference points.
 
     This function serves as the intended way to stitch spectra, though
     :py:func:`stitch.stitch_spectra_functional` is the
     work-horse function and more information can be found there. We build
     interpolators for said function using the input data and attempt to
     guess for any gaps.
 
     Parameters
     ----------
     wavelength_arrays : list[ndarray]
-        The list of the wavelength arrays representing each spectra.
+        The list of the wavelength arrays representing each spectrum.
     data_arrays : list[ndarray]
-        The list of the data arrays representing each spectra.
+        The list of the data arrays representing each spectrum.
     uncertainty_arrays : list[ndarray], default = None
         The list of the uncertainty arrays representing the data of each
-        spectra. The scale of the data arrays and uncertainty arrays should be
+        spectrum. The scale of the data arrays and uncertainty arrays should be
         the same. If None, we default to no uncertainty.
     weight_arrays : list[ndarray], default = None
-        The list of the weight arrays to weight each spectra for the average
+        The list of the weight arrays to weight each spectrum for the average
         routine. If None, we assume uniform weights.
     average_routine : Callable, default = None
         The averaging function. It must be able to support the propagation of
         uncertainties and weights. As such, it should have the form of
         :math:`\text{avg}(x, \sigma, w) \rightarrow \bar{x} \pm \sigma`.
         If None, we use a standard weighted average, ignoring NaNs.
     interpolate_routine : Generic1DInterpolate, default = None
         The 1D interpolation routine class used to handle interpolation.
     reference_wavelength : ndarray, default = None
-        The reference wavelength is where the stitched spectra wavelength
+        The reference wavelength is where the stitched spectrum wavelength
         values should be. If None, we attempt to construct it based on the
         overlap and ordering of the input wavelength arrays. We do not accept
         NaNs in either cases and remove them.
 
     Returns
     -------
     stitched_wavelength_points : ndarray
@@ -622,14 +635,20 @@
             np.zeros_like(wavedex) for wavedex in wavelength_arrays
         ]
     if weight_arrays is None:
         weight_arrays = [np.ones_like(wavedex) for wavedex in wavelength_arrays]
     if average_routine is None:
         average_routine = lezargus.library.math.nan_weighted_mean
 
+    # The weights should be normalized.
+    weight_arrays = [
+        lezargus.library.math.normalize_weights(weights=weightdex)
+        for weightdex in weight_arrays
+    ]
+
     # If a custom routine is provided, we need to make sure it is the right
     # type. Otherwise, we just use a default spline interpolator.
     interpolate_routine = (
         lezargus.library.interpolate.Spline1DInterpolate
         if interpolate_routine is None
         else interpolate_routine
     )
@@ -649,15 +668,15 @@
     # information provided or a custom inputted value.
     if reference_wavelength is None:
         # We try and parse the reference wavelength; we assume the defaults of
         # this function is good enough.
         reference_wavelength = stitch_wavelengths_discrete(*wavelength_arrays)
     # Still sorting it and making sure it is clean.
     reference_wavelength = np.sort(
-        *lezargus.library.array.clean_finite_arrays(reference_wavelength),
+        *lezargus.library.sanitize.clean_finite_arrays(reference_wavelength),
     )
 
     # We next need to check the shape and the broadcasting of values for all
     # data. This is mostly a check to make sure that the shapes are compatible
     # and to also format them to better broadcasted versions (in the event) of
     # single value entires.
     wavelength_broadcasts = []
@@ -675,29 +694,29 @@
     ):
         # We assume that the wavelength array is the canonical data shape
         # for each and every data.
         temp_wave = wavedex
         # We now check for all of the other arrays, checking notating any
         # irregularities. We of course log if there is an issue.
         verify_data, temp_data = (
-            lezargus.library.array.verify_shape_compatibility(
+            lezargus.library.sanitize.verify_broadcastability(
                 reference_array=temp_wave,
                 test_array=datadex,
                 return_broadcast=True,
             )
         )
         verify_uncert, temp_uncert = (
-            lezargus.library.array.verify_shape_compatibility(
+            lezargus.library.sanitize.verify_broadcastability(
                 reference_array=temp_wave,
                 test_array=uncertdex,
                 return_broadcast=True,
             )
         )
         verify_weight, temp_weight = (
-            lezargus.library.array.verify_shape_compatibility(
+            lezargus.library.sanitize.verify_broadcastability(
                 reference_array=temp_wave,
                 test_array=weightdex,
                 return_broadcast=True,
             )
         )
         if not (verify_data and verify_uncert and verify_weight):
             logging.error(
@@ -713,15 +732,15 @@
 
         # We use the broadcasted arrays as the main ones we will use.
         wavelength_broadcasts.append(temp_wave)
         data_broadcasts.append(temp_data)
         uncertainty_broadcasts.append(temp_uncert)
         weight_broadcasts.append(temp_weight)
 
-    # We need to build the interpolators for each section of the spectra, as
+    # We need to build the interpolators for each section of the spectrum, as
     # it is what we will input.
     # We attempt to find the gaps in the data, assuming that the wavelength
     # arrays are complete.
     gap_guess = [
         lezargus.library.interpolate.get_smallest_gap(wavelength=wavedex)
         for wavedex in wavelength_broadcasts
     ]
@@ -737,15 +756,15 @@
         uncertainty_broadcasts,
         weight_broadcasts,
         gap_guess,
         strict=True,
     ):
         # We clean up all of the data, the gap is not included.
         clean_wave, clean_data, clean_uncert, clean_weight = (
-            lezargus.library.array.clean_finite_arrays(
+            lezargus.library.sanitize.clean_finite_arrays(
                 wavedex,
                 datadex,
                 uncertdex,
                 weightdex,
             )
         )
         # If any of the arrays are lacking enough data points for interpolation
```

### Comparing `lezargus-0.0.4.dev44/src/lezargus/library/temporary.py` & `lezargus-0.0.4.dev51/src/lezargus/library/temporary.py`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/src/lezargus/library/wrapper.py` & `lezargus-0.0.4.dev51/src/lezargus/library/wrapper.py`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/src/lezargus/simulation/spectre.py` & `lezargus-0.0.4.dev51/src/lezargus/simulation/spectre.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     By default, all attributes are public to allow for maximum transparency.
     By convention, please treat the attributes as read-only. Consult the
     documentation for changing them. By default, they are None, this allows
     us to track the process of the simulation.
 
     Attributes
     ----------
-    astrophysical_object_spectra : LezargusSpectra
+    astrophysical_object_spectra : LezargusSpectrum
         The "perfect" spectra of the astrophysical object who's observation is
         being modeled.
     astrophysical_object_cube : LezargusCube
         The cube form of the perfect astrophysical object who's observation is
         being modeled.
     astrophysical_object_cube_atm_trn : LezargusCube
         The astrophysical object after applying the atmospheric transmission.
@@ -89,17 +89,17 @@
         """
         return self.astronomical_object_cube
 
     def create_astrophysical_object_spectra(
         self: hint.Self,
         temperature: float,
         magnitude: float,
-        filter_spectra: hint.LezargusSpectra,
+        filter_spectra: hint.LezargusSpectrum,
         filter_zero_point: float,
-    ) -> hint.LezargusSpectra:
+    ) -> hint.LezargusSpectrum:
         """Create the astrophysical object from first principles.
 
         This function creates and stores the astrophysical object spectra
         modeled as a blackbody of a specific temperature. If a custom spectra
         is to be provided, please see
         :py:meth:`custom_astrophysical_object_spectra`.
         The data is stored in this class internally as
@@ -108,24 +108,24 @@
         Parameters
         ----------
         temperature : float
             The temperature of the black body spectra.
         magnitude : float
             The magnitude of the object in the photometric filter system
             provided.
-        filter_spectra : LezargusSpectra
-            The filter transmission profile, packaged as a LezargusSpectra. It
+        filter_spectra : LezargusSpectrum
+            The filter transmission profile, packaged as a LezargusSpectrum. It
             does not need to have any header data. We assume a Vega-based
             photometric system.
         filter_zero_point : float
             The zero point value of the filter.
 
         Returns
         -------
-        spectra : LezargusSpectra
+        spectra : LezargusSpectrum
             The astrophysical object spectra; it is returned as a courtesy as
             the result is stored in this class.
 
         """
         # We need to construct our own wavelength base line, we rely on the
         # limits of SPECTRE itself.
         wavelength = np.linspace(
@@ -142,15 +142,15 @@
         # Then we evaluate the blackbody function, of course the scale of which
         # will be wrong but it will be fixed.
         blackbody_flux = blackbody_function(wavelength)
         # We integrate over the solid angle.
         solid_angle = np.pi
         integrated_blackbody_flux = blackbody_flux * solid_angle
         # Packaging the spectra.
-        blackbody_spectra = lezargus.container.LezargusSpectra(
+        blackbody_spectra = lezargus.container.LezargusSpectrum(
             wavelength=wavelength,
             data=integrated_blackbody_flux,
             uncertainty=None,
             wavelength_unit="m",
             data_unit="W m^-2 m^-1",
             pixel_scale=None,
             slice_scale=None,
@@ -185,15 +185,15 @@
         photon_flux = calibrated_flux / photon_energy
 
         # Although we do not need a fully fledged header, we add some small
         # information where we know.
         header = {"LZI_INST": "SPECTRE", "LZO_NAME": "Simulation"}
 
         # Compiling the spectra class and storing it.
-        self.astrophysical_object_spectra = lezargus.container.LezargusSpectra(
+        self.astrophysical_object_spectra = lezargus.container.LezargusSpectrum(
             wavelength=wavelength,
             data=photon_flux,
             uncertainty=None,
             wavelength_unit="m",
             data_unit="ph s^-1 m^-2 m^-1",
             pixel_scale=None,
             slice_scale=None,
@@ -202,16 +202,16 @@
             header=header,
         )
         # All done.
         return self.astrophysical_object_spectra
 
     def custom_astrophysical_object_spectra(
         self: hint.Self,
-        custom_spectra: hint.LezargusSpectra,
-    ) -> hint.LezargusSpectra:
+        custom_spectra: hint.LezargusSpectrum,
+    ) -> hint.LezargusSpectrum:
         """Use a provided spectra for a custom astrophysical object.
 
         This function is used to provide a custom spectra class to use to
         define the astrophysical object. If it should be derived instead from
         much simpler first principles, then please use
         :py:meth:`create_astrophysical_object_spectra` instead. The data is
         stored in this class internally as
@@ -224,33 +224,33 @@
         Note that the wavelength axis of the custom spectra is used to define
         the wavelength scaling of the astrophysical object. We do not add
         any unknown information.
 
 
         Parameters
         ----------
-        custom_spectra : LezargusSpectra
+        custom_spectra : LezargusSpectrum
             The custom provided spectral object to use for the custom
             astrophysical object.
 
         Returns
         -------
-        spectra : LezargusSpectra
+        spectra : LezargusSpectrum
             The astrophysical object spectra; it is returned as a courtesy as
             the result is stored in this class. This is the same as the input
             spectra and the return is for consistency.
 
         """
         # We really just use it as is, aside from a simple check to make sure
         # the input is not going to screw things up down the line.
-        if not isinstance(custom_spectra, lezargus.container.LezargusSpectra):
+        if not isinstance(custom_spectra, lezargus.container.LezargusSpectrum):
             logging.error(
                 error_type=logging.InputError,
                 message=(
-                    "The custom input spectra is not a LezargusSpectra"
+                    "The custom input spectra is not a LezargusSpectrum"
                     f" instance but is instead has type {type(custom_spectra)}."
                 ),
             )
         self.astrophysical_object_spectra = custom_spectra
         return self.astrophysical_object_spectra
 
     def generate_astrophysical_object_cube(
@@ -333,16 +333,16 @@
             flags=None,
             header=None,
         )
 
         # We use this template cube to broadcast it to a center-pixel to
         # simulate a point source target.
         self.astrophysical_object_cube = (
-            lezargus.container.broadcast.broadcast_spectra_to_cube_center(
-                input_spectra=self.astrophysical_object_spectra,
+            lezargus.container.broadcast.broadcast_spectrum_to_cube_center(
+                input_spectrum=self.astrophysical_object_spectra,
                 template_cube=template_cube,
                 wavelength_mode="error",
                 allow_even_center=True,
             )
         )
         # Just returning the cube as well.
         return self.astrophysical_object_cube
@@ -363,15 +363,15 @@
         Note that the wavelength axis of the custom cube is used to define
         the wavelength scaling of the astrophysical object. We do not add
         any unknown information.
 
 
         Parameters
         ----------
-        custom_cube : LezargusSpectra
+        custom_cube : LezargusSpectrum
             The custom provided spectral cube object to use for the custom
             astrophysical object field.
 
         Returns
         -------
         cube : LezargusCube
             The astrophysical object cube; it is returned as a courtesy as
@@ -390,19 +390,19 @@
                 ),
             )
         self.astrophysical_object_cube = custom_cube
         return self.astrophysical_object_cube
 
     def prepare_spectra(
         self: hint.Self,
-        spectra: hint.LezargusSpectra,
+        spectra: hint.LezargusSpectrum,
         *args: object,
         skip_convolve: bool = False,
         **kwargs: object,
-    ) -> hint.LezargusSpectra:
+    ) -> hint.LezargusSpectrum:
         """Prepare the provided spectra for future steps.
 
         Any provided spectra (transmission curves, emission curves, etc) must
         be properly prepared before its application to the simulation data.
         We do the following steps in order (if not otherwise skipped):
 
             - Convolve: We match the spectral resolution (or resolving power)
@@ -412,38 +412,38 @@
         Please see the linked functions in each of the steps for the parameters
         required for each step of the preparation, if it is not to be skipped.
         Without the required inputs, the preparation will likely fail; failure
         will likely be noisy (logged or raised).
 
         Parameters
         ----------
-        spectra : LezargusSpectra
+        spectra : LezargusSpectrum
             The input spectra which we will be preparing.
         skip_convolve : bool, default = False
             If True, we skip the resolution convolution step. The backend
             function will not be called.
         *args : Any
             The positional arguments. We forbid any positional arguments for
             informing the backend functions because of its ambiguity.
         **kwargs : Any
             The keyword arguments which will be fed into the backend functions.
 
         Returns
         -------
-        finished_spectra : LezargusSpectra
+        finished_spectra : LezargusSpectrum
             The finished prepared spectra after all of the steps have been
             done.
 
         """
         # Type check on the input spectra.
-        if not isinstance(spectra, lezargus.container.LezargusSpectra):
+        if not isinstance(spectra, lezargus.container.LezargusSpectrum):
             logging.error(
                 error_type=logging.InputError,
                 message=(
-                    "Input spectra is not a LezargusSpectra, is instead:"
+                    "Input spectra is not a LezargusSpectrum, is instead:"
                     f" {type(spectra)}"
                 ),
             )
 
         # There should be no positional arguments.
         if len(args) != 0:
             logging.critical(
@@ -467,35 +467,35 @@
 
         # All done.
         finished_spectra = convolved_spectra
         return finished_spectra
 
     def _prepare_spectra_convolve(
         self: hint.Self,
-        spectra: hint.LezargusSpectra,
+        spectra: hint.LezargusSpectrum,
         input_resolution: float | None = None,
         input_resolving: float | None = None,
         simulation_resolution: float | None = None,
         simulation_resolving: float | None = None,
         reference_wavelength: float | None = None,
         **kwargs: object,
-    ) -> hint.LezargusSpectra:
+    ) -> hint.LezargusSpectrum:
         """Convolve the input spectra to make its resolution match.
 
         Spectra comes in many resolutions. If the resolution of an input
         spectra is too high for the simulation, its application can give
         erroneous results. Here, we use a Gaussian kernel to convolve the
         spectral data to better match the resolution of the input and the
         simulation.
 
         We leverage :py:func:`kernel_1d_gaussian_resolution` to make the kernel.
 
         Parameters
         ----------
-        spectra : LezargusSpectra
+        spectra : LezargusSpectrum
             The transmission spectra which we will be preparing.
         input_resolution : float, default = None
             The spectral resolution of the input spectra. Must be in
             the same units as the spectra.
         input_resolving : float, default = None
             The spectral resolving power of the input spectra, relative
             to the wavelength `reference_wavelength`.
@@ -508,15 +508,15 @@
         reference_wavelength : float, default = None
             The reference wavelength for any needed conversion.
         **kwargs : dict
             Keyword argument catcher.
 
         Returns
         -------
-        convolved_spectra : LezargusSpectra
+        convolved_spectra : LezargusSpectrum
             The spectra, after convolution based on the input parameters.
 
         """
         # This is just to catch and use the keyword arguments.
         __ = kwargs
 
         # We assume the kernel size based on the wavelength of the input
@@ -545,15 +545,15 @@
         convolved_spectra = spectra.convolve(kernel=gaussian_kernel)
 
         # All done.
         return convolved_spectra
 
     def apply_atmospheric_transmission(
         self: hint.Self,
-        transmission_spectra: hint.LezargusSpectra,
+        transmission_spectra: hint.LezargusSpectrum,
     ) -> hint.LezargusCube:
         """Apply the atmospheric transmission to the object.
 
         The astrophysical object cube is required to use this function,
         see :py:meth:`create_astrophysical_object_cube` or
         :py:meth:`custom_astrophysical_object_cube` to create it. The results
         are stored in this class internally as
@@ -561,15 +561,15 @@
 
         Moreover, consider using :py:meth:`prepare_spectra`
         to properly match the resolving power or resolution of the simulation
         spectra and the transmission spectra.
 
         Parameters
         ----------
-        transmission_spectra : LezargusSpectra
+        transmission_spectra : LezargusSpectrum
             The atmospheric transmission spectra. The wavelength unit of
             this spectra should be meters.
 
         Returns
         -------
         cube : LezargusCube
             The cube of the object after atmospheric transmission has been
@@ -583,84 +583,84 @@
                 message=(
                     "There is no astrophysical object cube to apply the"
                     " atmospheric transmission to."
                 ),
             )
 
         # We also need to make sure the transmission spectra is a
-        # LezargusSpectra.
+        # LezargusSpectrum.
         if not isinstance(
             transmission_spectra,
-            lezargus.container.LezargusSpectra,
+            lezargus.container.LezargusSpectrum,
         ):
             logging.error(
                 error_type=logging.InputError,
                 message=(
                     "The atmospheric transmission spectra has type"
                     f" {type(transmission_spectra)}, not the expected"
-                    " LezargusSpectra."
+                    " LezargusSpectrum."
                 ),
             )
 
         # We need to align the transmission spectra to the Simulators
         # wavelength base.
         trans_wave = self.astrophysical_object_cube.wavelength
         trans_data, trans_uncert, trans_mask, trans_flags = (
             transmission_spectra.interpolate(
                 wavelength=trans_wave,
                 skip_flags=True,
                 skip_mask=True,
             )
         )
         # It is convenient to reconstruct a spectra for it.
-        aligned_transmission_spectra = lezargus.container.LezargusSpectra(
+        aligned_transmission_spectra = lezargus.container.LezargusSpectrum(
             wavelength=trans_wave,
             data=trans_data,
             uncertainty=trans_uncert,
             wavelength_unit=transmission_spectra.wavelength_unit,
             data_unit=transmission_spectra.data_unit,
             mask=trans_mask,
             flags=trans_flags,
             header=transmission_spectra.header,
         )
 
         # We then pad this spectra out to a cube for us to apply across the
         # board.
         aligned_transmission_cube = (
-            lezargus.container.broadcast.broadcast_spectra_to_cube_uniform(
-                input_spectra=aligned_transmission_spectra,
+            lezargus.container.broadcast.broadcast_spectrum_to_cube_uniform(
+                input_spectrum=aligned_transmission_spectra,
                 template_cube=self.astrophysical_object_cube,
             )
         )
 
         # Applying the transmission is simple multiplication.
         self.astrophysical_object_cube_atm_trn = (
             self.astrophysical_object_cube * aligned_transmission_cube
         )
         # All done.
         return self.astrophysical_object_cube_atm_trn
 
     def apply_atmospheric_radiance(
         self: hint.Self,
-        radiance_spectra: hint.LezargusSpectra,
+        radiance_spectra: hint.LezargusSpectrum,
     ) -> hint.LezargusCube:
         """Apply atmospheric radiance spectra to the object.
 
         The astrophysical object cube with transmission is required to use
         this function, see :py:meth:`apply_atmospheric_transmission`. The
         results are stored in this class internally as
         :py:attr:`astrophysical_object_cube_atm_rad`.
 
         Moreover, consider using :py:meth:`prepare_spectra`
         to properly match the resolving power or resolution of the simulation
         spectra and the radiance spectra.
 
         Parameters
         ----------
-        radiance_spectra : LezargusSpectra
+        radiance_spectra : LezargusSpectrum
             The atmospheric radiance spectra. The wavelength unit of
             this spectra should be meters.
 
         Returns
         -------
         cube : LezargusCube
             The cube of the object after atmospheric radiance has been added.
@@ -673,55 +673,55 @@
                 message=(
                     "There is no astrophysical object cube with atmospheric"
                     " transmission to apply the atmospheric radiance to."
                 ),
             )
 
         # We also need to make sure the transmission spectra is a
-        # LezargusSpectra.
+        # LezargusSpectrum.
         if not isinstance(
             radiance_spectra,
-            lezargus.container.LezargusSpectra,
+            lezargus.container.LezargusSpectrum,
         ):
             logging.error(
                 error_type=logging.InputError,
                 message=(
                     "The atmospheric radiance spectra has type"
                     f" {type(radiance_spectra)}, not the expected"
-                    " LezargusSpectra."
+                    " LezargusSpectrum."
                 ),
             )
 
         # We need to align the transmission spectra to the Simulators
         # wavelength base.
         rad_wave = self.astrophysical_object_cube_atm_trn.wavelength
         rad_data, rad_uncert, rad_mask, rad_flags = (
             radiance_spectra.interpolate(
                 wavelength=rad_wave,
                 skip_flags=True,
                 skip_mask=True,
             )
         )
         # It is convenient to reconstruct a spectra for it.
-        aligned_radiance_spectra = lezargus.container.LezargusSpectra(
+        aligned_radiance_spectra = lezargus.container.LezargusSpectrum(
             wavelength=rad_wave,
             data=rad_data,
             uncertainty=rad_uncert,
             wavelength_unit=radiance_spectra.wavelength_unit,
             data_unit=radiance_spectra.data_unit,
             mask=rad_mask,
             flags=rad_flags,
             header=radiance_spectra.header,
         )
 
         # We then pad this spectra out to a cube for us to apply across the
         # board.
         aligned_radiance_cube = (
-            lezargus.container.broadcast.broadcast_spectra_to_cube_uniform(
-                input_spectra=aligned_radiance_spectra,
+            lezargus.container.broadcast.broadcast_spectrum_to_cube_uniform(
+                input_spectrum=aligned_radiance_spectra,
                 template_cube=self.astrophysical_object_cube_atm_trn,
             )
         )
 
         # Adding the sky radiance.
         self.astrophysical_object_cube_atm_rad = (
             self.astrophysical_object_cube + aligned_radiance_cube
```

### Comparing `lezargus-0.0.4.dev44/tests/conftest.py` & `lezargus-0.0.4.dev51/tests/conftest.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 """We set up a few things for the testing environment."""
 
-import pytest
 import os
 
+import pytest
+
 import lezargus
 
 
 def pytest_sessionstart(session: pytest.Session) -> None:
-    """
-    Called after the Session object has been created and
+    """Called after the Session object has been created and
     before performing collection and entering the run test loop.
 
     Parameters
     ----------
     session : Session
 
     Returns
     -------
     None
+
     """
     # We need to load the new configuration file.
     test_directory = os.path.dirname(
         os.path.realpath(os.path.join(os.path.realpath(__file__))),
     )
     test_configuration_file = lezargus.library.path.merge_pathname(
         directory=test_directory,
         filename="test_configuration_overrides",
         extension="yaml",
     )
     lezargus.library.config.load_configuration_file(
-        filename=test_configuration_file
+        filename=test_configuration_file,
     )
 
 
 # Here and below are some convenience functions.
 
 
 def fetch_test_filename(basename: str) -> str:
@@ -44,14 +45,15 @@
     basename : str
         The basename of the file, plus the extension to grab.
 
     Returns
     -------
     test_filename : str
         The test filename.
+
     """
     # We need to load the new configuration file.
     test_directory = os.path.dirname(
         os.path.realpath(os.path.join(os.path.realpath(__file__))),
     )
     test_file_directory = os.path.join(test_directory, "test_files", "")
     test_filename = test_file_directory + basename
```

### Comparing `lezargus-0.0.4.dev44/tests/test_library_config.py` & `lezargus-0.0.4.dev51/tests/test_library_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,54 +1,55 @@
 """This file contains tests test the Lezargus config handling code."""
 
 import os
 
-import lezargus
-
 import conftest
 
+import lezargus
+
 
 def test_read_configuration_file():
     """Test the read_configuration_file function.
 
     Parameters
     ----------
     None
 
     Returns
     -------
     None
+
     """
     # We first test a failure of the file extension. It should not actually
     # fail, but a message should pop up.
     bad_filename = "config_filename_without_correct_extension.txt"
     try:
         __ = lezargus.library.config.read_configuration_file(
-            filename=bad_filename
+            filename=bad_filename,
         )
     except lezargus.library.logging.ElevatedError:
         # We ignore the elevated file error.
         pass
 
     # We next test if we can detect files which do not exist.
     no_filename = "config_filename_does_not_exist.yaml"
     try:
         __ = lezargus.library.config.read_configuration_file(
-            filename=no_filename
+            filename=no_filename,
         )
     except lezargus.library.logging.FileError:
         # We ignore the elevated file error.
         pass
 
     # Finally we test a configuration file which does exist, but is not flat.
     nonflat_filename = "config_filename_not_flat_configuration.yaml"
     nonflat_filename = conftest.fetch_test_filename(basename=nonflat_filename)
     try:
         __ = lezargus.library.config.read_configuration_file(
-            filename=nonflat_filename
+            filename=nonflat_filename,
         )
     except lezargus.library.logging.ElevatedError:
         # We ignore the elevated file error.
         pass
 
 
 def test_load_configuration_file() -> None:
@@ -57,26 +58,27 @@
     Parameters
     ----------
     None
 
     Returns
     -------
     None
+
     """
     # We test to see that the casefold check works.
     # Not sure how to test this.
 
     # We test differing capitalization on a configuration file.
     lowercase_filename = "config_filename_with_lowercase_keys.yaml"
     lowercase_filename = conftest.fetch_test_filename(
-        basename=lowercase_filename
+        basename=lowercase_filename,
     )
     try:
         __ = lezargus.library.config.load_configuration_file(
-            filename=lowercase_filename
+            filename=lowercase_filename,
         )
     except lezargus.library.logging.ElevatedError:
         # We ignore the elevated file error.
         pass
 
 
 def test_create_configuration_file() -> None:
@@ -85,34 +87,38 @@
     Parameters
     ----------
     None
 
     Returns
     -------
     None
+
     """
     # We test the overwriting functionality. Borrowing a filename from other
     # tests.
     same_filename = "config_filename_with_lowercase_keys.yaml"
     same_filename = conftest.fetch_test_filename(basename=same_filename)
     try:
         __ = lezargus.library.config.create_configuration_file(
-            filename=same_filename, overwrite=False
+            filename=same_filename,
+            overwrite=False,
         )
     except lezargus.library.logging.ElevatedError:
         # We ignore the elevated error of the file already existing.
         pass
 
     # We create two files with both a correct extension and one without.
     noext_filename = "config_filename_without_ext"
     ext_filename = noext_filename + ".yaml"
     # Fixing the path.
     noext_filename = conftest.fetch_test_filename(basename=noext_filename)
     ext_filename = conftest.fetch_test_filename(basename=ext_filename)
     __ = lezargus.library.config.create_configuration_file(
-        filename=noext_filename, overwrite=True
+        filename=noext_filename,
+        overwrite=True,
     )
     __ = lezargus.library.config.create_configuration_file(
-        filename=ext_filename, overwrite=True
+        filename=ext_filename,
+        overwrite=True,
     )
     # We don't want both files to actually stay so we can delete them.
     os.remove(ext_filename)
```

### Comparing `lezargus-0.0.4.dev44/tests/test_library_logging.py` & `lezargus-0.0.4.dev51/tests/test_library_logging.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,69 +1,71 @@
 """This file contains tests that test the Lezargus logging and error code."""
 
 import lezargus
 
-import conftest
-
 
 def test_update_global_minimum_logging_level() -> None:
     """Test the update_global_minimum_logging_level function.
 
     Parameters
     ----------
     None
 
     Returns
     -------
     None
+
     """
     # We just run the logging again to test it.
     __ = lezargus.library.logging.update_global_minimum_logging_level(
-        log_level=lezargus.library.logging.LOGGING_DEBUG_LEVEL
+        log_level=lezargus.library.logging.LOGGING_DEBUG_LEVEL,
     )
 
 
 def test_debug() -> None:
     """Test the debug function.
 
     Parameters
     ----------
     None
 
     Returns
     -------
     None
+
     """
     lezargus.library.logging.debug(message="Debug test.")
 
 
 def test_info() -> None:
     """Test the info function.
 
     Parameters
     ----------
     None
 
     Returns
     -------
     None
+
     """
     lezargus.library.logging.info(message="Info test.")
 
 
 def test_warning() -> None:
     """Test the warning function.
 
     Parameters
     ----------
     None
 
     Returns
     -------
     None
+
     """
     # We try to send a warning with a non-Lezargus warning type.
     try:
         lezargus.library.logging.warning(
             warning_type=lezargus.library.logging.LezargusError,
             message="Using an error for a warning.",
         )
@@ -96,14 +98,15 @@
     Parameters
     ----------
     None
 
     Returns
     -------
     None
+
     """
     # We try to send a warning with a non-Lezargus error type.
     try:
         lezargus.library.logging.error(
             error_type=lezargus.library.logging.LezargusWarning,
             message="Using a warning for an error.",
         )
@@ -136,14 +139,15 @@
     Parameters
     ----------
     None
 
     Returns
     -------
     None
+
     """
     # We try to send a warning with a non-Lezargus error/critical type.
     try:
         lezargus.library.logging.critical(
             critical_type=lezargus.library.logging.LezargusWarning,
             message="Using a warning for an error.",
         )
@@ -168,13 +172,14 @@
     Parameters
     ----------
     None
 
     Returns
     -------
     None
+
     """
     try:
         lezargus.library.logging.terminal()
     except lezargus.library.logging.LezargusBaseError:
         # The error is expected.
         pass
```

### Comparing `lezargus-0.0.4.dev44/tests/test_library_path.py` & `lezargus-0.0.4.dev51/tests/test_library_path.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,25 +17,26 @@
     Parameters
     ----------
     None
 
     Returns
     -------
     None
+
     """
     if IS_OPERATING_SYSTEM_WINDOWS:
         # Example of a Windows OS pathname with spaces and other interesting
         # characters.
         example_windows_pathname = (
             R"A:\Kalos\Music\Pokémon\Official Tracks\Mystery Dungeon\PMD"
             R" Explorers\Dialga's Fight to the Finish!.flac"
         )
         # Getting the directory.
         directory = lezargus.library.path.get_directory(
-            pathname=example_windows_pathname
+            pathname=example_windows_pathname,
         )
         expected_dir = (
             R"A:\Kalos\Music\Pokémon\Official Tracks\Mystery Dungeon\PMD"
             R" Explorers"
         )
         # Asserting.
         assert_message = "Windows based pathname fail."
@@ -46,77 +47,81 @@
         example_linux_pathname = (
             R"/home/sparrow/Kirby/星のカービィ (Hoshi no Kaabii) (2001) -"
             R" Episode 1 - Kirby"
             R" - Right Back at Ya! Japanese [a9vrQ3Ns0gg].mkv"
         )
         # Getting the directory.
         directory = lezargus.library.path.get_directory(
-            pathname=example_linux_pathname
+            pathname=example_linux_pathname,
         )
         expected_dir = R"/home/sparrow/Kirby"
         # Asserting.
         assert_message = "Linux based pathnames fail."
         assert directory == expected_dir, assert_message
 
-    return None
-
 
 def test_get_most_recent_filename_in_directory() -> None:
     """Test the get_most_recent_filename_in_directory function.
 
     Parameters
     ----------
     None
 
     Returns
     -------
     None
+
     """
     # First we test if we provide an invalid directory.
     try:
         no_directory = "/this/is/a/directory/which/really/should/not/exist/"
         __ = lezargus.library.path.get_most_recent_filename_in_directory(
-            directory=no_directory
+            directory=no_directory,
         )
     except lezargus.library.logging.InputError:
         # The error is expected.
         pass
 
     # We just use the test directory itself, because why not. We also test
     # different extensions.
     recent_directory = conftest.fetch_test_filename(basename="")
     __ = lezargus.library.path.get_most_recent_filename_in_directory(
-        directory=recent_directory, extension=None, recursive=True
+        directory=recent_directory,
+        extension=None,
+        recursive=True,
     )
     __ = lezargus.library.path.get_most_recent_filename_in_directory(
-        directory=recent_directory, extension=["yaml", ".fits"], recursive=True
+        directory=recent_directory,
+        extension=["yaml", ".fits"],
+        recursive=True,
     )
 
 
 def test_get_filename_without_extension() -> None:
     """Test the ability to get the filename without extension from a pathname.
 
     Parameters
     ----------
     None
 
     Returns
     -------
     None
+
     """
     if IS_OPERATING_SYSTEM_WINDOWS:
         # Example of a Windows OS pathname with spaces and other interesting
         # characters.
         example_windows_pathname = (
             R"A:\Kalos\Music\Pokémon\Official Tracks\Mystery Dungeon\PMD"
             R" Explorers\Dialga's Fight to the Finish!.flac"
         )
         # Getting the directory.
         filename = lezargus.library.path.get_filename_without_extension(
-            pathname=example_windows_pathname
+            pathname=example_windows_pathname,
         )
         expected_filename = R"Dialga's Fight to the Finish!"
         # Asserting.
         assert_message = "Windows based pathnames fail."
         assert filename == expected_filename, assert_message
     else:
         # Example of a Linux OS pathname with spaces and other interesting
@@ -124,48 +129,48 @@
         example_linux_pathname = (
             R"/home/sparrow/Kirby/星のカービィ (Hoshi no Kaabii) (2001) -"
             R" Episode 1 - Kirby"
             R" - Right Back at Ya! Japanese [a9vrQ3Ns0gg].mkv"
         )
         # Getting the directory.
         filename = lezargus.library.path.get_filename_without_extension(
-            pathname=example_linux_pathname
+            pathname=example_linux_pathname,
         )
         expected_filename = (
             R"星のカービィ (Hoshi no Kaabii) (2001) - Episode 1 - Kirby - Right"
             R" Back at Ya!"
             R" Japanese [a9vrQ3Ns0gg]"
         )
         # Asserting.
         assert_message = "Linux based pathnames fail."
         assert filename == expected_filename, assert_message
-    return None
 
 
 def test_get_filename_with_extension() -> None:
     """Test the ability to get the filename with extension from a pathname.
 
     Parameters
     ----------
     None
 
     Returns
     -------
     None
+
     """
     if IS_OPERATING_SYSTEM_WINDOWS:
         # Example of a Windows OS pathname with spaces and other interesting
         # characters.
         example_windows_pathname = (
             R"A:\Kalos\Music\Pokémon\Official Tracks\Mystery Dungeon\PMD"
             R" Explorers\Dialga's Fight to the Finish!.flac"
         )
         # Getting the directory.
         filename = lezargus.library.path.get_filename_with_extension(
-            pathname=example_windows_pathname
+            pathname=example_windows_pathname,
         )
         expected_filename = R"Dialga's Fight to the Finish!.flac"
         # Asserting.
         assert_message = "Windows based pathnames fail."
         assert filename == expected_filename, assert_message
     else:
         # Example of a Linux OS pathname with spaces and other interesting
@@ -173,48 +178,48 @@
         example_linux_pathname = (
             R"/home/sparrow/Kirby/星のカービィ (Hoshi no Kaabii) (2001) -"
             R" Episode 1 - Kirby"
             R" - Right Back at Ya! Japanese [a9vrQ3Ns0gg].mkv"
         )
         # Getting the directory.
         filename = lezargus.library.path.get_filename_with_extension(
-            pathname=example_linux_pathname
+            pathname=example_linux_pathname,
         )
         expected_filename = (
             R"星のカービィ (Hoshi no Kaabii) (2001) - Episode 1 - Kirby - Right"
             R" Back at Ya!"
             R" Japanese [a9vrQ3Ns0gg].mkv"
         )
         # Asserting.
         assert_message = "Linux based pathnames fail."
         assert filename == expected_filename, assert_message
-    return None
 
 
 def test_get_file_extension() -> None:
     """Test the ability to get the file extension from a pathname.
 
     Parameters
     ----------
     None
 
     Returns
     -------
     None
+
     """
     if IS_OPERATING_SYSTEM_WINDOWS:
         # Example of a Windows OS pathname with spaces and other interesting
         # characters.
         example_windows_pathname = (
             R"A:\Kalos\Music\Pokémon\Official Tracks\Mystery Dungeon\PMD"
             R" Explorers\Dialga's Fight to the Finish!.flac"
         )
         # Getting the directory.
         extension = lezargus.library.path.get_file_extension(
-            pathname=example_windows_pathname
+            pathname=example_windows_pathname,
         )
         expected_extension = R"flac"
         # Asserting.
         assert_message = "Windows based pathnames fail."
         assert extension == expected_extension, assert_message
     else:
         # Example of a Linux OS pathname with spaces and other interesting
@@ -222,33 +227,33 @@
         example_linux_pathname = (
             R"/home/sparrow/Kirby/星のカービィ (Hoshi no Kaabii) (2001) -"
             R" Episode 1 - Kirby"
             R" - Right Back at Ya! Japanese [a9vrQ3Ns0gg].mkv"
         )
         # Getting the directory.
         extension = lezargus.library.path.get_file_extension(
-            pathname=example_linux_pathname
+            pathname=example_linux_pathname,
         )
         expected_extension = R"mkv"
         # Asserting.
         assert_message = "Linux based pathnames fail."
         assert extension == expected_extension, assert_message
-    return None
 
 
 def test_merge_pathname() -> None:
     """Test the ability to merge a pathname.
 
     Parameters
     ----------
     None
 
     Returns
     -------
     None
+
     """
     if IS_OPERATING_SYSTEM_WINDOWS:
         # For Windows based pathnames.
         windows_directory = R"A:\Kalos\Pictures\Space Battleship Yamato"
         windows_filename = R"Space Battle Ship USS Arizona"
         windows_extension = R"jpg"
         # Merging with an extension.
@@ -303,27 +308,26 @@
         )
         linux_expected_pathname = R"/home/sparrow/test/wiki/docker-compose"
         assert_message = (
             "Linux pathname merging with an extension did not work."
         )
         assert linux_pathname == linux_expected_pathname, assert_message
 
-    return None
-
 
 def test_split_pathname() -> None:
     """Test the ability to split a pathname.
 
     Parameters
     ----------
     None
 
     Returns
     -------
     None
+
     """
     if IS_OPERATING_SYSTEM_WINDOWS:
         # For Windows based pathnames.
         windows_pathname = (
             R"A:\Kalos\Pictures\Space Battleship Yamato\Space Battle Ship USS"
             R" Arizona.jpg"
         )
@@ -360,8 +364,7 @@
 
         assert_message = "Linux pathname splitting did not work."
         assert (
             linux_directory == expected_linux_directory
             and linux_filename == expected_linux_filename
             and linux_extension == expected_linux_extension
         ), assert_message
-    return None
```

### Comparing `lezargus-0.0.4.dev44/tests/test_library_wrapper.py` & `lezargus-0.0.4.dev51/tests/test_library_wrapper.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 """Tests wrapper functions to ensure that they are behaving normally."""
 
-import sys
-
 import numpy as np
 
 import lezargus
 
 
 def test_wavelength_overlap_fraction() -> None:
     """Test the wavelength_overlap_fraction function.
@@ -13,14 +11,15 @@
     Parameters
     ----------
     None
 
     Returns
     -------
     None
+
     """
     # We first check the obvious cases, where two different arrays overlap
     # or do not.
     main_array = np.linspace(5, 15, 50)
     overlap_array = np.linspace(7, 13, 30)
     super_overlap_array = np.linspace(4, 20, 60)
     lower_outside_array = np.linspace(1, 3, 15)
@@ -28,72 +27,77 @@
     # These arrays partially overlap.
     lower_partial_array = np.linspace(3, 8, 20)
     upper_partial_array = np.linspace(11, 23, 22)
 
     # Testing them...
     # An overlapping array overlaps with itself perfectly.
     self_fraction = lezargus.library.wrapper.wavelength_overlap_fraction(
-        base=main_array, contain=main_array
+        base=main_array,
+        contain=main_array,
     )
     assert_message = (
-        "Overlap fraction for itself is expected to be 1, not {fr}".format(
-            fr=self_fraction
-        )
+        f"Overlap fraction for itself is expected to be 1, not {self_fraction}"
     )
     assert self_fraction == 1, assert_message
     # Then the expected overlap one.
     overlap_fraction = lezargus.library.wrapper.wavelength_overlap_fraction(
-        base=main_array, contain=overlap_array
+        base=main_array,
+        contain=overlap_array,
     )
     assert_message = (
         "Overlap fraction for the overlapping array is expected to be 1,"
-        " not {fr}".format(fr=overlap_fraction)
+        f" not {overlap_fraction}"
     )
     # And one where the contain array is much bigger. We expect this to
     # throw a warning.
     try:
         __ = lezargus.library.wrapper.wavelength_overlap_fraction(
-            base=main_array, contain=super_overlap_array
+            base=main_array,
+            contain=super_overlap_array,
         )
     except lezargus.library.logging.ElevatedError:
         # This error is expected.
         pass
     else:
         assert_message = (
             "The super overlap fraction call should have thrown some sort of"
             " elevated warning, which then should have been caught."
         )
         assert False, assert_message
     # Now we test the two arrays which are not overlapping at all.
     lower_fraction = lezargus.library.wrapper.wavelength_overlap_fraction(
-        base=main_array, contain=lower_outside_array
+        base=main_array,
+        contain=lower_outside_array,
     )
     assert_message = (
         "Overlap fraction for the lower non-overlapping array is expected to be"
-        " 0, not {fr}".format(fr=lower_fraction)
+        f" 0, not {lower_fraction}"
     )
     assert lower_fraction == 0, assert_message
     upper_fraction = lezargus.library.wrapper.wavelength_overlap_fraction(
-        base=main_array, contain=upper_outside_array
+        base=main_array,
+        contain=upper_outside_array,
     )
     assert_message = (
         "Overlap fraction for the upper non-overlapping array is expected to be"
-        " 0, not {fr}".format(fr=upper_fraction)
+        f" 0, not {upper_fraction}"
     )
     assert upper_fraction == 0, assert_message
     # And then the partial overlaps.
     lower_part_fraction = lezargus.library.wrapper.wavelength_overlap_fraction(
-        base=main_array, contain=lower_partial_array
+        base=main_array,
+        contain=lower_partial_array,
     )
     assert_message = (
         "Overlap fraction for the lower partial overlapping array is expected"
-        " to be between 0 and 1, not {fr}".format(fr=lower_part_fraction)
+        f" to be between 0 and 1, not {lower_part_fraction}"
     )
     assert 0 < lower_part_fraction < 1, assert_message
     upper_part_fraction = lezargus.library.wrapper.wavelength_overlap_fraction(
-        base=main_array, contain=upper_partial_array
+        base=main_array,
+        contain=upper_partial_array,
     )
     assert_message = (
         "Overlap fraction for the upper partial overlapping array is expected"
-        " to be between 0 and 1, not {fr}".format(fr=upper_part_fraction)
+        f" to be between 0 and 1, not {upper_part_fraction}"
     )
     assert 0 < upper_part_fraction < 1, assert_message
```

### Comparing `lezargus-0.0.4.dev44/.gitignore` & `lezargus-0.0.4.dev51/.gitignore`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/LICENSE.txt` & `lezargus-0.0.4.dev51/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/README.md` & `lezargus-0.0.4.dev51/README.md`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.4.dev44/pyproject.toml` & `lezargus-0.0.4.dev51/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -53,18 +53,18 @@
     "./utility/*"
 ]
 
 [tool.hatch.envs.default]
 dependencies = [
     "pyinstaller",
     "coverage[toml]>=7.3.4",
-    "pytest>=7.4.0",
-    "black[jupyter]>=23.12.0",
-    "pylint[spelling]>=3.0.0",
-    "ruff>=0.1.13",
+    "pytest>=8.1.0",
+    "black[jupyter]>=24.4.0",
+    "pylint[spelling]>=3.1.0",
+    "ruff>=0.3.7",
     "sphinx>=7.2.6",
     "sphinx-book-theme>=1.1.0",
 ]
 [tool.hatch.envs.default.scripts]
 test = "pytest {args:tests}"
 format = [
     "black {args:.}",
@@ -179,20 +179,21 @@
 recursive = true
 good-names-rgxs = [
     # Allow for 2-character names, following the usual snake case conventions.
     "[_a-z][_a-z0-9]?$",
 ]
 disable = [
     "R0801", # (duplicate-code)
+    "R0401", # (cyclic-import)
     "R0902", # (too-many-instance-attributes)
     "R0903", # (too-few-public-methods)
     "R0913", # (too-many-arguments)
     "R0914", # (too-many-locals)
-    "R0401", # (cyclic-import)
     "C0302", # (too-many-lines)
+    "C0413", # (wrong-import-position) - Let Ruff and isort handle imports.
 ]
 extension-pkg-allow-list = [
     "PySide6",
 ]
 generated-members = [
     # Configuration and parameters are generated on-the-fly. We need to inform 
     # pylint that they are okay as it does not do introspection on the fly as
```

### Comparing `lezargus-0.0.4.dev44/PKG-INFO` & `lezargus-0.0.4.dev51/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: lezargus
-Version: 0.0.4.dev44
+Version: 0.0.4.dev51
 Summary: The accompanying data software package to the IRTF SPECTRE Spectrograph.
 Project-URL: Homepage, http://irtfweb.ifa.hawaii.edu/~spectre/
 Project-URL: Documentation, https://psmd-iberutaru.github.io/Lezargus/
 Project-URL: Issues, https://github.com/psmd-iberutaru/Lezargus/issues
 Project-URL: Source, https://github.com/psmd-iberutaru/Lezargus/
 Author-email: Sparrow <psmd.iberutaru@gmail.com>
 License-Expression: MIT
```

