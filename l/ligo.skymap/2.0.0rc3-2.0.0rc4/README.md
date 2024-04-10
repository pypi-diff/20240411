# Comparing `tmp/ligo.skymap-2.0.0rc3.tar.gz` & `tmp/ligo.skymap-2.0.0rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ligo.skymap-2.0.0rc3.tar", last modified: Mon Apr  1 02:39:51 2024, max compression
+gzip compressed data, was "ligo.skymap-2.0.0rc4.tar", last modified: Wed Apr 10 23:32:16 2024, max compression
```

## Comparing `ligo.skymap-2.0.0rc3.tar` & `ligo.skymap-2.0.0rc4.tar`

### file list

```diff
@@ -1,299 +1,300 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 02:39:51.901490 ligo.skymap-2.0.0rc3/
--rw-rw-rw-   0 root         (0) root         (0)      602 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/.gitignore
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 02:39:51.659490 ligo.skymap-2.0.0rc3/.gitlab/
--rwxrwxrwx   0 root         (0) root         (0)     2033 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/.gitlab/combine-coverage.py
--rw-rw-rw-   0 root         (0) root         (0)    12856 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)    43754 2024-04-01 02:39:28.000000 ligo.skymap-2.0.0rc3/CHANGES.rst
--rw-rw-rw-   0 root         (0) root         (0)      677 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/CONTRIBUTING.rst
--rw-rw-rw-   0 root         (0) root         (0)      286 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     5175 2024-04-01 02:39:51.900490 ligo.skymap-2.0.0rc3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2777 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 02:39:51.633490 ligo.skymap-2.0.0rc3/cextern/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 02:39:51.661490 ligo.skymap-2.0.0rc3/cextern/chealpix/
--rw-rw-rw-   0 root         (0) root         (0)    30207 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/cextern/chealpix/chealpix.c
--rw-rw-rw-   0 root         (0) root         (0)     7407 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/cextern/chealpix/chealpix.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 02:39:51.670490 ligo.skymap-2.0.0rc3/docs/
--rw-rw-rw-   0 root         (0) root         (0)     4581 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/docs/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 02:39:51.675490 ligo.skymap-2.0.0rc3/docs/_static/
--rw-rw-rw-   0 root         (0) root         (0)    34751 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/docs/_static/benchmark.svg
--rw-rw-rw-   0 root         (0) root         (0)   567737 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/docs/_static/coinc.xml
--rw-rw-rw-   0 root         (0) root         (0)   260305 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/docs/_static/localization.svg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 02:39:51.634490 ligo.skymap-2.0.0rc3/docs/_templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 02:39:51.679490 ligo.skymap-2.0.0rc3/docs/_templates/autosummary/
--rw-rw-rw-   0 root         (0) root         (0)      250 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/docs/_templates/autosummary/base.rst
--rw-rw-rw-   0 root         (0) root         (0)      251 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/docs/_templates/autosummary/class.rst
--rw-rw-rw-   0 root         (0) root         (0)      252 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/docs/_templates/autosummary/module.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 02:39:51.686490 ligo.skymap-2.0.0rc3/docs/bayestar/
--rw-rw-rw-   0 root         (0) root         (0)    56171 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/docs/bayestar/eggbox.png
--rw-rw-rw-   0 root         (0) root         (0)      212 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/docs/bayestar/ez_emcee.rst
--rw-rw-rw-   0 root         (0) root         (0)      182 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/docs/bayestar/filter.rst
--rw-rw-rw-   0 root         (0) root         (0)      309 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/docs/bayestar/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      225 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/docs/bayestar/interpolation.rst
--rw-rw-rw-   0 root         (0) root         (0)    43754 2024-04-01 02:39:28.000000 ligo.skymap-2.0.0rc3/docs/changes.rst
--rw-rw-rw-   0 root         (0) root         (0)     8757 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)      677 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/docs/contributing.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 02:39:51.688490 ligo.skymap-2.0.0rc3/docs/coordinates/
--rw-rw-rw-   0 root         (0) root         (0)      191 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/docs/coordinates/detector.rst
--rw-rw-rw-   0 root         (0) root         (0)      189 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/docs/coordinates/eigenframe.rst
--rw-rw-rw-   0 root         (0) root         (0)     2393 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/docs/develop.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 02:39:51.689490 ligo.skymap-2.0.0rc3/docs/distance/
--rw-rw-rw-   0 root         (0) root         (0)     1243 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/docs/distance/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 02:39:51.690490 ligo.skymap-2.0.0rc3/docs/healpix_tree/
--rw-rw-rw-   0 root         (0) root         (0)      165 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/docs/healpix_tree/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      595 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/docs/help.rst
--rw-rw-rw-   0 root         (0) root         (0)     4574 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)    15650 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/docs/interface.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 02:39:51.692490 ligo.skymap-2.0.0rc3/docs/io/
--rw-rw-rw-   0 root         (0) root         (0)     3691 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/docs/io/events.rst
--rw-rw-rw-   0 root         (0) root         (0)      146 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/docs/io/fits.rst
--rw-rw-rw-   0 root         (0) root         (0)      166 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/docs/io/hdf5.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 02:39:51.693490 ligo.skymap-2.0.0rc3/docs/kde/
--rw-rw-rw-   0 root         (0) root         (0)      162 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/docs/kde/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     4549 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/docs/make.bat
--rw-rw-rw-   0 root         (0) root         (0)       13 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/docs/matplotlibrc
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 02:39:51.694490 ligo.skymap-2.0.0rc3/docs/moc/
--rw-rw-rw-   0 root         (0) root         (0)      308 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/docs/moc/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     1282 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/docs/performance.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 02:39:51.700490 ligo.skymap-2.0.0rc3/docs/plot/
--rw-rw-rw-   0 root         (0) root         (0)      186 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/docs/plot/allsky.rst
--rw-rw-rw-   0 root         (0) root         (0)      198 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/docs/plot/backdrop.rst
--rw-rw-rw-   0 root         (0) root         (0)      206 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/docs/plot/bayes_factor.rst
--rw-rw-rw-   0 root         (0) root         (0)      205 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/docs/plot/marker.rst
--rw-rw-rw-   0 root         (0) root         (0)      166 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/docs/plot/poly.rst
--rw-rw-rw-   0 root         (0) root         (0)      182 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/docs/plot/pp.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 02:39:51.705490 ligo.skymap-2.0.0rc3/docs/postprocess/
--rw-rw-rw-   0 root         (0) root         (0)      180 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/docs/postprocess/contour.rst
--rw-rw-rw-   0 root         (0) root         (0)      184 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/docs/postprocess/cosmology.rst
--rw-rw-rw-   0 root         (0) root         (0)      253 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/docs/postprocess/crossmatch.rst
--rw-rw-rw-   0 root         (0) root         (0)      200 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/docs/postprocess/ellipse.rst
--rw-rw-rw-   0 root         (0) root         (0)      195 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/docs/postprocess/util.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 02:39:51.707490 ligo.skymap-2.0.0rc3/docs/quickstart/
--rw-rw-rw-   0 root         (0) root         (0)     6351 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/docs/quickstart/bayestar-injections.rst
--rw-rw-rw-   0 root         (0) root         (0)     4449 2024-04-01 02:37:03.000000 ligo.skymap-2.0.0rc3/docs/quickstart/install.rst
--rw-rw-rw-   0 root         (0) root         (0)     6031 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/docs/testing.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 02:39:51.729490 ligo.skymap-2.0.0rc3/docs/tool/
--rw-rw-rw-   0 root         (0) root         (0)      314 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/docs/tool/bayestar_inject.rst
--rw-rw-rw-   0 root         (0) root         (0)      188 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/docs/tool/bayestar_localize_coincs.rst
--rw-rw-rw-   0 root         (0) root         (0)      204 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/docs/tool/bayestar_localize_lvalert.rst
--rw-rw-rw-   0 root         (0) root         (0)      189 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/docs/tool/bayestar_mcmc.rst
--rw-rw-rw-   0 root         (0) root         (0)      179 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/docs/tool/bayestar_realize_coincs.rst
--rw-rw-rw-   0 root         (0) root         (0)      175 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/docs/tool/bayestar_sample_model_psd.rst
--rw-rw-rw-   0 root         (0) root         (0)      175 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/docs/tool/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     1400 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/docs/tool/ligo_skymap_combine.rst
--rw-rw-rw-   0 root         (0) root         (0)     3709 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/docs/tool/ligo_skymap_constellations.rst
--rw-rw-rw-   0 root         (0) root         (0)      165 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/docs/tool/ligo_skymap_contour.rst
--rw-rw-rw-   0 root         (0) root         (0)      215 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/docs/tool/ligo_skymap_contour_moc.rst
--rw-rw-rw-   0 root         (0) root         (0)      199 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/docs/tool/ligo_skymap_flatten.rst
--rw-rw-rw-   0 root         (0) root         (0)     1387 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/docs/tool/ligo_skymap_from_samples.rst
--rw-rw-rw-   0 root         (0) root         (0)      747 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/docs/tool/ligo_skymap_plot.rst
--rw-rw-rw-   0 root         (0) root         (0)      795 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/docs/tool/ligo_skymap_plot_airmass.rst
--rw-rw-rw-   0 root         (0) root         (0)      779 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/docs/tool/ligo_skymap_plot_coherence.rst
--rw-rw-rw-   0 root         (0) root         (0)     1121 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/docs/tool/ligo_skymap_plot_observability.rst
--rw-rw-rw-   0 root         (0) root         (0)      188 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/docs/tool/ligo_skymap_plot_stats.rst
--rw-rw-rw-   0 root         (0) root         (0)      700 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/docs/tool/ligo_skymap_plot_volume.rst
--rw-rw-rw-   0 root         (0) root         (0)      177 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/docs/tool/ligo_skymap_stats.rst
--rw-rw-rw-   0 root         (0) root         (0)      209 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/docs/tool/ligo_skymap_unflatten.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 02:39:51.734490 ligo.skymap-2.0.0rc3/docs/util/
--rw-rw-rw-   0 root         (0) root         (0)      158 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/docs/util/file.rst
--rw-rw-rw-   0 root         (0) root         (0)      172 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/docs/util/ilwd.rst
--rw-rw-rw-   0 root         (0) root         (0)      163 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/docs/util/numpy.rst
--rw-rw-rw-   0 root         (0) root         (0)      168 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/docs/util/sqlite.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 02:39:51.739490 ligo.skymap-2.0.0rc3/licenses/
--rw-rw-rw-   0 root         (0) root         (0)     6360 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/licenses/CHEALPIX_LICENSE.rst
--rw-rw-rw-   0 root         (0) root         (0)    37565 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/licenses/LICENSE.rst
--rw-rw-rw-   0 root         (0) root         (0)     1792 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/licenses/NUMPY_LICENSE.rst
--rw-rw-rw-   0 root         (0) root         (0)      372 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/licenses/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     1659 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/licenses/TEMPLATE_LICENCE.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 02:39:51.640490 ligo.skymap-2.0.0rc3/ligo/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 02:39:51.751490 ligo.skymap-2.0.0rc3/ligo/skymap/
--rw-rw-rw-   0 root         (0) root         (0)     1012 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      698 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/_astropy_init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 02:39:51.755490 ligo.skymap-2.0.0rc3/ligo/skymap/bayestar/
--rw-rw-rw-   0 root         (0) root         (0)    20417 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/bayestar/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5864 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/bayestar/ez_emcee.py
--rw-rw-rw-   0 root         (0) root         (0)    19685 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/bayestar/filter.py
--rw-rw-rw-   0 root         (0) root         (0)    10348 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/bayestar/interpolation.py
--rw-rw-rw-   0 root         (0) root         (0)     2176 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/bayestar/ptemcee.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 02:39:51.757490 ligo.skymap-2.0.0rc3/ligo/skymap/bayestar/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-01 02:39:28.000000 ligo.skymap-2.0.0rc3/ligo/skymap/bayestar/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1545 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/bayestar/tests/test_bayestar.py
--rw-rw-rw-   0 root         (0) root         (0)     4573 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/bayestar/tests/test_interpolation.py
--rw-rw-rw-   0 root         (0) root         (0)     4287 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/bayestar/tests/test_signal_amplitude_model.py
--rw-rw-rw-   0 root         (0) root         (0)     2321 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 02:39:51.760490 ligo.skymap-2.0.0rc3/ligo/skymap/coordinates/
--rw-rw-rw-   0 root         (0) root         (0)      382 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/coordinates/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3645 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/coordinates/detector.py
--rw-rw-rw-   0 root         (0) root         (0)     4132 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/coordinates/eigenframe.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 02:39:51.762490 ligo.skymap-2.0.0rc3/ligo/skymap/coordinates/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-01 02:39:28.000000 ligo.skymap-2.0.0rc3/ligo/skymap/coordinates/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      996 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/coordinates/tests/test_detector.py
--rw-rw-rw-   0 root         (0) root         (0)    20879 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/distance.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 02:39:51.763490 ligo.skymap-2.0.0rc3/ligo/skymap/extern/
--rw-rw-rw-   0 root         (0) root         (0)      460 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/extern/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 02:39:51.765490 ligo.skymap-2.0.0rc3/ligo/skymap/extern/numpy/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-01 02:39:28.000000 ligo.skymap-2.0.0rc3/ligo/skymap/extern/numpy/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13938 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/extern/numpy/quantile.py
--rw-rw-rw-   0 root         (0) root         (0)    15264 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/healpix_tree.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 02:39:51.767490 ligo.skymap-2.0.0rc3/ligo/skymap/io/
--rw-rw-rw-   0 root         (0) root         (0)      382 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/io/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 02:39:51.775490 ligo.skymap-2.0.0rc3/ligo/skymap/io/events/
--rw-rw-rw-   0 root         (0) root         (0)      382 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/io/events/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3832 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/io/events/base.py
--rw-rw-rw-   0 root         (0) root         (0)     2664 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/io/events/detector_disabled.py
--rw-rw-rw-   0 root         (0) root         (0)     2274 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/io/events/gracedb.py
--rw-rw-rw-   0 root         (0) root         (0)     7809 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/io/events/hdf.py
--rw-rw-rw-   0 root         (0) root         (0)    11334 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/io/events/ligolw.py
--rw-rw-rw-   0 root         (0) root         (0)     2563 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/io/events/magic.py
--rw-rw-rw-   0 root         (0) root         (0)     1700 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/io/events/sqlite.py
--rwxrwxrwx   0 root         (0) root         (0)    19227 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/io/fits.py
--rwxrwxrwx   0 root         (0) root         (0)    10626 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/io/hdf5.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 02:39:51.776490 ligo.skymap-2.0.0rc3/ligo/skymap/io/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-01 02:39:28.000000 ligo.skymap-2.0.0rc3/ligo/skymap/io/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 02:39:51.785490 ligo.skymap-2.0.0rc3/ligo/skymap/io/tests/data/
--rw-rw-rw-   0 root         (0) root         (0)   492938 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/io/tests/data/2016_subset.xml.gz
--rw-rw-rw-   0 root         (0) root         (0)     1699 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/io/tests/data/G197392_coinc.xml.gz
--rw-rw-rw-   0 root         (0) root         (0)      675 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/io/tests/data/G197392_psd.xml.gz
--rw-rw-rw-   0 root         (0) root         (0)     2470 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/io/tests/data/G211117_coinc.xml.gz
--rw-rw-rw-   0 root         (0) root         (0)     2355 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/io/tests/data/G211117_psd.xml.gz
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-01 02:39:28.000000 ligo.skymap-2.0.0rc3/ligo/skymap/io/tests/data/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 02:39:51.787490 ligo.skymap-2.0.0rc3/ligo/skymap/io/tests/data/gstlal_reference_psd/
--rw-rw-rw-   0 root         (0) root         (0)      717 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/io/tests/data/gstlal_reference_psd/H1L1V1-REFERENCE_PSD-967234210-29963.xml.gz
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-01 02:39:28.000000 ligo.skymap-2.0.0rc3/ligo/skymap/io/tests/data/gstlal_reference_psd/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9120 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/io/tests/data/test.hdf5
--rw-rw-rw-   0 root         (0) root         (0)    12814 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/io/tests/test_io_events.py
--rw-rw-rw-   0 root         (0) root         (0)    17043 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/kde.py
--rw-rw-rw-   0 root         (0) root         (0)     7640 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/moc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 02:39:51.799490 ligo.skymap-2.0.0rc3/ligo/skymap/plot/
--rw-rw-rw-   0 root         (0) root         (0)      382 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/plot/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    29444 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/plot/allsky.py
--rw-rw-rw-   0 root         (0) root         (0)     1415 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/plot/angle.py
--rw-rw-rw-   0 root         (0) root         (0)     7312 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/plot/backdrop.py
--rw-rw-rw-   0 root         (0) root         (0)     3915 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/plot/bayes_factor.py
--rw-rw-rw-   0 root         (0) root         (0)     1530 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/plot/cmap.py
--rw-rw-rw-   0 root         (0) root         (0)     8714 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/plot/cylon.csv
--rw-rw-rw-   0 root         (0) root         (0)     2125 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/plot/cylon.py
--rw-rw-rw-   0 root         (0) root         (0)     2933 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/plot/marker.py
--rw-rw-rw-   0 root         (0) root         (0)    63275 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/plot/ne_simplified_coastline.json
--rw-rw-rw-   0 root         (0) root         (0)     7394 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/plot/poly.py
--rw-rw-rw-   0 root         (0) root         (0)     9445 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/plot/pp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 02:39:51.801490 ligo.skymap-2.0.0rc3/ligo/skymap/plot/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-01 02:39:28.000000 ligo.skymap-2.0.0rc3/ligo/skymap/plot/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 02:39:51.826490 ligo.skymap-2.0.0rc3/ligo/skymap/plot/tests/baseline/
--rw-rw-rw-   0 root         (0) root         (0)    67690 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/plot/tests/baseline/test_allsky_axes_astro-degrees-aitoff.png
--rw-rw-rw-   0 root         (0) root         (0)    65830 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/plot/tests/baseline/test_allsky_axes_astro-degrees-mollweide.png
--rw-rw-rw-   0 root         (0) root         (0)    65829 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/plot/tests/baseline/test_allsky_axes_astro-hours-aitoff.png
--rw-rw-rw-   0 root         (0) root         (0)    63879 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/plot/tests/baseline/test_allsky_axes_astro-hours-mollweide.png
--rw-rw-rw-   0 root         (0) root         (0)    71762 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/plot/tests/baseline/test_allsky_axes_galactic-degrees-aitoff.png
--rw-rw-rw-   0 root         (0) root         (0)    71509 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/plot/tests/baseline/test_allsky_axes_galactic-degrees-mollweide.png
--rw-rw-rw-   0 root         (0) root         (0)    70497 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/plot/tests/baseline/test_allsky_axes_galactic-hours-aitoff.png
--rw-rw-rw-   0 root         (0) root         (0)    69334 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/plot/tests/baseline/test_allsky_axes_galactic-hours-mollweide.png
--rw-rw-rw-   0 root         (0) root         (0)    64896 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/plot/tests/baseline/test_allsky_axes_geo-degrees-aitoff.png
--rw-rw-rw-   0 root         (0) root         (0)    63732 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/plot/tests/baseline/test_allsky_axes_geo-degrees-mollweide.png
--rw-rw-rw-   0 root         (0) root         (0)    63470 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/plot/tests/baseline/test_allsky_axes_geo-hours-aitoff.png
--rw-rw-rw-   0 root         (0) root         (0)    61561 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/plot/tests/baseline/test_allsky_axes_geo-hours-mollweide.png
--rw-rw-rw-   0 root         (0) root         (0)    33964 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/plot/tests/baseline/test_allsky_obstime.png
--rw-rw-rw-   0 root         (0) root         (0)    26192 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/plot/tests/baseline/test_center_projections_197.45d -23.38d-aitoff.png
--rw-rw-rw-   0 root         (0) root         (0)    25840 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/plot/tests/baseline/test_center_projections_197.45d -23.38d-mollweide.png
--rw-rw-rw-   0 root         (0) root         (0)    24254 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/plot/tests/baseline/test_center_projections_None-aitoff.png
--rw-rw-rw-   0 root         (0) root         (0)    22142 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/plot/tests/baseline/test_center_projections_None-mollweide.png
--rw-rw-rw-   0 root         (0) root         (0)    20330 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/plot/tests/baseline/test_globe_axes.png
--rw-rw-rw-   0 root         (0) root         (0)    19092 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/plot/tests/baseline/test_pp_plot_default.png
--rw-rw-rw-   0 root         (0) root         (0)    39991 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/plot/tests/baseline/test_pp_plot_lines.png
--rw-rw-rw-   0 root         (0) root         (0)    19092 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/plot/tests/baseline/test_pp_plot_steps.png
--rw-rw-rw-   0 root         (0) root         (0)     8866 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/plot/tests/baseline/test_reticle.png
--rw-rw-rw-   0 root         (0) root         (0)    19815 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/plot/tests/baseline/test_zoom_axes.png
--rw-rw-rw-   0 root         (0) root         (0)     6027 2024-04-01 02:37:03.000000 ligo.skymap-2.0.0rc3/ligo/skymap/plot/tests/test_plot.py
--rw-rw-rw-   0 root         (0) root         (0)     2400 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/plot/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 02:39:51.833490 ligo.skymap-2.0.0rc3/ligo/skymap/postprocess/
--rw-rw-rw-   0 root         (0) root         (0)      382 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/postprocess/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6348 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/postprocess/contour.py
--rw-rw-rw-   0 root         (0) root         (0)     2903 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/postprocess/cosmology.py
--rw-rw-rw-   0 root         (0) root         (0)    18512 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/postprocess/crossmatch.py
--rw-rw-rw-   0 root         (0) root         (0)    15257 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/postprocess/ellipse.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 02:39:51.835490 ligo.skymap-2.0.0rc3/ligo/skymap/postprocess/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-01 02:39:28.000000 ligo.skymap-2.0.0rc3/ligo/skymap/postprocess/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1210 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/postprocess/tests/test_cosmology.py
--rw-rw-rw-   0 root         (0) root         (0)     4373 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/postprocess/tests/test_crossmatch.py
--rw-rw-rw-   0 root         (0) root         (0)     3219 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/postprocess/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 02:39:51.837490 ligo.skymap-2.0.0rc3/ligo/skymap/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-01 02:39:28.000000 ligo.skymap-2.0.0rc3/ligo/skymap/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 02:39:51.838490 ligo.skymap-2.0.0rc3/ligo/skymap/tests/plugins/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-01 02:39:28.000000 ligo.skymap-2.0.0rc3/ligo/skymap/tests/plugins/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      578 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/tests/plugins/omp.py
--rw-rw-rw-   0 root         (0) root         (0)     4831 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/tests/test_moc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 02:39:51.861490 ligo.skymap-2.0.0rc3/ligo/skymap/tool/
--rw-rw-rw-   0 root         (0) root         (0)    15388 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/tool/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    21608 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/tool/bayestar_inject.py
--rw-rw-rw-   0 root         (0) root         (0)     7399 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/tool/bayestar_localize_coincs.py
--rwxrwxrwx   0 root         (0) root         (0)     6682 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/tool/bayestar_localize_lvalert.py
--rw-rw-rw-   0 root         (0) root         (0)     8137 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/tool/bayestar_mcmc.py
--rw-rw-rw-   0 root         (0) root         (0)    18761 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/tool/bayestar_realize_coincs.py
--rw-rw-rw-   0 root         (0) root         (0)     4600 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/tool/bayestar_sample_model_psd.py
--rw-rw-rw-   0 root         (0) root         (0)     5841 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/tool/ligo_skymap_combine.py
--rw-rw-rw-   0 root         (0) root         (0)     2011 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/tool/ligo_skymap_constellations.py
--rw-rw-rw-   0 root         (0) root         (0)     3341 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/tool/ligo_skymap_contour.py
--rw-rw-rw-   0 root         (0) root         (0)     2519 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/tool/ligo_skymap_contour_moc.py
--rw-rw-rw-   0 root         (0) root         (0)     2288 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/tool/ligo_skymap_flatten.py
--rw-rw-rw-   0 root         (0) root         (0)     7662 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/tool/ligo_skymap_from_samples.py
--rw-rw-rw-   0 root         (0) root         (0)     6732 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/tool/ligo_skymap_plot.py
--rw-rw-rw-   0 root         (0) root         (0)     8353 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/tool/ligo_skymap_plot_airmass.py
--rw-rw-rw-   0 root         (0) root         (0)     1713 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/tool/ligo_skymap_plot_coherence.py
--rw-rw-rw-   0 root         (0) root         (0)     5711 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/tool/ligo_skymap_plot_observability.py
--rw-rw-rw-   0 root         (0) root         (0)     5158 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/tool/ligo_skymap_plot_pp_samples.py
--rw-rw-rw-   0 root         (0) root         (0)     8048 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/tool/ligo_skymap_plot_stats.py
--rwxrwxrwx   0 root         (0) root         (0)     9391 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/tool/ligo_skymap_plot_volume.py
--rw-rw-rw-   0 root         (0) root         (0)    11830 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/tool/ligo_skymap_stats.py
--rw-rw-rw-   0 root         (0) root         (0)     1739 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/tool/ligo_skymap_unflatten.py
--rw-rw-rw-   0 root         (0) root         (0)     4508 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/tool/matplotlib.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 02:39:51.870490 ligo.skymap-2.0.0rc3/ligo/skymap/tool/tests/
--rw-rw-rw-   0 root         (0) root         (0)     3088 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/tool/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5271 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/tool/tests/test_bayestar.py
--rw-rw-rw-   0 root         (0) root         (0)     4496 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/tool/tests/test_bayestar_inject.py
--rw-rw-rw-   0 root         (0) root         (0)     2400 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/tool/tests/test_combine.py
--rw-rw-rw-   0 root         (0) root         (0)     4015 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/tool/tests/test_flatten.py
--rw-rw-rw-   0 root         (0) root         (0)     2631 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/tool/tests/test_from_samples.py
--rw-rw-rw-   0 root         (0) root         (0)      529 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/tool/tests/test_help.py
--rw-rw-rw-   0 root         (0) root         (0)     1826 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/tool/tests/test_plot.py
--rw-rw-rw-   0 root         (0) root         (0)     2065 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/tool/tests/test_plot_stats.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 02:39:51.876490 ligo.skymap-2.0.0rc3/ligo/skymap/util/
--rw-rw-rw-   0 root         (0) root         (0)      382 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/util/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1794 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/util/file.py
--rw-rw-rw-   0 root         (0) root         (0)     5170 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/util/ilwd.py
--rw-rw-rw-   0 root         (0) root         (0)      813 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/util/math.py
--rw-rw-rw-   0 root         (0) root         (0)     1680 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/util/numpy.py
--rw-rw-rw-   0 root         (0) root         (0)     2854 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/util/progress.py
--rw-rw-rw-   0 root         (0) root         (0)     4451 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/util/sqlite.py
--rw-rw-rw-   0 root         (0) root         (0)     2694 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/util/stopwatch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 02:39:51.877490 ligo.skymap-2.0.0rc3/ligo/skymap/util/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-01 02:39:28.000000 ligo.skymap-2.0.0rc3/ligo/skymap/util/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      363 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/ligo/skymap/util/tests/test_progress.py
--rw-r--r--   0 root         (0) root         (0)      340 2024-04-01 02:39:51.000000 ligo.skymap-2.0.0rc3/ligo/skymap/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 02:39:51.890490 ligo.skymap-2.0.0rc3/ligo.skymap.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5175 2024-04-01 02:39:51.000000 ligo.skymap-2.0.0rc3/ligo.skymap.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8652 2024-04-01 02:39:51.000000 ligo.skymap-2.0.0rc3/ligo.skymap.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-01 02:39:51.000000 ligo.skymap-2.0.0rc3/ligo.skymap.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1550 2024-04-01 02:39:51.000000 ligo.skymap-2.0.0rc3/ligo.skymap.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-01 02:39:51.000000 ligo.skymap-2.0.0rc3/ligo.skymap.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      423 2024-04-01 02:39:51.000000 ligo.skymap-2.0.0rc3/ligo.skymap.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2024-04-01 02:39:51.000000 ligo.skymap-2.0.0rc3/ligo.skymap.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      205 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     6369 2024-04-01 02:39:51.907490 ligo.skymap-2.0.0rc3/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     3807 2024-03-30 15:09:47.000000 ligo.skymap-2.0.0rc3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 02:39:51.888490 ligo.skymap-2.0.0rc3/src/
--rw-rw-rw-   0 root         (0) root         (0)    37062 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/src/bayestar_cosmology.h
--rw-rw-rw-   0 root         (0) root         (0)     4094 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/src/bayestar_cosmology.py
--rw-rw-rw-   0 root         (0) root         (0)    15859 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/src/bayestar_distance.c
--rw-rw-rw-   0 root         (0) root         (0)     2067 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/src/bayestar_distance.h
--rw-rw-rw-   0 root         (0) root         (0)     4286 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/src/bayestar_moc.c
--rw-rw-rw-   0 root         (0) root         (0)     1492 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/src/bayestar_moc.h
--rw-rw-rw-   0 root         (0) root         (0)    50371 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/src/bayestar_sky_map.c
--rw-rw-rw-   0 root         (0) root         (0)     7831 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/src/bayestar_sky_map.h
--rw-rw-rw-   0 root         (0) root         (0)      218 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/src/branch_prediction.h
--rw-rw-rw-   0 root         (0) root         (0)    38468 2024-03-30 15:09:47.000000 ligo.skymap-2.0.0rc3/src/core.c
--rw-rw-rw-   0 root         (0) root         (0)     5818 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/src/cubic_interp.c
--rw-rw-rw-   0 root         (0) root         (0)     2069 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/src/cubic_interp.h
--rw-rw-rw-   0 root         (0) root         (0)    13016 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/src/cubic_interp_test.c
--rw-rw-rw-   0 root         (0) root         (0)     6370 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/src/omp_interruptible.h
--rw-rw-rw-   0 root         (0) root         (0)     2377 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/src/vmath.h
--rw-rw-rw-   0 root         (0) root         (0)     1869 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/src/warnings.h
--rw-rw-rw-   0 root         (0) root         (0)     2595 2024-03-27 20:07:22.000000 ligo.skymap-2.0.0rc3/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 23:32:16.843763 ligo.skymap-2.0.0rc4/
+-rw-rw-rw-   0 root         (0) root         (0)      602 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/.gitignore
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 23:32:16.714759 ligo.skymap-2.0.0rc4/.gitlab/
+-rwxrwxrwx   0 root         (0) root         (0)     2033 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/.gitlab/combine-coverage.py
+-rw-rw-rw-   0 root         (0) root         (0)    13730 2024-04-10 23:32:03.000000 ligo.skymap-2.0.0rc4/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)    43840 2024-04-10 23:32:03.000000 ligo.skymap-2.0.0rc4/CHANGES.rst
+-rw-rw-rw-   0 root         (0) root         (0)      677 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/CONTRIBUTING.rst
+-rw-rw-rw-   0 root         (0) root         (0)      286 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     5226 2024-04-10 23:32:16.843763 ligo.skymap-2.0.0rc4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2777 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 23:32:16.706759 ligo.skymap-2.0.0rc4/cextern/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 23:32:16.715759 ligo.skymap-2.0.0rc4/cextern/chealpix/
+-rw-rw-rw-   0 root         (0) root         (0)    30207 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/cextern/chealpix/chealpix.c
+-rw-rw-rw-   0 root         (0) root         (0)     7407 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/cextern/chealpix/chealpix.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 23:32:16.720759 ligo.skymap-2.0.0rc4/docs/
+-rw-rw-rw-   0 root         (0) root         (0)     4581 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/docs/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 23:32:16.725760 ligo.skymap-2.0.0rc4/docs/_static/
+-rw-rw-rw-   0 root         (0) root         (0)    34751 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/docs/_static/benchmark.svg
+-rw-rw-rw-   0 root         (0) root         (0)   567737 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/docs/_static/coinc.xml
+-rw-rw-rw-   0 root         (0) root         (0)   260305 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/docs/_static/localization.svg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 23:32:16.706759 ligo.skymap-2.0.0rc4/docs/_templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 23:32:16.729760 ligo.skymap-2.0.0rc4/docs/_templates/autosummary/
+-rw-rw-rw-   0 root         (0) root         (0)      250 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/docs/_templates/autosummary/base.rst
+-rw-rw-rw-   0 root         (0) root         (0)      251 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/docs/_templates/autosummary/class.rst
+-rw-rw-rw-   0 root         (0) root         (0)      252 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/docs/_templates/autosummary/module.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 23:32:16.732760 ligo.skymap-2.0.0rc4/docs/bayestar/
+-rw-rw-rw-   0 root         (0) root         (0)    56171 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/docs/bayestar/eggbox.png
+-rw-rw-rw-   0 root         (0) root         (0)      212 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/docs/bayestar/ez_emcee.rst
+-rw-rw-rw-   0 root         (0) root         (0)      182 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/docs/bayestar/filter.rst
+-rw-rw-rw-   0 root         (0) root         (0)      309 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/docs/bayestar/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      225 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/docs/bayestar/interpolation.rst
+-rw-rw-rw-   0 root         (0) root         (0)    43840 2024-04-10 23:32:03.000000 ligo.skymap-2.0.0rc4/docs/changes.rst
+-rw-rw-rw-   0 root         (0) root         (0)     8757 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      677 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/docs/contributing.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 23:32:16.732760 ligo.skymap-2.0.0rc4/docs/coordinates/
+-rw-rw-rw-   0 root         (0) root         (0)      191 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/docs/coordinates/detector.rst
+-rw-rw-rw-   0 root         (0) root         (0)      189 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/docs/coordinates/eigenframe.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2393 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/docs/develop.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 23:32:16.733760 ligo.skymap-2.0.0rc4/docs/distance/
+-rw-rw-rw-   0 root         (0) root         (0)     1243 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/docs/distance/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 23:32:16.733760 ligo.skymap-2.0.0rc4/docs/healpix_tree/
+-rw-rw-rw-   0 root         (0) root         (0)      165 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/docs/healpix_tree/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      595 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/docs/help.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4574 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)    15650 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/docs/interface.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 23:32:16.734760 ligo.skymap-2.0.0rc4/docs/io/
+-rw-rw-rw-   0 root         (0) root         (0)     3691 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/docs/io/events.rst
+-rw-rw-rw-   0 root         (0) root         (0)      146 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/docs/io/fits.rst
+-rw-rw-rw-   0 root         (0) root         (0)      166 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/docs/io/hdf5.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 23:32:16.735760 ligo.skymap-2.0.0rc4/docs/kde/
+-rw-rw-rw-   0 root         (0) root         (0)      162 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/docs/kde/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4549 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/docs/make.bat
+-rw-rw-rw-   0 root         (0) root         (0)       13 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/docs/matplotlibrc
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 23:32:16.735760 ligo.skymap-2.0.0rc4/docs/moc/
+-rw-rw-rw-   0 root         (0) root         (0)      308 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/docs/moc/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1282 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/docs/performance.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 23:32:16.737760 ligo.skymap-2.0.0rc4/docs/plot/
+-rw-rw-rw-   0 root         (0) root         (0)      186 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/docs/plot/allsky.rst
+-rw-rw-rw-   0 root         (0) root         (0)      198 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/docs/plot/backdrop.rst
+-rw-rw-rw-   0 root         (0) root         (0)      206 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/docs/plot/bayes_factor.rst
+-rw-rw-rw-   0 root         (0) root         (0)      205 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/docs/plot/marker.rst
+-rw-rw-rw-   0 root         (0) root         (0)      166 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/docs/plot/poly.rst
+-rw-rw-rw-   0 root         (0) root         (0)      182 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/docs/plot/pp.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 23:32:16.739760 ligo.skymap-2.0.0rc4/docs/postprocess/
+-rw-rw-rw-   0 root         (0) root         (0)      180 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/docs/postprocess/contour.rst
+-rw-rw-rw-   0 root         (0) root         (0)      184 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/docs/postprocess/cosmology.rst
+-rw-rw-rw-   0 root         (0) root         (0)      253 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/docs/postprocess/crossmatch.rst
+-rw-rw-rw-   0 root         (0) root         (0)      200 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/docs/postprocess/ellipse.rst
+-rw-rw-rw-   0 root         (0) root         (0)      195 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/docs/postprocess/util.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 23:32:16.740760 ligo.skymap-2.0.0rc4/docs/quickstart/
+-rw-rw-rw-   0 root         (0) root         (0)     6351 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/docs/quickstart/bayestar-injections.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4449 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/docs/quickstart/install.rst
+-rw-rw-rw-   0 root         (0) root         (0)     6031 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/docs/testing.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 23:32:16.748761 ligo.skymap-2.0.0rc4/docs/tool/
+-rw-rw-rw-   0 root         (0) root         (0)      314 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/docs/tool/bayestar_inject.rst
+-rw-rw-rw-   0 root         (0) root         (0)      188 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/docs/tool/bayestar_localize_coincs.rst
+-rw-rw-rw-   0 root         (0) root         (0)      204 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/docs/tool/bayestar_localize_lvalert.rst
+-rw-rw-rw-   0 root         (0) root         (0)      189 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/docs/tool/bayestar_mcmc.rst
+-rw-rw-rw-   0 root         (0) root         (0)      179 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/docs/tool/bayestar_realize_coincs.rst
+-rw-rw-rw-   0 root         (0) root         (0)      175 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/docs/tool/bayestar_sample_model_psd.rst
+-rw-rw-rw-   0 root         (0) root         (0)      175 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/docs/tool/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1400 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/docs/tool/ligo_skymap_combine.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3709 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/docs/tool/ligo_skymap_constellations.rst
+-rw-rw-rw-   0 root         (0) root         (0)      165 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/docs/tool/ligo_skymap_contour.rst
+-rw-rw-rw-   0 root         (0) root         (0)      215 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/docs/tool/ligo_skymap_contour_moc.rst
+-rw-rw-rw-   0 root         (0) root         (0)      199 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/docs/tool/ligo_skymap_flatten.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1387 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/docs/tool/ligo_skymap_from_samples.rst
+-rw-rw-rw-   0 root         (0) root         (0)      747 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/docs/tool/ligo_skymap_plot.rst
+-rw-rw-rw-   0 root         (0) root         (0)      795 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/docs/tool/ligo_skymap_plot_airmass.rst
+-rw-rw-rw-   0 root         (0) root         (0)      779 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/docs/tool/ligo_skymap_plot_coherence.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1121 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/docs/tool/ligo_skymap_plot_observability.rst
+-rw-rw-rw-   0 root         (0) root         (0)      188 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/docs/tool/ligo_skymap_plot_stats.rst
+-rw-rw-rw-   0 root         (0) root         (0)      700 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/docs/tool/ligo_skymap_plot_volume.rst
+-rw-rw-rw-   0 root         (0) root         (0)      177 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/docs/tool/ligo_skymap_stats.rst
+-rw-rw-rw-   0 root         (0) root         (0)      209 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/docs/tool/ligo_skymap_unflatten.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 23:32:16.749760 ligo.skymap-2.0.0rc4/docs/util/
+-rw-rw-rw-   0 root         (0) root         (0)      158 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/docs/util/file.rst
+-rw-rw-rw-   0 root         (0) root         (0)      172 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/docs/util/ilwd.rst
+-rw-rw-rw-   0 root         (0) root         (0)      163 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/docs/util/numpy.rst
+-rw-rw-rw-   0 root         (0) root         (0)      168 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/docs/util/sqlite.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 23:32:16.751761 ligo.skymap-2.0.0rc4/licenses/
+-rw-rw-rw-   0 root         (0) root         (0)     6360 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/licenses/CHEALPIX_LICENSE.rst
+-rw-rw-rw-   0 root         (0) root         (0)    37565 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/licenses/LICENSE.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1792 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/licenses/NUMPY_LICENSE.rst
+-rw-rw-rw-   0 root         (0) root         (0)      372 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/licenses/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1659 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/licenses/TEMPLATE_LICENCE.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 23:32:16.708759 ligo.skymap-2.0.0rc4/ligo/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 23:32:16.757761 ligo.skymap-2.0.0rc4/ligo/skymap/
+-rw-rw-rw-   0 root         (0) root         (0)     1012 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      698 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/_astropy_init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 23:32:16.760761 ligo.skymap-2.0.0rc4/ligo/skymap/bayestar/
+-rw-rw-rw-   0 root         (0) root         (0)    20357 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/bayestar/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5864 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/bayestar/ez_emcee.py
+-rw-rw-rw-   0 root         (0) root         (0)    19685 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/bayestar/filter.py
+-rw-rw-rw-   0 root         (0) root         (0)    10348 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/bayestar/interpolation.py
+-rw-rw-rw-   0 root         (0) root         (0)     2176 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/bayestar/ptemcee.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 23:32:16.761761 ligo.skymap-2.0.0rc4/ligo/skymap/bayestar/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 23:32:03.000000 ligo.skymap-2.0.0rc4/ligo/skymap/bayestar/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1545 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/bayestar/tests/test_bayestar.py
+-rw-rw-rw-   0 root         (0) root         (0)     4573 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/bayestar/tests/test_interpolation.py
+-rw-rw-rw-   0 root         (0) root         (0)     4287 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/bayestar/tests/test_signal_amplitude_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     2321 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 23:32:16.763761 ligo.skymap-2.0.0rc4/ligo/skymap/coordinates/
+-rw-rw-rw-   0 root         (0) root         (0)      382 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/coordinates/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3645 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/coordinates/detector.py
+-rw-rw-rw-   0 root         (0) root         (0)     4132 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/coordinates/eigenframe.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 23:32:16.764761 ligo.skymap-2.0.0rc4/ligo/skymap/coordinates/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 23:32:03.000000 ligo.skymap-2.0.0rc4/ligo/skymap/coordinates/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      996 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/coordinates/tests/test_detector.py
+-rw-rw-rw-   0 root         (0) root         (0)    20545 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/distance.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 23:32:16.764761 ligo.skymap-2.0.0rc4/ligo/skymap/extern/
+-rw-rw-rw-   0 root         (0) root         (0)      460 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/extern/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 23:32:16.765761 ligo.skymap-2.0.0rc4/ligo/skymap/extern/numpy/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 23:32:03.000000 ligo.skymap-2.0.0rc4/ligo/skymap/extern/numpy/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13938 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/extern/numpy/quantile.py
+-rw-rw-rw-   0 root         (0) root         (0)    15264 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/healpix_tree.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 23:32:16.767761 ligo.skymap-2.0.0rc4/ligo/skymap/io/
+-rw-rw-rw-   0 root         (0) root         (0)      382 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/io/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 23:32:16.769761 ligo.skymap-2.0.0rc4/ligo/skymap/io/events/
+-rw-rw-rw-   0 root         (0) root         (0)      382 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/io/events/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3832 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/io/events/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     2664 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/io/events/detector_disabled.py
+-rw-rw-rw-   0 root         (0) root         (0)     2274 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/io/events/gracedb.py
+-rw-rw-rw-   0 root         (0) root         (0)     7809 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/io/events/hdf.py
+-rw-rw-rw-   0 root         (0) root         (0)    11536 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/io/events/ligolw.py
+-rw-rw-rw-   0 root         (0) root         (0)     2563 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/io/events/magic.py
+-rw-rw-rw-   0 root         (0) root         (0)     1700 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/io/events/sqlite.py
+-rwxrwxrwx   0 root         (0) root         (0)    19227 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/io/fits.py
+-rwxrwxrwx   0 root         (0) root         (0)    10626 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/io/hdf5.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 23:32:16.770761 ligo.skymap-2.0.0rc4/ligo/skymap/io/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 23:32:03.000000 ligo.skymap-2.0.0rc4/ligo/skymap/io/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 23:32:16.775761 ligo.skymap-2.0.0rc4/ligo/skymap/io/tests/data/
+-rw-rw-rw-   0 root         (0) root         (0)   492938 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/io/tests/data/2016_subset.xml.gz
+-rw-rw-rw-   0 root         (0) root         (0)     1699 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/io/tests/data/G197392_coinc.xml.gz
+-rw-rw-rw-   0 root         (0) root         (0)      675 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/io/tests/data/G197392_psd.xml.gz
+-rw-rw-rw-   0 root         (0) root         (0)     2470 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/io/tests/data/G211117_coinc.xml.gz
+-rw-rw-rw-   0 root         (0) root         (0)     2355 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/io/tests/data/G211117_psd.xml.gz
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 23:32:03.000000 ligo.skymap-2.0.0rc4/ligo/skymap/io/tests/data/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 23:32:16.776761 ligo.skymap-2.0.0rc4/ligo/skymap/io/tests/data/gstlal_reference_psd/
+-rw-rw-rw-   0 root         (0) root         (0)      717 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/io/tests/data/gstlal_reference_psd/H1L1V1-REFERENCE_PSD-967234210-29963.xml.gz
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 23:32:03.000000 ligo.skymap-2.0.0rc4/ligo/skymap/io/tests/data/gstlal_reference_psd/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9120 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/io/tests/data/test.hdf5
+-rw-rw-rw-   0 root         (0) root         (0)    12825 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/io/tests/test_io_events.py
+-rw-rw-rw-   0 root         (0) root         (0)    17043 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/kde.py
+-rw-rw-rw-   0 root         (0) root         (0)     7376 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/moc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 23:32:16.782761 ligo.skymap-2.0.0rc4/ligo/skymap/plot/
+-rw-rw-rw-   0 root         (0) root         (0)      382 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/plot/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    29444 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/plot/allsky.py
+-rw-rw-rw-   0 root         (0) root         (0)     1754 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/plot/angle.py
+-rw-rw-rw-   0 root         (0) root         (0)     7312 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/plot/backdrop.py
+-rw-rw-rw-   0 root         (0) root         (0)     3915 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/plot/bayes_factor.py
+-rw-rw-rw-   0 root         (0) root         (0)     1530 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/plot/cmap.py
+-rw-rw-rw-   0 root         (0) root         (0)     8714 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/plot/cylon.csv
+-rw-rw-rw-   0 root         (0) root         (0)     2125 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/plot/cylon.py
+-rw-rw-rw-   0 root         (0) root         (0)     2933 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/plot/marker.py
+-rw-rw-rw-   0 root         (0) root         (0)    63275 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/plot/ne_simplified_coastline.json
+-rw-rw-rw-   0 root         (0) root         (0)     7394 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/plot/poly.py
+-rw-rw-rw-   0 root         (0) root         (0)     9445 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/plot/pp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 23:32:16.782761 ligo.skymap-2.0.0rc4/ligo/skymap/plot/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 23:32:03.000000 ligo.skymap-2.0.0rc4/ligo/skymap/plot/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 23:32:16.808762 ligo.skymap-2.0.0rc4/ligo/skymap/plot/tests/baseline/
+-rw-rw-rw-   0 root         (0) root         (0)    67690 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/plot/tests/baseline/test_allsky_axes_astro-degrees-aitoff.png
+-rw-rw-rw-   0 root         (0) root         (0)    65830 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/plot/tests/baseline/test_allsky_axes_astro-degrees-mollweide.png
+-rw-rw-rw-   0 root         (0) root         (0)    65829 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/plot/tests/baseline/test_allsky_axes_astro-hours-aitoff.png
+-rw-rw-rw-   0 root         (0) root         (0)    63879 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/plot/tests/baseline/test_allsky_axes_astro-hours-mollweide.png
+-rw-rw-rw-   0 root         (0) root         (0)    71762 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/plot/tests/baseline/test_allsky_axes_galactic-degrees-aitoff.png
+-rw-rw-rw-   0 root         (0) root         (0)    71509 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/plot/tests/baseline/test_allsky_axes_galactic-degrees-mollweide.png
+-rw-rw-rw-   0 root         (0) root         (0)    70497 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/plot/tests/baseline/test_allsky_axes_galactic-hours-aitoff.png
+-rw-rw-rw-   0 root         (0) root         (0)    69334 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/plot/tests/baseline/test_allsky_axes_galactic-hours-mollweide.png
+-rw-rw-rw-   0 root         (0) root         (0)    64896 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/plot/tests/baseline/test_allsky_axes_geo-degrees-aitoff.png
+-rw-rw-rw-   0 root         (0) root         (0)    63732 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/plot/tests/baseline/test_allsky_axes_geo-degrees-mollweide.png
+-rw-rw-rw-   0 root         (0) root         (0)    63470 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/plot/tests/baseline/test_allsky_axes_geo-hours-aitoff.png
+-rw-rw-rw-   0 root         (0) root         (0)    61561 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/plot/tests/baseline/test_allsky_axes_geo-hours-mollweide.png
+-rw-rw-rw-   0 root         (0) root         (0)    33964 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/plot/tests/baseline/test_allsky_obstime.png
+-rw-rw-rw-   0 root         (0) root         (0)    26192 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/plot/tests/baseline/test_center_projections_197.45d -23.38d-aitoff.png
+-rw-rw-rw-   0 root         (0) root         (0)    25840 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/plot/tests/baseline/test_center_projections_197.45d -23.38d-mollweide.png
+-rw-rw-rw-   0 root         (0) root         (0)    24254 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/plot/tests/baseline/test_center_projections_None-aitoff.png
+-rw-rw-rw-   0 root         (0) root         (0)    22142 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/plot/tests/baseline/test_center_projections_None-mollweide.png
+-rw-rw-rw-   0 root         (0) root         (0)    20330 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/plot/tests/baseline/test_globe_axes.png
+-rw-rw-rw-   0 root         (0) root         (0)    15198 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/plot/tests/baseline/test_plot_bayes_factor.png
+-rw-rw-rw-   0 root         (0) root         (0)    19092 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/plot/tests/baseline/test_pp_plot_default.png
+-rw-rw-rw-   0 root         (0) root         (0)    39991 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/plot/tests/baseline/test_pp_plot_lines.png
+-rw-rw-rw-   0 root         (0) root         (0)    19092 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/plot/tests/baseline/test_pp_plot_steps.png
+-rw-rw-rw-   0 root         (0) root         (0)     8866 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/plot/tests/baseline/test_reticle.png
+-rw-rw-rw-   0 root         (0) root         (0)    19815 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/plot/tests/baseline/test_zoom_axes.png
+-rw-rw-rw-   0 root         (0) root         (0)     6245 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/plot/tests/test_plot.py
+-rw-rw-rw-   0 root         (0) root         (0)     2400 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/plot/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 23:32:16.812763 ligo.skymap-2.0.0rc4/ligo/skymap/postprocess/
+-rw-rw-rw-   0 root         (0) root         (0)      382 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/postprocess/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6348 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/postprocess/contour.py
+-rw-rw-rw-   0 root         (0) root         (0)     2903 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/postprocess/cosmology.py
+-rw-rw-rw-   0 root         (0) root         (0)    18512 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/postprocess/crossmatch.py
+-rw-rw-rw-   0 root         (0) root         (0)    15257 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/postprocess/ellipse.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 23:32:16.814762 ligo.skymap-2.0.0rc4/ligo/skymap/postprocess/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 23:32:03.000000 ligo.skymap-2.0.0rc4/ligo/skymap/postprocess/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1210 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/postprocess/tests/test_cosmology.py
+-rw-rw-rw-   0 root         (0) root         (0)     4373 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/postprocess/tests/test_crossmatch.py
+-rw-rw-rw-   0 root         (0) root         (0)     3219 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/postprocess/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 23:32:16.814762 ligo.skymap-2.0.0rc4/ligo/skymap/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 23:32:03.000000 ligo.skymap-2.0.0rc4/ligo/skymap/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 23:32:16.815763 ligo.skymap-2.0.0rc4/ligo/skymap/tests/plugins/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 23:32:03.000000 ligo.skymap-2.0.0rc4/ligo/skymap/tests/plugins/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      578 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/tests/plugins/omp.py
+-rw-rw-rw-   0 root         (0) root         (0)     4831 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/tests/test_moc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 23:32:16.827763 ligo.skymap-2.0.0rc4/ligo/skymap/tool/
+-rw-rw-rw-   0 root         (0) root         (0)    15388 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/tool/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    21608 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/tool/bayestar_inject.py
+-rw-rw-rw-   0 root         (0) root         (0)     7333 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/tool/bayestar_localize_coincs.py
+-rwxrwxrwx   0 root         (0) root         (0)     6682 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/tool/bayestar_localize_lvalert.py
+-rw-rw-rw-   0 root         (0) root         (0)     8071 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/tool/bayestar_mcmc.py
+-rw-rw-rw-   0 root         (0) root         (0)    18761 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/tool/bayestar_realize_coincs.py
+-rw-rw-rw-   0 root         (0) root         (0)     4600 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/tool/bayestar_sample_model_psd.py
+-rw-rw-rw-   0 root         (0) root         (0)     5841 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/tool/ligo_skymap_combine.py
+-rw-rw-rw-   0 root         (0) root         (0)     2011 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/tool/ligo_skymap_constellations.py
+-rw-rw-rw-   0 root         (0) root         (0)     3341 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/tool/ligo_skymap_contour.py
+-rw-rw-rw-   0 root         (0) root         (0)     2519 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/tool/ligo_skymap_contour_moc.py
+-rw-rw-rw-   0 root         (0) root         (0)     2288 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/tool/ligo_skymap_flatten.py
+-rw-rw-rw-   0 root         (0) root         (0)     7662 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/tool/ligo_skymap_from_samples.py
+-rw-rw-rw-   0 root         (0) root         (0)     6732 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/tool/ligo_skymap_plot.py
+-rw-rw-rw-   0 root         (0) root         (0)     8353 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/tool/ligo_skymap_plot_airmass.py
+-rw-rw-rw-   0 root         (0) root         (0)     1713 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/tool/ligo_skymap_plot_coherence.py
+-rw-rw-rw-   0 root         (0) root         (0)     5711 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/tool/ligo_skymap_plot_observability.py
+-rw-rw-rw-   0 root         (0) root         (0)     5158 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/tool/ligo_skymap_plot_pp_samples.py
+-rw-rw-rw-   0 root         (0) root         (0)     8048 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/tool/ligo_skymap_plot_stats.py
+-rwxrwxrwx   0 root         (0) root         (0)     9391 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/tool/ligo_skymap_plot_volume.py
+-rw-rw-rw-   0 root         (0) root         (0)    11830 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/tool/ligo_skymap_stats.py
+-rw-rw-rw-   0 root         (0) root         (0)     1739 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/tool/ligo_skymap_unflatten.py
+-rw-rw-rw-   0 root         (0) root         (0)     4508 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/tool/matplotlib.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 23:32:16.830763 ligo.skymap-2.0.0rc4/ligo/skymap/tool/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     3088 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/tool/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5271 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/tool/tests/test_bayestar.py
+-rw-rw-rw-   0 root         (0) root         (0)     4496 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/tool/tests/test_bayestar_inject.py
+-rw-rw-rw-   0 root         (0) root         (0)     2400 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/tool/tests/test_combine.py
+-rw-rw-rw-   0 root         (0) root         (0)     4015 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/tool/tests/test_flatten.py
+-rw-rw-rw-   0 root         (0) root         (0)     2631 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/tool/tests/test_from_samples.py
+-rw-rw-rw-   0 root         (0) root         (0)      529 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/tool/tests/test_help.py
+-rw-rw-rw-   0 root         (0) root         (0)     1826 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/tool/tests/test_plot.py
+-rw-rw-rw-   0 root         (0) root         (0)     2065 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/tool/tests/test_plot_stats.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 23:32:16.833763 ligo.skymap-2.0.0rc4/ligo/skymap/util/
+-rw-rw-rw-   0 root         (0) root         (0)      382 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/util/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1794 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/util/file.py
+-rw-rw-rw-   0 root         (0) root         (0)     5170 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/util/ilwd.py
+-rw-rw-rw-   0 root         (0) root         (0)      813 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/util/math.py
+-rw-rw-rw-   0 root         (0) root         (0)     2023 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/util/numpy.py
+-rw-rw-rw-   0 root         (0) root         (0)     2854 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/util/progress.py
+-rw-rw-rw-   0 root         (0) root         (0)     4451 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/util/sqlite.py
+-rw-rw-rw-   0 root         (0) root         (0)     2694 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/util/stopwatch.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 23:32:16.834763 ligo.skymap-2.0.0rc4/ligo/skymap/util/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 23:32:03.000000 ligo.skymap-2.0.0rc4/ligo/skymap/util/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      363 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/ligo/skymap/util/tests/test_progress.py
+-rw-r--r--   0 root         (0) root         (0)      340 2024-04-10 23:32:16.000000 ligo.skymap-2.0.0rc4/ligo/skymap/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 23:32:16.841763 ligo.skymap-2.0.0rc4/ligo.skymap.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5226 2024-04-10 23:32:16.000000 ligo.skymap-2.0.0rc4/ligo.skymap.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8711 2024-04-10 23:32:16.000000 ligo.skymap-2.0.0rc4/ligo.skymap.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 23:32:16.000000 ligo.skymap-2.0.0rc4/ligo.skymap.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1550 2024-04-10 23:32:16.000000 ligo.skymap-2.0.0rc4/ligo.skymap.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 23:32:16.000000 ligo.skymap-2.0.0rc4/ligo.skymap.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      423 2024-04-10 23:32:16.000000 ligo.skymap-2.0.0rc4/ligo.skymap.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2024-04-10 23:32:16.000000 ligo.skymap-2.0.0rc4/ligo.skymap.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      184 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     6409 2024-04-10 23:32:16.845764 ligo.skymap-2.0.0rc4/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     3807 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 23:32:16.840763 ligo.skymap-2.0.0rc4/src/
+-rw-rw-rw-   0 root         (0) root         (0)    37062 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/src/bayestar_cosmology.h
+-rw-rw-rw-   0 root         (0) root         (0)     4094 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/src/bayestar_cosmology.py
+-rw-rw-rw-   0 root         (0) root         (0)    15859 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/src/bayestar_distance.c
+-rw-rw-rw-   0 root         (0) root         (0)     2067 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/src/bayestar_distance.h
+-rw-rw-rw-   0 root         (0) root         (0)     4286 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/src/bayestar_moc.c
+-rw-rw-rw-   0 root         (0) root         (0)     1492 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/src/bayestar_moc.h
+-rw-rw-rw-   0 root         (0) root         (0)    50371 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/src/bayestar_sky_map.c
+-rw-rw-rw-   0 root         (0) root         (0)     7831 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/src/bayestar_sky_map.h
+-rw-rw-rw-   0 root         (0) root         (0)      218 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/src/branch_prediction.h
+-rw-rw-rw-   0 root         (0) root         (0)    41208 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/src/core.c
+-rw-rw-rw-   0 root         (0) root         (0)     5818 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/src/cubic_interp.c
+-rw-rw-rw-   0 root         (0) root         (0)     2069 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/src/cubic_interp.h
+-rw-rw-rw-   0 root         (0) root         (0)    13016 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/src/cubic_interp_test.c
+-rw-rw-rw-   0 root         (0) root         (0)     6370 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/src/omp_interruptible.h
+-rw-rw-rw-   0 root         (0) root         (0)     2377 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/src/vmath.h
+-rw-rw-rw-   0 root         (0) root         (0)     1869 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/src/warnings.h
+-rw-rw-rw-   0 root         (0) root         (0)     2595 2024-04-10 18:40:06.000000 ligo.skymap-2.0.0rc4/tox.ini
```

### Comparing `ligo.skymap-2.0.0rc3/.gitignore` & `ligo.skymap-2.0.0rc4/.gitignore`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/.gitlab/combine-coverage.py` & `ligo.skymap-2.0.0rc4/.gitlab/combine-coverage.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/.gitlab-ci.yml` & `ligo.skymap-2.0.0rc4/.gitlab-ci.yml`

 * *Files 6% similar despite different names*

```diff
@@ -141,35 +141,48 @@
     GIT_STRATEGY: none
   script:
     - docker login -u gitlab-ci-token -p $CI_JOB_TOKEN $CI_REGISTRY
     - |
       cat <<EOF > Dockerfile
       FROM python:${CI_JOB_NAME#*python}
       RUN apt-get update && apt-get -y install --no-install-recommends libchealpix-dev libgsl-dev pkg-config && rm -rf /var/lib/apt/lists/*
-      RUN pip --no-cache-dir install pytest-cov gcovr pycobertura flake8 coverage tox
+      # FIXME: Install h5py<3.11.0 on aarch64 because h5py has not released aarch64 wheels for 3.11.0.
+      RUN pip --no-cache-dir install pytest-cov gcovr pycobertura flake8 coverage tox 'pip>=24' 'h5py<3.11.0;platform_machine=="aarch64"'
       COPY requirements.txt .
       RUN pip --no-cache-dir install -r requirements.txt && rm -f requirements.txt
       EOF
     - docker build -t $IMAGE_TAG .
     - docker push $IMAGE_TAG
   needs:
     - requirements
+  tags:
+    - executor-docker
 
 deps-aarch64/python3.9:
   <<: *deps
   tags:
     - aarch64
+    # FIXME: Uncomment after the following issue is fixed.
+    # https://git.ligo.org/computing/helpdesk/-/issues/5775
+    # - executor-docker
 
 deps-x86_64/python3.9:
   <<: *deps
 
 deps-x86_64/python3.10:
   <<: *deps
 
-deps-x86_64/python3.11:
+# FIXME: Temporarily pin Python patch version due to bug affecting doctests.
+# See https://github.com/python/cpython/issues/117692.
+deps-x86_64/python3.11.8:
+  <<: *deps
+
+# FIXME: Temporarily pin Python patch version due to bug affecting doctests.
+# See https://github.com/python/cpython/issues/117692.
+deps-x86_64/python3.12.2:
   <<: *deps
 
 #
 # Generate documentation.
 #
 
 docs:
@@ -222,19 +235,26 @@
 test/linux/x86_64/python3.10:
   <<: *test
   image: $CI_REGISTRY_IMAGE/deps-x86_64/python3.10:$CI_COMMIT_REF_SLUG
   needs:
     - deps-x86_64/python3.10
     - wheel/linux/x86_64
 
-test/linux/x86_64/python3.11:
+test/linux/x86_64/python3.11.8:
+  <<: *test
+  image: $CI_REGISTRY_IMAGE/deps-x86_64/python3.11.8:$CI_COMMIT_REF_SLUG
+  needs:
+    - deps-x86_64/python3.11.8
+    - wheel/linux/x86_64
+
+test/linux/x86_64/python3.12.2:
   <<: *test
-  image: $CI_REGISTRY_IMAGE/deps-x86_64/python3.11:$CI_COMMIT_REF_SLUG
+  image: $CI_REGISTRY_IMAGE/deps-x86_64/python3.12.2:$CI_COMMIT_REF_SLUG
   needs:
-    - deps-x86_64/python3.11
+    - deps-x86_64/python3.12.2
     - wheel/linux/x86_64
 
 .test/macos: &test-macos
   <<: *in-tmpdir
   stage: test
   script:
     - . /opt/local/share/macports/setupenv.bash
@@ -313,22 +333,22 @@
     CC: gcc -coverage
     LDSHARED: gcc -pthread -shared -coverage
     CFLAGS: -UNDEBUG -fsanitize=undefined -fopenmp
   coverage: '/^TOTAL\s+.*\s+(\d+\.?\d*)%/'
   <<: *in-tmpdir
   script:
     - tar --strip-components 1 -xf ${CI_PROJECT_DIR}/*.tar.*
+    # Build and install package with pip, but save the intermediate files which
+    # include gcov's .gcno data files.
+    - mkdir obj
+    - pip install --no-deps -C--global-option=build_ext -C--global-option=--build-temp=$(pwd)/obj -ve .
     # Run tests.
-    # FIXME: C coverage relies on in-tree build/ directory.
-    # pip 21.3 uses an out-of-tree temporary directory.
-    - pip install 'pip<21.3'
-    - pip install -ve .[test]
     - pytest --capture=sys --doctest-plus --doctest-ufunc --mpl --mpl-results-path ${CI_PROJECT_DIR}/pytest-mpl-results --mpl-generate-summary=html --durations=10 --cov ligo/skymap --junit-xml=${CI_PROJECT_DIR}/junit.xml || FAILED=true
     # Write coverage reports in Cobertura format.
-    - gcovr --gcov-ignore-errors no_working_dir_found build/temp*/src -r . -x -o c-coverage.xml
+    - gcovr --gcov-ignore-errors no_working_dir_found obj -r . -x -o c-coverage.xml
     - coverage xml -o py-coverage.xml
     # Merge coverage reports.
     - ${CI_PROJECT_DIR}/.gitlab/combine-coverage.py py-coverage.xml c-coverage.xml coverage.xml
     # Write human-readable report.
     - pycobertura show coverage.xml -f html -o coverage.html
     - pycobertura show coverage.xml
     - cp coverage.html coverage.xml ${CI_PROJECT_DIR}
```

### Comparing `ligo.skymap-2.0.0rc3/CHANGES.rst` & `ligo.skymap-2.0.0rc4/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #########
 Changelog
 #########
 
-2.0.0rc3 (2024-03-31)
+2.0.0rc4 (2024-04-10)
 =====================
 
 - Added options to center ``mollweide`` and ``aitoff`` projections. Thanks go
   to Sam Wyatt for this contribution.
 
 - Added support for ``os.PathLike`` filenames when reading ligolw files. Thanks
   go to Thomas Sainrat for this contribution.
@@ -22,15 +22,17 @@
   the (lack of the) ``--transparent`` option. This improves text and label 
   readability against dark backgrounds when transparent mode is not on. Thanks
   go to Geoffrey Mo for this contribution.
 
 - Add documentation on the LIGO Scientific Collaboration (LSC) review process
   to the Testing section of the manual.
 
-- Require Numpy >= 1.23.0.
+- Require Numpy >= 1.23.0. Rebuild for binary compatibility with Numpy 2.0.0.
+
+- Add unit tests for Python 3.12.
 
 1.1.2 (2023-10-03)
 ==================
 
 - Update for compatibility with Matplotlib 3.8.0.
 
 - Binary wheels for macOS x86_64 are now built against Big Sur (10.15), because
```

### Comparing `ligo.skymap-2.0.0rc3/CONTRIBUTING.rst` & `ligo.skymap-2.0.0rc4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/PKG-INFO` & `ligo.skymap-2.0.0rc4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ligo.skymap
-Version: 2.0.0rc3
+Version: 2.0.0rc4
 Summary: Tools for reading, writing, manipulating, and making LIGO and Virgo sky maps
 Home-page: https://lscsoft.docs.ligo.org/ligo.skymap/
 Author: Leo Singer
 Author-email: leo.singer@ligo.org
 License: GNU GPL v3+
 Project-URL: Bug Tracker, https://git.ligo.org/lscsoft/ligo.skymap/issues
 Project-URL: Change Log, https://lscsoft.docs.ligo.org/ligo.skymap/changes.html
@@ -19,14 +19,15 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: licenses/LICENSE.rst
 Requires-Dist: astroplan>=0.7
 Requires-Dist: astropy>=5.0
```

### Comparing `ligo.skymap-2.0.0rc3/README.rst` & `ligo.skymap-2.0.0rc4/README.rst`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/cextern/chealpix/chealpix.c` & `ligo.skymap-2.0.0rc4/cextern/chealpix/chealpix.c`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/cextern/chealpix/chealpix.h` & `ligo.skymap-2.0.0rc4/cextern/chealpix/chealpix.h`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/docs/Makefile` & `ligo.skymap-2.0.0rc4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/docs/_static/benchmark.svg` & `ligo.skymap-2.0.0rc4/docs/_static/benchmark.svg`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/docs/_static/coinc.xml` & `ligo.skymap-2.0.0rc4/docs/_static/coinc.xml`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/docs/_static/localization.svg` & `ligo.skymap-2.0.0rc4/docs/_static/localization.svg`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/docs/bayestar/eggbox.png` & `ligo.skymap-2.0.0rc4/docs/bayestar/eggbox.png`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/docs/changes.rst` & `ligo.skymap-2.0.0rc4/docs/changes.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #########
 Changelog
 #########
 
-2.0.0rc3 (2024-03-31)
+2.0.0rc4 (2024-04-10)
 =====================
 
 - Added options to center ``mollweide`` and ``aitoff`` projections. Thanks go
   to Sam Wyatt for this contribution.
 
 - Added support for ``os.PathLike`` filenames when reading ligolw files. Thanks
   go to Thomas Sainrat for this contribution.
@@ -22,15 +22,17 @@
   the (lack of the) ``--transparent`` option. This improves text and label 
   readability against dark backgrounds when transparent mode is not on. Thanks
   go to Geoffrey Mo for this contribution.
 
 - Add documentation on the LIGO Scientific Collaboration (LSC) review process
   to the Testing section of the manual.
 
-- Require Numpy >= 1.23.0.
+- Require Numpy >= 1.23.0. Rebuild for binary compatibility with Numpy 2.0.0.
+
+- Add unit tests for Python 3.12.
 
 1.1.2 (2023-10-03)
 ==================
 
 - Update for compatibility with Matplotlib 3.8.0.
 
 - Binary wheels for macOS x86_64 are now built against Big Sur (10.15), because
```

### Comparing `ligo.skymap-2.0.0rc3/docs/conf.py` & `ligo.skymap-2.0.0rc4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/docs/contributing.rst` & `ligo.skymap-2.0.0rc4/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/docs/develop.rst` & `ligo.skymap-2.0.0rc4/docs/develop.rst`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/docs/distance/index.rst` & `ligo.skymap-2.0.0rc4/docs/distance/index.rst`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/docs/help.rst` & `ligo.skymap-2.0.0rc4/docs/help.rst`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/docs/index.rst` & `ligo.skymap-2.0.0rc4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/docs/interface.rst` & `ligo.skymap-2.0.0rc4/docs/interface.rst`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/docs/io/events.rst` & `ligo.skymap-2.0.0rc4/docs/io/events.rst`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/docs/make.bat` & `ligo.skymap-2.0.0rc4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/docs/performance.rst` & `ligo.skymap-2.0.0rc4/docs/performance.rst`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/docs/quickstart/bayestar-injections.rst` & `ligo.skymap-2.0.0rc4/docs/quickstart/bayestar-injections.rst`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/docs/quickstart/install.rst` & `ligo.skymap-2.0.0rc4/docs/quickstart/install.rst`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/docs/testing.rst` & `ligo.skymap-2.0.0rc4/docs/testing.rst`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/docs/tool/ligo_skymap_combine.rst` & `ligo.skymap-2.0.0rc4/docs/tool/ligo_skymap_combine.rst`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/docs/tool/ligo_skymap_constellations.rst` & `ligo.skymap-2.0.0rc4/docs/tool/ligo_skymap_constellations.rst`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/docs/tool/ligo_skymap_from_samples.rst` & `ligo.skymap-2.0.0rc4/docs/tool/ligo_skymap_from_samples.rst`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/docs/tool/ligo_skymap_plot.rst` & `ligo.skymap-2.0.0rc4/docs/tool/ligo_skymap_plot.rst`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/docs/tool/ligo_skymap_plot_airmass.rst` & `ligo.skymap-2.0.0rc4/docs/tool/ligo_skymap_plot_airmass.rst`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/docs/tool/ligo_skymap_plot_coherence.rst` & `ligo.skymap-2.0.0rc4/docs/tool/ligo_skymap_plot_coherence.rst`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/docs/tool/ligo_skymap_plot_observability.rst` & `ligo.skymap-2.0.0rc4/docs/tool/ligo_skymap_plot_observability.rst`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/docs/tool/ligo_skymap_plot_volume.rst` & `ligo.skymap-2.0.0rc4/docs/tool/ligo_skymap_plot_volume.rst`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/licenses/CHEALPIX_LICENSE.rst` & `ligo.skymap-2.0.0rc4/licenses/CHEALPIX_LICENSE.rst`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/licenses/LICENSE.rst` & `ligo.skymap-2.0.0rc4/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/licenses/NUMPY_LICENSE.rst` & `ligo.skymap-2.0.0rc4/licenses/NUMPY_LICENSE.rst`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/licenses/TEMPLATE_LICENCE.rst` & `ligo.skymap-2.0.0rc4/licenses/TEMPLATE_LICENCE.rst`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/ligo/skymap/__init__.py` & `ligo.skymap-2.0.0rc4/ligo/skymap/__init__.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/ligo/skymap/_astropy_init.py` & `ligo.skymap-2.0.0rc4/ligo/skymap/_astropy_init.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/ligo/skymap/bayestar/__init__.py` & `ligo.skymap-2.0.0rc4/ligo/skymap/bayestar/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (C) 2013-2020  Leo Singer
+# Copyright (C) 2013-2024  Leo Singer
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -56,15 +56,14 @@
 __all__ = ('derasterize', 'localize', 'rasterize', 'antenna_factor',
            'signal_amplitude_model')
 
 log = logging.getLogger('BAYESTAR')
 
 _RESCALE_LOGLIKELIHOOD = 0.83
 
-antenna_factor = require_contiguous_aligned(antenna_factor)
 signal_amplitude_model = require_contiguous_aligned(signal_amplitude_model)
 _log_posterior_toa_phoa_snr = require_contiguous_aligned(
     _log_posterior_toa_phoa_snr)
 
 
 # Wrap so that ufunc parameter names are known
 def log_posterior_toa_phoa_snr(
```

### Comparing `ligo.skymap-2.0.0rc3/ligo/skymap/bayestar/ez_emcee.py` & `ligo.skymap-2.0.0rc4/ligo/skymap/bayestar/ez_emcee.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/ligo/skymap/bayestar/filter.py` & `ligo.skymap-2.0.0rc4/ligo/skymap/bayestar/filter.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/ligo/skymap/bayestar/interpolation.py` & `ligo.skymap-2.0.0rc4/ligo/skymap/bayestar/interpolation.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/ligo/skymap/bayestar/ptemcee.py` & `ligo.skymap-2.0.0rc4/ligo/skymap/bayestar/ptemcee.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/ligo/skymap/bayestar/tests/test_bayestar.py` & `ligo.skymap-2.0.0rc4/ligo/skymap/bayestar/tests/test_bayestar.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/ligo/skymap/bayestar/tests/test_interpolation.py` & `ligo.skymap-2.0.0rc4/ligo/skymap/bayestar/tests/test_interpolation.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/ligo/skymap/bayestar/tests/test_signal_amplitude_model.py` & `ligo.skymap-2.0.0rc4/ligo/skymap/bayestar/tests/test_signal_amplitude_model.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/ligo/skymap/conftest.py` & `ligo.skymap-2.0.0rc4/ligo/skymap/conftest.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/ligo/skymap/coordinates/detector.py` & `ligo.skymap-2.0.0rc4/ligo/skymap/coordinates/detector.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/ligo/skymap/coordinates/eigenframe.py` & `ligo.skymap-2.0.0rc4/ligo/skymap/coordinates/eigenframe.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/ligo/skymap/coordinates/tests/test_detector.py` & `ligo.skymap-2.0.0rc4/ligo/skymap/coordinates/tests/test_detector.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/ligo/skymap/distance.py` & `ligo.skymap-2.0.0rc4/ligo/skymap/distance.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (C) 2017-2020  Leo Singer
+# Copyright (C) 2017-2024  Leo Singer
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -65,15 +65,14 @@
 
 Returns
 -------
 pdf : `numpy.ndarray`
     Conditional probability density according to ansatz.
 
 """)
-conditional_pdf = require_contiguous_aligned(conditional_pdf)
 
 
 add_newdoc_ufunc(conditional_cdf, """\
 Cumulative conditional distribution of distance (ansatz).
 
 Parameters
 ----------
@@ -104,15 +103,14 @@
 ...     conditional_pdf, 0, r,
 ...     (distmu, distsigma, distnorm))
 >>> result = conditional_cdf(
 ...     r, distmu, distsigma, distnorm)
 >>> np.testing.assert_almost_equal(result, expected)
 
 """)
-conditional_cdf = require_contiguous_aligned(conditional_cdf)
 
 
 add_newdoc_ufunc(conditional_ppf, """\
 Point percent function (inverse cdf) of distribution of distance (ansatz).
 
 Parameters
 ----------
@@ -141,15 +139,14 @@
 >>> p = 0.16  # "one-sigma" lower limit
 >>> expected_r16 = scipy.optimize.brentq(
 ... lambda r: conditional_cdf(r, distmu, distsigma, distnorm) - p, 0.0, 100.0)
 >>> r16 = conditional_ppf(p, distmu, distsigma, distnorm)
 >>> np.testing.assert_almost_equal(r16, expected_r16)
 
 """)
-conditional_ppf = require_contiguous_aligned(conditional_ppf)
 
 
 add_newdoc_ufunc(moments_to_parameters, """\
 Convert ansatz moments to parameters.
 
 This function is the inverse of `parameters_to_moments`.
 
@@ -166,15 +163,14 @@
     Distance location parameter (Mpc)
 distsigma : `numpy.ndarray`
     Distance scale parameter (Mpc)
 distnorm : `numpy.ndarray`
     Distance normalization factor (Mpc^-2)
 
 """)
-moments_to_parameters = require_contiguous_aligned(moments_to_parameters)
 
 
 add_newdoc_ufunc(parameters_to_moments, """\
 Convert ansatz parameters to moments.
 
 This function is the inverse of `moments_to_parameters`.
 
@@ -230,15 +226,14 @@
 ...     expected_mean, r2 = moments[1:] * expected_norm
 ...     expected_std = np.sqrt(r2 - np.square(expected_mean))
 ...     np.testing.assert_approx_equal(mean, expected_mean, 5)
 ...     np.testing.assert_approx_equal(std, expected_std, 5)
 ...     np.testing.assert_approx_equal(norm, expected_norm, 5)
 
 """)
-parameters_to_moments = require_contiguous_aligned(parameters_to_moments)
 
 
 add_newdoc_ufunc(volume_render, """\
 Perform volumetric rendering of a 3D sky map.
 
 Parameters
 ----------
```

### Comparing `ligo.skymap-2.0.0rc3/ligo/skymap/extern/numpy/quantile.py` & `ligo.skymap-2.0.0rc4/ligo/skymap/extern/numpy/quantile.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/ligo/skymap/healpix_tree.py` & `ligo.skymap-2.0.0rc4/ligo/skymap/healpix_tree.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/ligo/skymap/io/events/base.py` & `ligo.skymap-2.0.0rc4/ligo/skymap/io/events/base.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/ligo/skymap/io/events/detector_disabled.py` & `ligo.skymap-2.0.0rc4/ligo/skymap/io/events/detector_disabled.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/ligo/skymap/io/events/gracedb.py` & `ligo.skymap-2.0.0rc4/ligo/skymap/io/events/gracedb.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/ligo/skymap/io/events/hdf.py` & `ligo.skymap-2.0.0rc4/ligo/skymap/io/events/hdf.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/ligo/skymap/io/events/ligolw.py` & `ligo.skymap-2.0.0rc4/ligo/skymap/io/events/ligolw.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2017-2020  Leo Singer
+# Copyright (C) 2017-2024  Leo Singer
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -10,15 +10,15 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 #
 """Read events from pipedown/GstLal-style XML output."""
-from collections import OrderedDict, defaultdict
+from collections import defaultdict
 import errno
 from functools import lru_cache
 import itertools
 import logging
 import operator
 import os
 
@@ -70,15 +70,15 @@
         try:
             filename = f.name
         except AttributeError:
             filename = ''
     return doc, filename
 
 
-class LigoLWEventSource(OrderedDict, EventSource):
+class LigoLWEventSource(dict, EventSource):
     """Read events from LIGO-LW XML files.
 
     Parameters
     ----------
     f : str, file-like object, or `ligo.lw.ligolw.Document`
         The name of the file, or the file object, or the XML document object,
         containing the trigger tables.
@@ -104,14 +104,22 @@
                  fallbackpath=None, **kwargs):
         doc, filename = _read_xml(f)
         self._fallbackpath = (
             os.path.dirname(filename) if filename else fallbackpath)
         self._psds_for_file = lru_cache(maxsize=None)(self._psds_for_file)
         super().__init__(self._make_events(doc, psd_file, coinc_def))
 
+    def __str__(self):
+        contents = repr(self)
+        return '<{}>'.format(contents)
+
+    def __repr__(self):
+        contents = super().__repr__()
+        return '{}({})'.format(self.__class__.__name__, contents)
+
     _template_keys = '''mass1 mass2
                         spin1x spin1y spin1z spin2x spin2y spin2z
                         f_final'''.split()
 
     _invert_phases = {
         'pycbc': False,
         'gstlal_inspiral': True,
```

### Comparing `ligo.skymap-2.0.0rc3/ligo/skymap/io/events/magic.py` & `ligo.skymap-2.0.0rc4/ligo/skymap/io/events/magic.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/ligo/skymap/io/events/sqlite.py` & `ligo.skymap-2.0.0rc4/ligo/skymap/io/events/sqlite.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/ligo/skymap/io/fits.py` & `ligo.skymap-2.0.0rc4/ligo/skymap/io/fits.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/ligo/skymap/io/hdf5.py` & `ligo.skymap-2.0.0rc4/ligo/skymap/io/hdf5.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/ligo/skymap/io/tests/data/2016_subset.xml.gz` & `ligo.skymap-2.0.0rc4/ligo/skymap/io/tests/data/2016_subset.xml.gz`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/ligo/skymap/io/tests/data/G197392_coinc.xml.gz` & `ligo.skymap-2.0.0rc4/ligo/skymap/io/tests/data/G197392_coinc.xml.gz`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/ligo/skymap/io/tests/data/G197392_psd.xml.gz` & `ligo.skymap-2.0.0rc4/ligo/skymap/io/tests/data/G197392_psd.xml.gz`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/ligo/skymap/io/tests/data/G211117_coinc.xml.gz` & `ligo.skymap-2.0.0rc4/ligo/skymap/io/tests/data/G211117_coinc.xml.gz`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/ligo/skymap/io/tests/data/G211117_psd.xml.gz` & `ligo.skymap-2.0.0rc4/ligo/skymap/io/tests/data/G211117_psd.xml.gz`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/ligo/skymap/io/tests/data/gstlal_reference_psd/H1L1V1-REFERENCE_PSD-967234210-29963.xml.gz` & `ligo.skymap-2.0.0rc4/ligo/skymap/io/tests/data/gstlal_reference_psd/H1L1V1-REFERENCE_PSD-967234210-29963.xml.gz`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/ligo/skymap/io/tests/data/test.hdf5` & `ligo.skymap-2.0.0rc4/ligo/skymap/io/tests/data/test.hdf5`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/ligo/skymap/io/tests/test_io_events.py` & `ligo.skymap-2.0.0rc4/ligo/skymap/io/tests/test_io_events.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,16 +75,16 @@
 
 
 def test_ligolw():
     """Test reading events from LIGO-LW XML files."""
     source = events.open(os.path.join(DATA_PATH, '2016_subset.xml.gz'))
     ligolw_assertions(source)
 
-    assert str(source) == '<LigoLWEventSource({...250 items...})>'
-    assert repr(source).startswith('LigoLWEventSource([(288172, <LigoLWEvent(')
+    assert str(source).startswith('<LigoLWEventSource({288172: <LigoLWEvent(')
+    assert repr(source).startswith('LigoLWEventSource({288172: <LigoLWEvent(')
     event, *_ = source.values()
     assert str(event).startswith(
         "<LigoLWEvent(singles=(<LigoLWSingleEvent(detector='H1', snr=12.")
     assert repr(event).startswith(
         "<LigoLWEvent(singles=(<LigoLWSingleEvent(detector='H1', snr=12.")
     single_event, *_ = event.singles
     assert str(single_event) == "<LigoLWSingleEvent(detector='H1', snr=12.035994, phase=-1.0371021, time=970976257.4808338)>"  # noqa
```

### Comparing `ligo.skymap-2.0.0rc3/ligo/skymap/kde.py` & `ligo.skymap-2.0.0rc4/ligo/skymap/kde.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/ligo/skymap/moc.py` & `ligo.skymap-2.0.0rc4/ligo/skymap/moc.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (C) 2017-2023  Leo Singer
+# Copyright (C) 2017-2024  Leo Singer
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -31,15 +31,15 @@
 from astropy import units as u
 import astropy_healpix as ah
 import numpy as np
 from numpy.lib.recfunctions import repack_fields
 
 from .core import nest2uniq, uniq2nest, uniq2order, uniq2pixarea, uniq2ang
 from .core import rasterize as _rasterize
-from .util.numpy import add_newdoc_ufunc, require_contiguous_aligned
+from .util.numpy import add_newdoc_ufunc
 
 __all__ = ('nest2uniq', 'uniq2nest', 'uniq2order', 'uniq2pixarea',
            'uniq2ang', 'rasterize', 'bayestar_adaptive_grid')
 
 
 add_newdoc_ufunc(nest2uniq, """\
 Convert a pixel index from NESTED to NUNIQ ordering.
@@ -53,15 +53,14 @@
 
 Returns
 -------
 uniq : `numpy.ndarray`
     NUNIQ pixel index
 
 """)
-nest2uniq = require_contiguous_aligned(nest2uniq)
 
 
 add_newdoc_ufunc(uniq2order, """\
 Determine the HEALPix resolution order of a HEALPix NESTED index.
 
 Parameters
 ----------
@@ -70,15 +69,14 @@
 
 Returns
 -------
 order : `numpy.ndarray`
     HEALPix resolution order, the logarithm base 2 of `nside`
 
 """)
-uniq2order = require_contiguous_aligned(uniq2order)
 
 
 add_newdoc_ufunc(uniq2pixarea, """\
 Determine the area of a HEALPix NESTED index.
 
 Parameters
 ----------
@@ -87,15 +85,14 @@
 
 Returns
 -------
 area : `numpy.ndarray`
     The pixel's area in steradians
 
 """)
-uniq2pixarea = require_contiguous_aligned(uniq2pixarea)
 
 
 add_newdoc_ufunc(uniq2nest, """\
 Convert a pixel index from NUNIQ to NESTED ordering.
 
 Parameters
 ----------
@@ -106,15 +103,14 @@
 -------
 order : `numpy.ndarray`
     HEALPix resolution order (logarithm base 2 of `nside`)
 ipix : `numpy.ndarray`
     NESTED pixel index
 
 """)
-uniq2nest = require_contiguous_aligned(uniq2nest)
 
 
 def rasterize(moc_data, order=None):
     """Convert a multi-order HEALPix dataset to fixed-order NESTED ordering.
 
     Parameters
     ----------
@@ -223,8 +219,8 @@
     uniq = nest2uniq(order.astype(np.int8), ipix)
 
     # Done!
     return table.Table([uniq, post], names=['UNIQ', 'PROBDENSITY'],
                        copy=False)
 
 
-del add_newdoc_ufunc, require_contiguous_aligned
+del add_newdoc_ufunc
```

### Comparing `ligo.skymap-2.0.0rc3/ligo/skymap/plot/allsky.py` & `ligo.skymap-2.0.0rc4/ligo/skymap/plot/allsky.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (C) 2012-2020  Leo Singer
+# Copyright (C) 2012-2023  Leo Singer
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
```

### Comparing `ligo.skymap-2.0.0rc3/ligo/skymap/plot/backdrop.py` & `ligo.skymap-2.0.0rc4/ligo/skymap/plot/backdrop.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/ligo/skymap/plot/bayes_factor.py` & `ligo.skymap-2.0.0rc4/ligo/skymap/plot/bayes_factor.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/ligo/skymap/plot/cmap.py` & `ligo.skymap-2.0.0rc4/ligo/skymap/plot/cmap.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/ligo/skymap/plot/cylon.csv` & `ligo.skymap-2.0.0rc4/ligo/skymap/plot/cylon.csv`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/ligo/skymap/plot/cylon.py` & `ligo.skymap-2.0.0rc4/ligo/skymap/plot/cylon.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/ligo/skymap/plot/marker.py` & `ligo.skymap-2.0.0rc4/ligo/skymap/plot/marker.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/ligo/skymap/plot/ne_simplified_coastline.json` & `ligo.skymap-2.0.0rc4/ligo/skymap/plot/ne_simplified_coastline.json`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/ligo/skymap/plot/poly.py` & `ligo.skymap-2.0.0rc4/ligo/skymap/plot/poly.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/ligo/skymap/plot/pp.py` & `ligo.skymap-2.0.0rc4/ligo/skymap/plot/pp.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/ligo/skymap/plot/tests/baseline/test_allsky_axes_astro-degrees-aitoff.png` & `ligo.skymap-2.0.0rc4/ligo/skymap/plot/tests/baseline/test_allsky_axes_astro-degrees-aitoff.png`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/ligo/skymap/plot/tests/baseline/test_allsky_axes_astro-degrees-mollweide.png` & `ligo.skymap-2.0.0rc4/ligo/skymap/plot/tests/baseline/test_allsky_axes_astro-degrees-mollweide.png`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/ligo/skymap/plot/tests/baseline/test_allsky_axes_astro-hours-aitoff.png` & `ligo.skymap-2.0.0rc4/ligo/skymap/plot/tests/baseline/test_allsky_axes_astro-hours-aitoff.png`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/ligo/skymap/plot/tests/baseline/test_allsky_axes_astro-hours-mollweide.png` & `ligo.skymap-2.0.0rc4/ligo/skymap/plot/tests/baseline/test_allsky_axes_astro-hours-mollweide.png`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/ligo/skymap/plot/tests/baseline/test_allsky_axes_galactic-degrees-aitoff.png` & `ligo.skymap-2.0.0rc4/ligo/skymap/plot/tests/baseline/test_allsky_axes_galactic-degrees-aitoff.png`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/ligo/skymap/plot/tests/baseline/test_allsky_axes_galactic-degrees-mollweide.png` & `ligo.skymap-2.0.0rc4/ligo/skymap/plot/tests/baseline/test_allsky_axes_galactic-degrees-mollweide.png`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/ligo/skymap/plot/tests/baseline/test_allsky_axes_galactic-hours-aitoff.png` & `ligo.skymap-2.0.0rc4/ligo/skymap/plot/tests/baseline/test_allsky_axes_galactic-hours-aitoff.png`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/ligo/skymap/plot/tests/baseline/test_allsky_axes_galactic-hours-mollweide.png` & `ligo.skymap-2.0.0rc4/ligo/skymap/plot/tests/baseline/test_allsky_axes_galactic-hours-mollweide.png`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/ligo/skymap/plot/tests/baseline/test_allsky_axes_geo-degrees-aitoff.png` & `ligo.skymap-2.0.0rc4/ligo/skymap/plot/tests/baseline/test_allsky_axes_geo-degrees-aitoff.png`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/ligo/skymap/plot/tests/baseline/test_allsky_axes_geo-degrees-mollweide.png` & `ligo.skymap-2.0.0rc4/ligo/skymap/plot/tests/baseline/test_allsky_axes_geo-degrees-mollweide.png`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/ligo/skymap/plot/tests/baseline/test_allsky_axes_geo-hours-aitoff.png` & `ligo.skymap-2.0.0rc4/ligo/skymap/plot/tests/baseline/test_allsky_axes_geo-hours-aitoff.png`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/ligo/skymap/plot/tests/baseline/test_allsky_axes_geo-hours-mollweide.png` & `ligo.skymap-2.0.0rc4/ligo/skymap/plot/tests/baseline/test_allsky_axes_geo-hours-mollweide.png`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/ligo/skymap/plot/tests/baseline/test_allsky_obstime.png` & `ligo.skymap-2.0.0rc4/ligo/skymap/plot/tests/baseline/test_allsky_obstime.png`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/ligo/skymap/plot/tests/baseline/test_center_projections_197.45d -23.38d-aitoff.png` & `ligo.skymap-2.0.0rc4/ligo/skymap/plot/tests/baseline/test_center_projections_197.45d -23.38d-aitoff.png`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/ligo/skymap/plot/tests/baseline/test_center_projections_197.45d -23.38d-mollweide.png` & `ligo.skymap-2.0.0rc4/ligo/skymap/plot/tests/baseline/test_center_projections_197.45d -23.38d-mollweide.png`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/ligo/skymap/plot/tests/baseline/test_center_projections_None-aitoff.png` & `ligo.skymap-2.0.0rc4/ligo/skymap/plot/tests/baseline/test_center_projections_None-aitoff.png`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/ligo/skymap/plot/tests/baseline/test_center_projections_None-mollweide.png` & `ligo.skymap-2.0.0rc4/ligo/skymap/plot/tests/baseline/test_center_projections_None-mollweide.png`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/ligo/skymap/plot/tests/baseline/test_globe_axes.png` & `ligo.skymap-2.0.0rc4/ligo/skymap/plot/tests/baseline/test_globe_axes.png`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/ligo/skymap/plot/tests/baseline/test_pp_plot_default.png` & `ligo.skymap-2.0.0rc4/ligo/skymap/plot/tests/baseline/test_pp_plot_default.png`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/ligo/skymap/plot/tests/baseline/test_pp_plot_lines.png` & `ligo.skymap-2.0.0rc4/ligo/skymap/plot/tests/baseline/test_pp_plot_lines.png`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/ligo/skymap/plot/tests/baseline/test_pp_plot_steps.png` & `ligo.skymap-2.0.0rc4/ligo/skymap/plot/tests/baseline/test_pp_plot_steps.png`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/ligo/skymap/plot/tests/baseline/test_reticle.png` & `ligo.skymap-2.0.0rc4/ligo/skymap/plot/tests/baseline/test_reticle.png`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/ligo/skymap/plot/tests/baseline/test_zoom_axes.png` & `ligo.skymap-2.0.0rc4/ligo/skymap/plot/tests/baseline/test_zoom_axes.png`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/ligo/skymap/plot/tests/test_plot.py` & `ligo.skymap-2.0.0rc4/ligo/skymap/plot/tests/test_plot.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 matplotlib.use('agg')
 from astropy import units as u  # noqa: E402
 import numpy as np  # noqa: E402
 import healpy as hp  # noqa: E402
 import matplotlib.pyplot as plt  # noqa: E402
 import pytest  # noqa: E402
 
+from ..bayes_factor import plot_bayes_factor  # noqa: E402
 from ..marker import reticle  # noqa: E402
 
 skip_if_macos_arm64 = pytest.mark.skipif(
     platform.system() == 'Darwin' and platform.machine() == 'arm64',
     reason='Tick labels vary on macOS arm64')
 
 
@@ -175,7 +176,13 @@
 @pytest.mark.mpl_image_compare(remove_text=True, tolerance=1.5)
 def test_center_projections(rcparams, proj, cent):
     fig = plt.figure(figsize=(4, 4))
     ax = fig.add_axes(111, projection=f'astro {proj}',
                       center=cent)
     ax.grid()
     return fig
+
+
+@pytest.mark.mpl_image_compare(tolerance=1.5)
+def test_plot_bayes_factor():
+    fig, ax = plot_bayes_factor(6.3, title='BAYESTAR is awesome')
+    return fig
```

### Comparing `ligo.skymap-2.0.0rc3/ligo/skymap/plot/util.py` & `ligo.skymap-2.0.0rc4/ligo/skymap/plot/util.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/ligo/skymap/postprocess/contour.py` & `ligo.skymap-2.0.0rc4/ligo/skymap/postprocess/contour.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/ligo/skymap/postprocess/cosmology.py` & `ligo.skymap-2.0.0rc4/ligo/skymap/postprocess/cosmology.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (C) 2013-2023  Leo Singer, Rainer Corley
+# Copyright (C) 2013-2024  Leo Singer, Rainer Corley
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
```

### Comparing `ligo.skymap-2.0.0rc3/ligo/skymap/postprocess/crossmatch.py` & `ligo.skymap-2.0.0rc4/ligo/skymap/postprocess/crossmatch.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/ligo/skymap/postprocess/ellipse.py` & `ligo.skymap-2.0.0rc4/ligo/skymap/postprocess/ellipse.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/ligo/skymap/postprocess/tests/test_cosmology.py` & `ligo.skymap-2.0.0rc4/ligo/skymap/postprocess/tests/test_cosmology.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/ligo/skymap/postprocess/tests/test_crossmatch.py` & `ligo.skymap-2.0.0rc4/ligo/skymap/postprocess/tests/test_crossmatch.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/ligo/skymap/postprocess/util.py` & `ligo.skymap-2.0.0rc4/ligo/skymap/postprocess/util.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/ligo/skymap/tests/plugins/omp.py` & `ligo.skymap-2.0.0rc4/ligo/skymap/tests/plugins/omp.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/ligo/skymap/tests/test_moc.py` & `ligo.skymap-2.0.0rc4/ligo/skymap/tests/test_moc.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/ligo/skymap/tool/__init__.py` & `ligo.skymap-2.0.0rc4/ligo/skymap/tool/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (C) 2013-2023  Leo Singer
+# Copyright (C) 2013-2024  Leo Singer
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
```

### Comparing `ligo.skymap-2.0.0rc3/ligo/skymap/tool/bayestar_inject.py` & `ligo.skymap-2.0.0rc4/ligo/skymap/tool/bayestar_inject.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/ligo/skymap/tool/bayestar_localize_coincs.py` & `ligo.skymap-2.0.0rc4/ligo/skymap/tool/bayestar_localize_coincs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (C) 2013-2023  Leo Singer
+# Copyright (C) 2013-2024  Leo Singer
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -90,15 +90,14 @@
     # BAYESTAR imports.
     from .. import omp
     from ..io import fits, events
     from ..bayestar import localize
 
     # Other imports.
     import os
-    from collections import OrderedDict
     import subprocess
     import sys
 
     log.info('Using %d OpenMP thread(s)', omp.num_threads)
 
     # Read coinc file.
     log.info(
@@ -140,16 +139,15 @@
             print('arguments = "',
                   *(arg for arg in sys.argv if arg != '--condor-submit'),
                   '--coinc-event-id $(cid)"', file=f)
             print('queue cid in', *event_source, file=f)
         sys.exit(proc.returncode)
 
     if opts.coinc_event_id:
-        event_source = OrderedDict(
-            (key, event_source[key]) for key in opts.coinc_event_id)
+        event_source = {key: event_source[key] for key in opts.coinc_event_id}
 
     count_sky_maps_failed = 0
 
     # Loop over all sngl_inspiral <-> sngl_inspiral coincs.
     for coinc_event_id, event in event_source.items():
         # Loop over sky localization methods
         log.info('%d:computing sky map', coinc_event_id)
```

### Comparing `ligo.skymap-2.0.0rc3/ligo/skymap/tool/bayestar_localize_lvalert.py` & `ligo.skymap-2.0.0rc4/ligo/skymap/tool/bayestar_localize_lvalert.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/ligo/skymap/tool/bayestar_mcmc.py` & `ligo.skymap-2.0.0rc4/ligo/skymap/tool/bayestar_mcmc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (C) 2013-2023  Leo Singer
+# Copyright (C) 2013-2024  Leo Singer
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -78,15 +78,14 @@
     from ..io import events, hdf5
     from ..bayestar import condition, condition_prior, ez_emcee, log_post
 
     # Other imports.
     from astropy.table import Table
     import numpy as np
     import os
-    from collections import OrderedDict
     import subprocess
     import sys
 
     import lal
 
     # Read coinc file.
     log.info(
@@ -124,16 +123,15 @@
             print('arguments = "',
                   *(arg for arg in sys.argv if arg != '--condor-submit'),
                   '--coinc-event-id $(cid)"', file=f)
             print('queue cid in', *event_source, file=f)
         sys.exit(proc.returncode)
 
     if opts.coinc_event_id:
-        event_source = OrderedDict(
-            (key, event_source[key]) for key in opts.coinc_event_id)
+        event_source = {key: event_source[key] for key in opts.coinc_event_id}
 
     # Loop over all sngl_inspiral <-> sngl_inspiral coincs.
     for int_coinc_event_id, event in event_source.items():
         coinc_event_id = 'coinc_event:coinc_event_id:{}'.format(
             int_coinc_event_id)
 
         log.info('%s:preparing', coinc_event_id)
```

### Comparing `ligo.skymap-2.0.0rc3/ligo/skymap/tool/bayestar_realize_coincs.py` & `ligo.skymap-2.0.0rc4/ligo/skymap/tool/bayestar_realize_coincs.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/ligo/skymap/tool/bayestar_sample_model_psd.py` & `ligo.skymap-2.0.0rc4/ligo/skymap/tool/bayestar_sample_model_psd.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/ligo/skymap/tool/ligo_skymap_combine.py` & `ligo.skymap-2.0.0rc4/ligo/skymap/tool/ligo_skymap_combine.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/ligo/skymap/tool/ligo_skymap_constellations.py` & `ligo.skymap-2.0.0rc4/ligo/skymap/tool/ligo_skymap_constellations.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/ligo/skymap/tool/ligo_skymap_contour.py` & `ligo.skymap-2.0.0rc4/ligo/skymap/tool/ligo_skymap_contour.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/ligo/skymap/tool/ligo_skymap_contour_moc.py` & `ligo.skymap-2.0.0rc4/ligo/skymap/tool/ligo_skymap_contour_moc.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/ligo/skymap/tool/ligo_skymap_flatten.py` & `ligo.skymap-2.0.0rc4/ligo/skymap/tool/ligo_skymap_flatten.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/ligo/skymap/tool/ligo_skymap_from_samples.py` & `ligo.skymap-2.0.0rc4/ligo/skymap/tool/ligo_skymap_from_samples.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/ligo/skymap/tool/ligo_skymap_plot.py` & `ligo.skymap-2.0.0rc4/ligo/skymap/tool/ligo_skymap_plot.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/ligo/skymap/tool/ligo_skymap_plot_airmass.py` & `ligo.skymap-2.0.0rc4/ligo/skymap/tool/ligo_skymap_plot_airmass.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/ligo/skymap/tool/ligo_skymap_plot_coherence.py` & `ligo.skymap-2.0.0rc4/ligo/skymap/tool/ligo_skymap_plot_coherence.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/ligo/skymap/tool/ligo_skymap_plot_observability.py` & `ligo.skymap-2.0.0rc4/ligo/skymap/tool/ligo_skymap_plot_observability.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/ligo/skymap/tool/ligo_skymap_plot_pp_samples.py` & `ligo.skymap-2.0.0rc4/ligo/skymap/tool/ligo_skymap_plot_pp_samples.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/ligo/skymap/tool/ligo_skymap_plot_stats.py` & `ligo.skymap-2.0.0rc4/ligo/skymap/tool/ligo_skymap_plot_stats.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/ligo/skymap/tool/ligo_skymap_plot_volume.py` & `ligo.skymap-2.0.0rc4/ligo/skymap/tool/ligo_skymap_plot_volume.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (C) 2015-2020  Leo Singer
+# Copyright (C) 2015-2024  Leo Singer
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
```

### Comparing `ligo.skymap-2.0.0rc3/ligo/skymap/tool/ligo_skymap_stats.py` & `ligo.skymap-2.0.0rc4/ligo/skymap/tool/ligo_skymap_stats.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/ligo/skymap/tool/ligo_skymap_unflatten.py` & `ligo.skymap-2.0.0rc4/ligo/skymap/tool/ligo_skymap_unflatten.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/ligo/skymap/tool/matplotlib.py` & `ligo.skymap-2.0.0rc4/ligo/skymap/tool/matplotlib.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/ligo/skymap/tool/tests/__init__.py` & `ligo.skymap-2.0.0rc4/ligo/skymap/tool/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/ligo/skymap/tool/tests/test_bayestar.py` & `ligo.skymap-2.0.0rc4/ligo/skymap/tool/tests/test_bayestar.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/ligo/skymap/tool/tests/test_bayestar_inject.py` & `ligo.skymap-2.0.0rc4/ligo/skymap/tool/tests/test_bayestar_inject.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/ligo/skymap/tool/tests/test_combine.py` & `ligo.skymap-2.0.0rc4/ligo/skymap/tool/tests/test_combine.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/ligo/skymap/tool/tests/test_flatten.py` & `ligo.skymap-2.0.0rc4/ligo/skymap/tool/tests/test_flatten.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/ligo/skymap/tool/tests/test_from_samples.py` & `ligo.skymap-2.0.0rc4/ligo/skymap/tool/tests/test_from_samples.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/ligo/skymap/tool/tests/test_help.py` & `ligo.skymap-2.0.0rc4/ligo/skymap/tool/tests/test_help.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/ligo/skymap/tool/tests/test_plot.py` & `ligo.skymap-2.0.0rc4/ligo/skymap/tool/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/ligo/skymap/tool/tests/test_plot_stats.py` & `ligo.skymap-2.0.0rc4/ligo/skymap/tool/tests/test_plot_stats.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/ligo/skymap/util/file.py` & `ligo.skymap-2.0.0rc4/ligo/skymap/util/file.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/ligo/skymap/util/ilwd.py` & `ligo.skymap-2.0.0rc4/ligo/skymap/util/ilwd.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/ligo/skymap/util/math.py` & `ligo.skymap-2.0.0rc4/ligo/skymap/util/math.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/ligo/skymap/util/numpy.py` & `ligo.skymap-2.0.0rc4/ligo/skymap/util/numpy.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (C) 2018-2019  Leo Singer
+# Copyright (C) 2018-2014  Leo Singer
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -12,25 +12,36 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 #
 import functools
 import numpy as np
+from numpy.core.umath import _add_newdoc_ufunc
 
 __all__ = ('add_newdoc_ufunc', 'require_contiguous_aligned')
 
 
 def add_newdoc_ufunc(func, doc):  # pragma: no cover
-    """The function `np.lib.add_newdoc_ufunc` can only change a ufunc's
-    docstring if it is `NULL`. This workaround avoids an exception when the
-    user tries to `reload()` this module.
+    """Set the docstring for a Numpy ufunc.
+
+    The function :func:`numpy.core.umath._add_newdoc_ufunc` can only change a
+    ufunc's docstring if it is `NULL`. This workaround avoids an exception when
+    the user tries to `reload()` this module.
+
+    Notes
+    -----
+    :func:`numpy.core.umath._add_newdoc_ufunc` is not part of Numpy's public
+    API, but according to upstream developers it is unlikely to go away any
+    time soon.
+
+    See https://github.com/numpy/numpy/issues/26233.
     """
     try:
-        np.lib.add_newdoc_ufunc(func, doc)
+        _add_newdoc_ufunc(func, doc)
     except ValueError as e:
         msg = 'Cannot change docstring of ufunc with non-NULL docstring'
         if e.args[0] == msg:
             pass
 
 
 def require_contiguous_aligned(func):
```

### Comparing `ligo.skymap-2.0.0rc3/ligo/skymap/util/progress.py` & `ligo.skymap-2.0.0rc4/ligo/skymap/util/progress.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/ligo/skymap/util/sqlite.py` & `ligo.skymap-2.0.0rc4/ligo/skymap/util/sqlite.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/ligo/skymap/util/stopwatch.py` & `ligo.skymap-2.0.0rc4/ligo/skymap/util/stopwatch.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/ligo.skymap.egg-info/PKG-INFO` & `ligo.skymap-2.0.0rc4/ligo.skymap.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ligo.skymap
-Version: 2.0.0rc3
+Version: 2.0.0rc4
 Summary: Tools for reading, writing, manipulating, and making LIGO and Virgo sky maps
 Home-page: https://lscsoft.docs.ligo.org/ligo.skymap/
 Author: Leo Singer
 Author-email: leo.singer@ligo.org
 License: GNU GPL v3+
 Project-URL: Bug Tracker, https://git.ligo.org/lscsoft/ligo.skymap/issues
 Project-URL: Change Log, https://lscsoft.docs.ligo.org/ligo.skymap/changes.html
@@ -19,14 +19,15 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: licenses/LICENSE.rst
 Requires-Dist: astroplan>=0.7
 Requires-Dist: astropy>=5.0
```

### Comparing `ligo.skymap-2.0.0rc3/ligo.skymap.egg-info/SOURCES.txt` & `ligo.skymap-2.0.0rc4/ligo.skymap.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -169,14 +169,15 @@
 ligo/skymap/plot/tests/baseline/test_allsky_axes_geo-hours-mollweide.png
 ligo/skymap/plot/tests/baseline/test_allsky_obstime.png
 ligo/skymap/plot/tests/baseline/test_center_projections_197.45d -23.38d-aitoff.png
 ligo/skymap/plot/tests/baseline/test_center_projections_197.45d -23.38d-mollweide.png
 ligo/skymap/plot/tests/baseline/test_center_projections_None-aitoff.png
 ligo/skymap/plot/tests/baseline/test_center_projections_None-mollweide.png
 ligo/skymap/plot/tests/baseline/test_globe_axes.png
+ligo/skymap/plot/tests/baseline/test_plot_bayes_factor.png
 ligo/skymap/plot/tests/baseline/test_pp_plot_default.png
 ligo/skymap/plot/tests/baseline/test_pp_plot_lines.png
 ligo/skymap/plot/tests/baseline/test_pp_plot_steps.png
 ligo/skymap/plot/tests/baseline/test_reticle.png
 ligo/skymap/plot/tests/baseline/test_zoom_axes.png
 ligo/skymap/postprocess/__init__.py
 ligo/skymap/postprocess/contour.py
```

### Comparing `ligo.skymap-2.0.0rc3/ligo.skymap.egg-info/entry_points.txt` & `ligo.skymap-2.0.0rc4/ligo.skymap.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/setup.cfg` & `ligo.skymap-2.0.0rc4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 	Operating System :: POSIX :: Linux
 	Operating System :: Unix
 	Programming Language :: C
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
+	Programming Language :: Python :: 3.12
 	Topic :: Scientific/Engineering :: Astronomy
 	Topic :: Scientific/Engineering :: Physics
 project_urls = 
 	Bug Tracker = https://git.ligo.org/lscsoft/ligo.skymap/issues
 	Change Log = https://lscsoft.docs.ligo.org/ligo.skymap/changes.html
 	Documentation = https://lscsoft.docs.ligo.org/ligo.skymap
 	GitHub = https://github.com/lpsinger/ligo.skymap
```

### Comparing `ligo.skymap-2.0.0rc3/setup.py` & `ligo.skymap-2.0.0rc4/setup.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/src/bayestar_cosmology.h` & `ligo.skymap-2.0.0rc4/src/bayestar_cosmology.h`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/src/bayestar_cosmology.py` & `ligo.skymap-2.0.0rc4/src/bayestar_cosmology.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (C) 2017-2019  Leo Singer
+# Copyright (C) 2017-2014  Leo Singer
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
```

### Comparing `ligo.skymap-2.0.0rc3/src/bayestar_distance.c` & `ligo.skymap-2.0.0rc4/src/bayestar_distance.c`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/src/bayestar_distance.h` & `ligo.skymap-2.0.0rc4/src/bayestar_distance.h`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/src/bayestar_moc.c` & `ligo.skymap-2.0.0rc4/src/bayestar_moc.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /*
- * Copyright (C) 2017-2019  Leo Singer
+ * Copyright (C) 2017-2024  Leo Singer
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
  *
  * This program is distributed in the hope that it will be useful,
```

### Comparing `ligo.skymap-2.0.0rc3/src/bayestar_moc.h` & `ligo.skymap-2.0.0rc4/src/bayestar_moc.h`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/src/bayestar_sky_map.c` & `ligo.skymap-2.0.0rc4/src/bayestar_sky_map.c`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 **************  / __  / /| |\  / __/  \__ \ / / / /| | / /_/ /  ****************
 *************  / /_/ / ___ |/ / /___ ___/ // / / ___ |/ _, _/  *****************
 ************  /_____/_/  |_/_/_____//____//_/ /_/  |_/_/ |_|  ******************
 */
 
 
 /*
- * Copyright (C) 2013-2023  Leo Singer
+ * Copyright (C) 2013-2024  Leo Singer
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
  *
  * This program is distributed in the hope that it will be useful,
```

### Comparing `ligo.skymap-2.0.0rc3/src/bayestar_sky_map.h` & `ligo.skymap-2.0.0rc4/src/bayestar_sky_map.h`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 **************  / __  / /| |\  / __/  \__ \ / / / /| | / /_/ /  ****************
 *************  / /_/ / ___ |/ / /___ ___/ // / / ___ |/ _, _/  *****************
 ************  /_____/_/  |_/_/_____//____//_/ /_/  |_/_/ |_|  ******************
 */
 
 
 /*
- * Copyright (C) 2013-2020  Leo Singer
+ * Copyright (C) 2013-2024  Leo Singer
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
  *
  * This program is distributed in the hope that it will be useful,
```

### Comparing `ligo.skymap-2.0.0rc3/src/core.c` & `ligo.skymap-2.0.0rc4/src/core.c`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /*
- * Copyright (C) 2013-2023  Leo Singer
+ * Copyright (C) 2013-2024  Leo Singer
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
  *
  * This program is distributed in the hope that it will be useful,
@@ -14,14 +14,15 @@
  * You should have received a copy of the GNU General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
 #ifdef _OPENMP
 #include <omp.h>
 #endif
+#include <assert.h>
 #include <limits.h>
 #include <stddef.h>
 #include <chealpix.h>
 #include <gsl/gsl_errno.h>
 #include <gsl/gsl_nan.h>
 #include <Python.h>
 #include <numpy/arrayobject.h>
@@ -102,16 +103,16 @@
 ) {
     gsl_error_handler_t *old_handler = gsl_set_error_handler_off();
     const npy_intp n = dimensions[0];
 
     #pragma omp parallel for
     for (npy_intp i = 0; i < n; i ++)
     {
-        /* Alignment of the ufunc arguments is enforced in Python by the
-         * require_contiguous_aligned wrapper function. */
+        /* Alignment of the ufunc arguments is enforced by the ufunc API. See
+         * https://numpy.org/doc/stable/user/basics.ufuncs.html#use-of-internal-buffers. */
         WARNINGS_PUSH
         WARNINGS_IGNORE_CAST_ALIGN
         *(double *) &args[4][i * steps[4]] = bayestar_distance_conditional_pdf(
         *(double *) &args[0][i * steps[0]],
         *(double *) &args[1][i * steps[1]],
         *(double *) &args[2][i * steps[2]],
         *(double *) &args[3][i * steps[3]]);
@@ -130,16 +131,16 @@
 ) {
     gsl_error_handler_t *old_handler = gsl_set_error_handler_off();
     const npy_intp n = dimensions[0];
 
     #pragma omp parallel for
     for (npy_intp i = 0; i < n; i ++)
     {
-        /* Alignment of the ufunc arguments is enforced in Python by the
-         * require_contiguous_aligned wrapper function. */
+        /* Alignment of the ufunc arguments is enforced by the ufunc API. See
+         * https://numpy.org/doc/stable/user/basics.ufuncs.html#use-of-internal-buffers. */
         WARNINGS_PUSH
         WARNINGS_IGNORE_CAST_ALIGN
         *(double *) &args[4][i * steps[4]] = bayestar_distance_conditional_cdf(
         *(double *) &args[0][i * steps[0]],
         *(double *) &args[1][i * steps[1]],
         *(double *) &args[2][i * steps[2]],
         *(double *) &args[3][i * steps[3]]);
@@ -158,16 +159,16 @@
 ) {
     gsl_error_handler_t *old_handler = gsl_set_error_handler_off();
     const npy_intp n = dimensions[0];
 
     #pragma omp parallel for
     for (npy_intp i = 0; i < n; i ++)
     {
-        /* Alignment of the ufunc arguments is enforced in Python by the
-         * require_contiguous_aligned wrapper function. */
+        /* Alignment of the ufunc arguments is enforced by the ufunc API. See
+         * https://numpy.org/doc/stable/user/basics.ufuncs.html#use-of-internal-buffers. */
         WARNINGS_PUSH
         WARNINGS_IGNORE_CAST_ALIGN
         *(double *) &args[4][i * steps[4]] = bayestar_distance_conditional_ppf(
         *(double *) &args[0][i * steps[0]],
         *(double *) &args[1][i * steps[1]],
         *(double *) &args[2][i * steps[2]],
         *(double *) &args[3][i * steps[3]]);
@@ -186,16 +187,16 @@
 ) {
     gsl_error_handler_t *old_handler = gsl_set_error_handler_off();
     const npy_intp n = dimensions[0];
 
     #pragma omp parallel for
     for (npy_intp i = 0; i < n; i ++)
     {
-        /* Alignment of the ufunc arguments is enforced in Python by the
-         * require_contiguous_aligned wrapper function. */
+        /* Alignment of the ufunc arguments is enforced by the ufunc API. See
+         * https://numpy.org/doc/stable/user/basics.ufuncs.html#use-of-internal-buffers. */
         WARNINGS_PUSH
         WARNINGS_IGNORE_CAST_ALIGN
         bayestar_distance_moments_to_parameters(
             *(double *) &args[0][i * steps[0]],
             *(double *) &args[1][i * steps[1]],
              (double *) &args[2][i * steps[2]],
              (double *) &args[3][i * steps[3]],
@@ -215,16 +216,16 @@
 ) {
     gsl_error_handler_t *old_handler = gsl_set_error_handler_off();
     const npy_intp n = dimensions[0];
 
     #pragma omp parallel for
     for (npy_intp i = 0; i < n; i ++)
     {
-        /* Alignment of the ufunc arguments is enforced in Python by the
-         * require_contiguous_aligned wrapper function. */
+        /* Alignment of the ufunc arguments is enforced by the ufunc API. See
+         * https://numpy.org/doc/stable/user/basics.ufuncs.html#use-of-internal-buffers. */
         WARNINGS_PUSH
         WARNINGS_IGNORE_CAST_ALIGN
         bayestar_distance_parameters_to_moments(
             *(double *) &args[0][i * steps[0]],
             *(double *) &args[1][i * steps[1]],
              (double *) &args[2][i * steps[2]],
              (double *) &args[3][i * steps[3]],
@@ -238,26 +239,38 @@
 
 static void volume_render_loop(
     char **args,
     const npy_intp *dimensions,
     const npy_intp *steps,
     void *NPY_UNUSED(data)
 ) {
+    /* Check core dimensions. */
+    assert(dimensions[1] == 3);
+    /* The arguments with core dimensions must be C contiguous.
+     * This is enforced in Python by the require_contiguous_aligned wrapper.
+     * This ufunc loop must NOT be called without that wrapper. */
+    assert(steps[12] == sizeof(double) * 3);
+    assert(steps[13] == sizeof(double));
+    assert(steps[14] == sizeof(double));
+    assert(steps[15] == sizeof(double));
+    assert(steps[16] == sizeof(double));
+    assert(steps[17] == sizeof(double));
+
     gsl_error_handler_t *old_handler = gsl_set_error_handler_off();
     const npy_intp n = dimensions[0];
     const long long nside = npix2nside64(dimensions[2]);
 
     OMP_BEGIN_INTERRUPTIBLE
     #pragma omp parallel for
     for (npy_intp i = 0; i < n; i ++)
     {
         if (OMP_WAS_INTERRUPTED)
             OMP_EXIT_LOOP_EARLY
-        /* Alignment of the ufunc arguments is enforced in Python by the
-         * require_contiguous_aligned wrapper function. */
+        /* Alignment of the ufunc arguments is enforced by the ufunc API. See
+         * https://numpy.org/doc/stable/user/basics.ufuncs.html#use-of-internal-buffers. */
         WARNINGS_PUSH
         WARNINGS_IGNORE_CAST_ALIGN
         *(double *) &args[11][i * steps[11]] = bayestar_volume_render(
             *(double *)   &args[0][i * steps[0]],
             *(double *)   &args[1][i * steps[1]],
             *(double *)   &args[2][i * steps[2]],
             *(int *)      &args[3][i * steps[3]],
@@ -279,30 +292,31 @@
 
 static void marginal_pdf_loop(
     char **args,
     const npy_intp *dimensions,
     const npy_intp *steps,
     void *NPY_UNUSED(data)
 ) {
-    /* Assert that array arguments are stored contiguously */
-    if (steps[6] != sizeof(double))
-    {
-        PyErr_SetString(PyExc_RuntimeError, "Invalid dimension");
-        return;
-    }
+    /* The arguments with core dimensions must be C contiguous.
+     * This is enforced in Python by the require_contiguous_aligned wrapper.
+     * This ufunc loop must NOT be called without that wrapper. */
+    assert(steps[6] == sizeof(double));
+    assert(steps[7] == sizeof(double));
+    assert(steps[8] == sizeof(double));
+    assert(steps[9] == sizeof(double));
 
     gsl_error_handler_t *old_handler = gsl_set_error_handler_off();
     const npy_intp n = dimensions[0];
     const npy_intp npix = dimensions[1];
 
     #pragma omp parallel for
     for (npy_intp i = 0; i < n; i ++)
     {
-        /* Alignment of the ufunc arguments is enforced in Python by the
-         * require_contiguous_aligned wrapper function. */
+        /* Alignment of the ufunc arguments is enforced by the ufunc API. See
+         * https://numpy.org/doc/stable/user/basics.ufuncs.html#use-of-internal-buffers. */
         WARNINGS_PUSH
         WARNINGS_IGNORE_CAST_ALIGN
         *(double *) &args[5][i * steps[5]] =
             bayestar_distance_marginal_pdf(
             *(double *) &args[0][i * steps[0]], npix,
              (double *) &args[1][i * steps[1]],
              (double *) &args[2][i * steps[2]],
@@ -317,30 +331,31 @@
 
 static void marginal_cdf_loop(
     char **args,
     const npy_intp *dimensions,
     const npy_intp *steps,
     void *NPY_UNUSED(data)
 ) {
-    /* Assert that array arguments are stored contiguously */
-    if (steps[6] != sizeof(double))
-    {
-        PyErr_SetString(PyExc_RuntimeError, "Invalid dimension");
-        return;
-    }
+    /* The arguments with core dimensions must be C contiguous.
+     * This is enforced in Python by the require_contiguous_aligned wrapper.
+     * This ufunc loop must NOT be called without that wrapper. */
+    assert(steps[6] == sizeof(double));
+    assert(steps[7] == sizeof(double));
+    assert(steps[8] == sizeof(double));
+    assert(steps[9] == sizeof(double));
 
     gsl_error_handler_t *old_handler = gsl_set_error_handler_off();
     const npy_intp n = dimensions[0];
     const npy_intp npix = dimensions[1];
 
     #pragma omp parallel for
     for (npy_intp i = 0; i < n; i ++)
     {
-        /* Alignment of the ufunc arguments is enforced in Python by the
-         * require_contiguous_aligned wrapper function. */
+        /* Alignment of the ufunc arguments is enforced by the ufunc API. See
+         * https://numpy.org/doc/stable/user/basics.ufuncs.html#use-of-internal-buffers. */
         WARNINGS_PUSH
         WARNINGS_IGNORE_CAST_ALIGN
         *(double *) &args[5][i * steps[5]] =
             bayestar_distance_marginal_cdf(
             *(double *) &args[0][i * steps[0]], npix,
              (double *) &args[1][i * steps[1]],
              (double *) &args[2][i * steps[2]],
@@ -355,30 +370,31 @@
 
 static void marginal_ppf_loop(
     char **args,
     const npy_intp *dimensions,
     const npy_intp *steps,
     void *NPY_UNUSED(data)
 ) {
-    /* Assert that array arguments are stored contiguously */
-    if (steps[6] != sizeof(double))
-    {
-        PyErr_SetString(PyExc_RuntimeError, "Invalid dimension");
-        return;
-    }
+    /* The arguments with core dimensions must be C contiguous.
+     * This is enforced in Python by the require_contiguous_aligned wrapper.
+     * This ufunc loop must NOT be called without that wrapper. */
+    assert(steps[6] == sizeof(double));
+    assert(steps[7] == sizeof(double));
+    assert(steps[8] == sizeof(double));
+    assert(steps[9] == sizeof(double));
 
     gsl_error_handler_t *old_handler = gsl_set_error_handler_off();
     const npy_intp n = dimensions[0];
     const npy_intp npix = dimensions[1];
 
     #pragma omp parallel for
     for (npy_intp i = 0; i < n; i ++)
     {
-        /* Alignment of the ufunc arguments is enforced in Python by the
-         * require_contiguous_aligned wrapper function. */
+        /* Alignment of the ufunc arguments is enforced by the ufunc API. See
+         * https://numpy.org/doc/stable/user/basics.ufuncs.html#use-of-internal-buffers. */
         WARNINGS_PUSH
         WARNINGS_IGNORE_CAST_ALIGN
         *(double *) &args[5][i * steps[5]] =
             bayestar_distance_marginal_ppf(
             *(double *) &args[0][i * steps[0]], npix,
              (double *) &args[1][i * steps[1]],
              (double *) &args[2][i * steps[2]],
@@ -424,29 +440,29 @@
     PyObject *new_fields = PyDict_New();
     PyObject *capsule = NULL;
     PyArrayObject *ret = NULL;
 
     if (!arr || !uniq_key || !new_fields)
         goto done;
 
-    PyObject *fields = PyArray_DESCR(arr)->fields;
+    PyObject *fields = PyDataType_FIELDS(PyArray_DESCR(arr));
     if (!fields)
     {
         PyErr_SetString(PyExc_ValueError, "expected record array");
         goto done;
     }
 
     PyObject *uniq_field = PyDict_GetItem(fields, uniq_key);
     if (!uniq_field)
     {
         PyErr_SetString(PyExc_ValueError, "array does not have UNIQ column");
         goto done;
     }
 
-    PyObject *uniq_dtype;
+    PyArray_Descr *uniq_dtype;
     int uniq_offset;
     if (!PyArg_ParseTuple(uniq_field, "Oi", &uniq_dtype, &uniq_offset))
         return NULL;
 
     if (!PyArray_DescrCheck(uniq_dtype))
     {
         PyErr_SetString(PyExc_ValueError, "not a dtype");
@@ -463,15 +479,15 @@
     if (uniq_offset != 0)
     {
         PyErr_SetString(PyExc_ValueError, "'uniq' field must be at offset 0");
         goto done;
     }
 
     const void *pixels = PyArray_DATA(arr);
-    const size_t offset = ((PyArray_Descr *) uniq_dtype)->elsize;
+    const size_t offset = PyDataType_ELSIZE(uniq_dtype);
     const size_t itemsize = PyArray_ITEMSIZE(arr) - offset;
     const size_t len = PyArray_SIZE(arr);
     size_t npix;
 
     PyObject *key, *value;
     Py_ssize_t pos = 0;
 
@@ -539,16 +555,16 @@
 static void nest2uniq_loop(
     char **args, const npy_intp *dimensions, const npy_intp *steps, void *NPY_UNUSED(data))
 {
     const npy_intp n = dimensions[0];
 
     for (npy_intp i = 0; i < n; i ++)
     {
-        /* Alignment of the ufunc arguments is enforced in Python by the
-         * require_contiguous_aligned wrapper function. */
+        /* Alignment of the ufunc arguments is enforced by the ufunc API. See
+         * https://numpy.org/doc/stable/user/basics.ufuncs.html#use-of-internal-buffers. */
         WARNINGS_PUSH
         WARNINGS_IGNORE_CAST_ALIGN
         *(int64_t *) &args[2][i * steps[2]] = nest2uniq64(
         *(int8_t *)  &args[0][i * steps[0]],
         *(int64_t *) &args[1][i * steps[1]]);
         WARNINGS_POP
     }
@@ -558,16 +574,16 @@
 static void uniq2nest_loop(
     char **args, const npy_intp *dimensions, const npy_intp *steps, void *NPY_UNUSED(data))
 {
     const npy_intp n = dimensions[0];
 
     for (npy_intp i = 0; i < n; i ++)
     {
-        /* Alignment of the ufunc arguments is enforced in Python by the
-         * require_contiguous_aligned wrapper function. */
+        /* Alignment of the ufunc arguments is enforced by the ufunc API. See
+         * https://numpy.org/doc/stable/user/basics.ufuncs.html#use-of-internal-buffers. */
         WARNINGS_PUSH
         WARNINGS_IGNORE_CAST_ALIGN
         *(int8_t *)  &args[1][i * steps[1]] = uniq2nest64(
         *(int64_t *) &args[0][i * steps[0]],
          (int64_t *) &args[2][i * steps[2]]);
         WARNINGS_POP
     }
@@ -577,16 +593,16 @@
 static void uniq2order_loop(
     char **args, const npy_intp *dimensions, const npy_intp *steps, void *NPY_UNUSED(data))
 {
     const npy_intp n = dimensions[0];
 
     for (npy_intp i = 0; i < n; i ++)
     {
-        /* Alignment of the ufunc arguments is enforced in Python by the
-         * require_contiguous_aligned wrapper function. */
+        /* Alignment of the ufunc arguments is enforced by the ufunc API. See
+         * https://numpy.org/doc/stable/user/basics.ufuncs.html#use-of-internal-buffers. */
         WARNINGS_PUSH
         WARNINGS_IGNORE_CAST_ALIGN
         *(int8_t *)  &args[1][i * steps[1]] = uniq2order64(
         *(int64_t *) &args[0][i * steps[0]]);
         WARNINGS_POP
     }
 }
@@ -595,16 +611,16 @@
 static void uniq2pixarea_loop(
     char **args, const npy_intp *dimensions, const npy_intp *steps, void *NPY_UNUSED(data))
 {
     const npy_intp n = dimensions[0];
 
     for (npy_intp i = 0; i < n; i ++)
     {
-        /* Alignment of the ufunc arguments is enforced in Python by the
-         * require_contiguous_aligned wrapper function. */
+        /* Alignment of the ufunc arguments is enforced by the ufunc API. See
+         * https://numpy.org/doc/stable/user/basics.ufuncs.html#use-of-internal-buffers. */
         WARNINGS_PUSH
         WARNINGS_IGNORE_CAST_ALIGN
         *(double *)  &args[1][i * steps[1]] = uniq2pixarea64(
         *(int64_t *) &args[0][i * steps[0]]);
         WARNINGS_POP
     }
 }
@@ -613,16 +629,16 @@
 static void uniq2ang_loop(
     char **args, const npy_intp *dimensions, const npy_intp *steps, void *NPY_UNUSED(data))
 {
     const npy_intp n = dimensions[0];
 
     for (npy_intp i = 0; i < n; i ++)
     {
-        /* Alignment of the ufunc arguments is enforced in Python by the
-         * require_contiguous_aligned wrapper function. */
+        /* Alignment of the ufunc arguments is enforced by the ufunc API. See
+         * https://numpy.org/doc/stable/user/basics.ufuncs.html#use-of-internal-buffers. */
         WARNINGS_PUSH
         WARNINGS_IGNORE_CAST_ALIGN
         uniq2ang64(
             *(int64_t *) &args[0][i * steps[0]],
              (double *)  &args[1][i * steps[1]],
              (double *)  &args[2][i * steps[2]]);
         WARNINGS_POP
@@ -883,14 +899,27 @@
 static void log_posterior_toa_phoa_snr_loop(
     char **args, const npy_intp *dimensions, const npy_intp *steps, void *NPY_UNUSED(data))
 {
     const npy_intp n = dimensions[0],
                nifos = dimensions[1],
             nsamples = dimensions[2];
 
+    /* Check core dimensions. */
+    assert(dimensions[3] == 2);
+    assert(dimensions[4] == 3);
+    /* The arguments with core dimensions must be C contiguous.
+     * This is enforced in Python by the require_contiguous_aligned wrapper.
+     * This ufunc loop must NOT be called without that wrapper. */
+    assert(steps[19] == sizeof(double));
+    assert(steps[21] == sizeof(float) * 2);
+    assert(steps[22] == sizeof(float));
+    assert(steps[24] == sizeof(float) * 3);
+    assert(steps[25] == sizeof(float));
+    assert(steps[27] == sizeof(double));
+
     gsl_error_handler_t *old_handler = gsl_set_error_handler_off();
 
     #pragma omp parallel for
     for (npy_intp i = 0; i < n; i ++)
     {
         const float (*snrs[nifos])[2];
         const float (*responses[nifos])[3];
@@ -902,16 +931,16 @@
                 &args[13][i * steps[13] + j * steps[20]];
             responses[j] = (const float (*)[3])
                 &args[14][i * steps[14] + j * steps[23]];
             locations[j] = (const double *)
                 &args[15][i * steps[15] + j * steps[26]];
         }
 
-        /* Alignment of the ufunc arguments is enforced in Python by the
-         * require_contiguous_aligned wrapper function. */
+        /* Alignment of the ufunc arguments is enforced by the ufunc API. See
+         * https://numpy.org/doc/stable/user/basics.ufuncs.html#use-of-internal-buffers. */
         WARNINGS_PUSH
         WARNINGS_IGNORE_CAST_ALIGN
         *(double *)   &args[18][i * steps[18]] = bayestar_log_posterior_toa_phoa_snr(
         *(double *)   &args[0][i * steps[0]],
         *(double *)   &args[1][i * steps[1]],
         *(double *)   &args[2][i * steps[2]],
         *(double *)   &args[3][i * steps[3]],
@@ -934,22 +963,25 @@
     gsl_set_error_handler(old_handler);
 }
 
 
 static void antenna_factor_loop(
     char **args, const npy_intp *dimensions, const npy_intp *steps, void *NPY_UNUSED(data))
 {
+    /* Check core dimensions. */
+    assert(dimensions[1] == 3);
+
     const npy_intp n = dimensions[0];
 
     for (npy_intp i = 0; i < n; i ++)
     {
         float response[3][3];
 
-        /* Alignment of the ufunc arguments is enforced in Python by the
-         * require_contiguous_aligned wrapper function. */
+        /* Alignment of the ufunc arguments is enforced by the ufunc API. See
+         * https://numpy.org/doc/stable/user/basics.ufuncs.html#use-of-internal-buffers. */
         WARNINGS_PUSH
         WARNINGS_IGNORE_CAST_ALIGN
         for (int j = 0; j < 3; j ++)
             for (int k = 0; k < 3; k ++)
                 response[j][k] = *(float *) &args[0][
                     i * steps[0] + j * steps[5] + k * steps[6]];
 
@@ -966,16 +998,16 @@
 static void signal_amplitude_model_loop(
     char **args, const npy_intp *dimensions, const npy_intp *steps, void *NPY_UNUSED(data))
 {
     const npy_intp n = dimensions[0];
 
     for (npy_intp i = 0; i < n; i ++)
     {
-        /* Alignment of the ufunc arguments is enforced in Python by the
-         * require_contiguous_aligned wrapper function. */
+        /* Alignment of the ufunc arguments is enforced by the ufunc API. See
+         * https://numpy.org/doc/stable/user/basics.ufuncs.html#use-of-internal-buffers. */
         WARNINGS_PUSH
         WARNINGS_IGNORE_CAST_ALIGN
         *(float complex *) &args[4][i * steps[4]] =
             bayestar_signal_amplitude_model(
             *(float complex *) &args[0][i * steps[0]],
             *(float complex *) &args[1][i * steps[1]],
             *(float *)         &args[2][i * steps[2]],
@@ -1088,128 +1120,123 @@
     import_array();
     import_umath();
 
     module = PyModule_Create(&moduledef);
     if (!module)
         return NULL;
 
-    /* Ignore warnings in Numpy API.
-     * FIXME: remove once https://github.com/numpy/numpy/pull/23847 is merged.
-     */
-    WARNINGS_PUSH
-    WARNINGS_IGNORE_DISCARDED_QUALIFIERS
-
     MODULE_ADD_OBJECT(
         "sky_map_descr", (PyObject *) sky_map_create_descr());
 
+    /* FIXME: don't cast away constness from _loops variables.
+     * Fix once https://github.com/numpy/numpy/pull/26228 is merged. */
+
     MODULE_ADD_OBJECT(
         "log_posterior_toa_phoa_snr", PyUFunc_FromFuncAndDataAndSignature(
-            log_posterior_toa_phoa_snr_loops, NULL,
+            (PyUFuncGenericFunction *) log_posterior_toa_phoa_snr_loops, NULL,
             log_posterior_toa_phoa_snr_types, 1, 18, 1, PyUFunc_None,
             "log_posterior_toa_phoa_snr", NULL, 0,
             "(),(),(),(),(),(),(),(),(),(),(),(),(nifos),(nifos,nsamples,2),(nifos,3,3),(nifos,3),(nifos),()->()"));
 
     MODULE_ADD_OBJECT(
         "conditional_pdf", PyUFunc_FromFuncAndData(
-            conditional_pdf_loops, NULL,
+            (PyUFuncGenericFunction *) conditional_pdf_loops, NULL,
             double_ufunc_types, 1, 4, 1, PyUFunc_None,
             "conditional_pdf", NULL, 0));
 
     MODULE_ADD_OBJECT(
         "conditional_cdf", PyUFunc_FromFuncAndData(
-            conditional_cdf_loops, NULL,
+            (PyUFuncGenericFunction *) conditional_cdf_loops, NULL,
             double_ufunc_types, 1, 4, 1, PyUFunc_None,
             "conditional_cdf", NULL, 0));
 
     MODULE_ADD_OBJECT(
         "conditional_ppf", PyUFunc_FromFuncAndData(
-            conditional_ppf_loops, NULL,
+            (PyUFuncGenericFunction *) conditional_ppf_loops, NULL,
             double_ufunc_types, 1, 4, 1, PyUFunc_None,
             "conditional_ppf", NULL, 0));
 
     MODULE_ADD_OBJECT(
         "moments_to_parameters", PyUFunc_FromFuncAndData(
-            moments_to_parameters_loops, NULL,
+            (PyUFuncGenericFunction *) moments_to_parameters_loops, NULL,
             double_ufunc_types, 1, 2, 3, PyUFunc_None,
             "moments_to_parameters", NULL, 0));
 
     MODULE_ADD_OBJECT(
         "parameters_to_moments", PyUFunc_FromFuncAndData(
-            parameters_to_moments_loops, NULL,
+            (PyUFuncGenericFunction *) parameters_to_moments_loops, NULL,
             double_ufunc_types, 1, 2, 3, PyUFunc_None,
             "parameters_to_moments", NULL, 0));
 
     MODULE_ADD_OBJECT(
         "volume_render", PyUFunc_FromFuncAndDataAndSignature(
-            volume_render_loops, NULL,
+            (PyUFuncGenericFunction *) volume_render_loops, NULL,
             volume_render_ufunc_types, 1, 11, 1, PyUFunc_None,
             "volume_render", NULL, 0,
             "(),(),(),(),(),(3,3),(),(n),(n),(n),(n)->()"));
 
     MODULE_ADD_OBJECT(
         "marginal_pdf", PyUFunc_FromFuncAndDataAndSignature(
-            marginal_pdf_loops, NULL,
+            (PyUFuncGenericFunction *) marginal_pdf_loops, NULL,
             double_ufunc_types, 1, 5, 1, PyUFunc_None,
             "marginal_pdf", NULL, 0,
             "(),(n),(n),(n),(n)->()"));
 
     MODULE_ADD_OBJECT(
         "marginal_cdf", PyUFunc_FromFuncAndDataAndSignature(
-            marginal_cdf_loops, NULL,
+            (PyUFuncGenericFunction *) marginal_cdf_loops, NULL,
             double_ufunc_types, 1, 5, 1, PyUFunc_None,
             "marginal_cdf", NULL, 0,
             "(),(n),(n),(n),(n)->()"));
 
     MODULE_ADD_OBJECT(
         "marginal_ppf", PyUFunc_FromFuncAndDataAndSignature(
-            marginal_ppf_loops, NULL,
+            (PyUFuncGenericFunction *) marginal_ppf_loops, NULL,
             double_ufunc_types, 1, 5, 1, PyUFunc_None,
             "marginal_ppf", NULL, 0,
             "(),(n),(n),(n),(n)->()"));
 
     MODULE_ADD_OBJECT(
         "nest2uniq", PyUFunc_FromFuncAndData(
-            nest2uniq_loops, NULL,
+            (PyUFuncGenericFunction *) nest2uniq_loops, NULL,
             nest2uniq_types, 1, 2, 1, PyUFunc_None,
             "nest2uniq", NULL, 0));
 
     MODULE_ADD_OBJECT(
         "uniq2nest", PyUFunc_FromFuncAndData(
-            uniq2nest_loops, NULL,
+            (PyUFuncGenericFunction *) uniq2nest_loops, NULL,
             uniq2nest_types, 1, 1, 2, PyUFunc_None,
             "uniq2nest", NULL, 0));
 
     MODULE_ADD_OBJECT(
         "uniq2order", PyUFunc_FromFuncAndData(
-            uniq2order_loops, NULL,
+            (PyUFuncGenericFunction *) uniq2order_loops, NULL,
             uniq2order_types, 1, 1, 1, PyUFunc_None,
             "uniq2order", NULL, 0));
 
     MODULE_ADD_OBJECT(
         "uniq2pixarea", PyUFunc_FromFuncAndData(
-            uniq2pixarea_loops, NULL,
+            (PyUFuncGenericFunction *) uniq2pixarea_loops, NULL,
             uniq2pixarea_types, 1, 1, 1, PyUFunc_None,
             "uniq2pixarea", NULL, 0));
 
     MODULE_ADD_OBJECT(
         "uniq2ang", PyUFunc_FromFuncAndData(
-            uniq2ang_loops, NULL,
+            (PyUFuncGenericFunction *) uniq2ang_loops, NULL,
             uniq2ang_types, 1, 1, 2, PyUFunc_None,
             "uniq2ang", NULL, 0));
 
     MODULE_ADD_OBJECT(
         "antenna_factor", PyUFunc_FromFuncAndDataAndSignature(
-            antenna_factor_loops, NULL,
+            (PyUFuncGenericFunction *) antenna_factor_loops, NULL,
             antenna_factor_types, 1, 4, 1, PyUFunc_None,
             "antenna_factor", NULL, 0,
             "(3,3),(),(),()->()"));
 
     MODULE_ADD_OBJECT(
         "signal_amplitude_model", PyUFunc_FromFuncAndData(
-            signal_amplitude_model_loops, NULL,
+            (PyUFuncGenericFunction *) signal_amplitude_model_loops, NULL,
             signal_amplitude_model_ufunc_types, 1, 4, 1, PyUFunc_None,
             "signal_amplitude_model", NULL, 0));
 
-    WARNINGS_POP
-
     return module;
 }
```

### Comparing `ligo.skymap-2.0.0rc3/src/cubic_interp.c` & `ligo.skymap-2.0.0rc4/src/cubic_interp.c`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/src/cubic_interp.h` & `ligo.skymap-2.0.0rc4/src/cubic_interp.h`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/src/cubic_interp_test.c` & `ligo.skymap-2.0.0rc4/src/cubic_interp_test.c`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/src/omp_interruptible.h` & `ligo.skymap-2.0.0rc4/src/omp_interruptible.h`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/src/vmath.h` & `ligo.skymap-2.0.0rc4/src/vmath.h`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/src/warnings.h` & `ligo.skymap-2.0.0rc4/src/warnings.h`

 * *Files identical despite different names*

### Comparing `ligo.skymap-2.0.0rc3/tox.ini` & `ligo.skymap-2.0.0rc4/tox.ini`

 * *Files identical despite different names*

