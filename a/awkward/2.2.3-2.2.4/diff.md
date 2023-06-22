# Comparing `tmp/awkward-2.2.3.tar.gz` & `tmp/awkward-2.2.4.tar.gz`

## Comparing `awkward-2.2.3.tar` & `awkward-2.2.4.tar`

### file list

```diff
@@ -1,860 +1,865 @@
--rw-r--r--   0        0        0     1893 2023-06-15 15:47:29.000000 awkward-2.2.3/CITATION.cff
--rw-r--r--   0        0        0    13855 2023-06-15 15:47:29.000000 awkward-2.2.3/CONTRIBUTING.md
--rw-r--r--   0        0        0    22687 2023-06-15 15:47:29.000000 awkward-2.2.3/README.md
--rw-r--r--   0        0        0      241 2023-06-15 15:47:29.000000 awkward-2.2.3/requirements-test.txt
--rw-r--r--   0        0        0     7833 2023-06-15 15:47:29.000000 awkward-2.2.3/docs/_toc.yml
--rw-r--r--   0        0        0     7624 2023-06-15 15:47:29.000000 awkward-2.2.3/docs/conf.py
--rw-r--r--   0        0        0      346 2023-06-15 15:47:29.000000 awkward-2.2.3/docs/environment.yml.cog
--rw-r--r--   0        0        0     2603 2023-06-15 15:47:29.000000 awkward-2.2.3/docs/index.md
--rw-r--r--   0        0        0    11642 2023-06-15 15:47:29.000000 awkward-2.2.3/docs/prepare_docstrings.py
--rw-r--r--   0        0        0     4448 2023-06-15 15:47:29.000000 awkward-2.2.3/docs/redirects-user-guide.json
--rw-r--r--   0        0        0    11436 2023-06-15 15:47:29.000000 awkward-2.2.3/docs/redirects.json
--rw-r--r--   0        0        0      463 2023-06-15 15:47:29.000000 awkward-2.2.3/docs/requirements.txt
--rw-r--r--   0        0        0      460 2023-06-15 15:47:29.000000 awkward-2.2.3/docs/switcher.json
--rw-r--r--   0        0        0      930 2023-06-15 15:47:29.000000 awkward-2.2.3/docs/_static/css/awkward.css
--rw-r--r--   0        0        0      354 2023-06-15 15:47:29.000000 awkward-2.2.3/docs/_static/css/try-awkward-array.css
-lrwxr-xr-x   0        0        0        0 2023-06-15 15:47:29.000000 awkward-2.2.3/docs/_static/image/logo-300px-white.png -> ../../../docs-img/logo/logo-300px-white.png
-lrwxr-xr-x   0        0        0        0 2023-06-15 15:47:29.000000 awkward-2.2.3/docs/_static/image/logo-300px.png -> ../../../docs-img/logo/logo-300px.png
--rw-r--r--   0        0        0      469 2023-06-15 15:47:29.000000 awkward-2.2.3/docs/_templates/funding.html
--rw-r--r--   0        0        0      474 2023-06-15 15:47:29.000000 awkward-2.2.3/docs/_templates/redirect.html
--rw-r--r--   0        0        0     2968 2023-06-15 15:47:29.000000 awkward-2.2.3/docs/getting-started/community-tutorials.md
--rw-r--r--   0        0        0     4654 2023-06-15 15:47:29.000000 awkward-2.2.3/docs/getting-started/index.md
--rw-r--r--   0        0        0     3346 2023-06-15 15:47:29.000000 awkward-2.2.3/docs/getting-started/papers-and-talks.md
--rw-r--r--   0        0        0       82 2023-06-15 15:47:29.000000 awkward-2.2.3/docs/getting-started/try-awkward-array.md
-lrwxr-xr-x   0        0        0        0 2023-06-15 15:47:29.000000 awkward-2.2.3/docs/getting-started/demo/example-reduction-sum.svg -> ../../../docs-img/diagrams/example-reduction-sum.svg
--rw-r--r--   0        0        0    12847 2023-06-15 15:47:29.000000 awkward-2.2.3/docs/getting-started/demo/what-is-an-awkward-array.ipynb
-lrwxr-xr-x   0        0        0        0 2023-06-15 15:47:29.000000 awkward-2.2.3/docs/image/awkward-1-0-layers.svg -> ../../docs-img/diagrams/awkward-1-0-layers.svg
-lrwxr-xr-x   0        0        0        0 2023-06-15 15:47:29.000000 awkward-2.2.3/docs/image/bikeroutes-scaling.svg -> ../../docs-img/plots/bikeroutes-scaling.svg
-lrwxr-xr-x   0        0        0        0 2023-06-15 15:47:29.000000 awkward-2.2.3/docs/image/desire-path.jpg -> ../../docs-img/photos/desire-path.jpg
-lrwxr-xr-x   0        0        0        0 2023-06-15 15:47:29.000000 awkward-2.2.3/docs/image/example-array.svg -> ../../docs-img/diagrams/example-array.svg
--rw-r--r--   0        0        0    17067 2023-06-15 15:47:29.000000 awkward-2.2.3/docs/image/example-hierarchy.svg
-lrwxr-xr-x   0        0        0        0 2023-06-15 15:47:29.000000 awkward-2.2.3/docs/image/example-reduction-sum-only.svg -> ../../docs-img/diagrams/example-reduction-sum-only.svg
-lrwxr-xr-x   0        0        0        0 2023-06-15 15:47:29.000000 awkward-2.2.3/docs/image/example-reduction-sum.svg -> ../../docs-img/diagrams/example-reduction-sum.svg
-lrwxr-xr-x   0        0        0        0 2023-06-15 15:47:29.000000 awkward-2.2.3/docs/image/favicon.ico -> ../../docs-img/logo/favicon.ico
-lrwxr-xr-x   0        0        0        0 2023-06-15 15:47:29.000000 awkward-2.2.3/docs/image/github-issues-documentation.png -> ../../docs-img/screenshots/github-issues-documentation.png
-lrwxr-xr-x   0        0        0        0 2023-06-15 15:47:29.000000 awkward-2.2.3/docs/image/how-it-works.svg -> ../../docs-img/diagrams/how-it-works.svg
-lrwxr-xr-x   0        0        0        0 2023-06-15 15:47:29.000000 awkward-2.2.3/docs/image/logo-300px.png -> ../../docs-img/logo/logo-300px.png
--rw-r--r--   0        0        0    24165 2023-06-15 15:47:29.000000 awkward-2.2.3/docs/reference/ak.behavior.md
--rw-r--r--   0        0        0     1426 2023-06-15 15:47:29.000000 awkward-2.2.3/docs/reference/ak.builder.ArrayBuilder.rst
--rw-r--r--   0        0        0    64727 2023-06-15 15:47:29.000000 awkward-2.2.3/docs/reference/awkwardforth.rst
--rw-r--r--   0        0        0      270 2023-06-15 15:47:29.000000 awkward-2.2.3/docs/reference/index.md
--rw-r--r--   0        0        0     7349 2023-06-15 15:47:29.000000 awkward-2.2.3/docs/reference/toctree.txt
--rw-r--r--   0        0        0     8320 2023-06-15 15:47:29.000000 awkward-2.2.3/docs/user-guide/10-minutes-to-awkward-array.md
--rw-r--r--   0        0        0      926 2023-06-15 15:47:29.000000 awkward-2.2.3/docs/user-guide/how-to-combinatorics-best-match.md
--rw-r--r--   0        0        0      930 2023-06-15 15:47:29.000000 awkward-2.2.3/docs/user-guide/how-to-combinatorics-cartesian-combinations.md
--rw-r--r--   0        0        0      263 2023-06-15 15:47:29.000000 awkward-2.2.3/docs/user-guide/how-to-combinatorics.md
--rw-r--r--   0        0        0     8335 2023-06-15 15:47:29.000000 awkward-2.2.3/docs/user-guide/how-to-convert-arrow.md
--rw-r--r--   0        0        0     6392 2023-06-15 15:47:29.000000 awkward-2.2.3/docs/user-guide/how-to-convert-buffers.md
--rw-r--r--   0        0        0     2455 2023-06-15 15:47:29.000000 awkward-2.2.3/docs/user-guide/how-to-convert-json.md
--rw-r--r--   0        0        0    13475 2023-06-15 15:47:29.000000 awkward-2.2.3/docs/user-guide/how-to-convert-numpy.md
--rw-r--r--   0        0        0     7182 2023-06-15 15:47:29.000000 awkward-2.2.3/docs/user-guide/how-to-convert-pandas.md
--rw-r--r--   0        0        0    18830 2023-06-15 15:47:29.000000 awkward-2.2.3/docs/user-guide/how-to-convert-python.md
--rw-r--r--   0        0        0     3554 2023-06-15 15:47:29.000000 awkward-2.2.3/docs/user-guide/how-to-convert-rdataframe.md
--rw-r--r--   0        0        0      271 2023-06-15 15:47:29.000000 awkward-2.2.3/docs/user-guide/how-to-convert.md
--rw-r--r--   0        0        0    11973 2023-06-15 15:47:29.000000 awkward-2.2.3/docs/user-guide/how-to-create-arraybuilder.md
--rw-r--r--   0        0        0    36520 2023-06-15 15:47:29.000000 awkward-2.2.3/docs/user-guide/how-to-create-constructors.md
--rw-r--r--   0        0        0     7383 2023-06-15 15:47:29.000000 awkward-2.2.3/docs/user-guide/how-to-create-lists.md
--rw-r--r--   0        0        0     7456 2023-06-15 15:47:29.000000 awkward-2.2.3/docs/user-guide/how-to-create-missing.md
--rw-r--r--   0        0        0    11542 2023-06-15 15:47:29.000000 awkward-2.2.3/docs/user-guide/how-to-create-records.md
--rw-r--r--   0        0        0     4066 2023-06-15 15:47:29.000000 awkward-2.2.3/docs/user-guide/how-to-create-strings.md
--rw-r--r--   0        0        0      866 2023-06-15 15:47:29.000000 awkward-2.2.3/docs/user-guide/how-to-create-unflatten-group.md
--rw-r--r--   0        0        0      267 2023-06-15 15:47:29.000000 awkward-2.2.3/docs/user-guide/how-to-create.md
--rw-r--r--   0        0        0      834 2023-06-15 15:47:29.000000 awkward-2.2.3/docs/user-guide/how-to-examine-checking-validity.md
--rw-r--r--   0        0        0     2919 2023-06-15 15:47:29.000000 awkward-2.2.3/docs/user-guide/how-to-examine-list-fields.md
--rw-r--r--   0        0        0      848 2023-06-15 15:47:29.000000 awkward-2.2.3/docs/user-guide/how-to-examine-simple-slicing.md
--rw-r--r--   0        0        0      838 2023-06-15 15:47:29.000000 awkward-2.2.3/docs/user-guide/how-to-examine-single-item.md
--rw-r--r--   0        0        0     6778 2023-06-15 15:47:29.000000 awkward-2.2.3/docs/user-guide/how-to-examine-type.md
--rw-r--r--   0        0        0      269 2023-06-15 15:47:29.000000 awkward-2.2.3/docs/user-guide/how-to-examine.md
--rw-r--r--   0        0        0      844 2023-06-15 15:47:29.000000 awkward-2.2.3/docs/user-guide/how-to-filter-cut-mask.md
--rw-r--r--   0        0        0     3889 2023-06-15 15:47:29.000000 awkward-2.2.3/docs/user-guide/how-to-filter-masked.md
--rw-r--r--   0        0        0      840 2023-06-15 15:47:29.000000 awkward-2.2.3/docs/user-guide/how-to-filter-num.md
--rw-r--r--   0        0        0     7955 2023-06-15 15:47:29.000000 awkward-2.2.3/docs/user-guide/how-to-filter-ragged.md
--rw-r--r--   0        0        0      265 2023-06-15 15:47:29.000000 awkward-2.2.3/docs/user-guide/how-to-filter.md
--rw-r--r--   0        0        0      818 2023-06-15 15:47:29.000000 awkward-2.2.3/docs/user-guide/how-to-math-argminmax.md
--rw-r--r--   0        0        0      822 2023-06-15 15:47:29.000000 awkward-2.2.3/docs/user-guide/how-to-math-broadcasting.md
--rw-r--r--   0        0        0      828 2023-06-15 15:47:29.000000 awkward-2.2.3/docs/user-guide/how-to-math-gpu.md
--rw-r--r--   0        0        0      838 2023-06-15 15:47:29.000000 awkward-2.2.3/docs/user-guide/how-to-math-numpy.md
--rw-r--r--   0        0        0      846 2023-06-15 15:47:29.000000 awkward-2.2.3/docs/user-guide/how-to-math-reducing.md
--rw-r--r--   0        0        0      870 2023-06-15 15:47:29.000000 awkward-2.2.3/docs/user-guide/how-to-math-statistics.md
--rw-r--r--   0        0        0      265 2023-06-15 15:47:29.000000 awkward-2.2.3/docs/user-guide/how-to-math.md
--rw-r--r--   0        0        0     3411 2023-06-15 15:47:29.000000 awkward-2.2.3/docs/user-guide/how-to-restructure-add-fields.md
--rw-r--r--   0        0        0      842 2023-06-15 15:47:29.000000 awkward-2.2.3/docs/user-guide/how-to-restructure-concatenate.md
--rw-r--r--   0        0        0    19083 2023-06-15 15:47:29.000000 awkward-2.2.3/docs/user-guide/how-to-restructure-flatten.md
--rw-r--r--   0        0        0     7568 2023-06-15 15:47:29.000000 awkward-2.2.3/docs/user-guide/how-to-restructure-pad.md
--rw-r--r--   0        0        0      852 2023-06-15 15:47:29.000000 awkward-2.2.3/docs/user-guide/how-to-restructure-rename-records.md
--rw-r--r--   0        0        0      832 2023-06-15 15:47:29.000000 awkward-2.2.3/docs/user-guide/how-to-restructure-sort.md
--rw-r--r--   0        0        0     9624 2023-06-15 15:47:29.000000 awkward-2.2.3/docs/user-guide/how-to-restructure-zip-project.md
--rw-r--r--   0        0        0      273 2023-06-15 15:47:29.000000 awkward-2.2.3/docs/user-guide/how-to-restructure.md
--rw-r--r--   0        0        0     2599 2023-06-15 15:47:29.000000 awkward-2.2.3/docs/user-guide/how-to-specialize-differentiate-jax.md
--rw-r--r--   0        0        0      870 2023-06-15 15:47:29.000000 awkward-2.2.3/docs/user-guide/how-to-specialize-in-numba.md
--rw-r--r--   0        0        0      838 2023-06-15 15:47:29.000000 awkward-2.2.3/docs/user-guide/how-to-specialize-lorentz.md
--rw-r--r--   0        0        0      874 2023-06-15 15:47:29.000000 awkward-2.2.3/docs/user-guide/how-to-specialize-override-numpy.md
--rw-r--r--   0        0        0      870 2023-06-15 15:47:29.000000 awkward-2.2.3/docs/user-guide/how-to-specialize-subclass.md
--rw-r--r--   0        0        0      277 2023-06-15 15:47:29.000000 awkward-2.2.3/docs/user-guide/how-to-specialize.md
--rw-r--r--   0        0        0    11724 2023-06-15 15:47:29.000000 awkward-2.2.3/docs/user-guide/how-to-use-header-only-layoutbuilder.md
--rw-r--r--   0        0        0      900 2023-06-15 15:47:29.000000 awkward-2.2.3/docs/user-guide/how-to-use-in-numba-arraybuilder.md
--rw-r--r--   0        0        0     9973 2023-06-15 15:47:29.000000 awkward-2.2.3/docs/user-guide/how-to-use-in-numba-cuda.ipynb
--rw-r--r--   0        0        0      900 2023-06-15 15:47:29.000000 awkward-2.2.3/docs/user-guide/how-to-use-in-numba-features.md
--rw-r--r--   0        0        0      279 2023-06-15 15:47:29.000000 awkward-2.2.3/docs/user-guide/how-to-use-in-numba.md
--rw-r--r--   0        0        0      344 2023-06-15 15:47:29.000000 awkward-2.2.3/docs/user-guide/index.md
--rw-r--r--   0        0        0        0 2023-06-15 15:47:29.000000 awkward-2.2.3/docs/user-guide/requirements.txt
--rw-r--r--   0        0        0   367587 2023-06-15 15:47:29.000000 awkward-2.2.3/docs-img/panel-data-analysts.png
--rw-r--r--   0        0        0   794465 2023-06-15 15:47:29.000000 awkward-2.2.3/docs-img/panel-data-analysts.svg
--rw-r--r--   0        0        0   140700 2023-06-15 15:47:29.000000 awkward-2.2.3/docs-img/panel-developers.png
--rw-r--r--   0        0        0   328307 2023-06-15 15:47:29.000000 awkward-2.2.3/docs-img/panel-developers.svg
--rw-r--r--   0        0        0    73584 2023-06-15 15:47:29.000000 awkward-2.2.3/docs-img/panel-doxygen.png
--rw-r--r--   0        0        0    58179 2023-06-15 15:47:29.000000 awkward-2.2.3/docs-img/panel-sphinx.png
--rw-r--r--   0        0        0   127063 2023-06-15 15:47:29.000000 awkward-2.2.3/docs-img/panel-tutorials-alternate.png
--rw-r--r--   0        0        0   173327 2023-06-15 15:47:29.000000 awkward-2.2.3/docs-img/panel-tutorials.png
--rw-r--r--   0        0        0    12541 2023-06-15 15:47:29.000000 awkward-2.2.3/docs-img/diagrams/awkward-1-0-layers.pdf
--rw-r--r--   0        0        0    65246 2023-06-15 15:47:29.000000 awkward-2.2.3/docs-img/diagrams/awkward-1-0-layers.png
--rw-r--r--   0        0        0    41004 2023-06-15 15:47:29.000000 awkward-2.2.3/docs-img/diagrams/awkward-1-0-layers.svg
--rw-r--r--   0        0        0    14946 2023-06-15 15:47:29.000000 awkward-2.2.3/docs-img/diagrams/awkward-timeline.pdf
--rw-r--r--   0        0        0   125180 2023-06-15 15:47:29.000000 awkward-2.2.3/docs-img/diagrams/awkward-timeline.png
--rw-r--r--   0        0        0    70209 2023-06-15 15:47:29.000000 awkward-2.2.3/docs-img/diagrams/awkward-timeline.svg
--rw-r--r--   0        0        0   436595 2023-06-15 15:47:29.000000 awkward-2.2.3/docs-img/diagrams/awkward-uproot-timeline-pip-github.png
--rw-r--r--   0        0        0   426911 2023-06-15 15:47:29.000000 awkward-2.2.3/docs-img/diagrams/awkward-uproot-timeline-pip-github.svg
--rw-r--r--   0        0        0   335955 2023-06-15 15:47:29.000000 awkward-2.2.3/docs-img/diagrams/awkward-uproot-timeline-pip.png
--rw-r--r--   0        0        0   325268 2023-06-15 15:47:29.000000 awkward-2.2.3/docs-img/diagrams/awkward-uproot-timeline-pip.svg
--rw-r--r--   0        0        0   129696 2023-06-15 15:47:29.000000 awkward-2.2.3/docs-img/diagrams/awkward-uproot-timeline.png
--rw-r--r--   0        0        0   120554 2023-06-15 15:47:29.000000 awkward-2.2.3/docs-img/diagrams/awkward-uproot-timeline.svg
--rw-r--r--   0        0        0     5208 2023-06-15 15:47:29.000000 awkward-2.2.3/docs-img/diagrams/cartoon-broadcasting.png
--rw-r--r--   0        0        0    25065 2023-06-15 15:47:29.000000 awkward-2.2.3/docs-img/diagrams/cartoon-broadcasting.svg
--rw-r--r--   0        0        0     5754 2023-06-15 15:47:29.000000 awkward-2.2.3/docs-img/diagrams/cartoon-cartesian.png
--rw-r--r--   0        0        0    32616 2023-06-15 15:47:29.000000 awkward-2.2.3/docs-img/diagrams/cartoon-cartesian.svg
--rw-r--r--   0        0        0     9584 2023-06-15 15:47:29.000000 awkward-2.2.3/docs-img/diagrams/cartoon-combinations.png
--rw-r--r--   0        0        0    39524 2023-06-15 15:47:29.000000 awkward-2.2.3/docs-img/diagrams/cartoon-combinations.svg
--rw-r--r--   0        0        0    10808 2023-06-15 15:47:29.000000 awkward-2.2.3/docs-img/diagrams/cartoon-schematic.png
--rw-r--r--   0        0        0    25779 2023-06-15 15:47:29.000000 awkward-2.2.3/docs-img/diagrams/cartoon-schematic.svg
--rw-r--r--   0        0        0    18178 2023-06-15 15:47:29.000000 awkward-2.2.3/docs-img/diagrams/example-array.svg
--rw-r--r--   0        0        0    36024 2023-06-15 15:47:29.000000 awkward-2.2.3/docs-img/diagrams/example-hierarchy.png
--rw-r--r--   0        0        0    17092 2023-06-15 15:47:29.000000 awkward-2.2.3/docs-img/diagrams/example-hierarchy.svg
--rw-r--r--   0        0        0    21120 2023-06-15 15:47:29.000000 awkward-2.2.3/docs-img/diagrams/example-reduction-sum-only.svg
--rw-r--r--   0        0        0    29325 2023-06-15 15:47:29.000000 awkward-2.2.3/docs-img/diagrams/example-reduction-sum.svg
--rw-r--r--   0        0        0    55553 2023-06-15 15:47:29.000000 awkward-2.2.3/docs-img/diagrams/example-reduction.png
--rw-r--r--   0        0        0    21631 2023-06-15 15:47:29.000000 awkward-2.2.3/docs-img/diagrams/example-reduction.svg
--rw-r--r--   0        0        0    10978 2023-06-15 15:47:29.000000 awkward-2.2.3/docs-img/diagrams/git-strategy.pdf
--rw-r--r--   0        0        0    58904 2023-06-15 15:47:29.000000 awkward-2.2.3/docs-img/diagrams/git-strategy.png
--rw-r--r--   0        0        0    28990 2023-06-15 15:47:29.000000 awkward-2.2.3/docs-img/diagrams/git-strategy.svg
--rw-r--r--   0        0        0   113587 2023-06-15 15:47:29.000000 awkward-2.2.3/docs-img/diagrams/how-it-works-muons.png
--rw-r--r--   0        0        0    57471 2023-06-15 15:47:29.000000 awkward-2.2.3/docs-img/diagrams/how-it-works-muons.svg
--rw-r--r--   0        0        0    58475 2023-06-15 15:47:29.000000 awkward-2.2.3/docs-img/diagrams/how-it-works.svg
--rw-r--r--   0        0        0    63989 2023-06-15 15:47:29.000000 awkward-2.2.3/docs-img/diagrams/sorting-axis.svg
--rw-r--r--   0        0        0   124038 2023-06-15 15:47:29.000000 awkward-2.2.3/docs-img/diagrams/reducers/all.svg
--rw-r--r--   0        0        0   128558 2023-06-15 15:47:29.000000 awkward-2.2.3/docs-img/diagrams/reducers/any.svg
--rw-r--r--   0        0        0   134490 2023-06-15 15:47:29.000000 awkward-2.2.3/docs-img/diagrams/reducers/argmax.svg
--rw-r--r--   0        0        0   133192 2023-06-15 15:47:29.000000 awkward-2.2.3/docs-img/diagrams/reducers/argmin.svg
--rw-r--r--   0        0        0   106277 2023-06-15 15:47:29.000000 awkward-2.2.3/docs-img/diagrams/reducers/count.svg
--rw-r--r--   0        0        0   116417 2023-06-15 15:47:29.000000 awkward-2.2.3/docs-img/diagrams/reducers/count_nonzero.svg
--rw-r--r--   0        0        0   111789 2023-06-15 15:47:29.000000 awkward-2.2.3/docs-img/diagrams/reducers/max.svg
--rw-r--r--   0        0        0   109239 2023-06-15 15:47:29.000000 awkward-2.2.3/docs-img/diagrams/reducers/min.svg
--rw-r--r--   0        0        0   124702 2023-06-15 15:47:29.000000 awkward-2.2.3/docs-img/diagrams/reducers/product.svg
--rw-r--r--   0        0        0   108897 2023-06-15 15:47:29.000000 awkward-2.2.3/docs-img/diagrams/reducers/sum.svg
--rw-r--r--   0        0        0     8347 2023-06-15 15:47:29.000000 awkward-2.2.3/docs-img/logo/favicon.ico
--rw-r--r--   0        0        0     8984 2023-06-15 15:47:29.000000 awkward-2.2.3/docs-img/logo/logo-300px-white.png
--rw-r--r--   0        0        0    11964 2023-06-15 15:47:29.000000 awkward-2.2.3/docs-img/logo/logo-300px.png
--rw-r--r--   0        0        0    24707 2023-06-15 15:47:29.000000 awkward-2.2.3/docs-img/logo/logo-600px.png
--rw-r--r--   0        0        0    18767 2023-06-15 15:47:29.000000 awkward-2.2.3/docs-img/logo/logo.svg
--rw-r--r--   0        0        0    90413 2023-06-15 15:47:29.000000 awkward-2.2.3/docs-img/photos/desire-path.jpg
--rw-r--r--   0        0        0    52113 2023-06-15 15:47:29.000000 awkward-2.2.3/docs-img/plots/awkward-0-popularity.pdf
--rw-r--r--   0        0        0   146109 2023-06-15 15:47:29.000000 awkward-2.2.3/docs-img/plots/awkward-0-popularity.png
--rw-r--r--   0        0        0   147576 2023-06-15 15:47:29.000000 awkward-2.2.3/docs-img/plots/awkward-0-popularity.svg
--rw-r--r--   0        0        0    26938 2023-06-15 15:47:29.000000 awkward-2.2.3/docs-img/plots/bikeroutes-scaling.svg
--rw-r--r--   0        0        0     8891 2023-06-15 15:47:29.000000 awkward-2.2.3/docs-img/screenshots/github-issues-documentation.png
--rw-r--r--   0        0        0     1325 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/__init__.py
--rw-r--r--   0        0        0     4626 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_behavior.py
--rw-r--r--   0        0        0    38827 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_broadcasting.py
--rw-r--r--   0        0        0    13672 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_do.py
--rw-r--r--   0        0        0    12583 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_errors.py
--rw-r--r--   0        0        0     5727 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_kernels.py
--rw-r--r--   0        0        0     5860 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_layout.py
--rw-r--r--   0        0        0     9983 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_lookup.py
--rw-r--r--   0        0        0     5454 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_parameters.py
--rw-r--r--   0        0        0     9965 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_prettyprint.py
--rw-r--r--   0        0        0    28974 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_reducers.py
--rw-r--r--   0        0        0     1492 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_regularize.py
--rw-r--r--   0        0        0      420 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_singleton.py
--rw-r--r--   0        0        0    23934 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_slicing.py
--rw-r--r--   0        0        0      647 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_typetracer.py
--rw-r--r--   0        0        0     1163 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_typing.py
--rw-r--r--   0        0        0     2498 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_util.py
--rw-r--r--   0        0        0      758 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_v2.py
--rw-r--r--   0        0        0      233 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/builder.py
--rw-r--r--   0        0        0      866 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/cppyy.py
--rw-r--r--   0        0        0      271 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/forth.py
--rw-r--r--   0        0        0   103232 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/highlevel.py
--rw-r--r--   0        0        0     8044 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/index.py
--rw-r--r--   0        0        0     3988 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/jax.py
--rw-r--r--   0        0        0     6017 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/numba.py
--rw-r--r--   0        0        0     8272 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/record.py
--rw-r--r--   0        0        0     1679 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/typetracer.py
--rw-r--r--   0        0        0        0 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_backends/__init__.py
--rw-r--r--   0        0        0     2082 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_backends/backend.py
--rw-r--r--   0        0        0     1259 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_backends/cupy.py
--rw-r--r--   0        0        0     3763 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_backends/dispatch.py
--rw-r--r--   0        0        0     1453 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_backends/jax.py
--rw-r--r--   0        0        0      944 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_backends/numpy.py
--rw-r--r--   0        0        0     1425 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_backends/typetracer.py
--rw-r--r--   0        0        0       88 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_connect/__init__.py
--rw-r--r--   0        0        0    32504 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_connect/avro.py
--rw-r--r--   0        0        0    53532 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_connect/cling.py
--rw-r--r--   0        0        0      985 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_connect/hist.py
--rw-r--r--   0        0        0     4485 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_connect/numexpr.py
--rw-r--r--   0        0        0    11515 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_connect/numpy.py
--rw-r--r--   0        0        0    37988 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_connect/pyarrow.py
--rw-r--r--   0        0        0     7038 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_connect/cuda/__init__.py
--rw-r--r--   0        0        0     2555 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_BitMaskedArray_to_ByteMaskedArray.cu
--rw-r--r--   0        0        0     4326 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_BitMaskedArray_to_IndexedOptionArray.cu
--rw-r--r--   0        0        0      987 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_getitem_carry.cu
--rw-r--r--   0        0        0     2542 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_getitem_nextcarry.cu
--rw-r--r--   0        0        0     3034 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_getitem_nextcarry_outindex.cu
--rw-r--r--   0        0        0      630 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_mask.cu
--rw-r--r--   0        0        0      830 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_overlay_mask.cu
--rw-r--r--   0        0        0     3196 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_reduce_next_64.cu
--rw-r--r--   0        0        0     2668 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_reduce_next_nonlocal_nextshifts_64.cu
--rw-r--r--   0        0        0      749 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_toIndexedOptionArray.cu
--rw-r--r--   0        0        0     2749 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_Content_getitem_next_missing_jagged_getmaskstartstop.cu
--rw-r--r--   0        0        0      552 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_Index_to_Index64.cu
--rw-r--r--   0        0        0      637 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_fill_count.cu
--rw-r--r--   0        0        0     2886 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_flatten_nextcarry.cu
--rw-r--r--   0        0        0     2904 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_getitem_nextcarry.cu
--rw-r--r--   0        0        0     3416 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_getitem_nextcarry_outindex.cu
--rw-r--r--   0        0        0     3531 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_getitem_nextcarry_outindex_mask.cu
--rw-r--r--   0        0        0      556 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_mask.cu
--rw-r--r--   0        0        0      695 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_overlay_mask.cu
--rw-r--r--   0        0        0     3036 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_64.cu
--rw-r--r--   0        0        0      795 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_fix_offsets_64.cu
--rw-r--r--   0        0        0     2523 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_nonlocal_nextshifts_64.cu
--rw-r--r--   0        0        0     2729 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_nonlocal_nextshifts_fromshifts_64.cu
--rw-r--r--   0        0        0     1035 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_simplify.cu
--rw-r--r--   0        0        0      961 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_validity.cu
--rw-r--r--   0        0        0     2593 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedOptionArray_rpad_and_clip_mask_axis1.cu
--rw-r--r--   0        0        0     1536 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_compact_offsets.cu
--rw-r--r--   0        0        0     1710 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_getitem_jagged_expand.cu
--rw-r--r--   0        0        0     2012 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_getitem_next_array.cu
--rw-r--r--   0        0        0     1184 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_validity.cu
--rw-r--r--   0        0        0      806 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_flatten_offsets.cu
--rw-r--r--   0        0        0      744 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_reduce_global_startstop_64.cu
--rw-r--r--   0        0        0     1169 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_rpad_and_clip_axis1.cu
--rw-r--r--   0        0        0     1059 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_rpad_axis1.cu
--rw-r--r--   0        0        0     3208 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_MaskedArray_getitem_next_jagged_project.cu
--rw-r--r--   0        0        0      575 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_contiguous_init.cu
--rw-r--r--   0        0        0      830 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_contiguous_next.cu
--rw-r--r--   0        0        0      650 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_fill_tobool.cu
--rw-r--r--   0        0        0     2610 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_boolean_nonzero.cu
--rw-r--r--   0        0        0     1126 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_array.cu
--rw-r--r--   0        0        0      951 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_array_advanced.cu
--rw-r--r--   0        0        0      721 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_at.cu
--rw-r--r--   0        0        0     1003 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_range.cu
--rw-r--r--   0        0        0     1339 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_range_advanced.cu
--rw-r--r--   0        0        0      835 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_reduce_adjust_starts_64.cu
--rw-r--r--   0        0        0      975 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_reduce_adjust_starts_shifts_64.cu
--rw-r--r--   0        0        0      802 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_reduce_mask_ByteMaskedArray_64.cu
--rw-r--r--   0        0        0      789 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_carry.cu
--rw-r--r--   0        0        0     1040 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_jagged_expand.cu
--rw-r--r--   0        0        0     1020 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_array.cu
--rw-r--r--   0        0        0     1045 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_array_advanced.cu
--rw-r--r--   0        0        0      974 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_at.cu
--rw-r--r--   0        0        0      946 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_range.cu
--rw-r--r--   0        0        0      980 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_range_spreadadvanced.cu
--rw-r--r--   0        0        0      663 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_localindex.cu
--rw-r--r--   0        0        0      586 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_fillna.cu
--rw-r--r--   0        0        0     2580 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_project.cu
--rw-r--r--   0        0        0     1360 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_validity.cu
--rw-r--r--   0        0        0      461 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_carry_arange.cu
--rw-r--r--   0        0        0      534 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_combinations.cu
--rw-r--r--   0        0        0      529 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_content_reduce_zeroparents_64.cu
--rw-r--r--   0        0        0      830 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_index_carry.cu
--rw-r--r--   0        0        0      636 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_index_carry_nocheck.cu
--rw-r--r--   0        0        0      689 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_index_rpad_and_clip_axis1.cu
--rw-r--r--   0        0        0      457 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_localindex.cu
--rw-r--r--   0        0        0      830 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_missing_repeat.cu
--rw-r--r--   0        0        0     2043 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmax.cu
--rw-r--r--   0        0        0     2198 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmax_bool_64.cu
--rw-r--r--   0        0        0     2043 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmin.cu
--rw-r--r--   0        0        0     2198 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmin_bool_64.cu
--rw-r--r--   0        0        0     3054 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_count_64.cu
--rw-r--r--   0        0        0     3289 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_countnonzero.cu
--rw-r--r--   0        0        0     2022 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_max.cu
--rw-r--r--   0        0        0     2022 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_min.cu
--rw-r--r--   0        0        0     3202 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_prod_bool.cu
--rw-r--r--   0        0        0     3012 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum.cu
--rw-r--r--   0        0        0     3171 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum_bool.cu
--rw-r--r--   0        0        0     3439 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum_int32_bool_64.cu
--rw-r--r--   0        0        0     3439 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum_int64_bool_64.cu
--rw-r--r--   0        0        0      865 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_regularize_arrayslice.cu
--rw-r--r--   0        0        0      443 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_zero_mask.cu
--rw-r--r--   0        0        0     3195 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/cuda_common.cu
--rw-r--r--   0        0        0     1859 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_connect/header-only/awkward/BuilderOptions.h
--rw-r--r--   0        0        0    19822 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_connect/header-only/awkward/GrowableBuffer.h
--rw-r--r--   0        0        0    89307 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_connect/header-only/awkward/LayoutBuilder.h
--rw-r--r--   0        0        0      298 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_connect/header-only/awkward/demo_impl.h
--rw-r--r--   0        0        0     8025 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_connect/header-only/awkward/utils.h
--rw-r--r--   0        0        0      239 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_connect/jax/__init__.py
--rw-r--r--   0        0        0    11085 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_connect/jax/reducers.py
--rw-r--r--   0        0        0     5982 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_connect/jax/trees.py
--rw-r--r--   0        0        0       88 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_connect/numba/__init__.py
--rw-r--r--   0        0        0    35828 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_connect/numba/arrayview.py
--rw-r--r--   0        0        0     1182 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_connect/numba/arrayview_cuda.py
--rw-r--r--   0        0        0    31510 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_connect/numba/builder.py
--rw-r--r--   0        0        0     9624 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_connect/numba/growablebuffer.py
--rw-r--r--   0        0        0    49133 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_connect/numba/layout.py
--rw-r--r--   0        0        0       88 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_connect/rdataframe/__init__.py
--rw-r--r--   0        0        0     9377 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_connect/rdataframe/from_rdataframe.py
--rw-r--r--   0        0        0     9922 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_connect/rdataframe/to_rdataframe.py
--rw-r--r--   0        0        0     1487 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_connect/rdataframe/include/rdataframe/jagged_builders.h
--rw-r--r--   0        0        0     1111 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_nplikes/__init__.py
--rw-r--r--   0        0        0    16149 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_nplikes/array_module.py
--rw-r--r--   0        0        0     5365 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_nplikes/cupy.py
--rw-r--r--   0        0        0     1357 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_nplikes/dispatch.py
--rw-r--r--   0        0        0     2276 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_nplikes/jax.py
--rw-r--r--   0        0        0     3065 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_nplikes/numpy.py
--rw-r--r--   0        0        0    14154 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_nplikes/numpylike.py
--rw-r--r--   0        0        0     3579 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_nplikes/placeholder.py
--rw-r--r--   0        0        0     2379 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_nplikes/shape.py
--rw-r--r--   0        0        0    48307 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_nplikes/typetracer.py
--rw-r--r--   0        0        0     2527 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/_nplikes/ufuncs.py
--rw-r--r--   0        0        0       88 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/behaviors/__init__.py
--rw-r--r--   0        0        0     3479 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/behaviors/categorical.py
--rw-r--r--   0        0        0     3898 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/behaviors/mixins.py
--rw-r--r--   0        0        0     7884 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/behaviors/string.py
--rw-r--r--   0        0        0      986 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/contents/__init__.py
--rw-r--r--   0        0        0    28289 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/contents/bitmaskedarray.py
--rw-r--r--   0        0        0    41835 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/contents/bytemaskedarray.py
--rw-r--r--   0        0        0    44581 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/contents/content.py
--rw-r--r--   0        0        0    13853 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/contents/emptyarray.py
--rw-r--r--   0        0        0    41644 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/contents/indexedarray.py
--rw-r--r--   0        0        0    64499 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/contents/indexedoptionarray.py
--rw-r--r--   0        0        0    62401 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/contents/listarray.py
--rw-r--r--   0        0        0    84953 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/contents/listoffsetarray.py
--rw-r--r--   0        0        0    48679 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/contents/numpyarray.py
--rw-r--r--   0        0        0    46696 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/contents/recordarray.py
--rw-r--r--   0        0        0    56591 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/contents/regulararray.py
--rw-r--r--   0        0        0    58157 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/contents/unionarray.py
--rw-r--r--   0        0        0    19483 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/contents/unmaskedarray.py
--rw-r--r--   0        0        0      962 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/forms/__init__.py
--rw-r--r--   0        0        0     5955 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/forms/bitmaskedform.py
--rw-r--r--   0        0        0     5242 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/forms/bytemaskedform.py
--rw-r--r--   0        0        0     4484 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/forms/emptyform.py
--rw-r--r--   0        0        0    18686 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/forms/form.py
--rw-r--r--   0        0        0     5630 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/forms/indexedform.py
--rw-r--r--   0        0        0     5020 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/forms/indexedoptionform.py
--rw-r--r--   0        0        0     5508 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/forms/listform.py
--rw-r--r--   0        0        0     4753 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/forms/listoffsetform.py
--rw-r--r--   0        0        0     6391 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/forms/numpyform.py
--rw-r--r--   0        0        0     8095 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/forms/recordform.py
--rw-r--r--   0        0        0     4971 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/forms/regularform.py
--rw-r--r--   0        0        0     7647 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/forms/unionform.py
--rw-r--r--   0        0        0     4116 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/forms/unmaskedform.py
--rw-r--r--   0        0        0     4828 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/operations/__init__.py
--rw-r--r--   0        0        0     3500 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/operations/ak_all.py
--rw-r--r--   0        0        0     8181 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/operations/ak_almost_equal.py
--rw-r--r--   0        0        0     3503 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/operations/ak_any.py
--rw-r--r--   0        0        0     5109 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/operations/ak_argcartesian.py
--rw-r--r--   0        0        0     3819 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/operations/ak_argcombinations.py
--rw-r--r--   0        0        0     5924 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/operations/ak_argmax.py
--rw-r--r--   0        0        0     5881 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/operations/ak_argmin.py
--rw-r--r--   0        0        0     3158 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/operations/ak_argsort.py
--rw-r--r--   0        0        0      952 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/operations/ak_backend.py
--rw-r--r--   0        0        0     9855 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/operations/ak_broadcast_arrays.py
--rw-r--r--   0        0        0     6595 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/operations/ak_broadcast_fields.py
--rw-r--r--   0        0        0    15615 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/operations/ak_cartesian.py
--rw-r--r--   0        0        0     1420 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/operations/ak_categories.py
--rw-r--r--   0        0        0     8118 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/operations/ak_combinations.py
--rw-r--r--   0        0        0    12753 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/operations/ak_concatenate.py
--rw-r--r--   0        0        0     2715 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/operations/ak_copy.py
--rw-r--r--   0        0        0     5319 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/operations/ak_corr.py
--rw-r--r--   0        0        0     4730 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/operations/ak_count.py
--rw-r--r--   0        0        0     3537 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/operations/ak_count_nonzero.py
--rw-r--r--   0        0        0     4672 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/operations/ak_covar.py
--rw-r--r--   0        0        0     4581 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/operations/ak_drop_none.py
--rw-r--r--   0        0        0    50451 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/operations/ak_enforce_type.py
--rw-r--r--   0        0        0     1106 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/operations/ak_fields.py
--rw-r--r--   0        0        0     5323 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/operations/ak_fill_none.py
--rw-r--r--   0        0        0     3467 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/operations/ak_firsts.py
--rw-r--r--   0        0        0     7802 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/operations/ak_flatten.py
--rw-r--r--   0        0        0     3154 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/operations/ak_from_arrow.py
--rw-r--r--   0        0        0      813 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/operations/ak_from_arrow_schema.py
--rw-r--r--   0        0        0     2729 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/operations/ak_from_avro_file.py
--rw-r--r--   0        0        0    14486 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/operations/ak_from_buffers.py
--rw-r--r--   0        0        0     1839 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/operations/ak_from_categorical.py
--rw-r--r--   0        0        0     1651 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/operations/ak_from_cupy.py
--rw-r--r--   0        0        0     4109 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/operations/ak_from_iter.py
--rw-r--r--   0        0        0     1716 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/operations/ak_from_jax.py
--rw-r--r--   0        0        0    30024 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/operations/ak_from_json.py
--rw-r--r--   0        0        0     2282 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/operations/ak_from_numpy.py
--rw-r--r--   0        0        0    11931 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/operations/ak_from_parquet.py
--rw-r--r--   0        0        0     3324 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/operations/ak_from_rdataframe.py
--rw-r--r--   0        0        0     3000 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/operations/ak_from_regular.py
--rw-r--r--   0        0        0     8859 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/operations/ak_full_like.py
--rw-r--r--   0        0        0      873 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/operations/ak_is_categorical.py
--rw-r--r--   0        0        0     2513 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/operations/ak_is_none.py
--rw-r--r--   0        0        0      705 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/operations/ak_is_tuple.py
--rw-r--r--   0        0        0      930 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/operations/ak_is_valid.py
--rw-r--r--   0        0        0     2568 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/operations/ak_isclose.py
--rw-r--r--   0        0        0     8934 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/operations/ak_linear_fit.py
--rw-r--r--   0        0        0     3258 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/operations/ak_local_index.py
--rw-r--r--   0        0        0     4753 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/operations/ak_mask.py
--rw-r--r--   0        0        0     6466 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/operations/ak_max.py
--rw-r--r--   0        0        0     8103 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/operations/ak_mean.py
--rw-r--r--   0        0        0     3603 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/operations/ak_merge_option_of_records.py
--rw-r--r--   0        0        0    12413 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/operations/ak_merge_union_of_records.py
--rw-r--r--   0        0        0     3217 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/operations/ak_metadata_from_parquet.py
--rw-r--r--   0        0        0     6418 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/operations/ak_min.py
--rw-r--r--   0        0        0     4410 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/operations/ak_moment.py
--rw-r--r--   0        0        0     2081 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/operations/ak_nan_to_none.py
--rw-r--r--   0        0        0     5103 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/operations/ak_nan_to_num.py
--rw-r--r--   0        0        0     3909 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/operations/ak_num.py
--rw-r--r--   0        0        0     1951 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/operations/ak_ones_like.py
--rw-r--r--   0        0        0     4362 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/operations/ak_pad_none.py
--rw-r--r--   0        0        0     1786 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/operations/ak_parameters.py
--rw-r--r--   0        0        0     5396 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/operations/ak_prod.py
--rw-r--r--   0        0        0     4216 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/operations/ak_ptp.py
--rw-r--r--   0        0        0     2275 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/operations/ak_ravel.py
--rw-r--r--   0        0        0     9604 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/operations/ak_run_lengths.py
--rw-r--r--   0        0        0     3063 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/operations/ak_singletons.py
--rw-r--r--   0        0        0     2839 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/operations/ak_softmax.py
--rw-r--r--   0        0        0     2670 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/operations/ak_sort.py
--rw-r--r--   0        0        0     7160 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/operations/ak_std.py
--rw-r--r--   0        0        0     3058 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/operations/ak_strings_astype.py
--rw-r--r--   0        0        0    10754 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/operations/ak_sum.py
--rw-r--r--   0        0        0     4931 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/operations/ak_to_arrow.py
--rw-r--r--   0        0        0     6725 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/operations/ak_to_arrow_table.py
--rw-r--r--   0        0        0     2370 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/operations/ak_to_backend.py
--rw-r--r--   0        0        0     6378 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/operations/ak_to_buffers.py
--rw-r--r--   0        0        0     6050 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/operations/ak_to_categorical.py
--rw-r--r--   0        0        0     1107 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/operations/ak_to_cupy.py
--rw-r--r--   0        0        0    13370 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/operations/ak_to_dataframe.py
--rw-r--r--   0        0        0     1106 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/operations/ak_to_jax.py
--rw-r--r--   0        0        0    11673 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/operations/ak_to_json.py
--rw-r--r--   0        0        0     4507 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/operations/ak_to_layout.py
--rw-r--r--   0        0        0     2612 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/operations/ak_to_list.py
--rw-r--r--   0        0        0     2123 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/operations/ak_to_numpy.py
--rw-r--r--   0        0        0     3354 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/operations/ak_to_packed.py
--rw-r--r--   0        0        0    17280 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/operations/ak_to_parquet.py
--rw-r--r--   0        0        0     2785 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/operations/ak_to_rdataframe.py
--rw-r--r--   0        0        0     3382 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/operations/ak_to_regular.py
--rw-r--r--   0        0        0    23979 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/operations/ak_transform.py
--rw-r--r--   0        0        0     4422 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/operations/ak_type.py
--rw-r--r--   0        0        0     9461 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/operations/ak_unflatten.py
--rw-r--r--   0        0        0     2484 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/operations/ak_unzip.py
--rw-r--r--   0        0        0     1138 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/operations/ak_validity_error.py
--rw-r--r--   0        0        0     2659 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/operations/ak_values_astype.py
--rw-r--r--   0        0        0     8388 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/operations/ak_var.py
--rw-r--r--   0        0        0     5862 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/operations/ak_where.py
--rw-r--r--   0        0        0     6130 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/operations/ak_with_field.py
--rw-r--r--   0        0        0     2600 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/operations/ak_with_name.py
--rw-r--r--   0        0        0     1848 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/operations/ak_with_parameter.py
--rw-r--r--   0        0        0     3756 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/operations/ak_without_field.py
--rw-r--r--   0        0        0     1509 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/operations/ak_without_parameters.py
--rw-r--r--   0        0        0     2134 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/operations/ak_zeros_like.py
--rw-r--r--   0        0        0     8819 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/operations/ak_zip.py
--rw-r--r--   0        0        0      707 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/types/__init__.py
--rw-r--r--   0        0        0   163323 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/types/_awkward_datashape_parser.py
--rw-r--r--   0        0        0     2168 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/types/arraytype.py
--rw-r--r--   0        0        0     3007 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/types/listtype.py
--rw-r--r--   0        0        0     6171 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/types/numpytype.py
--rw-r--r--   0        0        0     4886 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/types/optiontype.py
--rw-r--r--   0        0        0     8774 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/types/recordtype.py
--rw-r--r--   0        0        0     3928 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/types/regulartype.py
--rw-r--r--   0        0        0     1341 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/types/scalartype.py
--rw-r--r--   0        0        0    10063 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/types/type.py
--rw-r--r--   0        0        0     4593 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/types/uniontype.py
--rw-r--r--   0        0        0     2489 2023-06-15 15:47:29.000000 awkward-2.2.3/src/awkward/types/unknowntype.py
--rw-r--r--   0        0        0       88 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/__init__.py
--rw-r--r--   0        0        0     3358 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0002_minimal_listarray.py
--rw-r--r--   0        0        0      487 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0006_deep_iteration.py
--rw-r--r--   0        0        0     5565 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0008_slices_and_getitem.py
--rw-r--r--   0        0        0    13378 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0011_listarray.py
--rw-r--r--   0        0        0     4462 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0013_error_handling_struct.py
--rw-r--r--   0        0        0    17019 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0014_finish_up_getitem.py
--rw-r--r--   0        0        0     5169 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0018_fromiter_fillable.py
--rw-r--r--   0        0        0     8833 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0019_use_json_library.py
--rw-r--r--   0        0        0    13687 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0020_support_unsigned_indexes.py
--rw-r--r--   0        0        0     6391 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0021_emptyarray.py
--rw-r--r--   0        0        0    10743 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0023_regular_array.py
--rw-r--r--   0        0        0     4890 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0024_use_regular_array.py
--rw-r--r--   0        0        0    25581 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0025_record_array.py
--rw-r--r--   0        0        0     3436 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0028_add_dressed_types.py
--rw-r--r--   0        0        0     6321 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0032_replace_dressedtype.py
--rw-r--r--   0        0        0    12027 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0046_start_indexedarray.py
--rw-r--r--   0        0        0      898 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0049_distinguish_record_and_recordarray_behaviors.py
--rw-r--r--   0        0        0    12231 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0057_introducing_forms.py
--rw-r--r--   0        0        0     5430 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0070_argmin_and_argmax.py
--rw-r--r--   0        0        0     5384 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0072_fillna_operation.py
--rw-r--r--   0        0        0    15655 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0074_argsort_and_sort.py
--rw-r--r--   0        0        0     2836 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0077_zip_operation.py
--rw-r--r--   0        0        0    11934 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0078_argcross_and_cross.py
--rw-r--r--   0        0        0    12124 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0079_argchoose_and_choose.py
--rw-r--r--   0        0        0     7071 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0080_flatpandas_multiindex_rows_and_columns.py
--rw-r--r--   0        0        0     6615 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0084_start_unionarray.py
--rw-r--r--   0        0        0     6551 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0086_nep13_ufunc.py
--rw-r--r--   0        0        0    12540 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0089_numpy_functions.py
--rw-r--r--   0        0        0    46684 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0093_simplify_uniontypes_and_optiontypes.py
--rw-r--r--   0        0        0     6959 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0107_assign_fields_to_records.py
--rw-r--r--   0        0        0    46658 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0111_jagged_and_masked_getitem.py
--rw-r--r--   0        0        0    77410 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0115_generic_reducer_operation.py
--rw-r--r--   0        0        0    35162 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0118_numba_cpointers.py
--rw-r--r--   0        0        0     1091 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0119_numexpr_and_broadcast_arrays.py
--rw-r--r--   0        0        0     1106 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0124_strings_in_numba.py
--rw-r--r--   0        0        0    32114 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0127_tomask_operation.py
--rw-r--r--   0        0        0     3683 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0127b_tomask_operation_numba.py
--rw-r--r--   0        0        0      838 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0138_emptyarray_type.py
--rw-r--r--   0        0        0    17923 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0150_flatten.py
--rw-r--r--   0        0        0     3602 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0163_negative_axis_wrap.py
--rw-r--r--   0        0        0     9779 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0166_0167_0170_random_issues.py
--rw-r--r--   0        0        0     4552 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0173_astype_operation.py
--rw-r--r--   0        0        0    24034 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0184_concatenate_operation.py
--rw-r--r--   0        0        0     2063 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0193_is_none_axis_parameter.py
--rw-r--r--   0        0        0     3352 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0198_tutorial_documentation_1.py
--rw-r--r--   0        0        0     8998 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0222_count_with_axis0.py
--rw-r--r--   0        0        0    75605 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0224_arrow_to_awkward.py
--rw-r--r--   0        0        0      581 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0264_reduce_last_empty.py
--rw-r--r--   0        0        0     3251 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0273_path_for_with_field.py
--rw-r--r--   0        0        0      743 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0286_broadcast_single_value_with_field.py
--rw-r--r--   0        0        0     2205 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0290_bug_fixes_for_hats.py
--rw-r--r--   0        0        0     4806 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0315_integerindex.py
--rw-r--r--   0        0        0     5745 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0331_pandas_indexedarray.py
--rw-r--r--   0        0        0     1257 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0334_fully_broadcastable_where.py
--rw-r--r--   0        0        0      566 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0339_highlevel_sorting_function.py
--rw-r--r--   0        0        0     6757 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0348_form_keys.py
--rw-r--r--   0        0        0     4523 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0355_mixins.py
--rw-r--r--   0        0        0    10396 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0395_complex_type_arrays.py
--rw-r--r--   0        0        0     4934 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0395_fix_numba_indexedarray.py
--rw-r--r--   0        0        0     3212 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0397_arrays_as_constants_in_numba.py
--rw-r--r--   0        0        0    14529 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0401_add_categorical_type_for_arrow_dictionary.py
--rw-r--r--   0        0        0    22467 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0404_array_validity_check.py
--rw-r--r--   0        0        0    14282 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0410_fix_argminmax_positions_for_missing_values.py
--rw-r--r--   0        0        0    17455 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0437_stream_of_many_json_files.py
--rw-r--r--   0        0        0    32921 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0447_preserve_regularness_in_reduce.py
--rw-r--r--   0        0        0    24075 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0449_merge_many_arrays_in_one_pass.py
--rw-r--r--   0        0        0     4059 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0493_zeros_ones_full_like.py
--rw-r--r--   0        0        0     1606 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0496_provide_local_index.py
--rw-r--r--   0        0        0     2059 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0499_getitem_indexedarray_bug.py
--rw-r--r--   0        0        0     1286 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0504_block_ufuncs_for_strings.py
--rw-r--r--   0        0        0     2926 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0511_copy_and_deepcopy.py
--rw-r--r--   0        0        0     9119 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0527_fix_unionarray_ufuncs_and_parameters_in_merging.py
--rw-r--r--   0        0        0      365 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0546_fill_none_replacement_value_type.py
--rw-r--r--   0        0        0     1102 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0549_numba_array_asarray.py
--rw-r--r--   0        0        0     4268 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0557_min_max_initial_argument.py
--rw-r--r--   0        0        0      537 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0559_fix_booleans_in_numba.py
--rw-r--r--   0        0        0      636 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0572_numba_array_ndim.py
--rw-r--r--   0        0        0     4901 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0582_propagate_context_in_broadcast_and_apply.py
--rw-r--r--   0        0        0     1099 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0583_implement_unflatten_function.py
--rw-r--r--   0        0        0     3084 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0590_allow_regulararray_size_zero.py
--rw-r--r--   0        0        0     5957 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0593_preserve_nullability_in_arrow_and_parquet.py
--rw-r--r--   0        0        0      478 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0627_behavior_from_dict_of_arrays.py
--rw-r--r--   0        0        0     8205 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0652_tests_of_complex_numbers.py
--rw-r--r--   0        0        0     2335 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0674_categorical_validation.py
--rw-r--r--   0        0        0      750 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0713_getitem_field_should_simplify_optiontype.py
--rw-r--r--   0        0        0     1242 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0723_ensure_that_jagged_slice_fits_array_length.py
--rw-r--r--   0        0        0     1055 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0730_unflatten_axis_parameter.py
--rw-r--r--   0        0        0     2569 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0733_run_lengths.py
--rw-r--r--   0        0        0     2127 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0736_implement_argsort_for_strings.py
--rw-r--r--   0        0        0      330 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0758_ak_zip_scallars.py
--rw-r--r--   0        0        0     1122 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0766_prevent_combinations_of_characters.py
--rw-r--r--   0        0        0    26349 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0773_typeparser.py
--rw-r--r--   0        0        0      779 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0788_indexedarray_carrying_recordarray_parameters.py
--rw-r--r--   0        0        0      871 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0794_ak_cartesian_on_empty_array.py
--rw-r--r--   0        0        0     1148 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0803_argsort_fix_type.py
--rw-r--r--   0        0        0     1364 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0806_empty_lists_cartesian_fix.py
--rw-r--r--   0        0        0     6311 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0813_full_like_dtype_arg.py
--rw-r--r--   0        0        0     1661 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0815_broadcast_union_types_to_all_possibilities.py
--rw-r--r--   0        0        0      488 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0819_issue.py
--rw-r--r--   0        0        0      682 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0828_arrow_datatype_null.py
--rw-r--r--   0        0        0    23609 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0835_datetime_type.py
--rw-r--r--   0        0        0      676 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0835_datetime_type_pandas.py
--rw-r--r--   0        0        0     4662 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0835_datetime_type_pyarrow.py
--rw-r--r--   0        0        0      680 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0850_argsort_mask_array.py
--rw-r--r--   0        0        0      449 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0863_is_none_numpy_array.py
--rw-r--r--   0        0        0     1029 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0866_getitem_field_and_flatten_unions.py
--rw-r--r--   0        0        0      929 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0875_arrow_null_type.py
--rw-r--r--   0        0        0      901 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0879_non_primitive_with_field.py
--rw-r--r--   0        0        0      563 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0884_index_and_identifier_refactoring.py
--rw-r--r--   0        0        0     1086 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0889_ptp.py
--rw-r--r--   0        0        0    53355 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0896_content_classes_refactoring.py
--rw-r--r--   0        0        0     1751 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0898_unzip_heterogeneous_records.py
--rw-r--r--   0        0        0      421 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0903_ArrayView_expects_contiguous_NumpyArrays.py
--rw-r--r--   0        0        0      530 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0905_leading_zeros_in_unflatten.py
--rw-r--r--   0        0        0     1048 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0906_arrow_fixed_size_list_type.py
--rw-r--r--   0        0        0      666 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0910_unflatten_counts_relation.py
--rw-r--r--   0        0        0     5261 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0912_packed.py
--rw-r--r--   0        0        0   115270 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0914_types_and_forms.py
--rw-r--r--   0        0        0     1877 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0916_datetime_values_astype.py
--rw-r--r--   0        0        0     5522 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0927_numpy_array_nbytes.py
--rw-r--r--   0        0        0      709 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0930_bug_in_unionarray_purelist_parameter.py
--rw-r--r--   0        0        0     1627 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0945_argsort_sort_nan_array.py
--rw-r--r--   0        0        0    28028 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0958_new_forms_must_accept_old_form_json.py
--rw-r--r--   0        0        0    28284 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0959__getitem_array_implementation.py
--rw-r--r--   0        0        0      651 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0975_mask_multidimensional_numpy_array.py
--rw-r--r--   0        0        0      644 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0979_where_multidimentional_numpy_array.py
--rw-r--r--   0        0        0     5803 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0982_missing_case_in_nonlocal_reducers.py
--rw-r--r--   0        0        0     1976 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0984_ravel.py
--rw-r--r--   0        0        0     1806 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_0992_correct_ptp_unmasking.py
--rw-r--r--   0        0        0     2100 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1000_fixes_argmax_for_ListOffsetArray_with_nonzero_start.py
--rw-r--r--   0        0        0      429 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1006_packed_regular_array_zero_size.py
--rw-r--r--   0        0        0      416 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1007_from_buffers_empty_ndarray.py
--rw-r--r--   0        0        0      551 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1017_numpyarray_broadcast.py
--rw-r--r--   0        0        0      785 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1030_mixin_class_name.py
--rw-r--r--   0        0        0    52114 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1031_start_getitem_next.py
--rw-r--r--   0        0        0    18007 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1031b_start_getitem_next_specialized.py
--rw-r--r--   0        0        0     1146 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1049_concatenate_single_array.py
--rw-r--r--   0        0        0     1559 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1055_fill_none_numpy_dimension.py
--rw-r--r--   0        0        0    42250 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1059_localindex.py
--rw-r--r--   0        0        0      551 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1066_to_numpy_masked_structured_array.py
--rw-r--r--   0        0        0      685 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1071_mask_identity_false_should_not_return_option_type.py
--rw-r--r--   0        0        0    27714 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1072_sort.py
--rw-r--r--   0        0        0    44140 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1074_combinations.py
--rw-r--r--   0        0        0     5181 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1075_validityerror.py
--rw-r--r--   0        0        0      273 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1106_argminmax_axis_None_missing_values.py
--rw-r--r--   0        0        0    25531 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1110_type_tracer_1.py
--rw-r--r--   0        0        0     1870 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1116_project_maskedarrays.py
--rw-r--r--   0        0        0    28376 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1125_to_arrow_from_arrow.py
--rw-r--r--   0        0        0     6276 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1132_utility_methods_for_highlevel_functions.py
--rw-r--r--   0        0        0    21098 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1134_from_buffers_to_buffers.py
--rw-r--r--   0        0        0    57322 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1135_rpad_operation.py
--rw-r--r--   0        0        0     4639 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1136_regulararray_zeros_in_shape.py
--rw-r--r--   0        0        0    10487 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1137_num.py
--rw-r--r--   0        0        0    10222 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1142_numbers_to_type.py
--rw-r--r--   0        0        0     2559 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1149_datetime_sort.py
--rw-r--r--   0        0        0      630 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1154_arrow_tables_should_preserve_parameters.py
--rw-r--r--   0        0        0    27983 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1162_ak_from_json_schema.py
--rw-r--r--   0        0        0      766 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1183_bugs_found_by_dask_project_2.py
--rw-r--r--   0        0        0     1286 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1189_fix_singletons_for_non_optional_data.py
--rw-r--r--   0        0        0      551 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1192_iterables_in___array_function__.py
--rw-r--r--   0        0        0      608 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1193_is_none_nested_option.py
--rw-r--r--   0        0        0     2601 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1233_ak_with_name.py
--rw-r--r--   0        0        0    26468 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1240_v2_implementation_of_numba_1.py
--rw-r--r--   0        0        0     1146 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1259_simplify_optiontype.py
--rw-r--r--   0        0        0     1560 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1260_simplify_masked_option_types.py
--rw-r--r--   0        0        0      681 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1271_fix_4D_reducers.py
--rw-r--r--   0        0        0    33145 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1294_to_and_from_parquet.py
--rw-r--r--   0        0        0     1945 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1298_allow_nan_to_num_arguments_to_be_arrays.py
--rw-r--r--   0        0        0    62340 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1300_awkward_to_cpp_converter_with_cling.py
--rw-r--r--   0        0        0    39474 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1300b_same_for_numba.py
--rw-r--r--   0        0        0      367 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1305_mixed_awkward_numpy_slicing.py
--rw-r--r--   0        0        0     1702 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1308_zip_after_option.py
--rw-r--r--   0        0        0     1703 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1318_array_function_types.py
--rw-r--r--   0        0        0     1730 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1320_mask_identity_defaults.py
--rw-r--r--   0        0        0      647 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1344_broadcast_arrays_depth_limit.py
--rw-r--r--   0        0        0     6621 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1345_avro_reader.py
--rw-r--r--   0        0        0     4562 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1351_is_tuple.py
--rw-r--r--   0        0        0     8362 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1374_to_rdataframe.py
--rw-r--r--   0        0        0     1755 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1377_ravel_string.py
--rw-r--r--   0        0        0     1468 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1379_reducers_with_axis_None_and_typetracers.py
--rw-r--r--   0        0        0     1384 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1399_from_jax.py
--rw-r--r--   0        0        0     1227 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1399_to_jax.py
--rw-r--r--   0        0        0      297 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1400_with_name_record.py
--rw-r--r--   0        0        0      449 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1403_from_numpy_strings.py
--rw-r--r--   0        0        0     3470 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1405_slicing_untested_cases.py
--rw-r--r--   0        0        0     6909 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1415_behaviour_forwarding.py
--rw-r--r--   0        0        0    18809 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1440_start_v2_to_parquet.py
--rw-r--r--   0        0        0    14402 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1447_jax_autodiff_slices_ufuncs.py
--rw-r--r--   0        0        0     8591 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1449_v2_to_json_from_json_functions.py
--rw-r--r--   0        0        0      692 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1453_write_single_records_to_parquet.py
--rw-r--r--   0        0        0     9828 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1473_from_rdataframe.py
--rw-r--r--   0        0        0    24648 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1477_generator_entry_type_as_rvec.py
--rw-r--r--   0        0        0     3579 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1490_jax_reducers_combinations.py
--rw-r--r--   0        0        0     3905 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1502_getitem_jagged_issue1406.py
--rw-r--r--   0        0        0     1733 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1504_typetracer_like.py
--rw-r--r--   0        0        0     4913 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1508_awkward_from_rdataframe.py
--rw-r--r--   0        0        0     2186 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1511_set_attribute.py
--rw-r--r--   0        0        0      754 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1539_isnone_axis_check_issue1417.py
--rw-r--r--   0        0        0     1570 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1559_fix_ufuncs_records_1439.py
--rw-r--r--   0        0        0      990 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1565_axis_wrap_if_negative_record.py
--rw-r--r--   0        0        0     1085 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1567_fix_longlong_in_Index.py
--rw-r--r--   0        0        0     3022 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1568_fix_lengths_empty_regular_slices.py
--rw-r--r--   0        0        0      385 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1578_to_arrow_empty_recordarray.py
--rw-r--r--   0        0        0     5911 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1586_concatenate_should_preserve_regulararray.py
--rw-r--r--   0        0        0      216 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1593_empty_slice_list_record.py
--rw-r--r--   0        0        0     7260 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1604_preserve_form_in_concatenate.py
--rw-r--r--   0        0        0     4372 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1607_no_reducers_on_records.py
--rw-r--r--   0        0        0    10035 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1613_generator_tolayout_records.py
--rw-r--r--   0        0        0      727 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1619_from_parquet_empty_field.py
--rw-r--r--   0        0        0     6024 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1620_layout_builders.py
--rw-r--r--   0        0        0     8122 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1625_multiple_columns_from_rdataframe.py
--rw-r--r--   0        0        0      770 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1642_from_iter_of_tuples.py
--rw-r--r--   0        0        0      389 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1644_concatenate_zeros_length.py
--rw-r--r--   0        0        0     4317 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1650_Record_to_list_should_listify_itself.py
--rw-r--r--   0        0        0      560 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1671_categorical_type.py
--rw-r--r--   0        0        0    11761 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1672_broadcast_parameters.py
--rw-r--r--   0        0        0     4453 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1677_array_builder_in_numba.py
--rw-r--r--   0        0        0      544 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1685_IndexedArray_project_parameters.py
--rw-r--r--   0        0        0      778 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1686_UnionArray_simplified_preserve_parameters.py
--rw-r--r--   0        0        0      936 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1688_pack_categorical.py
--rw-r--r--   0        0        0      525 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1703_fill_none_typetracer.py
--rw-r--r--   0        0        0     1743 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1707_broadcast_parameters_ufunc.py
--rw-r--r--   0        0        0      512 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1709_ak_array_constructor_behavior.py
--rw-r--r--   0        0        0      398 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1735_from_numpy_mask.py
--rw-r--r--   0        0        0      577 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1747_bytemaskedarray_mergemany.py
--rw-r--r--   0        0        0      824 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1753_indexedarray_merge_kernel.py
--rw-r--r--   0        0        0     1480 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1762_jax_behavior_support.py
--rw-r--r--   0        0        0      589 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1764_jax_jacobian.py
--rw-r--r--   0        0        0      962 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1765_add_ioanas_test_of_to_arraylib.py
--rw-r--r--   0        0        0     4790 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1766_record_form_fields.py
--rw-r--r--   0        0        0     2905 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1781_rdataframe_snapshot.py
--rw-r--r--   0        0        0      701 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1784_reduce_leading_sublist.py
--rw-r--r--   0        0        0      567 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1790_reduce_regulararray.py
--rw-r--r--   0        0        0     4191 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1791_reduce_trailing_sublist.py
--rw-r--r--   0        0        0     1027 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1794_run_lengths_empty_sublist.py
--rw-r--r--   0        0        0      407 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1823_fill_none_axis_none.py
--rw-r--r--   0        0        0      481 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1826_ravel_preserve_none.py
--rw-r--r--   0        0        0     1451 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1829_to_from_rdataframe_bool.py
--rw-r--r--   0        0        0      588 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1840_ak_type_to_handle_ndarray_dtype_and_nptypes.py
--rw-r--r--   0        0        0     1097 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1847_numpy_array_contiguous.py
--rw-r--r--   0        0        0      681 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1850_bytemasked_array_to_bytemaskedarray.py
--rw-r--r--   0        0        0     1640 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1867_pass_behavior_through_combinations.py
--rw-r--r--   0        0        0    17239 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1904_drop_none.py
--rw-r--r--   0        0        0     3553 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1914_improved_axis_to_posaxis.py
--rw-r--r--   0        0        0     4607 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1928_replace_simplify_method_with_classmethod_constructor.py
--rw-r--r--   0        0        0      921 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1930_unflatten_counts_checks.py
--rw-r--r--   0        0        0      769 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1936_with_field_broadcasting.py
--rw-r--r--   0        0        0      551 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1940_ak_backend.py
--rw-r--r--   0        0        0     1457 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1943_regular_indexing.py
--rw-r--r--   0        0        0      188 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1944_to_numpy_empty_record_array.py
--rw-r--r--   0        0        0     1131 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1960_awkward_from_rdataframe.py
--rw-r--r--   0        0        0     3286 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1961_ak_without_field.py
--rw-r--r--   0        0        0      280 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1978_akRecord_constructor_should_retain_type.py
--rw-r--r--   0        0        0      349 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_1991_missed_a_NumpyArray_raw_call_without_underscore.py
--rw-r--r--   0        0        0      371 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_2008_ak_type_layout.py
--rw-r--r--   0        0        0    10222 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_2020_reduce_axis_none.py
--rw-r--r--   0        0        0      803 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_2021_check_TypeTracerArray_in_ak_where.py
--rw-r--r--   0        0        0      645 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_2023_from_rdataframe.py
--rw-r--r--   0        0        0     2845 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_2027_add_data_touch_reporting_to_TypeTracerArray.py
--rw-r--r--   0        0        0     1219 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_2047_ak_transform_regular_to_jagged.py
--rw-r--r--   0        0        0      406 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_2051_arraybuilder_behavior_propagation.py
--rw-r--r--   0        0        0     1275 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_2055_array_builder_check.py
--rw-r--r--   0        0        0     1659 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_2058_merge_numpy_array.py
--rw-r--r--   0        0        0      708 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_2064_fill_none_record.py
--rw-r--r--   0        0        0      799 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_2067_to_buffers_byteorder.py
--rw-r--r--   0        0        0      741 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_2070_to_layout_string.py
--rw-r--r--   0        0        0     1172 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_2071_unflatten_non_packed_counts.py
--rw-r--r--   0        0        0      291 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_2076_ak_unzip_record.py
--rw-r--r--   0        0        0      545 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_2078_array_function_wrap.py
--rw-r--r--   0        0        0      589 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_2082_broadcast_zero_size.py
--rw-r--r--   0        0        0     1716 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_2085_empty_if_typetracer.py
--rw-r--r--   0        0        0     2765 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_2096_ak_scalar_type.py
--rw-r--r--   0        0        0      977 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_2101_pickle_behavior_class.py
--rw-r--r--   0        0        0      519 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_2104_numpy_merge_option.py
--rw-r--r--   0        0        0     2715 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_2106_pickle_class.py
--rw-r--r--   0        0        0      722 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_2108_fill_none_indexed.py
--rw-r--r--   0        0        0     2100 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_2115_fix_up_typetracers.py
--rw-r--r--   0        0        0      487 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_2120_missing_field_error.py
--rw-r--r--   0        0        0     1110 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_2125_type_of_scalar.py
--rw-r--r--   0        0        0     1893 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_2150_typetracer_high_level_ufunc.py
--rw-r--r--   0        0        0     1898 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_2179_parameter_merging_rules.py
--rw-r--r--   0        0        0      510 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_2181_with_name_len.py
--rw-r--r--   0        0        0     2957 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_2185_merge_union_of_records.py
--rw-r--r--   0        0        0      528 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_2188_values_astype_turns_EmptyArray_into_NumpyArray.py
--rw-r--r--   0        0        0     6059 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_2198_almost_equal.py
--rw-r--r--   0        0        0     1252 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_2202_filter_multiple_columns_from_rdataframe.py
--rw-r--r--   0        0        0     1453 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_2214_offset_bool_index.py
--rw-r--r--   0        0        0      334 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_2219_flatten_empty.py
--rw-r--r--   0        0        0      663 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_2226_slice_regulararray_typetracer.py
--rw-r--r--   0        0        0     1728 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_2229_getitem_range_slice.py
--rw-r--r--   0        0        0     4003 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_2234_from_rdataframe_keep_order.py
--rw-r--r--   0        0        0     4104 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_2236_merge_union_of_records_option.py
--rw-r--r--   0        0        0      485 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_2240_merge_union_parameters.py
--rw-r--r--   0        0        0     1338 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_2240_simplify_merge_as_union.py
--rw-r--r--   0        0        0      512 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_2246_slice_not_packed.py
--rw-r--r--   0        0        0      733 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_2250_full_like_bool.py
--rw-r--r--   0        0        0     1835 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_2258_from_rdataframe_with_arguments.py
--rw-r--r--   0        0        0      492 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_2259_run_lengths_typetracer.py
--rw-r--r--   0        0        0      560 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_2263_to_packed_list.py
--rw-r--r--   0        0        0      877 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_2266_fix_nan_to_num.py
--rw-r--r--   0        0        0      909 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_2267_broadcast_fields.py
--rw-r--r--   0        0        0     1336 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_2293_unflatten_typetracer.py
--rw-r--r--   0        0        0      406 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_2294_view_unknown_scalar.py
--rw-r--r--   0        0        0      720 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_2296_duplicate_field.py
--rw-r--r--   0        0        0     2262 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_2297_common_backend.py
--rw-r--r--   0        0        0      455 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_2304_index_typetracer.py
--rw-r--r--   0        0        0      648 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_2305_nep_18_lazy_conversion.py
--rw-r--r--   0        0        0     2929 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_2306_cppyy_git.py
--rw-r--r--   0        0        0     4386 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_2319_from_buffers_array.py
--rw-r--r--   0        0        0      721 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_2327_array_interface.py
--rw-r--r--   0        0        0     1728 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_2329_cartesian_broadcasting_fixes.py
--rw-r--r--   0        0        0      489 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_2346_broadcast_depth_limit.py
--rw-r--r--   0        0        0    15615 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_2349_growablebuffer_in_numba.py
--rw-r--r--   0        0        0      618 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_2354_ufunc_same_backend.py
--rw-r--r--   0        0        0      647 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_2355_to_backend_record.py
--rw-r--r--   0        0        0     1435 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_2361_typetracer_asarray_nd.py
--rw-r--r--   0        0        0      934 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_2364_empty_list_of_string.py
--rw-r--r--   0        0        0    37200 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_2365_enforce_type.py
--rw-r--r--   0        0        0     2921 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_2368_type_is_equal.py
--rw-r--r--   0        0        0     5250 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_2373_unzip_touching.py
--rw-r--r--   0        0        0     5848 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_2374_cartesian_touching.py
--rw-r--r--   0        0        0     1037 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_2385_with_field_empty_record.py
--rw-r--r--   0        0        0      956 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_2395_copy_asarray_touch.py
--rw-r--r--   0        0        0      212 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_2407_broadcast_no_arrays.py
--rw-r--r--   0        0        0     1070 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_2410_string_broadcast.py
--rw-r--r--   0        0        0      800 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_2411_cartesian_axis_validation.py
--rw-r--r--   0        0        0      704 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_2417_bytemasked_singletons.py
--rw-r--r--   0        0        0      351 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_2418_union_broadcast_unknown.py
--rw-r--r--   0        0        0     1563 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_2424_almost_equal_union_record.py
--rw-r--r--   0        0        0     1211 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_2425_forms_from_type.py
--rw-r--r--   0        0        0      545 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_2426_is_equal_to.py
--rw-r--r--   0        0        0      495 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_2444_minimal_listarray.py
--rw-r--r--   0        0        0      857 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_2471_flatten_string.py
--rw-r--r--   0        0        0     1032 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_2484_reduce_starts_empty.py
--rw-r--r--   0        0        0      659 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_2487_broadcast_list_offsets.py
--rw-r--r--   0        0        0     1319 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_2490_reduce_regulararray_positional.py
--rw-r--r--   0        0        0     1816 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_2495_concatenate_typetracer.py
--rw-r--r--   0        0        0     3800 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_2501_positional_record_reducer.py
--rw-r--r--   0        0        0      603 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_2503_deprecate_to_numpyform.py
--rw-r--r--   0        0        0     4942 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_2512_record_array_carry.py
--rw-r--r--   0        0        0     1014 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/test_2518_datetime_units_as_parameter.py
--rw-r--r--   0        0        0      128 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/samples/__init__.py
--rw-r--r--   0        0        0      218 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/samples/array_enum_test_data.avro
--rw-r--r--   0        0        0      176 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/samples/array_string_test_data.avro
--rw-r--r--   0        0        0      152 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/samples/array_test_data.avro
--rw-r--r--   0        0        0      115 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/samples/bool_test_data.avro
--rw-r--r--   0        0        0      130 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/samples/bytes_test_data.avro
--rw-r--r--   0        0        0      158 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/samples/double_test_data.avro
--rw-r--r--   0        0        0      191 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/samples/enum_null_test_data.avro
--rw-r--r--   0        0        0      180 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/samples/enum_test_data.avro
--rw-r--r--   0        0        0      218 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/samples/fixed_test_data.avro
--rw-r--r--   0        0        0      116 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/samples/float_test_data.avro
--rw-r--r--   0        0        0      106 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/samples/int_null_test_data.avro
--rw-r--r--   0        0        0      128 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/samples/int_string_null_test_data.avro
--rw-r--r--   0        0        0       89 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/samples/int_test_data.avro
--rw-r--r--   0        0        0     3035 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/samples/list-depths-records-list.parquet
--rw-r--r--   0        0        0     2871 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/samples/list-depths-records.parquet
--rw-r--r--   0        0        0      497 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/samples/list-depths-simple.parquet
--rw-r--r--   0        0        0     1136 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/samples/list-depths-strings.parquet
--rw-r--r--   0        0        0     1060 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/samples/list-depths.parquet
--rw-r--r--   0        0        0      465 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/samples/list-lengths.parquet
--rw-r--r--   0        0        0      116 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/samples/long_test_data.avro
--rw-r--r--   0        0        0      681 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/samples/nonnullable-depths.parquet
--rw-r--r--   0        0        0       75 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/samples/null_test_data.avro
--rw-r--r--   0        0        0      719 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/samples/nullable-depths.parquet
--rw-r--r--   0        0        0      635 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/samples/nullable-levels.parquet
--rw-r--r--   0        0        0     3050 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/samples/nullable-list-depths-records-list.parquet
--rw-r--r--   0        0        0     2926 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/samples/nullable-list-depths-records.parquet
--rw-r--r--   0        0        0     1179 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/samples/nullable-list-depths-strings.parquet
--rw-r--r--   0        0        0     1101 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/samples/nullable-list-depths.parquet
--rw-r--r--   0        0        0      430 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/samples/nullable-record-primitives-simple.parquet
--rw-r--r--   0        0        0     1181 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/samples/nullable-record-primitives.parquet
--rw-r--r--   0        0        0     1193 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/samples/record-primitives.parquet
--rw-r--r--   0        0        0      326 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/samples/record_0_test_data.avro
--rw-r--r--   0        0        0      368 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/samples/record_1_test_data.avro
--rw-r--r--   0        0        0      263 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/samples/record_null_test_data.avro
--rw-r--r--   0        0        0      423 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/samples/record_test_data.avro
--rw-r--r--   0        0        0      116 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/samples/string_null_test_data.avro
--rw-r--r--   0        0        0      125 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/samples/string_test_data.avro
--rw-r--r--   0        0        0      544 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/samples/test-nan-inf.json
--rw-r--r--   0        0        0      155 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/samples/test-record-array.json
--rw-r--r--   0        0        0      803 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/samples/test-two-arrays.json
--rw-r--r--   0        0        0      535 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/samples/test.json
--rw-r--r--   0        0        0      180 2023-06-15 15:47:29.000000 awkward-2.2.3/tests/samples/zero-record-batches.parquet
--rw-r--r--   0        0        0       88 2023-06-15 15:47:29.000000 awkward-2.2.3/tests-cuda/__init__.py
--rw-r--r--   0        0        0     7072 2023-06-15 15:47:29.000000 awkward-2.2.3/tests-cuda/test_1276_cuda_num.py
--rw-r--r--   0        0        0     9757 2023-06-15 15:47:29.000000 awkward-2.2.3/tests-cuda/test_1276_cuda_transfers.py
--rw-r--r--   0        0        0     1197 2023-06-15 15:47:29.000000 awkward-2.2.3/tests-cuda/test_1276_cupy_interop.py
--rw-r--r--   0        0        0     1629 2023-06-15 15:47:29.000000 awkward-2.2.3/tests-cuda/test_1276_from_cupy.py
--rw-r--r--   0        0        0    42786 2023-06-15 15:47:29.000000 awkward-2.2.3/tests-cuda/test_1300_same_for_numba_cuda.py
--rw-r--r--   0        0        0      834 2023-06-15 15:47:29.000000 awkward-2.2.3/tests-cuda/test_1381_check_errors.py
--rw-r--r--   0        0        0    11252 2023-06-15 15:47:29.000000 awkward-2.2.3/tests-cuda/test_1809_array_cuda_jit.py
--rw-r--r--   0        0        0     2212 2023-06-15 15:47:29.000000 awkward-2.2.3/.gitignore
--rw-r--r--   0        0        0     1520 2023-06-15 15:47:29.000000 awkward-2.2.3/LICENSE
--rw-r--r--   0        0        0     8479 2023-06-15 15:47:29.000000 awkward-2.2.3/pyproject.toml
--rw-r--r--   0        0        0     6933 2023-06-15 15:47:29.000000 awkward-2.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1893 2023-06-15 15:47:29.000000 awkward-2.2.4/CITATION.cff
+-rw-r--r--   0        0        0    13855 2023-06-15 15:47:29.000000 awkward-2.2.4/CONTRIBUTING.md
+-rw-r--r--   0        0        0    22687 2023-06-15 15:47:29.000000 awkward-2.2.4/README.md
+-rw-r--r--   0        0        0      241 2023-06-15 15:47:29.000000 awkward-2.2.4/requirements-test.txt
+-rw-r--r--   0        0        0     7833 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/_toc.yml
+-rw-r--r--   0        0        0     7624 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/conf.py
+-rw-r--r--   0        0        0      346 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/environment.yml.cog
+-rw-r--r--   0        0        0     2603 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/index.md
+-rw-r--r--   0        0        0    11642 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/prepare_docstrings.py
+-rw-r--r--   0        0        0     4448 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/redirects-user-guide.json
+-rw-r--r--   0        0        0    11436 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/redirects.json
+-rw-r--r--   0        0        0       22 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/requirements-wasm.txt
+-rw-r--r--   0        0        0      574 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/requirements.txt
+-rw-r--r--   0        0        0      460 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/switcher.json
+-rw-r--r--   0        0        0      930 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/_static/css/awkward.css
+-rw-r--r--   0        0        0      354 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/_static/css/try-awkward-array.css
+lrwxr-xr-x   0        0        0        0 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/_static/image/logo-300px-white.png -> ../../../docs-img/logo/logo-300px-white.png
+lrwxr-xr-x   0        0        0        0 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/_static/image/logo-300px.png -> ../../../docs-img/logo/logo-300px.png
+-rw-r--r--   0        0        0      469 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/_templates/funding.html
+-rw-r--r--   0        0        0      474 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/_templates/redirect.html
+-rw-r--r--   0        0        0     2968 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/getting-started/community-tutorials.md
+-rw-r--r--   0        0        0     4654 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/getting-started/index.md
+-rw-r--r--   0        0        0     3346 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/getting-started/papers-and-talks.md
+-rw-r--r--   0        0        0       82 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/getting-started/try-awkward-array.md
+lrwxr-xr-x   0        0        0        0 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/getting-started/demo/example-reduction-sum.svg -> ../../../docs-img/diagrams/example-reduction-sum.svg
+-rw-r--r--   0        0        0    12847 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/getting-started/demo/what-is-an-awkward-array.ipynb
+lrwxr-xr-x   0        0        0        0 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/image/awkward-1-0-layers.svg -> ../../docs-img/diagrams/awkward-1-0-layers.svg
+lrwxr-xr-x   0        0        0        0 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/image/bikeroutes-scaling.svg -> ../../docs-img/plots/bikeroutes-scaling.svg
+lrwxr-xr-x   0        0        0        0 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/image/desire-path.jpg -> ../../docs-img/photos/desire-path.jpg
+lrwxr-xr-x   0        0        0        0 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/image/example-array.svg -> ../../docs-img/diagrams/example-array.svg
+-rw-r--r--   0        0        0    17067 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/image/example-hierarchy.svg
+lrwxr-xr-x   0        0        0        0 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/image/example-reduction-sum-only.svg -> ../../docs-img/diagrams/example-reduction-sum-only.svg
+lrwxr-xr-x   0        0        0        0 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/image/example-reduction-sum.svg -> ../../docs-img/diagrams/example-reduction-sum.svg
+lrwxr-xr-x   0        0        0        0 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/image/favicon.ico -> ../../docs-img/logo/favicon.ico
+lrwxr-xr-x   0        0        0        0 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/image/github-issues-documentation.png -> ../../docs-img/screenshots/github-issues-documentation.png
+lrwxr-xr-x   0        0        0        0 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/image/how-it-works.svg -> ../../docs-img/diagrams/how-it-works.svg
+lrwxr-xr-x   0        0        0        0 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/image/logo-300px.png -> ../../docs-img/logo/logo-300px.png
+-rw-r--r--   0        0        0    24165 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/reference/ak.behavior.md
+-rw-r--r--   0        0        0     1426 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/reference/ak.builder.ArrayBuilder.rst
+-rw-r--r--   0        0        0    64727 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/reference/awkwardforth.rst
+-rw-r--r--   0        0        0      270 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/reference/index.md
+-rw-r--r--   0        0        0     7349 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/reference/toctree.txt
+-rw-r--r--   0        0        0     8320 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/user-guide/10-minutes-to-awkward-array.md
+-rw-r--r--   0        0        0      926 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/user-guide/how-to-combinatorics-best-match.md
+-rw-r--r--   0        0        0      930 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/user-guide/how-to-combinatorics-cartesian-combinations.md
+-rw-r--r--   0        0        0      263 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/user-guide/how-to-combinatorics.md
+-rw-r--r--   0        0        0     8335 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/user-guide/how-to-convert-arrow.md
+-rw-r--r--   0        0        0     6392 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/user-guide/how-to-convert-buffers.md
+-rw-r--r--   0        0        0     2455 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/user-guide/how-to-convert-json.md
+-rw-r--r--   0        0        0    13475 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/user-guide/how-to-convert-numpy.md
+-rw-r--r--   0        0        0     7182 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/user-guide/how-to-convert-pandas.md
+-rw-r--r--   0        0        0    18830 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/user-guide/how-to-convert-python.md
+-rw-r--r--   0        0        0     3554 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/user-guide/how-to-convert-rdataframe.md
+-rw-r--r--   0        0        0      271 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/user-guide/how-to-convert.md
+-rw-r--r--   0        0        0    11973 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/user-guide/how-to-create-arraybuilder.md
+-rw-r--r--   0        0        0    36520 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/user-guide/how-to-create-constructors.md
+-rw-r--r--   0        0        0     7383 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/user-guide/how-to-create-lists.md
+-rw-r--r--   0        0        0     7456 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/user-guide/how-to-create-missing.md
+-rw-r--r--   0        0        0    11542 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/user-guide/how-to-create-records.md
+-rw-r--r--   0        0        0     4066 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/user-guide/how-to-create-strings.md
+-rw-r--r--   0        0        0      866 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/user-guide/how-to-create-unflatten-group.md
+-rw-r--r--   0        0        0      267 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/user-guide/how-to-create.md
+-rw-r--r--   0        0        0      834 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/user-guide/how-to-examine-checking-validity.md
+-rw-r--r--   0        0        0     2919 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/user-guide/how-to-examine-list-fields.md
+-rw-r--r--   0        0        0      848 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/user-guide/how-to-examine-simple-slicing.md
+-rw-r--r--   0        0        0      838 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/user-guide/how-to-examine-single-item.md
+-rw-r--r--   0        0        0     6778 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/user-guide/how-to-examine-type.md
+-rw-r--r--   0        0        0      269 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/user-guide/how-to-examine.md
+-rw-r--r--   0        0        0      844 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/user-guide/how-to-filter-cut-mask.md
+-rw-r--r--   0        0        0     3889 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/user-guide/how-to-filter-masked.md
+-rw-r--r--   0        0        0      840 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/user-guide/how-to-filter-num.md
+-rw-r--r--   0        0        0     7955 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/user-guide/how-to-filter-ragged.md
+-rw-r--r--   0        0        0      265 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/user-guide/how-to-filter.md
+-rw-r--r--   0        0        0      818 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/user-guide/how-to-math-argminmax.md
+-rw-r--r--   0        0        0      822 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/user-guide/how-to-math-broadcasting.md
+-rw-r--r--   0        0        0      828 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/user-guide/how-to-math-gpu.md
+-rw-r--r--   0        0        0      838 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/user-guide/how-to-math-numpy.md
+-rw-r--r--   0        0        0      846 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/user-guide/how-to-math-reducing.md
+-rw-r--r--   0        0        0      870 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/user-guide/how-to-math-statistics.md
+-rw-r--r--   0        0        0      265 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/user-guide/how-to-math.md
+-rw-r--r--   0        0        0     3411 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/user-guide/how-to-restructure-add-fields.md
+-rw-r--r--   0        0        0      842 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/user-guide/how-to-restructure-concatenate.md
+-rw-r--r--   0        0        0    19083 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/user-guide/how-to-restructure-flatten.md
+-rw-r--r--   0        0        0     7568 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/user-guide/how-to-restructure-pad.md
+-rw-r--r--   0        0        0      852 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/user-guide/how-to-restructure-rename-records.md
+-rw-r--r--   0        0        0      832 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/user-guide/how-to-restructure-sort.md
+-rw-r--r--   0        0        0     9624 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/user-guide/how-to-restructure-zip-project.md
+-rw-r--r--   0        0        0      273 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/user-guide/how-to-restructure.md
+-rw-r--r--   0        0        0     2599 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/user-guide/how-to-specialize-differentiate-jax.md
+-rw-r--r--   0        0        0      870 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/user-guide/how-to-specialize-in-numba.md
+-rw-r--r--   0        0        0      838 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/user-guide/how-to-specialize-lorentz.md
+-rw-r--r--   0        0        0      874 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/user-guide/how-to-specialize-override-numpy.md
+-rw-r--r--   0        0        0      870 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/user-guide/how-to-specialize-subclass.md
+-rw-r--r--   0        0        0      277 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/user-guide/how-to-specialize.md
+-rw-r--r--   0        0        0    11724 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/user-guide/how-to-use-header-only-layoutbuilder.md
+-rw-r--r--   0        0        0      900 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/user-guide/how-to-use-in-numba-arraybuilder.md
+-rw-r--r--   0        0        0     9973 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/user-guide/how-to-use-in-numba-cuda.ipynb
+-rw-r--r--   0        0        0      900 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/user-guide/how-to-use-in-numba-features.md
+-rw-r--r--   0        0        0      279 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/user-guide/how-to-use-in-numba.md
+-rw-r--r--   0        0        0      344 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/user-guide/index.md
+-rw-r--r--   0        0        0        0 2023-06-15 15:47:29.000000 awkward-2.2.4/docs/user-guide/requirements.txt
+-rw-r--r--   0        0        0   367587 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/panel-data-analysts.png
+-rw-r--r--   0        0        0   794465 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/panel-data-analysts.svg
+-rw-r--r--   0        0        0   140700 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/panel-developers.png
+-rw-r--r--   0        0        0   328307 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/panel-developers.svg
+-rw-r--r--   0        0        0    73584 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/panel-doxygen.png
+-rw-r--r--   0        0        0    58179 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/panel-sphinx.png
+-rw-r--r--   0        0        0   127063 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/panel-tutorials-alternate.png
+-rw-r--r--   0        0        0   173327 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/panel-tutorials.png
+-rw-r--r--   0        0        0    12541 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/diagrams/awkward-1-0-layers.pdf
+-rw-r--r--   0        0        0    65246 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/diagrams/awkward-1-0-layers.png
+-rw-r--r--   0        0        0    41004 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/diagrams/awkward-1-0-layers.svg
+-rw-r--r--   0        0        0    14946 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/diagrams/awkward-timeline.pdf
+-rw-r--r--   0        0        0   125180 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/diagrams/awkward-timeline.png
+-rw-r--r--   0        0        0    70209 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/diagrams/awkward-timeline.svg
+-rw-r--r--   0        0        0   436595 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/diagrams/awkward-uproot-timeline-pip-github.png
+-rw-r--r--   0        0        0   426911 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/diagrams/awkward-uproot-timeline-pip-github.svg
+-rw-r--r--   0        0        0   335955 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/diagrams/awkward-uproot-timeline-pip.png
+-rw-r--r--   0        0        0   325268 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/diagrams/awkward-uproot-timeline-pip.svg
+-rw-r--r--   0        0        0   129696 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/diagrams/awkward-uproot-timeline.png
+-rw-r--r--   0        0        0   120554 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/diagrams/awkward-uproot-timeline.svg
+-rw-r--r--   0        0        0     5208 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/diagrams/cartoon-broadcasting.png
+-rw-r--r--   0        0        0    25065 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/diagrams/cartoon-broadcasting.svg
+-rw-r--r--   0        0        0     5754 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/diagrams/cartoon-cartesian.png
+-rw-r--r--   0        0        0    32616 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/diagrams/cartoon-cartesian.svg
+-rw-r--r--   0        0        0     9584 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/diagrams/cartoon-combinations.png
+-rw-r--r--   0        0        0    39524 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/diagrams/cartoon-combinations.svg
+-rw-r--r--   0        0        0    10808 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/diagrams/cartoon-schematic.png
+-rw-r--r--   0        0        0    25779 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/diagrams/cartoon-schematic.svg
+-rw-r--r--   0        0        0    18178 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/diagrams/example-array.svg
+-rw-r--r--   0        0        0    36024 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/diagrams/example-hierarchy.png
+-rw-r--r--   0        0        0    17092 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/diagrams/example-hierarchy.svg
+-rw-r--r--   0        0        0    21120 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/diagrams/example-reduction-sum-only.svg
+-rw-r--r--   0        0        0    29325 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/diagrams/example-reduction-sum.svg
+-rw-r--r--   0        0        0    55553 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/diagrams/example-reduction.png
+-rw-r--r--   0        0        0    21631 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/diagrams/example-reduction.svg
+-rw-r--r--   0        0        0    10978 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/diagrams/git-strategy.pdf
+-rw-r--r--   0        0        0    58904 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/diagrams/git-strategy.png
+-rw-r--r--   0        0        0    28990 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/diagrams/git-strategy.svg
+-rw-r--r--   0        0        0   113587 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/diagrams/how-it-works-muons.png
+-rw-r--r--   0        0        0    57471 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/diagrams/how-it-works-muons.svg
+-rw-r--r--   0        0        0    58475 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/diagrams/how-it-works.svg
+-rw-r--r--   0        0        0    63989 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/diagrams/sorting-axis.svg
+-rw-r--r--   0        0        0   124038 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/diagrams/reducers/all.svg
+-rw-r--r--   0        0        0   128558 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/diagrams/reducers/any.svg
+-rw-r--r--   0        0        0   134490 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/diagrams/reducers/argmax.svg
+-rw-r--r--   0        0        0   133192 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/diagrams/reducers/argmin.svg
+-rw-r--r--   0        0        0   106277 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/diagrams/reducers/count.svg
+-rw-r--r--   0        0        0   116417 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/diagrams/reducers/count_nonzero.svg
+-rw-r--r--   0        0        0   111789 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/diagrams/reducers/max.svg
+-rw-r--r--   0        0        0   109239 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/diagrams/reducers/min.svg
+-rw-r--r--   0        0        0   124702 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/diagrams/reducers/product.svg
+-rw-r--r--   0        0        0   108897 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/diagrams/reducers/sum.svg
+-rw-r--r--   0        0        0     8347 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/logo/favicon.ico
+-rw-r--r--   0        0        0     8984 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/logo/logo-300px-white.png
+-rw-r--r--   0        0        0    11964 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/logo/logo-300px.png
+-rw-r--r--   0        0        0    24707 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/logo/logo-600px.png
+-rw-r--r--   0        0        0    18767 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/logo/logo.svg
+-rw-r--r--   0        0        0    90413 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/photos/desire-path.jpg
+-rw-r--r--   0        0        0    52113 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/plots/awkward-0-popularity.pdf
+-rw-r--r--   0        0        0   146109 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/plots/awkward-0-popularity.png
+-rw-r--r--   0        0        0   147576 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/plots/awkward-0-popularity.svg
+-rw-r--r--   0        0        0    26938 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/plots/bikeroutes-scaling.svg
+-rw-r--r--   0        0        0     8891 2023-06-15 15:47:29.000000 awkward-2.2.4/docs-img/screenshots/github-issues-documentation.png
+-rw-r--r--   0        0        0     1325 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/__init__.py
+-rw-r--r--   0        0        0     4626 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_behavior.py
+-rw-r--r--   0        0        0    38827 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_broadcasting.py
+-rw-r--r--   0        0        0     2221 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_dispatch.py
+-rw-r--r--   0        0        0    13672 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_do.py
+-rw-r--r--   0        0        0    14536 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_errors.py
+-rw-r--r--   0        0        0     5727 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_kernels.py
+-rw-r--r--   0        0        0     5860 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_layout.py
+-rw-r--r--   0        0        0     9983 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_lookup.py
+-rw-r--r--   0        0        0     8456 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_operators.py
+-rw-r--r--   0        0        0     5454 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_parameters.py
+-rw-r--r--   0        0        0     9965 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_prettyprint.py
+-rw-r--r--   0        0        0    28974 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_reducers.py
+-rw-r--r--   0        0        0     1492 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_regularize.py
+-rw-r--r--   0        0        0      420 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_singleton.py
+-rw-r--r--   0        0        0    23934 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_slicing.py
+-rw-r--r--   0        0        0      647 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_typetracer.py
+-rw-r--r--   0        0        0     1163 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_typing.py
+-rw-r--r--   0        0        0     2263 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_util.py
+-rw-r--r--   0        0        0      758 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_v2.py
+-rw-r--r--   0        0        0      233 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/builder.py
+-rw-r--r--   0        0        0      866 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/cppyy.py
+-rw-r--r--   0        0        0      271 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/forth.py
+-rw-r--r--   0        0        0   102730 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/highlevel.py
+-rw-r--r--   0        0        0     8044 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/index.py
+-rw-r--r--   0        0        0     3988 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/jax.py
+-rw-r--r--   0        0        0     6052 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/numba.py
+-rw-r--r--   0        0        0     8272 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/record.py
+-rw-r--r--   0        0        0     1679 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/typetracer.py
+-rw-r--r--   0        0        0        0 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_backends/__init__.py
+-rw-r--r--   0        0        0     2082 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_backends/backend.py
+-rw-r--r--   0        0        0     1259 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_backends/cupy.py
+-rw-r--r--   0        0        0     3763 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_backends/dispatch.py
+-rw-r--r--   0        0        0     1453 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_backends/jax.py
+-rw-r--r--   0        0        0      944 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_backends/numpy.py
+-rw-r--r--   0        0        0     1425 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_backends/typetracer.py
+-rw-r--r--   0        0        0       88 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/__init__.py
+-rw-r--r--   0        0        0    32504 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/avro.py
+-rw-r--r--   0        0        0    53532 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cling.py
+-rw-r--r--   0        0        0      985 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/hist.py
+-rw-r--r--   0        0        0     4491 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/numexpr.py
+-rw-r--r--   0        0        0    11582 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/numpy.py
+-rw-r--r--   0        0        0    38024 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/pyarrow.py
+-rw-r--r--   0        0        0     7038 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/__init__.py
+-rw-r--r--   0        0        0     2555 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_BitMaskedArray_to_ByteMaskedArray.cu
+-rw-r--r--   0        0        0     4326 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_BitMaskedArray_to_IndexedOptionArray.cu
+-rw-r--r--   0        0        0      987 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_getitem_carry.cu
+-rw-r--r--   0        0        0     2542 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_getitem_nextcarry.cu
+-rw-r--r--   0        0        0     3034 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_getitem_nextcarry_outindex.cu
+-rw-r--r--   0        0        0      630 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_mask.cu
+-rw-r--r--   0        0        0      830 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_overlay_mask.cu
+-rw-r--r--   0        0        0     3196 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_reduce_next_64.cu
+-rw-r--r--   0        0        0     2668 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_reduce_next_nonlocal_nextshifts_64.cu
+-rw-r--r--   0        0        0      749 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_toIndexedOptionArray.cu
+-rw-r--r--   0        0        0     2749 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_Content_getitem_next_missing_jagged_getmaskstartstop.cu
+-rw-r--r--   0        0        0      552 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_Index_to_Index64.cu
+-rw-r--r--   0        0        0      637 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_fill_count.cu
+-rw-r--r--   0        0        0     2886 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_flatten_nextcarry.cu
+-rw-r--r--   0        0        0     2904 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_getitem_nextcarry.cu
+-rw-r--r--   0        0        0     3416 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_getitem_nextcarry_outindex.cu
+-rw-r--r--   0        0        0     3531 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_getitem_nextcarry_outindex_mask.cu
+-rw-r--r--   0        0        0      556 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_mask.cu
+-rw-r--r--   0        0        0      695 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_overlay_mask.cu
+-rw-r--r--   0        0        0     3036 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_64.cu
+-rw-r--r--   0        0        0      795 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_fix_offsets_64.cu
+-rw-r--r--   0        0        0     2523 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_nonlocal_nextshifts_64.cu
+-rw-r--r--   0        0        0     2729 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_nonlocal_nextshifts_fromshifts_64.cu
+-rw-r--r--   0        0        0     1035 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_simplify.cu
+-rw-r--r--   0        0        0      961 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_validity.cu
+-rw-r--r--   0        0        0     2593 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedOptionArray_rpad_and_clip_mask_axis1.cu
+-rw-r--r--   0        0        0     1536 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_compact_offsets.cu
+-rw-r--r--   0        0        0     1710 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_getitem_jagged_expand.cu
+-rw-r--r--   0        0        0     2012 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_getitem_next_array.cu
+-rw-r--r--   0        0        0     1184 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_validity.cu
+-rw-r--r--   0        0        0      806 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_flatten_offsets.cu
+-rw-r--r--   0        0        0      744 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_reduce_global_startstop_64.cu
+-rw-r--r--   0        0        0     1169 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_rpad_and_clip_axis1.cu
+-rw-r--r--   0        0        0     1059 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_rpad_axis1.cu
+-rw-r--r--   0        0        0     3208 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_MaskedArray_getitem_next_jagged_project.cu
+-rw-r--r--   0        0        0      575 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_contiguous_init.cu
+-rw-r--r--   0        0        0      830 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_contiguous_next.cu
+-rw-r--r--   0        0        0      650 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_fill_tobool.cu
+-rw-r--r--   0        0        0     2610 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_boolean_nonzero.cu
+-rw-r--r--   0        0        0     1126 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_array.cu
+-rw-r--r--   0        0        0      951 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_array_advanced.cu
+-rw-r--r--   0        0        0      721 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_at.cu
+-rw-r--r--   0        0        0     1003 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_range.cu
+-rw-r--r--   0        0        0     1339 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_range_advanced.cu
+-rw-r--r--   0        0        0      835 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_reduce_adjust_starts_64.cu
+-rw-r--r--   0        0        0      975 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_reduce_adjust_starts_shifts_64.cu
+-rw-r--r--   0        0        0      802 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_reduce_mask_ByteMaskedArray_64.cu
+-rw-r--r--   0        0        0      789 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_carry.cu
+-rw-r--r--   0        0        0     1040 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_jagged_expand.cu
+-rw-r--r--   0        0        0     1020 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_array.cu
+-rw-r--r--   0        0        0     1045 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_array_advanced.cu
+-rw-r--r--   0        0        0      974 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_at.cu
+-rw-r--r--   0        0        0      946 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_range.cu
+-rw-r--r--   0        0        0      980 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_range_spreadadvanced.cu
+-rw-r--r--   0        0        0      663 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_localindex.cu
+-rw-r--r--   0        0        0      586 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_fillna.cu
+-rw-r--r--   0        0        0     2580 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_project.cu
+-rw-r--r--   0        0        0     1360 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_validity.cu
+-rw-r--r--   0        0        0      461 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_carry_arange.cu
+-rw-r--r--   0        0        0      534 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_combinations.cu
+-rw-r--r--   0        0        0      529 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_content_reduce_zeroparents_64.cu
+-rw-r--r--   0        0        0      830 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_index_carry.cu
+-rw-r--r--   0        0        0      636 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_index_carry_nocheck.cu
+-rw-r--r--   0        0        0      689 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_index_rpad_and_clip_axis1.cu
+-rw-r--r--   0        0        0      457 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_localindex.cu
+-rw-r--r--   0        0        0      830 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_missing_repeat.cu
+-rw-r--r--   0        0        0     2043 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmax.cu
+-rw-r--r--   0        0        0     2198 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmax_bool_64.cu
+-rw-r--r--   0        0        0     2043 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmin.cu
+-rw-r--r--   0        0        0     2198 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmin_bool_64.cu
+-rw-r--r--   0        0        0     3054 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_count_64.cu
+-rw-r--r--   0        0        0     3289 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_countnonzero.cu
+-rw-r--r--   0        0        0     2022 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_max.cu
+-rw-r--r--   0        0        0     2022 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_min.cu
+-rw-r--r--   0        0        0     3202 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_prod_bool.cu
+-rw-r--r--   0        0        0     3012 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum.cu
+-rw-r--r--   0        0        0     3171 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum_bool.cu
+-rw-r--r--   0        0        0     3439 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum_int32_bool_64.cu
+-rw-r--r--   0        0        0     3439 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum_int64_bool_64.cu
+-rw-r--r--   0        0        0      865 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_regularize_arrayslice.cu
+-rw-r--r--   0        0        0      443 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_zero_mask.cu
+-rw-r--r--   0        0        0     3195 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/cuda_common.cu
+-rw-r--r--   0        0        0     1859 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/header-only/awkward/BuilderOptions.h
+-rw-r--r--   0        0        0    19822 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/header-only/awkward/GrowableBuffer.h
+-rw-r--r--   0        0        0    89307 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/header-only/awkward/LayoutBuilder.h
+-rw-r--r--   0        0        0      298 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/header-only/awkward/demo_impl.h
+-rw-r--r--   0        0        0     8025 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/header-only/awkward/utils.h
+-rw-r--r--   0        0        0      239 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/jax/__init__.py
+-rw-r--r--   0        0        0    11085 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/jax/reducers.py
+-rw-r--r--   0        0        0     5982 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/jax/trees.py
+-rw-r--r--   0        0        0       88 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/numba/__init__.py
+-rw-r--r--   0        0        0    35828 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/numba/arrayview.py
+-rw-r--r--   0        0        0     1182 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/numba/arrayview_cuda.py
+-rw-r--r--   0        0        0    31510 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/numba/builder.py
+-rw-r--r--   0        0        0     9624 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/numba/growablebuffer.py
+-rw-r--r--   0        0        0    49133 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/numba/layout.py
+-rw-r--r--   0        0        0       88 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/rdataframe/__init__.py
+-rw-r--r--   0        0        0     9377 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/rdataframe/from_rdataframe.py
+-rw-r--r--   0        0        0     9922 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/rdataframe/to_rdataframe.py
+-rw-r--r--   0        0        0     1487 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_connect/rdataframe/include/rdataframe/jagged_builders.h
+-rw-r--r--   0        0        0     1111 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_nplikes/__init__.py
+-rw-r--r--   0        0        0    16149 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_nplikes/array_module.py
+-rw-r--r--   0        0        0     5365 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_nplikes/cupy.py
+-rw-r--r--   0        0        0     1357 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_nplikes/dispatch.py
+-rw-r--r--   0        0        0     2276 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_nplikes/jax.py
+-rw-r--r--   0        0        0     3149 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_nplikes/numpy.py
+-rw-r--r--   0        0        0    14154 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_nplikes/numpylike.py
+-rw-r--r--   0        0        0     3579 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_nplikes/placeholder.py
+-rw-r--r--   0        0        0     2379 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_nplikes/shape.py
+-rw-r--r--   0        0        0    48309 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_nplikes/typetracer.py
+-rw-r--r--   0        0        0     2527 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/_nplikes/ufuncs.py
+-rw-r--r--   0        0        0       88 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/behaviors/__init__.py
+-rw-r--r--   0        0        0     3479 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/behaviors/categorical.py
+-rw-r--r--   0        0        0     3898 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/behaviors/mixins.py
+-rw-r--r--   0        0        0     7884 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/behaviors/string.py
+-rw-r--r--   0        0        0      986 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/contents/__init__.py
+-rw-r--r--   0        0        0    28289 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/contents/bitmaskedarray.py
+-rw-r--r--   0        0        0    41835 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/contents/bytemaskedarray.py
+-rw-r--r--   0        0        0    44583 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/contents/content.py
+-rw-r--r--   0        0        0    13853 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/contents/emptyarray.py
+-rw-r--r--   0        0        0    41644 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/contents/indexedarray.py
+-rw-r--r--   0        0        0    64475 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/contents/indexedoptionarray.py
+-rw-r--r--   0        0        0    62401 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/contents/listarray.py
+-rw-r--r--   0        0        0    84953 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/contents/listoffsetarray.py
+-rw-r--r--   0        0        0    48679 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/contents/numpyarray.py
+-rw-r--r--   0        0        0    46696 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/contents/recordarray.py
+-rw-r--r--   0        0        0    56591 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/contents/regulararray.py
+-rw-r--r--   0        0        0    61396 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/contents/unionarray.py
+-rw-r--r--   0        0        0    19483 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/contents/unmaskedarray.py
+-rw-r--r--   0        0        0      962 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/forms/__init__.py
+-rw-r--r--   0        0        0     6413 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/forms/bitmaskedform.py
+-rw-r--r--   0        0        0     5668 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/forms/bytemaskedform.py
+-rw-r--r--   0        0        0     4443 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/forms/emptyform.py
+-rw-r--r--   0        0        0    21398 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/forms/form.py
+-rw-r--r--   0        0        0     6020 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/forms/indexedform.py
+-rw-r--r--   0        0        0     5416 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/forms/indexedoptionform.py
+-rw-r--r--   0        0        0     5904 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/forms/listform.py
+-rw-r--r--   0        0        0     5127 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/forms/listoffsetform.py
+-rw-r--r--   0        0        0     6350 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/forms/numpyform.py
+-rw-r--r--   0        0        0     8967 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/forms/recordform.py
+-rw-r--r--   0        0        0     5339 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/forms/regularform.py
+-rw-r--r--   0        0        0     8125 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/forms/unionform.py
+-rw-r--r--   0        0        0     4478 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/forms/unmaskedform.py
+-rw-r--r--   0        0        0     4828 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/__init__.py
+-rw-r--r--   0        0        0     3332 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_all.py
+-rw-r--r--   0        0        0     8301 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_almost_equal.py
+-rw-r--r--   0        0        0     3335 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_any.py
+-rw-r--r--   0        0        0     5019 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_argcartesian.py
+-rw-r--r--   0        0        0     3513 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_argcombinations.py
+-rw-r--r--   0        0        0     5561 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_argmax.py
+-rw-r--r--   0        0        0     5518 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_argmin.py
+-rw-r--r--   0        0        0     2998 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_argsort.py
+-rw-r--r--   0        0        0      943 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_backend.py
+-rw-r--r--   0        0        0     9540 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_broadcast_arrays.py
+-rw-r--r--   0        0        0     6499 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_broadcast_fields.py
+-rw-r--r--   0        0        0    15528 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_cartesian.py
+-rw-r--r--   0        0        0     1418 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_categories.py
+-rw-r--r--   0        0        0     7815 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_combinations.py
+-rw-r--r--   0        0        0    12728 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_concatenate.py
+-rw-r--r--   0        0        0     2737 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_copy.py
+-rw-r--r--   0        0        0     5151 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_corr.py
+-rw-r--r--   0        0        0     4560 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_count.py
+-rw-r--r--   0        0        0     3359 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_count_nonzero.py
+-rw-r--r--   0        0        0     4503 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_covar.py
+-rw-r--r--   0        0        0     4544 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_drop_none.py
+-rw-r--r--   0        0        0    50327 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_enforce_type.py
+-rw-r--r--   0        0        0     1131 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_fields.py
+-rw-r--r--   0        0        0     5203 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_fill_none.py
+-rw-r--r--   0        0        0     3433 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_firsts.py
+-rw-r--r--   0        0        0     7767 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_flatten.py
+-rw-r--r--   0        0        0     2975 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_from_arrow.py
+-rw-r--r--   0        0        0      748 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_from_arrow_schema.py
+-rw-r--r--   0        0        0     2417 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_from_avro_file.py
+-rw-r--r--   0        0        0    14159 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_from_buffers.py
+-rw-r--r--   0        0        0     1809 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_from_categorical.py
+-rw-r--r--   0        0        0     1446 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_from_cupy.py
+-rw-r--r--   0        0        0     3872 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_from_iter.py
+-rw-r--r--   0        0        0     1522 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_from_jax.py
+-rw-r--r--   0        0        0    29428 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_from_json.py
+-rw-r--r--   0        0        0     2036 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_from_numpy.py
+-rw-r--r--   0        0        0    11457 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_from_parquet.py
+-rw-r--r--   0        0        0     3025 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_from_rdataframe.py
+-rw-r--r--   0        0        0     2960 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_from_regular.py
+-rw-r--r--   0        0        0     8680 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_full_like.py
+-rw-r--r--   0        0        0      890 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_is_categorical.py
+-rw-r--r--   0        0        0     2478 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_is_none.py
+-rw-r--r--   0        0        0      728 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_is_tuple.py
+-rw-r--r--   0        0        0      929 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_is_valid.py
+-rw-r--r--   0        0        0     2396 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_isclose.py
+-rw-r--r--   0        0        0     8760 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_linear_fit.py
+-rw-r--r--   0        0        0     3219 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_local_index.py
+-rw-r--r--   0        0        0     4627 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_mask.py
+-rw-r--r--   0        0        0     5926 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_max.py
+-rw-r--r--   0        0        0     7760 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_mean.py
+-rw-r--r--   0        0        0     3552 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_merge_option_of_records.py
+-rw-r--r--   0        0        0    12363 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_merge_union_of_records.py
+-rw-r--r--   0        0        0     3078 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_metadata_from_parquet.py
+-rw-r--r--   0        0        0     5948 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_min.py
+-rw-r--r--   0        0        0     4237 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_moment.py
+-rw-r--r--   0        0        0     2009 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_nan_to_none.py
+-rw-r--r--   0        0        0     4922 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_nan_to_num.py
+-rw-r--r--   0        0        0     3878 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_num.py
+-rw-r--r--   0        0        0     1800 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_ones_like.py
+-rw-r--r--   0        0        0     4211 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_pad_none.py
+-rw-r--r--   0        0        0     1807 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_parameters.py
+-rw-r--r--   0        0        0     5037 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_prod.py
+-rw-r--r--   0        0        0     4118 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_ptp.py
+-rw-r--r--   0        0        0     2256 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_ravel.py
+-rw-r--r--   0        0        0     9532 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_run_lengths.py
+-rw-r--r--   0        0        0     3025 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_singletons.py
+-rw-r--r--   0        0        0     2741 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_softmax.py
+-rw-r--r--   0        0        0     2513 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_sort.py
+-rw-r--r--   0        0        0     6788 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_std.py
+-rw-r--r--   0        0        0     3020 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_strings_astype.py
+-rw-r--r--   0        0        0    10397 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_sum.py
+-rw-r--r--   0        0        0     4573 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_to_arrow.py
+-rw-r--r--   0        0        0     6361 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_to_arrow_table.py
+-rw-r--r--   0        0        0     2267 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_to_backend.py
+-rw-r--r--   0        0        0     6144 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_to_buffers.py
+-rw-r--r--   0        0        0     6022 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_to_categorical.py
+-rw-r--r--   0        0        0     1131 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_to_cupy.py
+-rw-r--r--   0        0        0    13339 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_to_dataframe.py
+-rw-r--r--   0        0        0     1131 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_to_jax.py
+-rw-r--r--   0        0        0    11167 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_to_json.py
+-rw-r--r--   0        0        0     4357 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_to_layout.py
+-rw-r--r--   0        0        0     2636 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_to_list.py
+-rw-r--r--   0        0        0     2115 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_to_numpy.py
+-rw-r--r--   0        0        0     3331 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_to_packed.py
+-rw-r--r--   0        0        0    17406 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_to_parquet.py
+-rw-r--r--   0        0        0     2797 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_to_rdataframe.py
+-rw-r--r--   0        0        0     3344 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_to_regular.py
+-rw-r--r--   0        0        0    23334 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_transform.py
+-rw-r--r--   0        0        0     4428 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_type.py
+-rw-r--r--   0        0        0     9335 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_unflatten.py
+-rw-r--r--   0        0        0     2465 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_unzip.py
+-rw-r--r--   0        0        0     1131 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_validity_error.py
+-rw-r--r--   0        0        0     2511 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_values_astype.py
+-rw-r--r--   0        0        0     8016 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_var.py
+-rw-r--r--   0        0        0     5505 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_where.py
+-rw-r--r--   0        0        0     6008 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_with_field.py
+-rw-r--r--   0        0        0     2563 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_with_name.py
+-rw-r--r--   0        0        0     1709 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_with_parameter.py
+-rw-r--r--   0        0        0     3713 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_without_field.py
+-rw-r--r--   0        0        0     1477 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_without_parameters.py
+-rw-r--r--   0        0        0     1982 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_zeros_like.py
+-rw-r--r--   0        0        0     8602 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/operations/ak_zip.py
+-rw-r--r--   0        0        0      707 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/types/__init__.py
+-rw-r--r--   0        0        0   163323 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/types/_awkward_datashape_parser.py
+-rw-r--r--   0        0        0     2168 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/types/arraytype.py
+-rw-r--r--   0        0        0     3007 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/types/listtype.py
+-rw-r--r--   0        0        0     6171 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/types/numpytype.py
+-rw-r--r--   0        0        0     4886 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/types/optiontype.py
+-rw-r--r--   0        0        0     8774 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/types/recordtype.py
+-rw-r--r--   0        0        0     3928 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/types/regulartype.py
+-rw-r--r--   0        0        0     1341 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/types/scalartype.py
+-rw-r--r--   0        0        0    10063 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/types/type.py
+-rw-r--r--   0        0        0     4593 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/types/uniontype.py
+-rw-r--r--   0        0        0     2489 2023-06-15 15:47:29.000000 awkward-2.2.4/src/awkward/types/unknowntype.py
+-rw-r--r--   0        0        0       88 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/__init__.py
+-rw-r--r--   0        0        0     3358 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0002_minimal_listarray.py
+-rw-r--r--   0        0        0      487 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0006_deep_iteration.py
+-rw-r--r--   0        0        0     5565 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0008_slices_and_getitem.py
+-rw-r--r--   0        0        0    13378 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0011_listarray.py
+-rw-r--r--   0        0        0     4462 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0013_error_handling_struct.py
+-rw-r--r--   0        0        0    17019 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0014_finish_up_getitem.py
+-rw-r--r--   0        0        0     5169 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0018_fromiter_fillable.py
+-rw-r--r--   0        0        0     8833 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0019_use_json_library.py
+-rw-r--r--   0        0        0    13687 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0020_support_unsigned_indexes.py
+-rw-r--r--   0        0        0     6391 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0021_emptyarray.py
+-rw-r--r--   0        0        0    10743 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0023_regular_array.py
+-rw-r--r--   0        0        0     4890 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0024_use_regular_array.py
+-rw-r--r--   0        0        0    25581 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0025_record_array.py
+-rw-r--r--   0        0        0     3436 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0028_add_dressed_types.py
+-rw-r--r--   0        0        0     6321 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0032_replace_dressedtype.py
+-rw-r--r--   0        0        0    12027 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0046_start_indexedarray.py
+-rw-r--r--   0        0        0      898 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0049_distinguish_record_and_recordarray_behaviors.py
+-rw-r--r--   0        0        0    12231 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0057_introducing_forms.py
+-rw-r--r--   0        0        0     5430 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0070_argmin_and_argmax.py
+-rw-r--r--   0        0        0     5384 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0072_fillna_operation.py
+-rw-r--r--   0        0        0    15655 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0074_argsort_and_sort.py
+-rw-r--r--   0        0        0     2836 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0077_zip_operation.py
+-rw-r--r--   0        0        0    11934 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0078_argcross_and_cross.py
+-rw-r--r--   0        0        0    12124 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0079_argchoose_and_choose.py
+-rw-r--r--   0        0        0     7071 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0080_flatpandas_multiindex_rows_and_columns.py
+-rw-r--r--   0        0        0     6615 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0084_start_unionarray.py
+-rw-r--r--   0        0        0     6551 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0086_nep13_ufunc.py
+-rw-r--r--   0        0        0    12540 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0089_numpy_functions.py
+-rw-r--r--   0        0        0    46684 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0093_simplify_uniontypes_and_optiontypes.py
+-rw-r--r--   0        0        0     6959 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0107_assign_fields_to_records.py
+-rw-r--r--   0        0        0    46658 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0111_jagged_and_masked_getitem.py
+-rw-r--r--   0        0        0    77410 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0115_generic_reducer_operation.py
+-rw-r--r--   0        0        0    35162 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0118_numba_cpointers.py
+-rw-r--r--   0        0        0     1091 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0119_numexpr_and_broadcast_arrays.py
+-rw-r--r--   0        0        0     1106 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0124_strings_in_numba.py
+-rw-r--r--   0        0        0    32114 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0127_tomask_operation.py
+-rw-r--r--   0        0        0     3683 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0127b_tomask_operation_numba.py
+-rw-r--r--   0        0        0      838 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0138_emptyarray_type.py
+-rw-r--r--   0        0        0    17923 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0150_flatten.py
+-rw-r--r--   0        0        0     3602 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0163_negative_axis_wrap.py
+-rw-r--r--   0        0        0     9779 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0166_0167_0170_random_issues.py
+-rw-r--r--   0        0        0     4552 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0173_astype_operation.py
+-rw-r--r--   0        0        0    24034 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0184_concatenate_operation.py
+-rw-r--r--   0        0        0     2063 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0193_is_none_axis_parameter.py
+-rw-r--r--   0        0        0     3352 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0198_tutorial_documentation_1.py
+-rw-r--r--   0        0        0     8998 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0222_count_with_axis0.py
+-rw-r--r--   0        0        0    75605 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0224_arrow_to_awkward.py
+-rw-r--r--   0        0        0      581 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0264_reduce_last_empty.py
+-rw-r--r--   0        0        0     3251 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0273_path_for_with_field.py
+-rw-r--r--   0        0        0      743 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0286_broadcast_single_value_with_field.py
+-rw-r--r--   0        0        0     2205 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0290_bug_fixes_for_hats.py
+-rw-r--r--   0        0        0     4806 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0315_integerindex.py
+-rw-r--r--   0        0        0     5745 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0331_pandas_indexedarray.py
+-rw-r--r--   0        0        0     1257 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0334_fully_broadcastable_where.py
+-rw-r--r--   0        0        0      566 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0339_highlevel_sorting_function.py
+-rw-r--r--   0        0        0     6757 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0348_form_keys.py
+-rw-r--r--   0        0        0     4523 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0355_mixins.py
+-rw-r--r--   0        0        0    10396 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0395_complex_type_arrays.py
+-rw-r--r--   0        0        0     4934 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0395_fix_numba_indexedarray.py
+-rw-r--r--   0        0        0     3212 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0397_arrays_as_constants_in_numba.py
+-rw-r--r--   0        0        0    14529 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0401_add_categorical_type_for_arrow_dictionary.py
+-rw-r--r--   0        0        0    22467 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0404_array_validity_check.py
+-rw-r--r--   0        0        0    14282 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0410_fix_argminmax_positions_for_missing_values.py
+-rw-r--r--   0        0        0    17455 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0437_stream_of_many_json_files.py
+-rw-r--r--   0        0        0    32921 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0447_preserve_regularness_in_reduce.py
+-rw-r--r--   0        0        0    24075 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0449_merge_many_arrays_in_one_pass.py
+-rw-r--r--   0        0        0     4059 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0493_zeros_ones_full_like.py
+-rw-r--r--   0        0        0     1606 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0496_provide_local_index.py
+-rw-r--r--   0        0        0     2059 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0499_getitem_indexedarray_bug.py
+-rw-r--r--   0        0        0     1286 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0504_block_ufuncs_for_strings.py
+-rw-r--r--   0        0        0     2926 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0511_copy_and_deepcopy.py
+-rw-r--r--   0        0        0     9119 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0527_fix_unionarray_ufuncs_and_parameters_in_merging.py
+-rw-r--r--   0        0        0      365 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0546_fill_none_replacement_value_type.py
+-rw-r--r--   0        0        0     1102 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0549_numba_array_asarray.py
+-rw-r--r--   0        0        0     4268 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0557_min_max_initial_argument.py
+-rw-r--r--   0        0        0      537 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0559_fix_booleans_in_numba.py
+-rw-r--r--   0        0        0      636 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0572_numba_array_ndim.py
+-rw-r--r--   0        0        0     4901 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0582_propagate_context_in_broadcast_and_apply.py
+-rw-r--r--   0        0        0     1099 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0583_implement_unflatten_function.py
+-rw-r--r--   0        0        0     3084 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0590_allow_regulararray_size_zero.py
+-rw-r--r--   0        0        0     5957 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0593_preserve_nullability_in_arrow_and_parquet.py
+-rw-r--r--   0        0        0      478 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0627_behavior_from_dict_of_arrays.py
+-rw-r--r--   0        0        0     8205 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0652_tests_of_complex_numbers.py
+-rw-r--r--   0        0        0     2335 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0674_categorical_validation.py
+-rw-r--r--   0        0        0      750 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0713_getitem_field_should_simplify_optiontype.py
+-rw-r--r--   0        0        0     1242 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0723_ensure_that_jagged_slice_fits_array_length.py
+-rw-r--r--   0        0        0     1055 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0730_unflatten_axis_parameter.py
+-rw-r--r--   0        0        0     2569 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0733_run_lengths.py
+-rw-r--r--   0        0        0     2127 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0736_implement_argsort_for_strings.py
+-rw-r--r--   0        0        0      330 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0758_ak_zip_scallars.py
+-rw-r--r--   0        0        0     1122 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0766_prevent_combinations_of_characters.py
+-rw-r--r--   0        0        0    26349 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0773_typeparser.py
+-rw-r--r--   0        0        0      779 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0788_indexedarray_carrying_recordarray_parameters.py
+-rw-r--r--   0        0        0      871 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0794_ak_cartesian_on_empty_array.py
+-rw-r--r--   0        0        0     1148 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0803_argsort_fix_type.py
+-rw-r--r--   0        0        0     1364 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0806_empty_lists_cartesian_fix.py
+-rw-r--r--   0        0        0     6311 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0813_full_like_dtype_arg.py
+-rw-r--r--   0        0        0     1661 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0815_broadcast_union_types_to_all_possibilities.py
+-rw-r--r--   0        0        0      488 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0819_issue.py
+-rw-r--r--   0        0        0      682 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0828_arrow_datatype_null.py
+-rw-r--r--   0        0        0    23609 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0835_datetime_type.py
+-rw-r--r--   0        0        0      676 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0835_datetime_type_pandas.py
+-rw-r--r--   0        0        0     4662 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0835_datetime_type_pyarrow.py
+-rw-r--r--   0        0        0      680 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0850_argsort_mask_array.py
+-rw-r--r--   0        0        0      449 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0863_is_none_numpy_array.py
+-rw-r--r--   0        0        0     1029 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0866_getitem_field_and_flatten_unions.py
+-rw-r--r--   0        0        0      929 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0875_arrow_null_type.py
+-rw-r--r--   0        0        0      901 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0879_non_primitive_with_field.py
+-rw-r--r--   0        0        0      563 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0884_index_and_identifier_refactoring.py
+-rw-r--r--   0        0        0     1086 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0889_ptp.py
+-rw-r--r--   0        0        0    53355 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0896_content_classes_refactoring.py
+-rw-r--r--   0        0        0     1751 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0898_unzip_heterogeneous_records.py
+-rw-r--r--   0        0        0      421 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0903_ArrayView_expects_contiguous_NumpyArrays.py
+-rw-r--r--   0        0        0      530 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0905_leading_zeros_in_unflatten.py
+-rw-r--r--   0        0        0     1048 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0906_arrow_fixed_size_list_type.py
+-rw-r--r--   0        0        0      666 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0910_unflatten_counts_relation.py
+-rw-r--r--   0        0        0     5261 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0912_packed.py
+-rw-r--r--   0        0        0   115270 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0914_types_and_forms.py
+-rw-r--r--   0        0        0     1877 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0916_datetime_values_astype.py
+-rw-r--r--   0        0        0     5522 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0927_numpy_array_nbytes.py
+-rw-r--r--   0        0        0      709 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0930_bug_in_unionarray_purelist_parameter.py
+-rw-r--r--   0        0        0     1627 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0945_argsort_sort_nan_array.py
+-rw-r--r--   0        0        0    28028 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0958_new_forms_must_accept_old_form_json.py
+-rw-r--r--   0        0        0    28284 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0959__getitem_array_implementation.py
+-rw-r--r--   0        0        0      651 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0975_mask_multidimensional_numpy_array.py
+-rw-r--r--   0        0        0      644 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0979_where_multidimentional_numpy_array.py
+-rw-r--r--   0        0        0     5803 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0982_missing_case_in_nonlocal_reducers.py
+-rw-r--r--   0        0        0     1976 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0984_ravel.py
+-rw-r--r--   0        0        0     1806 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_0992_correct_ptp_unmasking.py
+-rw-r--r--   0        0        0     2100 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1000_fixes_argmax_for_ListOffsetArray_with_nonzero_start.py
+-rw-r--r--   0        0        0      429 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1006_packed_regular_array_zero_size.py
+-rw-r--r--   0        0        0      416 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1007_from_buffers_empty_ndarray.py
+-rw-r--r--   0        0        0      551 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1017_numpyarray_broadcast.py
+-rw-r--r--   0        0        0      785 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1030_mixin_class_name.py
+-rw-r--r--   0        0        0    52114 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1031_start_getitem_next.py
+-rw-r--r--   0        0        0    18007 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1031b_start_getitem_next_specialized.py
+-rw-r--r--   0        0        0     1146 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1049_concatenate_single_array.py
+-rw-r--r--   0        0        0     1559 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1055_fill_none_numpy_dimension.py
+-rw-r--r--   0        0        0    42250 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1059_localindex.py
+-rw-r--r--   0        0        0      551 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1066_to_numpy_masked_structured_array.py
+-rw-r--r--   0        0        0      685 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1071_mask_identity_false_should_not_return_option_type.py
+-rw-r--r--   0        0        0    27714 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1072_sort.py
+-rw-r--r--   0        0        0    44140 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1074_combinations.py
+-rw-r--r--   0        0        0     5181 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1075_validityerror.py
+-rw-r--r--   0        0        0      273 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1106_argminmax_axis_None_missing_values.py
+-rw-r--r--   0        0        0    25531 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1110_type_tracer_1.py
+-rw-r--r--   0        0        0     1870 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1116_project_maskedarrays.py
+-rw-r--r--   0        0        0    28454 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1125_to_arrow_from_arrow.py
+-rw-r--r--   0        0        0     6276 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1132_utility_methods_for_highlevel_functions.py
+-rw-r--r--   0        0        0    21098 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1134_from_buffers_to_buffers.py
+-rw-r--r--   0        0        0    57322 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1135_rpad_operation.py
+-rw-r--r--   0        0        0     4639 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1136_regulararray_zeros_in_shape.py
+-rw-r--r--   0        0        0    10487 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1137_num.py
+-rw-r--r--   0        0        0    10222 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1142_numbers_to_type.py
+-rw-r--r--   0        0        0     2559 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1149_datetime_sort.py
+-rw-r--r--   0        0        0      630 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1154_arrow_tables_should_preserve_parameters.py
+-rw-r--r--   0        0        0    27983 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1162_ak_from_json_schema.py
+-rw-r--r--   0        0        0      766 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1183_bugs_found_by_dask_project_2.py
+-rw-r--r--   0        0        0     1286 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1189_fix_singletons_for_non_optional_data.py
+-rw-r--r--   0        0        0      551 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1192_iterables_in___array_function__.py
+-rw-r--r--   0        0        0      608 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1193_is_none_nested_option.py
+-rw-r--r--   0        0        0     2601 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1233_ak_with_name.py
+-rw-r--r--   0        0        0    26468 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1240_v2_implementation_of_numba_1.py
+-rw-r--r--   0        0        0     1146 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1259_simplify_optiontype.py
+-rw-r--r--   0        0        0     1560 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1260_simplify_masked_option_types.py
+-rw-r--r--   0        0        0      681 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1271_fix_4D_reducers.py
+-rw-r--r--   0        0        0    33243 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1294_to_and_from_parquet.py
+-rw-r--r--   0        0        0     1945 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1298_allow_nan_to_num_arguments_to_be_arrays.py
+-rw-r--r--   0        0        0    62340 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1300_awkward_to_cpp_converter_with_cling.py
+-rw-r--r--   0        0        0    39474 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1300b_same_for_numba.py
+-rw-r--r--   0        0        0      367 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1305_mixed_awkward_numpy_slicing.py
+-rw-r--r--   0        0        0     1702 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1308_zip_after_option.py
+-rw-r--r--   0        0        0     1703 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1318_array_function_types.py
+-rw-r--r--   0        0        0     1730 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1320_mask_identity_defaults.py
+-rw-r--r--   0        0        0      647 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1344_broadcast_arrays_depth_limit.py
+-rw-r--r--   0        0        0     6621 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1345_avro_reader.py
+-rw-r--r--   0        0        0     4562 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1351_is_tuple.py
+-rw-r--r--   0        0        0     8362 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1374_to_rdataframe.py
+-rw-r--r--   0        0        0     1755 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1377_ravel_string.py
+-rw-r--r--   0        0        0     1468 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1379_reducers_with_axis_None_and_typetracers.py
+-rw-r--r--   0        0        0     1384 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1399_from_jax.py
+-rw-r--r--   0        0        0     1227 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1399_to_jax.py
+-rw-r--r--   0        0        0      297 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1400_with_name_record.py
+-rw-r--r--   0        0        0      449 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1403_from_numpy_strings.py
+-rw-r--r--   0        0        0     3470 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1405_slicing_untested_cases.py
+-rw-r--r--   0        0        0     6909 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1415_behaviour_forwarding.py
+-rw-r--r--   0        0        0    18848 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1440_start_v2_to_parquet.py
+-rw-r--r--   0        0        0    14402 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1447_jax_autodiff_slices_ufuncs.py
+-rw-r--r--   0        0        0     8591 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1449_v2_to_json_from_json_functions.py
+-rw-r--r--   0        0        0      692 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1453_write_single_records_to_parquet.py
+-rw-r--r--   0        0        0     9828 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1473_from_rdataframe.py
+-rw-r--r--   0        0        0    24648 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1477_generator_entry_type_as_rvec.py
+-rw-r--r--   0        0        0     3579 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1490_jax_reducers_combinations.py
+-rw-r--r--   0        0        0     3905 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1502_getitem_jagged_issue1406.py
+-rw-r--r--   0        0        0     1733 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1504_typetracer_like.py
+-rw-r--r--   0        0        0     4913 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1508_awkward_from_rdataframe.py
+-rw-r--r--   0        0        0     2186 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1511_set_attribute.py
+-rw-r--r--   0        0        0      754 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1539_isnone_axis_check_issue1417.py
+-rw-r--r--   0        0        0     1570 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1559_fix_ufuncs_records_1439.py
+-rw-r--r--   0        0        0      990 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1565_axis_wrap_if_negative_record.py
+-rw-r--r--   0        0        0     1085 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1567_fix_longlong_in_Index.py
+-rw-r--r--   0        0        0     3022 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1568_fix_lengths_empty_regular_slices.py
+-rw-r--r--   0        0        0      385 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1578_to_arrow_empty_recordarray.py
+-rw-r--r--   0        0        0     5911 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1586_concatenate_should_preserve_regulararray.py
+-rw-r--r--   0        0        0      216 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1593_empty_slice_list_record.py
+-rw-r--r--   0        0        0     7260 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1604_preserve_form_in_concatenate.py
+-rw-r--r--   0        0        0     4372 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1607_no_reducers_on_records.py
+-rw-r--r--   0        0        0    10035 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1613_generator_tolayout_records.py
+-rw-r--r--   0        0        0      757 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1619_from_parquet_empty_field.py
+-rw-r--r--   0        0        0     6024 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1620_layout_builders.py
+-rw-r--r--   0        0        0     8122 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1625_multiple_columns_from_rdataframe.py
+-rw-r--r--   0        0        0      770 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1642_from_iter_of_tuples.py
+-rw-r--r--   0        0        0      389 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1644_concatenate_zeros_length.py
+-rw-r--r--   0        0        0     4317 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1650_Record_to_list_should_listify_itself.py
+-rw-r--r--   0        0        0      560 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1671_categorical_type.py
+-rw-r--r--   0        0        0    11761 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1672_broadcast_parameters.py
+-rw-r--r--   0        0        0     4453 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1677_array_builder_in_numba.py
+-rw-r--r--   0        0        0      544 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1685_IndexedArray_project_parameters.py
+-rw-r--r--   0        0        0      778 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1686_UnionArray_simplified_preserve_parameters.py
+-rw-r--r--   0        0        0      936 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1688_pack_categorical.py
+-rw-r--r--   0        0        0      525 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1703_fill_none_typetracer.py
+-rw-r--r--   0        0        0     1743 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1707_broadcast_parameters_ufunc.py
+-rw-r--r--   0        0        0      512 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1709_ak_array_constructor_behavior.py
+-rw-r--r--   0        0        0      398 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1735_from_numpy_mask.py
+-rw-r--r--   0        0        0      577 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1747_bytemaskedarray_mergemany.py
+-rw-r--r--   0        0        0      824 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1753_indexedarray_merge_kernel.py
+-rw-r--r--   0        0        0     1480 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1762_jax_behavior_support.py
+-rw-r--r--   0        0        0      589 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1764_jax_jacobian.py
+-rw-r--r--   0        0        0      962 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1765_add_ioanas_test_of_to_arraylib.py
+-rw-r--r--   0        0        0     4790 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1766_record_form_fields.py
+-rw-r--r--   0        0        0     2905 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1781_rdataframe_snapshot.py
+-rw-r--r--   0        0        0      701 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1784_reduce_leading_sublist.py
+-rw-r--r--   0        0        0      567 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1790_reduce_regulararray.py
+-rw-r--r--   0        0        0     4191 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1791_reduce_trailing_sublist.py
+-rw-r--r--   0        0        0     1027 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1794_run_lengths_empty_sublist.py
+-rw-r--r--   0        0        0      407 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1823_fill_none_axis_none.py
+-rw-r--r--   0        0        0      481 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1826_ravel_preserve_none.py
+-rw-r--r--   0        0        0     1451 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1829_to_from_rdataframe_bool.py
+-rw-r--r--   0        0        0      588 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1840_ak_type_to_handle_ndarray_dtype_and_nptypes.py
+-rw-r--r--   0        0        0     1097 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1847_numpy_array_contiguous.py
+-rw-r--r--   0        0        0      681 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1850_bytemasked_array_to_bytemaskedarray.py
+-rw-r--r--   0        0        0     1640 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1867_pass_behavior_through_combinations.py
+-rw-r--r--   0        0        0    17239 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1904_drop_none.py
+-rw-r--r--   0        0        0     3553 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1914_improved_axis_to_posaxis.py
+-rw-r--r--   0        0        0     4607 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1928_replace_simplify_method_with_classmethod_constructor.py
+-rw-r--r--   0        0        0      921 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1930_unflatten_counts_checks.py
+-rw-r--r--   0        0        0      769 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1936_with_field_broadcasting.py
+-rw-r--r--   0        0        0      551 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1940_ak_backend.py
+-rw-r--r--   0        0        0     1457 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1943_regular_indexing.py
+-rw-r--r--   0        0        0      188 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1944_to_numpy_empty_record_array.py
+-rw-r--r--   0        0        0     1131 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1960_awkward_from_rdataframe.py
+-rw-r--r--   0        0        0     3286 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1961_ak_without_field.py
+-rw-r--r--   0        0        0      280 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1978_akRecord_constructor_should_retain_type.py
+-rw-r--r--   0        0        0      349 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_1991_missed_a_NumpyArray_raw_call_without_underscore.py
+-rw-r--r--   0        0        0      371 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2008_ak_type_layout.py
+-rw-r--r--   0        0        0    10222 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2020_reduce_axis_none.py
+-rw-r--r--   0        0        0      803 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2021_check_TypeTracerArray_in_ak_where.py
+-rw-r--r--   0        0        0      645 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2023_from_rdataframe.py
+-rw-r--r--   0        0        0     2845 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2027_add_data_touch_reporting_to_TypeTracerArray.py
+-rw-r--r--   0        0        0     1219 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2047_ak_transform_regular_to_jagged.py
+-rw-r--r--   0        0        0      406 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2051_arraybuilder_behavior_propagation.py
+-rw-r--r--   0        0        0     1275 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2055_array_builder_check.py
+-rw-r--r--   0        0        0     1659 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2058_merge_numpy_array.py
+-rw-r--r--   0        0        0      708 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2064_fill_none_record.py
+-rw-r--r--   0        0        0      799 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2067_to_buffers_byteorder.py
+-rw-r--r--   0        0        0      741 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2070_to_layout_string.py
+-rw-r--r--   0        0        0     1172 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2071_unflatten_non_packed_counts.py
+-rw-r--r--   0        0        0      291 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2076_ak_unzip_record.py
+-rw-r--r--   0        0        0      545 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2078_array_function_wrap.py
+-rw-r--r--   0        0        0      589 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2082_broadcast_zero_size.py
+-rw-r--r--   0        0        0     1716 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2085_empty_if_typetracer.py
+-rw-r--r--   0        0        0     2765 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2096_ak_scalar_type.py
+-rw-r--r--   0        0        0      977 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2101_pickle_behavior_class.py
+-rw-r--r--   0        0        0      519 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2104_numpy_merge_option.py
+-rw-r--r--   0        0        0     2715 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2106_pickle_class.py
+-rw-r--r--   0        0        0      722 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2108_fill_none_indexed.py
+-rw-r--r--   0        0        0     2100 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2115_fix_up_typetracers.py
+-rw-r--r--   0        0        0      487 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2120_missing_field_error.py
+-rw-r--r--   0        0        0     1110 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2125_type_of_scalar.py
+-rw-r--r--   0        0        0     1893 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2150_typetracer_high_level_ufunc.py
+-rw-r--r--   0        0        0     1898 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2179_parameter_merging_rules.py
+-rw-r--r--   0        0        0      510 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2181_with_name_len.py
+-rw-r--r--   0        0        0     2957 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2185_merge_union_of_records.py
+-rw-r--r--   0        0        0      528 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2188_values_astype_turns_EmptyArray_into_NumpyArray.py
+-rw-r--r--   0        0        0     6369 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2192_union_absorb_indexed.py
+-rw-r--r--   0        0        0     6059 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2198_almost_equal.py
+-rw-r--r--   0        0        0     1252 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2202_filter_multiple_columns_from_rdataframe.py
+-rw-r--r--   0        0        0     1453 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2214_offset_bool_index.py
+-rw-r--r--   0        0        0      334 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2219_flatten_empty.py
+-rw-r--r--   0        0        0      663 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2226_slice_regulararray_typetracer.py
+-rw-r--r--   0        0        0     1728 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2229_getitem_range_slice.py
+-rw-r--r--   0        0        0     4003 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2234_from_rdataframe_keep_order.py
+-rw-r--r--   0        0        0     4104 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2236_merge_union_of_records_option.py
+-rw-r--r--   0        0        0      485 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2240_merge_union_parameters.py
+-rw-r--r--   0        0        0     1338 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2240_simplify_merge_as_union.py
+-rw-r--r--   0        0        0      512 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2246_slice_not_packed.py
+-rw-r--r--   0        0        0      733 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2250_full_like_bool.py
+-rw-r--r--   0        0        0     1835 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2258_from_rdataframe_with_arguments.py
+-rw-r--r--   0        0        0      492 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2259_run_lengths_typetracer.py
+-rw-r--r--   0        0        0      560 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2263_to_packed_list.py
+-rw-r--r--   0        0        0      315 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2266_fix_nan_to_num.py
+-rw-r--r--   0        0        0      909 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2267_broadcast_fields.py
+-rw-r--r--   0        0        0     1336 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2293_unflatten_typetracer.py
+-rw-r--r--   0        0        0      406 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2294_view_unknown_scalar.py
+-rw-r--r--   0        0        0      720 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2296_duplicate_field.py
+-rw-r--r--   0        0        0     2262 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2297_common_backend.py
+-rw-r--r--   0        0        0      455 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2304_index_typetracer.py
+-rw-r--r--   0        0        0      648 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2305_nep_18_lazy_conversion.py
+-rw-r--r--   0        0        0     2929 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2306_cppyy_git.py
+-rw-r--r--   0        0        0     4386 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2319_from_buffers_array.py
+-rw-r--r--   0        0        0      721 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2327_array_interface.py
+-rw-r--r--   0        0        0     1728 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2329_cartesian_broadcasting_fixes.py
+-rw-r--r--   0        0        0      489 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2346_broadcast_depth_limit.py
+-rw-r--r--   0        0        0    15615 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2349_growablebuffer_in_numba.py
+-rw-r--r--   0        0        0      618 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2354_ufunc_same_backend.py
+-rw-r--r--   0        0        0      647 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2355_to_backend_record.py
+-rw-r--r--   0        0        0     1435 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2361_typetracer_asarray_nd.py
+-rw-r--r--   0        0        0      934 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2364_empty_list_of_string.py
+-rw-r--r--   0        0        0    37200 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2365_enforce_type.py
+-rw-r--r--   0        0        0     2921 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2368_type_is_equal.py
+-rw-r--r--   0        0        0     5250 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2373_unzip_touching.py
+-rw-r--r--   0        0        0     5848 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2374_cartesian_touching.py
+-rw-r--r--   0        0        0     1037 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2385_with_field_empty_record.py
+-rw-r--r--   0        0        0      956 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2395_copy_asarray_touch.py
+-rw-r--r--   0        0        0      212 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2407_broadcast_no_arrays.py
+-rw-r--r--   0        0        0     1070 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2410_string_broadcast.py
+-rw-r--r--   0        0        0      800 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2411_cartesian_axis_validation.py
+-rw-r--r--   0        0        0      704 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2417_bytemasked_singletons.py
+-rw-r--r--   0        0        0      351 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2418_union_broadcast_unknown.py
+-rw-r--r--   0        0        0     1563 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2424_almost_equal_union_record.py
+-rw-r--r--   0        0        0     1211 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2425_forms_from_type.py
+-rw-r--r--   0        0        0      545 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2426_is_equal_to.py
+-rw-r--r--   0        0        0      495 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2444_minimal_listarray.py
+-rw-r--r--   0        0        0      857 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2471_flatten_string.py
+-rw-r--r--   0        0        0     1032 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2484_reduce_starts_empty.py
+-rw-r--r--   0        0        0      659 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2487_broadcast_list_offsets.py
+-rw-r--r--   0        0        0     1319 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2490_reduce_regulararray_positional.py
+-rw-r--r--   0        0        0     1816 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2495_concatenate_typetracer.py
+-rw-r--r--   0        0        0     3800 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2501_positional_record_reducer.py
+-rw-r--r--   0        0        0      603 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2503_deprecate_to_numpyform.py
+-rw-r--r--   0        0        0     4942 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2512_record_array_carry.py
+-rw-r--r--   0        0        0     1014 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2518_datetime_units_as_parameter.py
+-rw-r--r--   0        0        0     5946 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/test_2536_select_columns.py
+-rw-r--r--   0        0        0      128 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/samples/__init__.py
+-rw-r--r--   0        0        0      218 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/samples/array_enum_test_data.avro
+-rw-r--r--   0        0        0      176 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/samples/array_string_test_data.avro
+-rw-r--r--   0        0        0      152 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/samples/array_test_data.avro
+-rw-r--r--   0        0        0      115 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/samples/bool_test_data.avro
+-rw-r--r--   0        0        0      130 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/samples/bytes_test_data.avro
+-rw-r--r--   0        0        0      158 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/samples/double_test_data.avro
+-rw-r--r--   0        0        0      191 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/samples/enum_null_test_data.avro
+-rw-r--r--   0        0        0      180 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/samples/enum_test_data.avro
+-rw-r--r--   0        0        0      218 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/samples/fixed_test_data.avro
+-rw-r--r--   0        0        0      116 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/samples/float_test_data.avro
+-rw-r--r--   0        0        0      106 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/samples/int_null_test_data.avro
+-rw-r--r--   0        0        0      128 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/samples/int_string_null_test_data.avro
+-rw-r--r--   0        0        0       89 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/samples/int_test_data.avro
+-rw-r--r--   0        0        0     3035 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/samples/list-depths-records-list.parquet
+-rw-r--r--   0        0        0     2871 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/samples/list-depths-records.parquet
+-rw-r--r--   0        0        0      497 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/samples/list-depths-simple.parquet
+-rw-r--r--   0        0        0     1136 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/samples/list-depths-strings.parquet
+-rw-r--r--   0        0        0     1060 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/samples/list-depths.parquet
+-rw-r--r--   0        0        0      465 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/samples/list-lengths.parquet
+-rw-r--r--   0        0        0      116 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/samples/long_test_data.avro
+-rw-r--r--   0        0        0      681 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/samples/nonnullable-depths.parquet
+-rw-r--r--   0        0        0       75 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/samples/null_test_data.avro
+-rw-r--r--   0        0        0      719 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/samples/nullable-depths.parquet
+-rw-r--r--   0        0        0      635 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/samples/nullable-levels.parquet
+-rw-r--r--   0        0        0     3050 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/samples/nullable-list-depths-records-list.parquet
+-rw-r--r--   0        0        0     2926 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/samples/nullable-list-depths-records.parquet
+-rw-r--r--   0        0        0     1179 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/samples/nullable-list-depths-strings.parquet
+-rw-r--r--   0        0        0     1101 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/samples/nullable-list-depths.parquet
+-rw-r--r--   0        0        0      430 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/samples/nullable-record-primitives-simple.parquet
+-rw-r--r--   0        0        0     1181 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/samples/nullable-record-primitives.parquet
+-rw-r--r--   0        0        0     1193 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/samples/record-primitives.parquet
+-rw-r--r--   0        0        0      326 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/samples/record_0_test_data.avro
+-rw-r--r--   0        0        0      368 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/samples/record_1_test_data.avro
+-rw-r--r--   0        0        0      263 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/samples/record_null_test_data.avro
+-rw-r--r--   0        0        0      423 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/samples/record_test_data.avro
+-rw-r--r--   0        0        0      116 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/samples/string_null_test_data.avro
+-rw-r--r--   0        0        0      125 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/samples/string_test_data.avro
+-rw-r--r--   0        0        0      544 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/samples/test-nan-inf.json
+-rw-r--r--   0        0        0      155 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/samples/test-record-array.json
+-rw-r--r--   0        0        0      803 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/samples/test-two-arrays.json
+-rw-r--r--   0        0        0      535 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/samples/test.json
+-rw-r--r--   0        0        0      180 2023-06-15 15:47:29.000000 awkward-2.2.4/tests/samples/zero-record-batches.parquet
+-rw-r--r--   0        0        0       88 2023-06-15 15:47:29.000000 awkward-2.2.4/tests-cuda/__init__.py
+-rw-r--r--   0        0        0     7072 2023-06-15 15:47:29.000000 awkward-2.2.4/tests-cuda/test_1276_cuda_num.py
+-rw-r--r--   0        0        0     9757 2023-06-15 15:47:29.000000 awkward-2.2.4/tests-cuda/test_1276_cuda_transfers.py
+-rw-r--r--   0        0        0     1197 2023-06-15 15:47:29.000000 awkward-2.2.4/tests-cuda/test_1276_cupy_interop.py
+-rw-r--r--   0        0        0     1629 2023-06-15 15:47:29.000000 awkward-2.2.4/tests-cuda/test_1276_from_cupy.py
+-rw-r--r--   0        0        0    42786 2023-06-15 15:47:29.000000 awkward-2.2.4/tests-cuda/test_1300_same_for_numba_cuda.py
+-rw-r--r--   0        0        0      834 2023-06-15 15:47:29.000000 awkward-2.2.4/tests-cuda/test_1381_check_errors.py
+-rw-r--r--   0        0        0    11252 2023-06-15 15:47:29.000000 awkward-2.2.4/tests-cuda/test_1809_array_cuda_jit.py
+-rw-r--r--   0        0        0     2212 2023-06-15 15:47:29.000000 awkward-2.2.4/.gitignore
+-rw-r--r--   0        0        0     1520 2023-06-15 15:47:29.000000 awkward-2.2.4/LICENSE
+-rw-r--r--   0        0        0     8520 2023-06-15 15:47:29.000000 awkward-2.2.4/pyproject.toml
+-rw-r--r--   0        0        0     6933 2023-06-15 15:47:29.000000 awkward-2.2.4/PKG-INFO
```

### Comparing `awkward-2.2.3/CITATION.cff` & `awkward-2.2.4/CITATION.cff`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/CONTRIBUTING.md` & `awkward-2.2.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/README.md` & `awkward-2.2.4/README.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs/_toc.yml` & `awkward-2.2.4/docs/_toc.yml`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs/conf.py` & `awkward-2.2.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs/index.md` & `awkward-2.2.4/docs/index.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs/prepare_docstrings.py` & `awkward-2.2.4/docs/prepare_docstrings.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs/redirects-user-guide.json` & `awkward-2.2.4/docs/redirects-user-guide.json`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs/redirects.json` & `awkward-2.2.4/docs/redirects.json`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs/_static/css/awkward.css` & `awkward-2.2.4/docs/_static/css/awkward.css`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs/getting-started/community-tutorials.md` & `awkward-2.2.4/docs/getting-started/community-tutorials.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs/getting-started/index.md` & `awkward-2.2.4/docs/getting-started/index.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs/getting-started/papers-and-talks.md` & `awkward-2.2.4/docs/getting-started/papers-and-talks.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs/getting-started/demo/what-is-an-awkward-array.ipynb` & `awkward-2.2.4/docs/getting-started/demo/what-is-an-awkward-array.ipynb`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs/image/example-hierarchy.svg` & `awkward-2.2.4/docs/image/example-hierarchy.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs/reference/ak.behavior.md` & `awkward-2.2.4/docs/reference/ak.behavior.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs/reference/ak.builder.ArrayBuilder.rst` & `awkward-2.2.4/docs/reference/ak.builder.ArrayBuilder.rst`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs/reference/awkwardforth.rst` & `awkward-2.2.4/docs/reference/awkwardforth.rst`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs/reference/toctree.txt` & `awkward-2.2.4/docs/reference/toctree.txt`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs/user-guide/10-minutes-to-awkward-array.md` & `awkward-2.2.4/docs/user-guide/10-minutes-to-awkward-array.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs/user-guide/how-to-combinatorics-best-match.md` & `awkward-2.2.4/docs/user-guide/how-to-combinatorics-best-match.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs/user-guide/how-to-combinatorics-cartesian-combinations.md` & `awkward-2.2.4/docs/user-guide/how-to-combinatorics-cartesian-combinations.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs/user-guide/how-to-convert-arrow.md` & `awkward-2.2.4/docs/user-guide/how-to-convert-arrow.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs/user-guide/how-to-convert-buffers.md` & `awkward-2.2.4/docs/user-guide/how-to-convert-buffers.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs/user-guide/how-to-convert-json.md` & `awkward-2.2.4/docs/user-guide/how-to-convert-json.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs/user-guide/how-to-convert-numpy.md` & `awkward-2.2.4/docs/user-guide/how-to-convert-numpy.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs/user-guide/how-to-convert-pandas.md` & `awkward-2.2.4/docs/user-guide/how-to-convert-pandas.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs/user-guide/how-to-convert-python.md` & `awkward-2.2.4/docs/user-guide/how-to-convert-python.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs/user-guide/how-to-convert-rdataframe.md` & `awkward-2.2.4/docs/user-guide/how-to-convert-rdataframe.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs/user-guide/how-to-create-arraybuilder.md` & `awkward-2.2.4/docs/user-guide/how-to-create-arraybuilder.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs/user-guide/how-to-create-constructors.md` & `awkward-2.2.4/docs/user-guide/how-to-create-constructors.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs/user-guide/how-to-create-lists.md` & `awkward-2.2.4/docs/user-guide/how-to-create-lists.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs/user-guide/how-to-create-missing.md` & `awkward-2.2.4/docs/user-guide/how-to-create-missing.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs/user-guide/how-to-create-records.md` & `awkward-2.2.4/docs/user-guide/how-to-create-records.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs/user-guide/how-to-create-strings.md` & `awkward-2.2.4/docs/user-guide/how-to-create-strings.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs/user-guide/how-to-create-unflatten-group.md` & `awkward-2.2.4/docs/user-guide/how-to-create-unflatten-group.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs/user-guide/how-to-examine-checking-validity.md` & `awkward-2.2.4/docs/user-guide/how-to-examine-checking-validity.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs/user-guide/how-to-examine-list-fields.md` & `awkward-2.2.4/docs/user-guide/how-to-examine-list-fields.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs/user-guide/how-to-examine-simple-slicing.md` & `awkward-2.2.4/docs/user-guide/how-to-examine-simple-slicing.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs/user-guide/how-to-examine-single-item.md` & `awkward-2.2.4/docs/user-guide/how-to-examine-single-item.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs/user-guide/how-to-examine-type.md` & `awkward-2.2.4/docs/user-guide/how-to-examine-type.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs/user-guide/how-to-filter-cut-mask.md` & `awkward-2.2.4/docs/user-guide/how-to-filter-cut-mask.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs/user-guide/how-to-filter-masked.md` & `awkward-2.2.4/docs/user-guide/how-to-filter-masked.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs/user-guide/how-to-filter-num.md` & `awkward-2.2.4/docs/user-guide/how-to-filter-num.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs/user-guide/how-to-filter-ragged.md` & `awkward-2.2.4/docs/user-guide/how-to-filter-ragged.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs/user-guide/how-to-math-argminmax.md` & `awkward-2.2.4/docs/user-guide/how-to-math-argminmax.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs/user-guide/how-to-math-broadcasting.md` & `awkward-2.2.4/docs/user-guide/how-to-math-broadcasting.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs/user-guide/how-to-math-gpu.md` & `awkward-2.2.4/docs/user-guide/how-to-math-gpu.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs/user-guide/how-to-math-numpy.md` & `awkward-2.2.4/docs/user-guide/how-to-math-numpy.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs/user-guide/how-to-math-reducing.md` & `awkward-2.2.4/docs/user-guide/how-to-math-reducing.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs/user-guide/how-to-math-statistics.md` & `awkward-2.2.4/docs/user-guide/how-to-math-statistics.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs/user-guide/how-to-restructure-add-fields.md` & `awkward-2.2.4/docs/user-guide/how-to-restructure-add-fields.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs/user-guide/how-to-restructure-concatenate.md` & `awkward-2.2.4/docs/user-guide/how-to-restructure-concatenate.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs/user-guide/how-to-restructure-flatten.md` & `awkward-2.2.4/docs/user-guide/how-to-restructure-flatten.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs/user-guide/how-to-restructure-pad.md` & `awkward-2.2.4/docs/user-guide/how-to-restructure-pad.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs/user-guide/how-to-restructure-rename-records.md` & `awkward-2.2.4/docs/user-guide/how-to-restructure-rename-records.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs/user-guide/how-to-restructure-sort.md` & `awkward-2.2.4/docs/user-guide/how-to-restructure-sort.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs/user-guide/how-to-restructure-zip-project.md` & `awkward-2.2.4/docs/user-guide/how-to-restructure-zip-project.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs/user-guide/how-to-specialize-differentiate-jax.md` & `awkward-2.2.4/docs/user-guide/how-to-specialize-differentiate-jax.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs/user-guide/how-to-specialize-in-numba.md` & `awkward-2.2.4/docs/user-guide/how-to-specialize-in-numba.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs/user-guide/how-to-specialize-lorentz.md` & `awkward-2.2.4/docs/user-guide/how-to-specialize-lorentz.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs/user-guide/how-to-specialize-override-numpy.md` & `awkward-2.2.4/docs/user-guide/how-to-specialize-override-numpy.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs/user-guide/how-to-specialize-subclass.md` & `awkward-2.2.4/docs/user-guide/how-to-specialize-subclass.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs/user-guide/how-to-use-header-only-layoutbuilder.md` & `awkward-2.2.4/docs/user-guide/how-to-use-header-only-layoutbuilder.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs/user-guide/how-to-use-in-numba-arraybuilder.md` & `awkward-2.2.4/docs/user-guide/how-to-use-in-numba-arraybuilder.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs/user-guide/how-to-use-in-numba-cuda.ipynb` & `awkward-2.2.4/docs/user-guide/how-to-use-in-numba-cuda.ipynb`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs/user-guide/how-to-use-in-numba-features.md` & `awkward-2.2.4/docs/user-guide/how-to-use-in-numba-features.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs-img/panel-data-analysts.png` & `awkward-2.2.4/docs-img/panel-data-analysts.png`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs-img/panel-data-analysts.svg` & `awkward-2.2.4/docs-img/panel-data-analysts.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs-img/panel-developers.png` & `awkward-2.2.4/docs-img/panel-developers.png`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs-img/panel-developers.svg` & `awkward-2.2.4/docs-img/panel-developers.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs-img/panel-doxygen.png` & `awkward-2.2.4/docs-img/panel-doxygen.png`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs-img/panel-sphinx.png` & `awkward-2.2.4/docs-img/panel-sphinx.png`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs-img/panel-tutorials-alternate.png` & `awkward-2.2.4/docs-img/panel-tutorials-alternate.png`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs-img/panel-tutorials.png` & `awkward-2.2.4/docs-img/panel-tutorials.png`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs-img/diagrams/awkward-1-0-layers.pdf` & `awkward-2.2.4/docs-img/diagrams/awkward-1-0-layers.pdf`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs-img/diagrams/awkward-1-0-layers.png` & `awkward-2.2.4/docs-img/diagrams/awkward-1-0-layers.png`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs-img/diagrams/awkward-1-0-layers.svg` & `awkward-2.2.4/docs-img/diagrams/awkward-1-0-layers.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs-img/diagrams/awkward-timeline.pdf` & `awkward-2.2.4/docs-img/diagrams/awkward-timeline.pdf`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs-img/diagrams/awkward-timeline.png` & `awkward-2.2.4/docs-img/diagrams/awkward-timeline.png`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs-img/diagrams/awkward-timeline.svg` & `awkward-2.2.4/docs-img/diagrams/awkward-timeline.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs-img/diagrams/awkward-uproot-timeline-pip-github.png` & `awkward-2.2.4/docs-img/diagrams/awkward-uproot-timeline-pip-github.png`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs-img/diagrams/awkward-uproot-timeline-pip-github.svg` & `awkward-2.2.4/docs-img/diagrams/awkward-uproot-timeline-pip-github.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs-img/diagrams/awkward-uproot-timeline-pip.png` & `awkward-2.2.4/docs-img/diagrams/awkward-uproot-timeline-pip.png`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs-img/diagrams/awkward-uproot-timeline-pip.svg` & `awkward-2.2.4/docs-img/diagrams/awkward-uproot-timeline-pip.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs-img/diagrams/awkward-uproot-timeline.png` & `awkward-2.2.4/docs-img/diagrams/awkward-uproot-timeline.png`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs-img/diagrams/awkward-uproot-timeline.svg` & `awkward-2.2.4/docs-img/diagrams/awkward-uproot-timeline.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs-img/diagrams/cartoon-broadcasting.png` & `awkward-2.2.4/docs-img/diagrams/cartoon-broadcasting.png`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs-img/diagrams/cartoon-broadcasting.svg` & `awkward-2.2.4/docs-img/diagrams/cartoon-broadcasting.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs-img/diagrams/cartoon-cartesian.png` & `awkward-2.2.4/docs-img/diagrams/cartoon-cartesian.png`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs-img/diagrams/cartoon-cartesian.svg` & `awkward-2.2.4/docs-img/diagrams/cartoon-cartesian.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs-img/diagrams/cartoon-combinations.png` & `awkward-2.2.4/docs-img/diagrams/cartoon-combinations.png`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs-img/diagrams/cartoon-combinations.svg` & `awkward-2.2.4/docs-img/diagrams/cartoon-combinations.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs-img/diagrams/cartoon-schematic.png` & `awkward-2.2.4/docs-img/diagrams/cartoon-schematic.png`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs-img/diagrams/cartoon-schematic.svg` & `awkward-2.2.4/docs-img/diagrams/cartoon-schematic.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs-img/diagrams/example-array.svg` & `awkward-2.2.4/docs-img/diagrams/example-array.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs-img/diagrams/example-hierarchy.png` & `awkward-2.2.4/docs-img/diagrams/example-hierarchy.png`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs-img/diagrams/example-hierarchy.svg` & `awkward-2.2.4/docs-img/diagrams/example-hierarchy.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs-img/diagrams/example-reduction-sum-only.svg` & `awkward-2.2.4/docs-img/diagrams/example-reduction-sum-only.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs-img/diagrams/example-reduction-sum.svg` & `awkward-2.2.4/docs-img/diagrams/example-reduction-sum.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs-img/diagrams/example-reduction.png` & `awkward-2.2.4/docs-img/diagrams/example-reduction.png`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs-img/diagrams/example-reduction.svg` & `awkward-2.2.4/docs-img/diagrams/example-reduction.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs-img/diagrams/git-strategy.pdf` & `awkward-2.2.4/docs-img/diagrams/git-strategy.pdf`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs-img/diagrams/git-strategy.png` & `awkward-2.2.4/docs-img/diagrams/git-strategy.png`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs-img/diagrams/git-strategy.svg` & `awkward-2.2.4/docs-img/diagrams/git-strategy.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs-img/diagrams/how-it-works-muons.png` & `awkward-2.2.4/docs-img/diagrams/how-it-works-muons.png`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs-img/diagrams/how-it-works-muons.svg` & `awkward-2.2.4/docs-img/diagrams/how-it-works-muons.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs-img/diagrams/how-it-works.svg` & `awkward-2.2.4/docs-img/diagrams/how-it-works.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs-img/diagrams/sorting-axis.svg` & `awkward-2.2.4/docs-img/diagrams/sorting-axis.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs-img/diagrams/reducers/all.svg` & `awkward-2.2.4/docs-img/diagrams/reducers/all.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs-img/diagrams/reducers/any.svg` & `awkward-2.2.4/docs-img/diagrams/reducers/any.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs-img/diagrams/reducers/argmax.svg` & `awkward-2.2.4/docs-img/diagrams/reducers/argmax.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs-img/diagrams/reducers/argmin.svg` & `awkward-2.2.4/docs-img/diagrams/reducers/argmin.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs-img/diagrams/reducers/count.svg` & `awkward-2.2.4/docs-img/diagrams/reducers/count.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs-img/diagrams/reducers/count_nonzero.svg` & `awkward-2.2.4/docs-img/diagrams/reducers/count_nonzero.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs-img/diagrams/reducers/max.svg` & `awkward-2.2.4/docs-img/diagrams/reducers/max.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs-img/diagrams/reducers/min.svg` & `awkward-2.2.4/docs-img/diagrams/reducers/min.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs-img/diagrams/reducers/product.svg` & `awkward-2.2.4/docs-img/diagrams/reducers/product.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs-img/diagrams/reducers/sum.svg` & `awkward-2.2.4/docs-img/diagrams/reducers/sum.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs-img/logo/favicon.ico` & `awkward-2.2.4/docs-img/logo/favicon.ico`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs-img/logo/logo-300px-white.png` & `awkward-2.2.4/docs-img/logo/logo-300px-white.png`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs-img/logo/logo-300px.png` & `awkward-2.2.4/docs-img/logo/logo-300px.png`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs-img/logo/logo-600px.png` & `awkward-2.2.4/docs-img/logo/logo-600px.png`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs-img/logo/logo.svg` & `awkward-2.2.4/docs-img/logo/logo.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs-img/photos/desire-path.jpg` & `awkward-2.2.4/docs-img/photos/desire-path.jpg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs-img/plots/awkward-0-popularity.pdf` & `awkward-2.2.4/docs-img/plots/awkward-0-popularity.pdf`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs-img/plots/awkward-0-popularity.png` & `awkward-2.2.4/docs-img/plots/awkward-0-popularity.png`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs-img/plots/awkward-0-popularity.svg` & `awkward-2.2.4/docs-img/plots/awkward-0-popularity.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs-img/plots/bikeroutes-scaling.svg` & `awkward-2.2.4/docs-img/plots/bikeroutes-scaling.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/docs-img/screenshots/github-issues-documentation.png` & `awkward-2.2.4/docs-img/screenshots/github-issues-documentation.png`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/__init__.py` & `awkward-2.2.4/src/awkward/__init__.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_behavior.py` & `awkward-2.2.4/src/awkward/_behavior.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_broadcasting.py` & `awkward-2.2.4/src/awkward/_broadcasting.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_do.py` & `awkward-2.2.4/src/awkward/_do.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_errors.py` & `awkward-2.2.4/src/awkward/_errors.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 from __future__ import annotations
 
 import builtins
 import sys
 import threading
 import warnings
-from collections.abc import Mapping, Sequence
+from collections.abc import Callable, Collection, Iterable, Mapping
+from functools import wraps
 
 import numpy  # noqa: TID251
 
 from awkward._nplikes.numpylike import NumpyMetadata
-from awkward._typing import TypeVar
+from awkward._typing import Any, TypeVar
 
 np = NumpyMetadata.instance()
 
 
 E = TypeVar("E", bound=Exception)
 
 
@@ -157,15 +158,15 @@
                     while last > width:
                         last = valuestr[: last - 3].rfind("...") + 3
                     valuestr = valuestr[:last]
 
                 if len(valuestr) > width:
                     valuestr = valuestr[: width - 3] + "..."
 
-        elif isinstance(value, (Sequence, Mapping)) and len(value) < 10000:
+        elif isinstance(value, (Collection, Mapping)) and len(value) < 10000:
             valuestr = repr(value)
             if len(valuestr) > width:
                 valuestr = valuestr[: width - 3] + "..."
 
         if valuestr is None:
             return f"{type(value).__name__}-instance"
         else:
@@ -178,74 +179,113 @@
     def note(self) -> str:
         raise NotImplementedError
 
 
 class OperationErrorContext(ErrorContext):
     _width = 80 - 8
 
-    def __init__(self, name, arguments):
+    def any_backend_is_delayed(
+        self, iterable: Iterable, *, depth: int = 1, depth_limit: int = 2
+    ) -> bool:
         from awkward._backends.dispatch import backend_of
-        from awkward._backends.numpy import NumpyBackend
 
-        numpy_backend = NumpyBackend.instance()
-        if self.primary() is not None or all(
-            backend_of(x, default=numpy_backend).nplike.is_eager for x in arguments
+        for obj in iterable:
+            backend = backend_of(obj, default=None)
+            # Do we not recognise this as an object with a backend?
+            if backend is None:
+                # Is this an iterable object, and are we permitted to recurse?
+                if isinstance(obj, Collection) and depth != depth_limit:
+                    return self.any_backend_is_delayed(
+                        obj, depth=depth + 1, depth_limit=depth_limit
+                    )
+                # Assume not delayed!
+                else:
+                    return False
+            # Eager backends aren't delayed!
+            elif backend.nplike.is_eager:
+                continue
+            else:
+                return True
+        return False
+
+    def __init__(self, name, args: Iterable[Any], kwargs: Mapping[str, Any]):
+        if self.primary() is None and (
+            self.any_backend_is_delayed(args)
+            or self.any_backend_is_delayed(kwargs.values())
         ):
+            string_args = self._format_args(args)
+            string_kwargs = self._format_kwargs(kwargs)
+        else:
             # if primary is not None: we won't be setting an ErrorContext
             # if all nplikes are eager: no accumulation of large arrays
             # --> in either case, delay string generation
-            string_arguments = PartialFunction(self._string_arguments, arguments)
-        else:
-            string_arguments = self._string_arguments(arguments)
+            string_args = PartialFunction(self._format_args, args)
+            string_kwargs = PartialFunction(self._format_kwargs, kwargs)
 
         super().__init__(
             name=name,
-            arguments=string_arguments,
+            args=string_args,
+            kwargs=string_kwargs,
         )
 
-    def _string_arguments(self, arguments):
+    def _format_args(self, arguments: Iterable) -> list[str]:
+        string_arguments = []
+        for value in arguments:
+            string_arguments.append(self.format_argument(self._width, value))
+
+        return string_arguments
+
+    def _format_kwargs(self, arguments: Mapping[str, Any]) -> dict[str, str]:
         string_arguments = {}
         for key, value in arguments.items():
             if isinstance(key, str):
                 width = self._width - len(key) - 3
             else:
                 width = self._width
-
             string_arguments[key] = self.format_argument(width, value)
-
         return string_arguments
 
     @property
     def name(self):
         return self._kwargs["name"]
 
     @property
-    def arguments(self):
-        out = self._kwargs["arguments"]
+    def args(self) -> list:
+        out = self._kwargs["args"]
         if isinstance(out, PartialFunction):
-            out = self._kwargs["arguments"] = out()
+            out = self._kwargs["args"] = out()
         return out
 
-    def format_exception(self, exception):
+    @property
+    def kwargs(self) -> dict:
+        out = self._kwargs["kwargs"]
+        if isinstance(out, PartialFunction):
+            out = self._kwargs["kwargs"] = out()
+        return out
+
+    def format_exception(self, exception: Exception) -> str:
         return f"{exception}\n{self.note}"
 
     @property
     def note(self) -> str:
         arguments = []
-        for name, valuestr in self.arguments.items():
+        for valuestr in self.args:
+            arguments.append(f"\n        {valuestr}")
+        for name, valuestr in self.kwargs.items():
             if isinstance(name, str):
                 arguments.append(f"\n        {name} = {valuestr}")
             else:
                 arguments.append(f"\n        {valuestr}")
 
         extra_line = "" if len(arguments) == 0 else "\n    "
+        calling_note = f'{self.name}({"".join(arguments)}{extra_line})'
         return f"""
 This error occurred while calling
 
-    {self.name}({"".join(arguments)}{extra_line})"""
+    {calling_note}"""
 
 
 class SlicingErrorContext(ErrorContext):
     _width = 80 - 4
 
     def __init__(self, array, where):
         from awkward._backends.dispatch import backend_of
@@ -377,7 +417,20 @@
 
 
 class FieldNotFoundError(IndexError):
     ...
 
 
 AxisError = numpy.AxisError
+
+
+T = TypeVar("T", bound=Callable)
+
+
+def with_operation_context(func: T) -> T:
+    @wraps(func)
+    def wrapper(*args, **kwargs):
+        # NOTE: this decorator assumes that the operation is exposed under `ak.`
+        with OperationErrorContext(f"ak.{func.__qualname__}", args, kwargs):
+            return func(*args, **kwargs)
+
+    return wrapper
```

### Comparing `awkward-2.2.3/src/awkward/_kernels.py` & `awkward-2.2.4/src/awkward/_kernels.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_layout.py` & `awkward-2.2.4/src/awkward/_layout.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_lookup.py` & `awkward-2.2.4/src/awkward/_lookup.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_parameters.py` & `awkward-2.2.4/src/awkward/_parameters.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_prettyprint.py` & `awkward-2.2.4/src/awkward/_prettyprint.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_reducers.py` & `awkward-2.2.4/src/awkward/_reducers.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_regularize.py` & `awkward-2.2.4/src/awkward/_regularize.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_slicing.py` & `awkward-2.2.4/src/awkward/_slicing.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_typetracer.py` & `awkward-2.2.4/src/awkward/_typetracer.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_typing.py` & `awkward-2.2.4/src/awkward/_typing.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_util.py` & `awkward-2.2.4/src/awkward/_util.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,16 +3,14 @@
 
 import base64
 import os
 import struct
 import sys
 from collections.abc import Collection
 
-import packaging.version
-
 from awkward._typing import TypeVar
 
 win = os.name == "nt"
 bits32 = struct.calcsize("P") * 8 == 32
 
 # matches include/awkward/common.h
 kMaxInt8 = 127  # 2**7  - 1
@@ -20,24 +18,14 @@
 kMaxInt32 = 2147483647  # 2**31 - 1
 kMaxUInt32 = 4294967295  # 2**32 - 1
 kMaxInt64 = 9223372036854775806  # 2**63 - 2: see below
 kSliceNone = kMaxInt64 + 1  # for Slice::none()
 kMaxLevels = 48
 
 
-def parse_version(version):
-    return packaging.version.parse(version)
-
-
-def numpy_at_least(version):
-    import numpy  # noqa: TID251
-
-    return parse_version(numpy.__version__) >= parse_version(version)
-
-
 def in_module(obj, modulename: str) -> bool:
     m = type(obj).__module__
     return m == modulename or m.startswith(modulename + ".")
 
 
 def tobytes(array):
     if hasattr(array, "tobytes"):
```

### Comparing `awkward-2.2.3/src/awkward/_v2.py` & `awkward-2.2.4/src/awkward/_v2.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/cppyy.py` & `awkward-2.2.4/src/awkward/cppyy.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/highlevel.py` & `awkward-2.2.4/src/awkward/highlevel.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,24 +7,24 @@
 import itertools
 import keyword
 import re
 import sys
 from collections.abc import Iterable, Mapping, Sized
 
 from awkward_cpp.lib import _ext
-from numpy.lib.mixins import NDArrayOperatorsMixin  # noqa: TID251
 
 import awkward as ak
 import awkward._connect.hist
 from awkward._backends.dispatch import register_backend_lookup_factory
 from awkward._backends.numpy import NumpyBackend
 from awkward._behavior import behavior_of, get_array_class, get_record_class
 from awkward._layout import wrap_layout
 from awkward._nplikes.numpy import Numpy
 from awkward._nplikes.numpylike import NumpyMetadata
+from awkward._operators import NDArrayOperatorsMixin
 from awkward._regularize import is_non_string_like_iterable
 
 np = NumpyMetadata.instance()
 numpy = Numpy.instance()
 
 _dir_pattern = re.compile(r"^[a-zA-Z_]\w*$")
 
@@ -323,15 +323,15 @@
 
     class Mask:
         def __init__(self, array):
             self._array = array
 
         def __getitem__(self, where):
             with ak._errors.OperationErrorContext(
-                "ak.Array.mask", {0: self._array, 1: where}
+                "ak.Array.mask", args=[self._array, where], kwargs={}
             ):
                 return ak.operations.mask(self._array, where, valid_when=True)
 
     @property
     def mask(self):
         """
         Whereas
@@ -1014,15 +1014,16 @@
 
         See #ak.with_field for a variant that does not change the #ak.Array
         in-place. (Internally, this method uses #ak.with_field, so performance
         is not a factor in choosing one over the other.)
         """
         with ak._errors.OperationErrorContext(
             "ak.Array.__setitem__",
-            {"self": self, "field_name": where, "field_value": what},
+            (self,),
+            {"where": where, "what": what},
         ):
             if not (
                 isinstance(where, str)
                 or (isinstance(where, tuple) and all(isinstance(x, str) for x in where))
             ):
                 raise TypeError("only fields may be assigned in-place (by field name)")
 
@@ -1045,15 +1046,16 @@
 
         See #ak.without_field for a variant that does not change the #ak.Array
         in-place. (Internally, this method uses #ak.without_field, so performance
         is not a factor in choosing one over the other.)
         """
         with ak._errors.OperationErrorContext(
             "ak.Array.__delitem__",
-            {"self": self, "field_name": where},
+            (self,),
+            {"where": where},
         ):
             if not (
                 isinstance(where, str)
                 or (isinstance(where, tuple) and all(isinstance(x, str) for x in where))
             ):
                 raise TypeError("only fields may be removed in-place (by field name)")
 
@@ -1277,19 +1279,15 @@
         array with dtype `"O"` for `np.object_` (see the
         [note on object_ type](https://docs.scipy.org/doc/numpy/reference/arrays.scalars.html#arrays-scalars-built-in))
         since silent conversions to dtype `"O"` arrays would not only be a
         significant performance hit, but would also break functionality, since
         nested lists in a NumPy `"O"` array are severed from the array and
         cannot be sliced as dimensions.
         """
-        arguments = {0: self}
-        for i, arg in enumerate(args):
-            arguments[i + 1] = arg
-        arguments.update(kwargs)
-        with ak._errors.OperationErrorContext("numpy.asarray", arguments):
+        with ak._errors.OperationErrorContext("numpy.asarray", (self, *args), kwargs):
             return ak._connect.numpy.convert_to_array(self._layout, args, kwargs)
 
     def __array_ufunc__(self, ufunc, method, *inputs, **kwargs):
         """
         Intercepts attempts to pass this Array to a NumPy
         [universal functions](https://docs.scipy.org/doc/numpy/reference/ufuncs.html)
         (ufuncs) and passes it through the Array's structure.
@@ -1350,19 +1348,15 @@
             [[1.21, 4.84, 10.9],
              [],
              [19.4, 30.2]]
 
         See also #__array_function__.
         """
         name = f"{type(ufunc).__module__}.{ufunc.__name__}.{method!s}"
-        arguments = {}
-        for i, arg in enumerate(inputs):
-            arguments[i] = arg
-        arguments.update(kwargs)
-        with ak._errors.OperationErrorContext(name, arguments):
+        with ak._errors.OperationErrorContext(name, inputs, kwargs):
             return ak._connect.numpy.array_ufunc(ufunc, method, inputs, kwargs)
 
     def __array_function__(self, func, types, args, kwargs):
         """
         Intercepts attempts to pass this Array to those NumPy functions other
         than universal functions that have an Awkward equivalent.
 
@@ -1783,15 +1777,16 @@
 
         See #ak.with_field for a variant that does not change the #ak.Record
         in-place. (Internally, this method uses #ak.with_field, so performance
         is not a factor in choosing one over the other.)
         """
         with ak._errors.OperationErrorContext(
             "ak.Record.__setitem__",
-            {"self": self, "field_name": where, "field_value": what},
+            (self,),
+            {"where": where, "what": what},
         ):
             if not (
                 isinstance(where, str)
                 or (isinstance(where, tuple) and all(isinstance(x, str) for x in where))
             ):
                 raise TypeError("only fields may be assigned in-place (by field name)")
 
@@ -1815,15 +1810,16 @@
 
         See #ak.without_field for a variant that does not change the #ak.Record
         in-place. (Internally, this method uses #ak.without_field, so performance
         is not a factor in choosing one over the other.)
         """
         with ak._errors.OperationErrorContext(
             "ak.Record.__delitem__",
-            {"self": self, "field_name": where},
+            (self,),
+            {"where": where},
         ):
             if not (
                 isinstance(where, str)
                 or (isinstance(where, tuple) and all(isinstance(x, str) for x in where))
             ):
                 raise TypeError("only fields may be removed in-place (by field name)")
 
@@ -2026,19 +2022,15 @@
         for overriding ufuncs, which has been
         [available since NumPy 1.13](https://numpy.org/devdocs/release/1.13.0-notes.html#array-ufunc-added)
         (and thus NumPy 1.13 is the minimum allowed version).
 
         See #ak.Array.__array_ufunc__ for a more complete description.
         """
         name = f"{type(ufunc).__module__}.{ufunc.__name__}.{method!s}"
-        arguments = {}
-        for i, arg in enumerate(inputs):
-            arguments[i] = arg
-        arguments.update(kwargs)
-        with ak._errors.OperationErrorContext(name, arguments):
+        with ak._errors.OperationErrorContext(name, inputs, kwargs):
             return ak._connect.numpy.array_ufunc(ufunc, method, inputs, kwargs)
 
     @property
     def numba_type(self):
         """
         The type of this Record when it is used in Numba. It contains enough
         information to generate low-level code for accessing any element,
@@ -2372,19 +2364,15 @@
         """
         Intercepts attempts to convert a #snapshot of this array into a
         NumPy array and either performs a zero-copy conversion or raises
         an error.
 
         See #ak.Array.__array__ for a more complete description.
         """
-        arguments = {0: self}
-        for i, arg in enumerate(args):
-            arguments[i + 1] = arg
-        arguments.update(kwargs)
-        with ak._errors.OperationErrorContext("numpy.asarray", arguments):
+        with ak._errors.OperationErrorContext("numpy.asarray", (self, *args), kwargs):
             return ak._connect.numpy.convert_to_array(self.snapshot(), args, kwargs)
 
     @property
     def numba_type(self):
         """
         The type of this Array when it is used in Numba. It contains enough
         information to generate low-level code for accessing any element,
@@ -2411,15 +2399,15 @@
         Converts the currently accumulated data into an #ak.Array.
 
         The currently accumulated data are *copied* into the new array.
         """
         formstr, length, container = self._layout.to_buffers()
         form = ak.forms.from_json(formstr)
 
-        with ak._errors.OperationErrorContext("ak.ArrayBuilder.snapshot", {}):
+        with ak._errors.OperationErrorContext("ak.ArrayBuilder.snapshot", [], {}):
             return ak.operations.ak_from_buffers._impl(
                 form,
                 length,
                 container,
                 buffer_key="{form_key}-{attribute}",
                 backend="cpu",
                 byteorder=ak._util.native_byteorder,
```

### Comparing `awkward-2.2.3/src/awkward/index.py` & `awkward-2.2.4/src/awkward/index.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/jax.py` & `awkward-2.2.4/src/awkward/jax.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/numba.py` & `awkward-2.2.4/src/awkward/numba.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 
 import math
 
 import numpy  # noqa: TID251
+from packaging.version import parse as parse_version
 
 import awkward as ak
 
 _has_checked_version = False
 _is_registered = False
 
 
@@ -23,15 +24,15 @@
 
 or
 
 conda install numba"""
         ) from err
 
     if not _has_checked_version:
-        if ak._util.parse_version(numba.__version__) < ak._util.parse_version("0.50"):
+        if parse_version(numba.__version__) < parse_version("0.50"):
             raise ImportError(
                 "Awkward Array can only work with numba 0.50 or later "
                 "(you have version {})".format(numba.__version__)
             )
         _has_checked_version = True
 
     _register()
```

### Comparing `awkward-2.2.3/src/awkward/record.py` & `awkward-2.2.4/src/awkward/record.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/typetracer.py` & `awkward-2.2.4/src/awkward/typetracer.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_backends/backend.py` & `awkward-2.2.4/src/awkward/_backends/backend.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_backends/cupy.py` & `awkward-2.2.4/src/awkward/_backends/cupy.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_backends/dispatch.py` & `awkward-2.2.4/src/awkward/_backends/dispatch.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_backends/jax.py` & `awkward-2.2.4/src/awkward/_backends/jax.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_backends/numpy.py` & `awkward-2.2.4/src/awkward/_backends/numpy.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_backends/typetracer.py` & `awkward-2.2.4/src/awkward/_backends/typetracer.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_connect/avro.py` & `awkward-2.2.4/src/awkward/_connect/avro.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_connect/cling.py` & `awkward-2.2.4/src/awkward/_connect/cling.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_connect/hist.py` & `awkward-2.2.4/src/awkward/_connect/hist.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_connect/numexpr.py` & `awkward-2.2.4/src/awkward/_connect/numexpr.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 import sys
 import warnings
 
+from packaging.version import parse as parse_version
+
 import awkward as ak
 from awkward._behavior import behavior_of
 from awkward._layout import wrap_layout
 
 _has_checked_version = False
 
 
@@ -21,17 +23,15 @@
 
 or
 
     conda install numexpr"""
         ) from err
     else:
         if not _has_checked_version:
-            if ak._util.parse_version(numexpr.__version__) < ak._util.parse_version(
-                "2.7.1"
-            ):
+            if parse_version(numexpr.__version__) < parse_version("2.7.1"):
                 warnings.warn(
                     "Awkward Array is only known to work with numexpr 2.7.1 or later"
                     "(you have version {})".format(numexpr.__version__),
                     RuntimeWarning,
                     stacklevel=1,
                 )
             _has_checked_version = True
```

### Comparing `awkward-2.2.3/src/awkward/_connect/numpy.py` & `awkward-2.2.4/src/awkward/_connect/numpy.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,35 +2,36 @@
 import collections
 import functools
 import inspect
 from collections.abc import Iterable
 from itertools import chain
 
 import numpy
+from packaging.version import parse as parse_version
 
 import awkward as ak
 from awkward._backends.backend import Backend
 from awkward._backends.dispatch import backend_of, common_backend
 from awkward._behavior import (
     behavior_of,
     find_custom_cast,
     find_ufunc,
     find_ufunc_generic,
 )
 from awkward._layout import wrap_layout
 from awkward._nplikes import to_nplike
 from awkward._regularize import is_non_string_like_iterable
 from awkward._typing import Iterator
-from awkward._util import Sentinel, numpy_at_least
+from awkward._util import Sentinel
 from awkward.contents.numpyarray import NumpyArray
 
 # NumPy 1.13.1 introduced NEP13, without which Awkward ufuncs won't work, which
 # would be worse than lacking a feature: it would cause unexpected output.
 # NumPy 1.17.0 introduced NEP18, which is optional (use ak.* instead of np.*).
-if not numpy_at_least("1.13.1"):
+if parse_version(numpy.__version__) < parse_version("1.13.1"):
     raise ImportError("NumPy 1.13.1 or later required")
 
 
 UNSUPPORTED = Sentinel("UNSUPPORTED", __name__)
 
 
 def convert_to_array(layout, args, kwargs):
```

### Comparing `awkward-2.2.3/src/awkward/_connect/pyarrow.py` & `awkward-2.2.4/src/awkward/_connect/pyarrow.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 
 import json
 from collections.abc import Iterable, Sized
 
+from packaging.version import parse as parse_version
+
 import awkward as ak
 from awkward._backends.numpy import NumpyBackend
 from awkward._nplikes.numpy import Numpy
 from awkward._nplikes.numpylike import NumpyMetadata
 from awkward._parameters import parameters_union
 
 np = NumpyMetadata.instance()
@@ -25,15 +27,15 @@
 
 or
 
     conda install -c conda-forge pyarrow
 """
 
 else:
-    if ak._util.parse_version(pyarrow.__version__) < ak._util.parse_version("7.0.0"):
+    if parse_version(pyarrow.__version__) < parse_version("7.0.0"):
         pyarrow = None
         error_message = "pyarrow 7.0.0 or later required for {0}"
 
 
 def import_pyarrow(name):
     if pyarrow is None:
         raise ImportError(error_message.format(name))
```

### Comparing `awkward-2.2.3/src/awkward/_connect/cuda/__init__.py` & `awkward-2.2.4/src/awkward/_connect/cuda/__init__.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_BitMaskedArray_to_ByteMaskedArray.cu` & `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_BitMaskedArray_to_ByteMaskedArray.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_BitMaskedArray_to_IndexedOptionArray.cu` & `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_BitMaskedArray_to_IndexedOptionArray.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_getitem_carry.cu` & `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_getitem_carry.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_getitem_nextcarry.cu` & `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_getitem_nextcarry.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_getitem_nextcarry_outindex.cu` & `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_getitem_nextcarry_outindex.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_mask.cu` & `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_mask.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_overlay_mask.cu` & `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_overlay_mask.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_reduce_next_64.cu` & `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_reduce_next_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_reduce_next_nonlocal_nextshifts_64.cu` & `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_reduce_next_nonlocal_nextshifts_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_toIndexedOptionArray.cu` & `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_toIndexedOptionArray.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_Content_getitem_next_missing_jagged_getmaskstartstop.cu` & `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_Content_getitem_next_missing_jagged_getmaskstartstop.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_Index_to_Index64.cu` & `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_Index_to_Index64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_fill_count.cu` & `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_fill_count.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_flatten_nextcarry.cu` & `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_flatten_nextcarry.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_getitem_nextcarry.cu` & `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_getitem_nextcarry.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_getitem_nextcarry_outindex.cu` & `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_getitem_nextcarry_outindex.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_getitem_nextcarry_outindex_mask.cu` & `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_getitem_nextcarry_outindex_mask.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_mask.cu` & `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_mask.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_overlay_mask.cu` & `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_overlay_mask.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_64.cu` & `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_fix_offsets_64.cu` & `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_fix_offsets_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_nonlocal_nextshifts_64.cu` & `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_nonlocal_nextshifts_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_nonlocal_nextshifts_fromshifts_64.cu` & `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_nonlocal_nextshifts_fromshifts_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_simplify.cu` & `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_simplify.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_validity.cu` & `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_validity.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedOptionArray_rpad_and_clip_mask_axis1.cu` & `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedOptionArray_rpad_and_clip_mask_axis1.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_compact_offsets.cu` & `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_compact_offsets.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_getitem_jagged_expand.cu` & `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_getitem_jagged_expand.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_getitem_next_array.cu` & `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_getitem_next_array.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_validity.cu` & `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_validity.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_flatten_offsets.cu` & `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_flatten_offsets.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_reduce_global_startstop_64.cu` & `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_reduce_global_startstop_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_rpad_and_clip_axis1.cu` & `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_rpad_and_clip_axis1.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_rpad_axis1.cu` & `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_rpad_axis1.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_MaskedArray_getitem_next_jagged_project.cu` & `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_MaskedArray_getitem_next_jagged_project.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_contiguous_init.cu` & `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_contiguous_init.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_contiguous_next.cu` & `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_contiguous_next.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_fill_tobool.cu` & `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_fill_tobool.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_boolean_nonzero.cu` & `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_boolean_nonzero.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_array.cu` & `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_array.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_array_advanced.cu` & `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_array_advanced.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_at.cu` & `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_at.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_range.cu` & `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_range.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_range_advanced.cu` & `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_range_advanced.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_reduce_adjust_starts_64.cu` & `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_reduce_adjust_starts_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_reduce_adjust_starts_shifts_64.cu` & `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_reduce_adjust_starts_shifts_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_reduce_mask_ByteMaskedArray_64.cu` & `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_reduce_mask_ByteMaskedArray_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_carry.cu` & `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_carry.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_jagged_expand.cu` & `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_jagged_expand.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_array.cu` & `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_array.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_array_advanced.cu` & `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_array_advanced.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_at.cu` & `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_at.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_range.cu` & `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_range.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_range_spreadadvanced.cu` & `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_range_spreadadvanced.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_localindex.cu` & `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_localindex.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_fillna.cu` & `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_fillna.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_project.cu` & `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_project.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_validity.cu` & `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_validity.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_combinations.cu` & `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_combinations.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_content_reduce_zeroparents_64.cu` & `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_content_reduce_zeroparents_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_index_carry.cu` & `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_index_carry.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_index_carry_nocheck.cu` & `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_index_carry_nocheck.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_index_rpad_and_clip_axis1.cu` & `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_index_rpad_and_clip_axis1.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_missing_repeat.cu` & `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_missing_repeat.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmax.cu` & `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmax.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmax_bool_64.cu` & `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmax_bool_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmin.cu` & `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmin.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmin_bool_64.cu` & `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmin_bool_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_count_64.cu` & `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_count_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_countnonzero.cu` & `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_countnonzero.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_max.cu` & `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_max.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_min.cu` & `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_min.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_prod_bool.cu` & `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_prod_bool.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum.cu` & `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum_bool.cu` & `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum_bool.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum_int32_bool_64.cu` & `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum_int32_bool_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum_int64_bool_64.cu` & `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum_int64_bool_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/awkward_regularize_arrayslice.cu` & `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/awkward_regularize_arrayslice.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_connect/cuda/cuda_kernels/cuda_common.cu` & `awkward-2.2.4/src/awkward/_connect/cuda/cuda_kernels/cuda_common.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_connect/header-only/awkward/BuilderOptions.h` & `awkward-2.2.4/src/awkward/_connect/header-only/awkward/BuilderOptions.h`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_connect/header-only/awkward/GrowableBuffer.h` & `awkward-2.2.4/src/awkward/_connect/header-only/awkward/GrowableBuffer.h`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_connect/header-only/awkward/LayoutBuilder.h` & `awkward-2.2.4/src/awkward/_connect/header-only/awkward/LayoutBuilder.h`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_connect/header-only/awkward/utils.h` & `awkward-2.2.4/src/awkward/_connect/header-only/awkward/utils.h`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_connect/jax/reducers.py` & `awkward-2.2.4/src/awkward/_connect/jax/reducers.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_connect/jax/trees.py` & `awkward-2.2.4/src/awkward/_connect/jax/trees.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_connect/numba/arrayview.py` & `awkward-2.2.4/src/awkward/_connect/numba/arrayview.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_connect/numba/arrayview_cuda.py` & `awkward-2.2.4/src/awkward/_connect/numba/arrayview_cuda.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_connect/numba/builder.py` & `awkward-2.2.4/src/awkward/_connect/numba/builder.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_connect/numba/growablebuffer.py` & `awkward-2.2.4/src/awkward/_connect/numba/growablebuffer.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_connect/numba/layout.py` & `awkward-2.2.4/src/awkward/_connect/numba/layout.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_connect/rdataframe/from_rdataframe.py` & `awkward-2.2.4/src/awkward/_connect/rdataframe/from_rdataframe.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_connect/rdataframe/to_rdataframe.py` & `awkward-2.2.4/src/awkward/_connect/rdataframe/to_rdataframe.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_connect/rdataframe/include/rdataframe/jagged_builders.h` & `awkward-2.2.4/src/awkward/_connect/rdataframe/include/rdataframe/jagged_builders.h`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_nplikes/__init__.py` & `awkward-2.2.4/src/awkward/_nplikes/__init__.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_nplikes/array_module.py` & `awkward-2.2.4/src/awkward/_nplikes/array_module.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_nplikes/cupy.py` & `awkward-2.2.4/src/awkward/_nplikes/cupy.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_nplikes/dispatch.py` & `awkward-2.2.4/src/awkward/_nplikes/dispatch.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_nplikes/jax.py` & `awkward-2.2.4/src/awkward/_nplikes/jax.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_nplikes/numpy.py` & `awkward-2.2.4/src/awkward/_nplikes/numpy.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 from __future__ import annotations
 
 import numpy
+from packaging.version import parse as parse_version
 
-import awkward as ak
 from awkward._nplikes.array_module import ArrayModuleNumpyLike
 from awkward._nplikes.dispatch import register_nplike
 from awkward._nplikes.numpylike import ArrayLike, NumpyMetadata
 from awkward._nplikes.placeholder import PlaceholderArray
 from awkward._typing import Final, Literal
 
 np = NumpyMetadata.instance()
@@ -53,15 +53,15 @@
         self,
         x: ArrayLike,
         *,
         axis: int | None = None,
         bitorder: Literal["big", "little"] = "big",
     ):
         assert not isinstance(x, PlaceholderArray)
-        if ak._util.numpy_at_least("1.17.0"):
+        if parse_version(numpy.__version__) >= parse_version("1.17.0"):
             return numpy.packbits(x, axis=axis, bitorder=bitorder)
         else:
             assert axis is None, "unsupported argument value for axis given"
             if bitorder == "little":
                 if len(x) % 8 == 0:
                     ready_to_pack = x
                 else:
@@ -81,15 +81,15 @@
         x: ArrayLike,
         *,
         axis: int | None = None,
         count: int | None = None,
         bitorder: Literal["big", "little"] = "big",
     ):
         assert not isinstance(x, PlaceholderArray)
-        if ak._util.numpy_at_least("1.17.0"):
+        if parse_version(numpy.__version__) >= parse_version("1.17.0"):
             return numpy.unpackbits(x, axis=axis, count=count, bitorder=bitorder)
         else:
             assert axis is None, "unsupported argument value for axis given"
             assert count is None, "unsupported argument value for count given"
             ready_to_bitswap = numpy.unpackbits(x)
             if bitorder == "little":
                 return ready_to_bitswap.reshape(-1, 8)[:, ::-1].reshape(-1)
```

### Comparing `awkward-2.2.3/src/awkward/_nplikes/numpylike.py` & `awkward-2.2.4/src/awkward/_nplikes/numpylike.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_nplikes/placeholder.py` & `awkward-2.2.4/src/awkward/_nplikes/placeholder.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_nplikes/shape.py` & `awkward-2.2.4/src/awkward/_nplikes/shape.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/_nplikes/typetracer.py` & `awkward-2.2.4/src/awkward/_nplikes/typetracer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 from __future__ import annotations
 
 from numbers import Number
 
 import numpy
-from numpy.lib.mixins import NDArrayOperatorsMixin
 
 import awkward as ak
 from awkward._nplikes.dispatch import register_nplike
 from awkward._nplikes.numpylike import (
     ArrayLike,
     IndexType,
     NumpyLike,
     NumpyMetadata,
     UniqueAllResult,
 )
 from awkward._nplikes.placeholder import PlaceholderArray
 from awkward._nplikes.shape import ShapeItem, unknown_length
+from awkward._operators import NDArrayOperatorsMixin
 from awkward._regularize import is_integer, is_non_string_like_sequence
 from awkward._typing import (
     Any,
     Final,
     Literal,
     Self,
     SupportsIndex,
```

### Comparing `awkward-2.2.3/src/awkward/_nplikes/ufuncs.py` & `awkward-2.2.4/src/awkward/_nplikes/ufuncs.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/behaviors/categorical.py` & `awkward-2.2.4/src/awkward/behaviors/categorical.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/behaviors/mixins.py` & `awkward-2.2.4/src/awkward/behaviors/mixins.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/behaviors/string.py` & `awkward-2.2.4/src/awkward/behaviors/string.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/contents/__init__.py` & `awkward-2.2.4/src/awkward/contents/__init__.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/contents/bitmaskedarray.py` & `awkward-2.2.4/src/awkward/contents/bitmaskedarray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/contents/bytemaskedarray.py` & `awkward-2.2.4/src/awkward/contents/bytemaskedarray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/contents/content.py` & `awkward-2.2.4/src/awkward/contents/content.py`

 * *Files 0% similar despite different names*

```diff
@@ -1272,15 +1272,15 @@
 
     def is_equal_to(
         self, other: Content, index_dtype: bool = True, numpyarray: bool = True
     ) -> bool:
         return (
             self.__class__ is other.__class__
             and len(self) == len(other)
-            and type_parameters_equal(self.parameters, other.parameters)
+            and type_parameters_equal(self._parameters, other._parameters)
             and self._is_equal_to(other, index_dtype, numpyarray)
         )
 
     def _is_equal_to(self, other: Self, index_dtype: bool, numpyarray: bool) -> bool:
         raise NotImplementedError
 
     def _repr(self, indent: str, pre: str, post: str) -> str:
```

### Comparing `awkward-2.2.3/src/awkward/contents/emptyarray.py` & `awkward-2.2.4/src/awkward/contents/emptyarray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/contents/indexedarray.py` & `awkward-2.2.4/src/awkward/contents/indexedarray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/contents/indexedoptionarray.py` & `awkward-2.2.4/src/awkward/contents/indexedoptionarray.py`

 * *Files 0% similar despite different names*

```diff
@@ -831,15 +831,14 @@
             ](index.data, self._index.data, tags.length)
         )
         return ak.contents.UnionArray.simplified(
             tags,
             index,
             contents,
             parameters=self._parameters,
-            merge=True,
             mergebool=True,
         )
 
     def _local_index(self, axis, depth):
         posaxis = maybe_posaxis(self, axis, depth)
         if posaxis is not None and posaxis + 1 == depth:
             return self._local_index_axis0()
```

### Comparing `awkward-2.2.3/src/awkward/contents/listarray.py` & `awkward-2.2.4/src/awkward/contents/listarray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/contents/listoffsetarray.py` & `awkward-2.2.4/src/awkward/contents/listoffsetarray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/contents/numpyarray.py` & `awkward-2.2.4/src/awkward/contents/numpyarray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/contents/recordarray.py` & `awkward-2.2.4/src/awkward/contents/recordarray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/contents/regulararray.py` & `awkward-2.2.4/src/awkward/contents/regulararray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/contents/unionarray.py` & `awkward-2.2.4/src/awkward/contents/unionarray.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import copy
 import ctypes
 from collections.abc import Iterable, MutableMapping, Sequence
 
 import awkward as ak
 from awkward._backends.backend import Backend
-from awkward._errors import AxisError
+from awkward._errors import AxisError, deprecate
 from awkward._layout import maybe_posaxis
 from awkward._nplikes.jax import Jax
 from awkward._nplikes.numpy import Numpy
 from awkward._nplikes.numpylike import ArrayLike, IndexType, NumpyMetadata
 from awkward._nplikes.shape import ShapeItem, unknown_length
 from awkward._nplikes.typetracer import OneOf, TypeTracer
 from awkward._parameters import parameters_intersect, parameters_union
@@ -131,14 +131,21 @@
                 raise TypeError(
                     "{0} cannot contain union-types in its 'contents' ({1}); try {0}.simplified instead".format(
                         type(self).__name__, type(content).__name__
                     )
                 )
             elif content.is_option:
                 n_seen_options += 1
+            elif content.is_indexed and content.parameter("__array__") != "categorical":
+                raise TypeError(
+                    (
+                        "{0} cannot contain non-categorical indexed-types in its 'contents' ({1}); "
+                        "try {0}.simplified instead"
+                    ).format(type(self).__name__, type(content).__name__)
+                )
 
         if n_seen_options not in {0, len(contents)}:
             raise TypeError(
                 "{0} must either be comprised of entirely optional contents, or no optional contents; "
                 "try {0}.simplified instead".format(type(self).__name__)
             )
 
@@ -217,17 +224,25 @@
     def simplified(
         cls,
         tags,
         index,
         contents,
         *,
         parameters=None,
-        merge=True,
+        merge=UNSET,
         mergebool=False,
     ):
+        if merge is UNSET:
+            merge = True
+        else:
+            deprecate(
+                "The `merge` argument to UnionArray.simplified(...) is deprecated; "
+                "it is no longer possible to construct UnionArrays with mergeable contents.",
+                version="2.4.0",
+            )
         self_index = index
         self_tags = tags
         self_contents = contents
 
         backend = None
         for content in contents:
             if backend is None:
@@ -392,14 +407,35 @@
                     contents.append(self_cont)
 
         if len(contents) > 2**7:
             raise NotImplementedError(
                 "FIXME: handle UnionArray with more than 127 contents"
             )
 
+        # If any contents are non-categorical index types, we can merge them into the union
+        # This is safe, because any remaining index types at this point in the routine are not considered
+        # mergeable with the other contents. This means none of the other contents are option or index types,
+        # nor are any contents mergeable with these index types' contents. We already know that the
+        # other contents cannot be unions. Thus, it's safe to simply erase the outer indexed type.
+        for tag, content in enumerate(contents):
+            if (
+                isinstance(content, ak.contents.IndexedArray)
+                and content.parameter("__array__") != "categorical"
+            ):
+                # only want to affect the part of the UnionArray.index for this tag
+                selection = tags.data == tag
+                # function-composition of this part of the UnionArray.index with the IndexedArray.index
+                index.data[selection] = content.index.data[index.data[selection]]
+                # now we don't have an IndexedArray anymore, but we want to preserve its parameters
+                contents[tag] = content.content.copy(
+                    parameters=parameters_union(
+                        content.content.parameters, content.parameters
+                    )
+                )
+
         # If any contents are options, ensure all contents are options!
         if any(c.is_option for c in contents):
             contents = [
                 c
                 if c.is_option
                 else c.to_IndexedOptionArray64()
                 if c.is_indexed
@@ -1053,26 +1089,23 @@
             tags, index, contents, parameters=self._parameters
         )
 
     def _mergemany(self, others: Sequence[Content]) -> Content:
         if len(others) == 0:
             return self
 
+        index_nplike = self._backend.index_nplike
         head, tail = self._merging_strategy(others)
 
         total_length = 0
         for array in head:
             total_length += array.length
 
-        nexttags = ak.index.Index8.empty(
-            total_length, nplike=self._backend.index_nplike
-        )
-        nextindex = ak.index.Index64.empty(
-            total_length, nplike=self._backend.index_nplike
-        )
+        nexttags = ak.index.Index8.empty(total_length, nplike=index_nplike)
+        nextindex = ak.index.Index64.empty(total_length, nplike=index_nplike)
 
         nextcontents = []
         length_so_far = 0
 
         parameters = self._parameters
         for array in head:
             if isinstance(array, ak.contents.EmptyArray):
@@ -1080,16 +1113,16 @@
 
             parameters = parameters_intersect(parameters, array._parameters)
             if isinstance(array, ak.contents.UnionArray):
                 union_tags = array.tags
                 union_index = array.index
                 union_contents = array.contents
                 assert (
-                    nexttags.nplike is self._backend.index_nplike
-                    and union_tags.nplike is self._backend.index_nplike
+                    nexttags.nplike is index_nplike
+                    and union_tags.nplike is index_nplike
                 )
                 self._backend.maybe_kernel_error(
                     self._backend[
                         "awkward_UnionArray_filltags",
                         nexttags.dtype.type,
                         union_tags.dtype.type,
                     ](
@@ -1097,16 +1130,16 @@
                         length_so_far,
                         union_tags.data,
                         array.length,
                         len(nextcontents),
                     )
                 )
                 assert (
-                    nextindex.nplike is self._backend.index_nplike
-                    and union_index.nplike is self._backend.index_nplike
+                    nextindex.nplike is index_nplike
+                    and union_index.nplike is index_nplike
                 )
                 self._backend.maybe_kernel_error(
                     self._backend[
                         "awkward_UnionArray_fillindex",
                         nextindex.dtype.type,
                         union_index.dtype.type,
                     ](
@@ -1116,29 +1149,62 @@
                         array.length,
                     )
                 )
                 length_so_far += array.length
 
                 nextcontents.extend(union_contents)
 
+            # This pathway is covered by `.simplified`, but we can avoid an extra array operation
+            # by performing this now
+            elif (
+                isinstance(array, ak.contents.IndexedArray)
+                and array.parameter("__array__") != "categorical"
+            ):
+                assert nexttags.nplike is index_nplike
+                self._backend.maybe_kernel_error(
+                    self._backend[
+                        "awkward_UnionArray_filltags_const",
+                        nexttags.dtype.type,
+                    ](
+                        nexttags.data,
+                        length_so_far,
+                        array.length,
+                        len(nextcontents),
+                    )
+                )
+                nextindex.data[
+                    index_nplike.shape_item_as_index(
+                        length_so_far
+                    ) : index_nplike.shape_item_as_index(length_so_far + array.length)
+                ] = array.index.data
+
+                length_so_far += array.length
+
+                nextcontents.append(
+                    array.content.copy(
+                        parameters=parameters_union(
+                            array.content._parameters, array._parameters
+                        )
+                    )
+                )
             else:
-                assert nexttags.nplike is self._backend.index_nplike
+                assert nexttags.nplike is index_nplike
                 self._backend.maybe_kernel_error(
                     self._backend[
                         "awkward_UnionArray_filltags_const",
                         nexttags.dtype.type,
                     ](
                         nexttags.data,
                         length_so_far,
                         array.length,
                         len(nextcontents),
                     )
                 )
 
-                assert nextindex.nplike is self._backend.index_nplike
+                assert nextindex.nplike is index_nplike
                 self._backend.maybe_kernel_error(
                     self._backend[
                         "awkward_UnionArray_fillindex_count", nextindex.dtype.type
                     ](nextindex.data, length_so_far, array.length)
                 )
 
                 length_so_far += array.length
@@ -1217,29 +1283,27 @@
 
     def _is_unique(self, negaxis, starts, parents, outlength):
         simplified = type(self).simplified(
             self._tags,
             self._index,
             self._contents,
             parameters=self._parameters,
-            merge=True,
             mergebool=True,
         )
         if isinstance(simplified, ak.contents.UnionArray):
             raise ValueError("cannot check if an irreducible UnionArray is unique")
 
         return simplified._is_unique(negaxis, starts, parents, outlength)
 
     def _unique(self, negaxis, starts, parents, outlength):
         simplified = type(self).simplified(
             self._tags,
             self._index,
             self._contents,
             parameters=self._parameters,
-            merge=True,
             mergebool=True,
         )
         if isinstance(simplified, ak.contents.UnionArray):
             raise ValueError("cannot make a unique irreducible UnionArray")
 
         return simplified._unique(negaxis, starts, parents, outlength)
```

### Comparing `awkward-2.2.3/src/awkward/contents/unmaskedarray.py` & `awkward-2.2.4/src/awkward/contents/unmaskedarray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/forms/__init__.py` & `awkward-2.2.4/src/awkward/forms/__init__.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/forms/bitmaskedform.py` & `awkward-2.2.4/src/awkward/forms/bitmaskedform.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 import awkward as ak
 from awkward._parameters import type_parameters_equal
-from awkward._typing import final
+from awkward._typing import Self, final
 from awkward._util import UNSET
 from awkward.forms.form import Form
 
 
 @final
 class BitMaskedForm(Form):
     is_option = True
@@ -193,18 +193,32 @@
     @property
     def dimension_optiontype(self):
         return True
 
     def _columns(self, path, output, list_indicator):
         self._content._columns(path, output, list_indicator)
 
-    def _select_columns(self, index, specifier, matches, output):
+    def _prune_columns(self, is_inside_record_or_union: bool) -> Self | None:
+        next_content = self._content._prune_columns(is_inside_record_or_union)
+        if next_content is None:
+            return None
+        else:
+            return BitMaskedForm(
+                self._mask,
+                next_content,
+                self._valid_when,
+                self._lsb_order,
+                parameters=self._parameters,
+                form_key=self._form_key,
+            )
+
+    def _select_columns(self, match_specifier):
         return BitMaskedForm(
             self._mask,
-            self._content._select_columns(index, specifier, matches, output),
+            self._content._select_columns(match_specifier),
             self._valid_when,
             self._lsb_order,
             parameters=self._parameters,
             form_key=self._form_key,
         )
 
     def _column_types(self):
```

### Comparing `awkward-2.2.3/src/awkward/forms/bytemaskedform.py` & `awkward-2.2.4/src/awkward/forms/bytemaskedform.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 import awkward as ak
 from awkward._parameters import type_parameters_equal
-from awkward._typing import final
+from awkward._typing import Self, final
 from awkward._util import UNSET
 from awkward.forms.form import Form
 
 
 @final
 class ByteMaskedForm(Form):
     is_option = True
@@ -170,18 +170,31 @@
     @property
     def dimension_optiontype(self):
         return True
 
     def _columns(self, path, output, list_indicator):
         self._content._columns(path, output, list_indicator)
 
-    def _select_columns(self, index, specifier, matches, output):
+    def _prune_columns(self, is_inside_record_or_union: bool) -> Self | None:
+        next_content = self._content._prune_columns(is_inside_record_or_union)
+        if next_content is None:
+            return None
+        else:
+            return ByteMaskedForm(
+                self._mask,
+                next_content,
+                self._valid_when,
+                parameters=self._parameters,
+                form_key=self._form_key,
+            )
+
+    def _select_columns(self, match_specifier):
         return ByteMaskedForm(
             self._mask,
-            self._content._select_columns(index, specifier, matches, output),
+            self._content._select_columns(match_specifier),
             self._valid_when,
             parameters=self._parameters,
             form_key=self._form_key,
         )
 
     def _column_types(self):
         return self._content._column_types()
```

### Comparing `awkward-2.2.3/src/awkward/forms/emptyform.py` & `awkward-2.2.4/src/awkward/forms/emptyform.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from __future__ import annotations
 
 from inspect import signature
 
 import awkward as ak
 from awkward._errors import deprecate
 from awkward._nplikes.shape import ShapeItem
-from awkward._typing import Iterator, final
+from awkward._typing import Iterator, Self, final
 from awkward._util import UNSET
 from awkward.forms.form import Form, JSONMapping
 
 
 @final
 class EmptyForm(Form):
     is_numpy = True
@@ -121,17 +121,18 @@
     @property
     def dimension_optiontype(self) -> bool:
         return False
 
     def _columns(self, path, output, list_indicator):
         output.append(".".join(path))
 
-    def _select_columns(self, index, specifier, matches, output):
-        if any(match and index >= len(item) for item, match in zip(specifier, matches)):
-            output.append(None)
+    def _select_columns(self, match_specifier):
+        return self
+
+    def _prune_columns(self, is_inside_record_or_union: bool) -> Self:
         return self
 
     def _column_types(self) -> tuple[str, ...]:
         return ("empty",)
 
     def _length_one_buffer_lengths(self) -> Iterator[ShapeItem]:
         yield 0
```

### Comparing `awkward-2.2.3/src/awkward/forms/form.py` & `awkward-2.2.4/src/awkward/forms/form.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 from __future__ import annotations
 
 import itertools
 import json
 import re
-from collections.abc import Mapping
+from collections import defaultdict
+from collections.abc import Iterable, Mapping
+from fnmatch import fnmatchcase
+from glob import escape as escape_glob
 
 import awkward as ak
 from awkward._backends.numpy import NumpyBackend
 from awkward._errors import deprecate
 from awkward._nplikes.numpylike import NumpyMetadata
 from awkward._nplikes.shape import ShapeItem, unknown_length
 from awkward._parameters import parameters_union
-from awkward._typing import Final, JSONMapping, JSONSerializable
+from awkward._typing import Final, JSONMapping, JSONSerializable, Self
 
 np = NumpyMetadata.instance()
 numpy_backend = NumpyBackend.instance()
 
 
 reserved_nominal_parameters: Final = frozenset(
     {
@@ -265,14 +268,74 @@
         for combo in itertools.product(*alts):
             replaced = list(text)
             for (start, stop), replacement in zip(spans, combo):
                 replaced[start:stop] = replacement
             yield from _expand_braces("".join(replaced), seen)
 
 
+class _SpecifierMatcher:
+    def __init__(
+        self, specifiers: Iterable[list[str]], *, match_if_empty: bool = False
+    ):
+        # We'll build two sets of unique fixed-strings and patterns
+        fixed_strings = set()
+        patterns = set()
+        # And then map these unique strings to their child specifiers
+        match_to_next_specifiers: defaultdict[str, list[list[str]]] = defaultdict(list)
+
+        # For each specifier, categorise it as a fixed-string or pattern,
+        # and build the next-specifier table
+        parent: str
+        child: list[str]
+        for item in specifiers:
+            parent, *child = item
+
+            if escape_glob(parent) == parent:
+                fixed_strings.add(parent)
+            else:
+                patterns.add(parent)
+
+            # Only include child specifier list if it is non-empty
+            if child:
+                match_to_next_specifiers[parent].append(child)
+
+        self._match_to_next_specifiers = match_to_next_specifiers
+        self._fixed_strings = fixed_strings
+        self._patterns = patterns
+        self._match_if_empty = match_if_empty
+
+    @property
+    def is_empty(self) -> bool:
+        return not (self._patterns or self._fixed_strings)
+
+    def __call__(self, field: str, *, next_match_if_empty: bool = False) -> Self | None:
+        has_matched = False
+
+        # Fixed-strings are an O(log n) lookup
+        next_specifiers = []
+        if field in self._fixed_strings:
+            has_matched = True
+            next_specifiers.extend(self._match_to_next_specifiers[field])
+
+        # Fixed-strings are an O(n) lookup
+        for pattern in self._patterns:
+            if fnmatchcase(field, pattern):
+                has_matched = True
+                next_specifiers.extend(self._match_to_next_specifiers[pattern])
+
+        if has_matched:
+            return _SpecifierMatcher(
+                next_specifiers, match_if_empty=next_match_if_empty
+            )
+        elif self.is_empty and self._match_if_empty:
+            return self
+        else:
+            return
+
+
 class Form:
     is_numpy = False
     is_unknown = False
     is_list = False
     is_regular = False
     is_option = False
     is_indexed = False
@@ -389,44 +452,56 @@
         return self.type
 
     def columns(self, list_indicator=None, column_prefix=()):
         output = []
         self._columns(column_prefix, output, list_indicator)
         return output
 
-    def select_columns(self, specifier, expand_braces=True):
+    def select_columns(
+        self, specifier, expand_braces=True, *, prune_unions_and_records: bool = True
+    ):
         if isinstance(specifier, str):
-            specifier = [specifier]
+            specifier = {specifier}
 
+        # Only take unique specifiers
         for item in specifier:
             if not isinstance(item, str):
                 raise TypeError(
-                    "a column-selection specifier must be a list of strings"
+                    "a column-selection specifier must be a list of non-empty strings"
+                )
+            if not item:
+                raise ValueError(
+                    "a column-selection specifier must be a list of non-empty strings"
                 )
 
         if expand_braces:
             next_specifier = []
             for item in specifier:
                 for result in _expand_braces(item):
                     next_specifier.append(result)
             specifier = next_specifier
 
         specifier = [[] if item == "" else item.split(".") for item in set(specifier)]
-        matches = [True] * len(specifier)
-
-        output = []
-        return self._select_columns(0, specifier, matches, output)
+        match_specifier = _SpecifierMatcher(specifier, match_if_empty=False)
+        selection = self._select_columns(match_specifier)
+        if prune_unions_and_records:
+            return selection._prune_columns(False)
+        else:
+            return selection
 
     def column_types(self):
         return self._column_types()
 
     def _columns(self, path, output, list_indicator):
         raise NotImplementedError
 
-    def _select_columns(self, index, specifier, matches, output):
+    def _prune_columns(self, is_inside_record_or_union: bool) -> Self | None:
+        raise NotImplementedError
+
+    def _select_columns(self, match_specifier) -> Self | None:
         raise NotImplementedError
 
     def _column_types(self):
         raise NotImplementedError
 
     def _to_dict_part(self, verbose, toplevel):
         raise NotImplementedError
```

### Comparing `awkward-2.2.3/src/awkward/forms/indexedform.py` & `awkward-2.2.4/src/awkward/forms/indexedoptionform.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
-
 import awkward as ak
 from awkward._parameters import parameters_union, type_parameters_equal
-from awkward._typing import final
+from awkward._typing import Self, final
 from awkward._util import UNSET
 from awkward.forms.form import Form
 
 
 @final
-class IndexedForm(Form):
+class IndexedOptionForm(Form):
+    is_option = True
     is_indexed = True
 
     def __init__(
         self,
         index,
-        content=None,
+        content,
         *,
         parameters=None,
         form_key=None,
     ):
         if not isinstance(index, str):
             raise TypeError(
                 "{} 'index' must be of type str, not {}".format(
@@ -48,15 +48,15 @@
         self,
         index=UNSET,
         content=UNSET,
         *,
         parameters=UNSET,
         form_key=UNSET,
     ):
-        return IndexedForm(
+        return IndexedOptionForm(
             self._index if index is UNSET else index,
             self._content if content is UNSET else content,
             parameters=self._parameters if parameters is UNSET else parameters,
             form_key=self._form_key if form_key is UNSET else form_key,
         )
 
     @classmethod
@@ -67,75 +67,56 @@
         *,
         parameters=None,
         form_key=None,
     ):
         is_cat = parameters is not None and parameters.get("__array__") == "categorical"
 
         if content.is_union and not is_cat:
-            return content.copy(
-                parameters=parameters_union(content._parameters, parameters)
-            )
+            return content._union_of_optionarrays(index, parameters)
 
-        elif content.is_option:
+        elif content.is_indexed or content.is_option:
             return ak.forms.IndexedOptionForm.simplified(
                 "i64",
                 content.content,
                 parameters=parameters_union(content._parameters, parameters),
             )
 
-        elif content.is_indexed:
-            return IndexedForm(
-                "i64",
-                content.content,
-                parameters=parameters_union(content._parameters, parameters),
-            )
-
         else:
             return cls(index, content, parameters=parameters, form_key=form_key)
 
     def __repr__(self):
         args = [repr(self._index), repr(self._content), *self._repr_args()]
         return "{}({})".format(type(self).__name__, ", ".join(args))
 
     def _to_dict_part(self, verbose, toplevel):
         return self._to_dict_extra(
             {
-                "class": "IndexedArray",
+                "class": "IndexedOptionArray",
                 "index": self._index,
                 "content": self._content._to_dict_part(verbose, toplevel=False),
             },
             verbose,
         )
 
     @property
     def type(self):
-        out = self._content.type
-
-        if self._parameters is not None:
-            if out._parameters is None:
-                out._parameters = self._parameters
-            else:
-                out._parameters = parameters_union(out._parameters, self._parameters)
-
-            if self._parameters.get("__array__") == "categorical":
-                if out._parameters is self._parameters:
-                    out._parameters = dict(out._parameters)
-
-                # Restore content __array__
-                out_array = self._content.parameter("__array__")
-                if out_array is not None:
-                    out._parameters["__array__"] = out_array
-                else:
-                    del out._parameters["__array__"]
-                out._parameters["__categorical__"] = True
+        if self.parameter("__array__") == "categorical":
+            parameters = dict(self._parameters)
+            del parameters["__array__"]
+            parameters["__categorical__"] = True
+        else:
+            parameters = self._parameters
 
-        return out
+        return ak.types.OptionType(
+            self._content.type,
+            parameters=parameters,
+        ).simplify_option_union()
 
     def __eq__(self, other):
-        if isinstance(other, IndexedForm):
+        if isinstance(other, IndexedOptionForm):
             return (
                 self._form_key == other._form_key
                 and self._index == other._index
                 and type_parameters_equal(self._parameters, other._parameters)
                 and self._content == other._content
             )
         else:
@@ -153,15 +134,15 @@
 
     @property
     def purelist_depth(self):
         return self._content.purelist_depth
 
     @property
     def is_identity_like(self):
-        return False
+        return self._content.is_identity_like
 
     @property
     def minmax_depth(self):
         return self._content.minmax_depth
 
     @property
     def branch_depth(self):
@@ -173,22 +154,34 @@
 
     @property
     def is_tuple(self):
         return self._content.is_tuple
 
     @property
     def dimension_optiontype(self):
-        return False
+        return True
 
     def _columns(self, path, output, list_indicator):
         self._content._columns(path, output, list_indicator)
 
-    def _select_columns(self, index, specifier, matches, output):
-        return IndexedForm(
+    def _prune_columns(self, is_inside_record_or_union: bool) -> Self | None:
+        next_content = self._content._prune_columns(is_inside_record_or_union)
+        if next_content is None:
+            return None
+        else:
+            return IndexedOptionForm(
+                self._index,
+                next_content,
+                parameters=self._parameters,
+                form_key=self._form_key,
+            )
+
+    def _select_columns(self, match_specifier):
+        return IndexedOptionForm(
             self._index,
-            self._content._select_columns(index, specifier, matches, output),
+            self._content._select_columns(match_specifier),
             parameters=self._parameters,
             form_key=self._form_key,
         )
 
     def _column_types(self):
         return self._content._column_types()
```

### Comparing `awkward-2.2.3/src/awkward/forms/indexedoptionform.py` & `awkward-2.2.4/src/awkward/forms/listoffsetform.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,175 +1,174 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
+from __future__ import annotations
+
 import awkward as ak
-from awkward._parameters import parameters_union, type_parameters_equal
-from awkward._typing import final
+from awkward._parameters import type_parameters_equal
+from awkward._typing import JSONMapping, final
 from awkward._util import UNSET
 from awkward.forms.form import Form
 
 
 @final
-class IndexedOptionForm(Form):
-    is_option = True
-    is_indexed = True
+class ListOffsetForm(Form):
+    is_list = True
 
     def __init__(
         self,
-        index,
-        content,
+        offsets: str,
+        content: Form,
         *,
-        parameters=None,
-        form_key=None,
+        parameters: JSONMapping | None = None,
+        form_key: str | None = None,
     ):
-        if not isinstance(index, str):
-            raise TypeError(
-                "{} 'index' must be of type str, not {}".format(
-                    type(self).__name__, repr(index)
-                )
-            )
-        if not isinstance(content, Form):
+        if not isinstance(offsets, str):
             raise TypeError(
-                "{} all 'contents' must be Form subclasses, not {}".format(
-                    type(self).__name__, repr(content)
+                "{} 'offsets' must be of type str, not {}".format(
+                    type(self).__name__, repr(offsets)
                 )
             )
 
-        self._index = index
+        self._offsets = offsets
         self._content = content
         self._init(parameters=parameters, form_key=form_key)
 
     @property
-    def index(self):
-        return self._index
+    def offsets(self):
+        return self._offsets
 
     @property
     def content(self):
         return self._content
 
     def copy(
         self,
-        index=UNSET,
+        offsets=UNSET,
         content=UNSET,
         *,
         parameters=UNSET,
         form_key=UNSET,
     ):
-        return IndexedOptionForm(
-            self._index if index is UNSET else index,
+        return ListOffsetForm(
+            self._offsets if offsets is UNSET else offsets,
             self._content if content is UNSET else content,
             parameters=self._parameters if parameters is UNSET else parameters,
             form_key=self._form_key if form_key is UNSET else form_key,
         )
 
     @classmethod
-    def simplified(
-        cls,
-        index,
-        content,
-        *,
-        parameters=None,
-        form_key=None,
-    ):
-        is_cat = parameters is not None and parameters.get("__array__") == "categorical"
-
-        if content.is_union and not is_cat:
-            return content._union_of_optionarrays(index, parameters)
-
-        elif content.is_indexed or content.is_option:
-            return ak.forms.IndexedOptionForm.simplified(
-                "i64",
-                content.content,
-                parameters=parameters_union(content._parameters, parameters),
-            )
-
-        else:
-            return cls(index, content, parameters=parameters, form_key=form_key)
+    def simplified(cls, offsets, content, *, parameters=None, form_key=None):
+        return cls(offsets, content, parameters=parameters, form_key=form_key)
 
     def __repr__(self):
-        args = [repr(self._index), repr(self._content), *self._repr_args()]
+        args = [repr(self._offsets), repr(self._content), *self._repr_args()]
         return "{}({})".format(type(self).__name__, ", ".join(args))
 
     def _to_dict_part(self, verbose, toplevel):
         return self._to_dict_extra(
             {
-                "class": "IndexedOptionArray",
-                "index": self._index,
+                "class": "ListOffsetArray",
+                "offsets": self._offsets,
                 "content": self._content._to_dict_part(verbose, toplevel=False),
             },
             verbose,
         )
 
     @property
     def type(self):
-        if self.parameter("__array__") == "categorical":
-            parameters = dict(self._parameters)
-            del parameters["__array__"]
-            parameters["__categorical__"] = True
-        else:
-            parameters = self._parameters
-
-        return ak.types.OptionType(
+        return ak.types.ListType(
             self._content.type,
-            parameters=parameters,
-        ).simplify_option_union()
+            parameters=self._parameters,
+        )
 
     def __eq__(self, other):
-        if isinstance(other, IndexedOptionForm):
+        if isinstance(other, ListOffsetForm):
             return (
                 self._form_key == other._form_key
-                and self._index == other._index
+                and self._offsets == other._offsets
                 and type_parameters_equal(self._parameters, other._parameters)
                 and self._content == other._content
             )
         else:
             return False
 
     def purelist_parameter(self, key):
         if self._parameters is None or key not in self._parameters:
             return self._content.purelist_parameter(key)
         else:
             return self._parameters[key]
 
     @property
     def purelist_isregular(self):
-        return self._content.purelist_isregular
+        return False
 
     @property
     def purelist_depth(self):
-        return self._content.purelist_depth
+        if self.parameter("__array__") in ("string", "bytestring"):
+            return 1
+        else:
+            return self._content.purelist_depth + 1
 
     @property
     def is_identity_like(self):
-        return self._content.is_identity_like
+        return False
 
     @property
     def minmax_depth(self):
-        return self._content.minmax_depth
+        if self.parameter("__array__") in ("string", "bytestring"):
+            return (1, 1)
+        else:
+            mindepth, maxdepth = self._content.minmax_depth
+            return (mindepth + 1, maxdepth + 1)
 
     @property
     def branch_depth(self):
-        return self._content.branch_depth
+        if self.parameter("__array__") in ("string", "bytestring"):
+            return (False, 1)
+        else:
+            branch, depth = self._content.branch_depth
+            return (branch, depth + 1)
 
     @property
     def fields(self):
         return self._content.fields
 
     @property
     def is_tuple(self):
         return self._content.is_tuple
 
     @property
     def dimension_optiontype(self):
-        return True
+        return False
 
     def _columns(self, path, output, list_indicator):
+        if (
+            self.parameter("__array__") not in ("string", "bytestring")
+            and list_indicator is not None
+        ):
+            path = (*path, list_indicator)
         self._content._columns(path, output, list_indicator)
 
-    def _select_columns(self, index, specifier, matches, output):
-        return IndexedOptionForm(
-            self._index,
-            self._content._select_columns(index, specifier, matches, output),
+    def _prune_columns(self, is_inside_record_or_union: bool):
+        next_content = self._content._prune_columns(is_inside_record_or_union)
+        if next_content is None:
+            return None
+        else:
+            return ListOffsetForm(
+                self._offsets,
+                next_content,
+                parameters=self._parameters,
+                form_key=self._form_key,
+            )
+
+    def _select_columns(self, match_specifier):
+        return ListOffsetForm(
+            self._offsets,
+            self._content._select_columns(match_specifier),
             parameters=self._parameters,
             form_key=self._form_key,
         )
 
     def _column_types(self):
-        return self._content._column_types()
+        if self.parameter("__array__") in ("string", "bytestring"):
+            return ("string",)
+        else:
+            return self._content._column_types()
```

### Comparing `awkward-2.2.3/src/awkward/forms/listform.py` & `awkward-2.2.4/src/awkward/forms/listform.py`

 * *Files 3% similar despite different names*

```diff
@@ -176,19 +176,32 @@
         if (
             self.parameter("__array__") not in ("string", "bytestring")
             and list_indicator is not None
         ):
             path = (*path, list_indicator)
         self._content._columns(path, output, list_indicator)
 
-    def _select_columns(self, index, specifier, matches, output):
+    def _prune_columns(self, is_inside_record_or_union: bool):
+        next_content = self._content._prune_columns(is_inside_record_or_union)
+        if next_content is None:
+            return None
+        else:
+            return ListForm(
+                self._starts,
+                self._stops,
+                next_content,
+                parameters=self._parameters,
+                form_key=self._form_key,
+            )
+
+    def _select_columns(self, match_specifier):
         return ListForm(
             self._starts,
             self._stops,
-            self._content._select_columns(index, specifier, matches, output),
+            self._content._select_columns(match_specifier),
             parameters=self._parameters,
             form_key=self._form_key,
         )
 
     def _column_types(self):
         if self.parameter("__array__") in ("string", "bytestring"):
             return ("string",)
```

### Comparing `awkward-2.2.3/src/awkward/forms/listoffsetform.py` & `awkward-2.2.4/src/awkward/forms/unmaskedform.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,162 +1,157 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
-from __future__ import annotations
-
 import awkward as ak
-from awkward._parameters import type_parameters_equal
-from awkward._typing import JSONMapping, final
+from awkward._parameters import parameters_union, type_parameters_equal
+from awkward._typing import Self, final
 from awkward._util import UNSET
 from awkward.forms.form import Form
 
 
 @final
-class ListOffsetForm(Form):
-    is_list = True
+class UnmaskedForm(Form):
+    is_option = True
 
     def __init__(
         self,
-        offsets: str,
-        content: Form,
+        content,
         *,
-        parameters: JSONMapping | None = None,
-        form_key: str | None = None,
+        parameters=None,
+        form_key=None,
     ):
-        if not isinstance(offsets, str):
+        if not isinstance(content, Form):
             raise TypeError(
-                "{} 'offsets' must be of type str, not {}".format(
-                    type(self).__name__, repr(offsets)
+                "{} all 'contents' must be Form subclasses, not {}".format(
+                    type(self).__name__, repr(content)
                 )
             )
 
-        self._offsets = offsets
         self._content = content
         self._init(parameters=parameters, form_key=form_key)
 
     @property
-    def offsets(self):
-        return self._offsets
-
-    @property
     def content(self):
         return self._content
 
     def copy(
         self,
-        offsets=UNSET,
         content=UNSET,
         *,
         parameters=UNSET,
         form_key=UNSET,
     ):
-        return ListOffsetForm(
-            self._offsets if offsets is UNSET else offsets,
+        return UnmaskedForm(
             self._content if content is UNSET else content,
             parameters=self._parameters if parameters is UNSET else parameters,
             form_key=self._form_key if form_key is UNSET else form_key,
         )
 
     @classmethod
-    def simplified(cls, offsets, content, *, parameters=None, form_key=None):
-        return cls(offsets, content, parameters=parameters, form_key=form_key)
+    def simplified(
+        cls,
+        content,
+        *,
+        parameters=None,
+        form_key=None,
+    ):
+        if content.is_union:
+            return content.copy(
+                contents=[cls.simplified(x) for x in content.contents],
+                parameters=parameters_union(content._parameters, parameters),
+            )
+        elif content.is_indexed or content.is_option:
+            return content.copy(
+                parameters=parameters_union(content._parameters, parameters)
+            )
+        else:
+            return cls(content, parameters=parameters, form_key=form_key)
 
     def __repr__(self):
-        args = [repr(self._offsets), repr(self._content), *self._repr_args()]
+        args = [repr(self._content), *self._repr_args()]
         return "{}({})".format(type(self).__name__, ", ".join(args))
 
     def _to_dict_part(self, verbose, toplevel):
         return self._to_dict_extra(
             {
-                "class": "ListOffsetArray",
-                "offsets": self._offsets,
+                "class": "UnmaskedArray",
                 "content": self._content._to_dict_part(verbose, toplevel=False),
             },
             verbose,
         )
 
     @property
     def type(self):
-        return ak.types.ListType(
+        return ak.types.OptionType(
             self._content.type,
             parameters=self._parameters,
-        )
+        ).simplify_option_union()
 
     def __eq__(self, other):
-        if isinstance(other, ListOffsetForm):
+        if isinstance(other, UnmaskedForm):
             return (
                 self._form_key == other._form_key
-                and self._offsets == other._offsets
                 and type_parameters_equal(self._parameters, other._parameters)
                 and self._content == other._content
             )
         else:
             return False
 
     def purelist_parameter(self, key):
         if self._parameters is None or key not in self._parameters:
             return self._content.purelist_parameter(key)
         else:
             return self._parameters[key]
 
     @property
     def purelist_isregular(self):
-        return False
+        return self._content.purelist_isregular
 
     @property
     def purelist_depth(self):
-        if self.parameter("__array__") in ("string", "bytestring"):
-            return 1
-        else:
-            return self._content.purelist_depth + 1
+        return self._content.purelist_depth
 
     @property
     def is_identity_like(self):
-        return False
+        return self._content.is_identity_like
 
     @property
     def minmax_depth(self):
-        if self.parameter("__array__") in ("string", "bytestring"):
-            return (1, 1)
-        else:
-            mindepth, maxdepth = self._content.minmax_depth
-            return (mindepth + 1, maxdepth + 1)
+        return self._content.minmax_depth
 
     @property
     def branch_depth(self):
-        if self.parameter("__array__") in ("string", "bytestring"):
-            return (False, 1)
-        else:
-            branch, depth = self._content.branch_depth
-            return (branch, depth + 1)
+        return self._content.branch_depth
 
     @property
     def fields(self):
         return self._content.fields
 
     @property
     def is_tuple(self):
         return self._content.is_tuple
 
     @property
     def dimension_optiontype(self):
-        return False
+        return True
 
     def _columns(self, path, output, list_indicator):
-        if (
-            self.parameter("__array__") not in ("string", "bytestring")
-            and list_indicator is not None
-        ):
-            path = (*path, list_indicator)
         self._content._columns(path, output, list_indicator)
 
-    def _select_columns(self, index, specifier, matches, output):
-        return ListOffsetForm(
-            self._offsets,
-            self._content._select_columns(index, specifier, matches, output),
+    def _prune_columns(self, is_inside_record_or_union: bool) -> Self | None:
+        next_content = self._content._prune_columns(is_inside_record_or_union)
+        if next_content is None:
+            return None
+        else:
+            return UnmaskedForm(
+                next_content,
+                parameters=self._parameters,
+                form_key=self._form_key,
+            )
+
+    def _select_columns(self, match_specifier):
+        return UnmaskedForm(
+            self._content._select_columns(match_specifier),
             parameters=self._parameters,
             form_key=self._form_key,
         )
 
     def _column_types(self):
-        if self.parameter("__array__") in ("string", "bytestring"):
-            return ("string",)
-        else:
-            return self._content._column_types()
+        return self._content._column_types()
```

### Comparing `awkward-2.2.3/src/awkward/forms/numpyform.py` & `awkward-2.2.4/src/awkward/forms/numpyform.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 from collections.abc import Iterable
 
 import awkward as ak
 from awkward._errors import deprecate
 from awkward._nplikes.numpylike import NumpyMetadata
 from awkward._parameters import type_parameters_equal
-from awkward._typing import final
+from awkward._typing import Self, final
 from awkward._util import UNSET
 from awkward.forms.form import Form
 
 np = NumpyMetadata.instance()
 
 
 def from_dtype(dtype, parameters=None, *, time_units_as_parameter: bool = UNSET):
@@ -208,14 +208,15 @@
     @property
     def dimension_optiontype(self):
         return False
 
     def _columns(self, path, output, list_indicator):
         output.append(".".join(path))
 
-    def _select_columns(self, index, specifier, matches, output):
-        if any(match and index >= len(item) for item, match in zip(specifier, matches)):
-            output.append(None)
+    def _select_columns(self, match_specifier):
+        return self
+
+    def _prune_columns(self, is_inside_record_or_union: bool) -> Self:
         return self
 
     def _column_types(self):
         return (ak.types.numpytype.primitive_to_dtype(self._primitive),)
```

### Comparing `awkward-2.2.3/src/awkward/forms/recordform.py` & `awkward-2.2.4/src/awkward/forms/recordform.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
-import glob
 from collections.abc import Iterable
 
 import awkward as ak
 from awkward._parameters import type_parameters_equal
 from awkward._regularize import is_integer
 from awkward._typing import final
 from awkward._util import UNSET
@@ -237,31 +236,50 @@
     def dimension_optiontype(self):
         return False
 
     def _columns(self, path, output, list_indicator):
         for content, field in zip(self._contents, self.fields):
             content._columns((*path, field), output, list_indicator)
 
-    def _select_columns(self, index, specifier, matches, output):
+    def _prune_columns(self, is_inside_record_or_union: bool):
         contents = []
         fields = []
         for content, field in zip(self._contents, self.fields):
-            next_matches = [
-                matches[i]
-                and (index >= len(item) or glob.fnmatch.fnmatchcase(field, item[index]))
-                for i, item in enumerate(specifier)
-            ]
-            if any(next_matches):
-                len_output = len(output)
-                next_content = content._select_columns(
-                    index + 1, specifier, next_matches, output
-                )
-                if len_output != len(output):
-                    contents.append(next_content)
-                    fields.append(field)
+            next_content = content._prune_columns(True)
+            if next_content is None:
+                continue
+            contents.append(next_content)
+            fields.append(field)
+
+        if fields or not is_inside_record_or_union:
+            return RecordForm(
+                contents,
+                fields,
+                parameters=self._parameters,
+                form_key=self._form_key,
+            )
+        # If all subtrees are pruned (or we have no subtrees!), then we should prune this form too
+        else:
+            return None
+
+    def _select_columns(self, match_specifier):
+        contents = []
+        fields = []
+        for content, field in zip(self._contents, self.fields):
+            # Try and match this field, allowing derived matcher to match any field if empty
+            next_match_specifier = match_specifier(field, next_match_if_empty=True)
+            if next_match_specifier is None:
+                continue
+
+            # NOTE: we could optimise this by avoiding column selection if we know the entire subtree will match
+            #       this is given by `next_match_specifier.is_empty`, *but* we also want to perform column pruning
+            #       meaning this optimisation is less useful, we we'd require a special prune-only pass
+            next_content = content._select_columns(next_match_specifier)
+            contents.append(next_content)
+            fields.append(field)
 
         return RecordForm(
             contents,
             fields,
             parameters=self._parameters,
             form_key=self._form_key,
         )
```

### Comparing `awkward-2.2.3/src/awkward/forms/regularform.py` & `awkward-2.2.4/src/awkward/forms/regularform.py`

 * *Files 21% similar despite different names*

```diff
@@ -137,17 +137,29 @@
         if (
             self.parameter("__array__") not in ("string", "bytestring")
             and list_indicator is not None
         ):
             path = (*path, list_indicator)
         self._content._columns(path, output, list_indicator)
 
-    def _select_columns(self, index, specifier, matches, output):
+    def _prune_columns(self, is_inside_record_or_union: bool):
+        next_content = self._content._prune_columns(is_inside_record_or_union)
+        if next_content is None:
+            return None
+        else:
+            return RegularForm(
+                next_content,
+                self._size,
+                parameters=self._parameters,
+                form_key=self._form_key,
+            )
+
+    def _select_columns(self, match_specifier):
         return RegularForm(
-            self._content._select_columns(index, specifier, matches, output),
+            self._content._select_columns(match_specifier),
             self._size,
             parameters=self._parameters,
             form_key=self._form_key,
         )
 
     def _column_types(self):
         if self.parameter("__array__") in ("string", "bytestring"):
```

### Comparing `awkward-2.2.3/src/awkward/forms/unionform.py` & `awkward-2.2.4/src/awkward/forms/unionform.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 from collections import Counter
 from collections.abc import Iterable
 
 import awkward as ak
 from awkward._parameters import type_parameters_equal
-from awkward._typing import final
+from awkward._typing import Self, final
 from awkward._util import UNSET
 from awkward.forms.form import Form
 
 
 @final
 class UnionForm(Form):
     is_union = True
@@ -227,30 +227,47 @@
                 return True
         return False
 
     def _columns(self, path, output, list_indicator):
         for content, field in zip(self._contents, self.fields):
             content._columns((*path, field), output, list_indicator)
 
-    def _select_columns(self, index, specifier, matches, output):
+    def _prune_columns(self, is_inside_record_or_union: bool) -> Self | None:
         contents = []
         for content in self._contents:
-            len_output = len(output)
-            next_content = content._select_columns(index, specifier, matches, output)
-            if len_output != len(output):
-                contents.append(next_content)
+            next_content = content._prune_columns(True)
+            if next_content is None:
+                continue
+            contents.append(next_content)
 
         if len(contents) == 0:
-            return ak.forms.EmptyForm(form_key=self._form_key)
+            if is_inside_record_or_union:
+                return None
+            else:
+                # outermost unions should return an EmptyForm instead
+                return ak.forms.EmptyForm(form_key=self._form_key)
         elif len(contents) == 1:
             return contents[0]
         else:
             return UnionForm(
                 self._tags,
                 self._index,
                 contents,
                 parameters=self._parameters,
                 form_key=self._form_key,
             )
 
+    def _select_columns(self, match_specifier):
+        contents = [
+            content._select_columns(match_specifier) for content in self._contents
+        ]
+
+        return UnionForm(
+            self._tags,
+            self._index,
+            contents,
+            parameters=self._parameters,
+            form_key=self._form_key,
+        )
+
     def _column_types(self):
         return sum((x._column_types() for x in self._contents), ())
```

### Comparing `awkward-2.2.3/src/awkward/operations/__init__.py` & `awkward-2.2.4/src/awkward/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/operations/ak_all.py` & `awkward-2.2.4/src/awkward/operations/ak_all.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("all",)
 import awkward as ak
 from awkward._behavior import behavior_of
 from awkward._connect.numpy import UNSUPPORTED
+from awkward._dispatch import high_level_function
 from awkward._layout import wrap_layout
 from awkward._nplikes.numpylike import NumpyMetadata
 from awkward._regularize import regularize_axis
 
 np = NumpyMetadata.instance()
 
 
+@high_level_function
 def all(
     array,
     axis=None,
     *,
     keepdims=False,
     mask_identity=False,
     highlevel=True,
@@ -47,26 +49,19 @@
     [all](https://docs.scipy.org/doc/numpy/reference/generated/numpy.all.html)
     if all lists at a given dimension have the same length and no None values,
     but it generalizes to cases where they do not.
 
     See #ak.sum for a more complete description of nested list and missing
     value (None) handling in reducers.
     """
-    with ak._errors.OperationErrorContext(
-        "ak.all",
-        {
-            "array": array,
-            "axis": axis,
-            "keepdims": keepdims,
-            "mask_identity": mask_identity,
-            "highlevel": highlevel,
-            "behavior": behavior,
-        },
-    ):
-        return _impl(array, axis, keepdims, mask_identity, highlevel, behavior)
+    # Dispatch
+    yield (array,)
+
+    # Implementation
+    return _impl(array, axis, keepdims, mask_identity, highlevel, behavior)
 
 
 def _impl(array, axis, keepdims, mask_identity, highlevel, behavior):
     axis = regularize_axis(axis)
     layout = ak.operations.to_layout(array, allow_record=False, allow_other=False)
     behavior = behavior_of(array, behavior=behavior)
     reducer = ak._reducers.All()
```

### Comparing `awkward-2.2.3/src/awkward/operations/ak_almost_equal.py` & `awkward-2.2.4/src/awkward/operations/ak_almost_equal.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 from __future__ import annotations
 
 __all__ = ("almost_equal",)
-
-
 from awkward._backends.dispatch import backend_of
 from awkward._behavior import behavior_of, get_array_class, get_record_class
+from awkward._dispatch import high_level_function
 from awkward._nplikes.numpylike import NumpyMetadata
 from awkward._parameters import parameters_are_equal
 from awkward.operations.ak_to_layout import to_layout
 
 np = NumpyMetadata.instance()
 
 
+@high_level_function
 def almost_equal(
     left,
     right,
     *,
     rtol: float = 1e-5,
     atol: float = 1e-8,
     dtype_exact: bool = True,
     check_parameters: bool = True,
     check_regular: bool = True,
-) -> bool:
+):
     """
     Args:
         left: Array-like data (anything #ak.to_layout recognizes).
         right: Array-like data (anything #ak.to_layout recognizes).
         rtol: the relative tolerance parameter (see below).
         atol: the absolute tolerance parameter (see below).
         dtype_exact: whether the dtypes must be exactly the same, or just the
@@ -41,14 +41,18 @@
     The relative difference (`rtol * abs(b)`) and the absolute difference `atol`
     are added together to compare against the absolute difference between `left`
     and `right`.
 
     TypeTracer arrays are not supported, as there is very little information to
     be compared.
     """
+    # Dispatch
+    yield left, right
+
+    # Implementation
     left_behavior = behavior_of(left)
     right_behavior = behavior_of(right)
 
     left = to_layout(left, allow_record=False).to_packed()
     right = to_layout(right, allow_record=False).to_packed()
 
     backend = backend_of(left, right)
```

### Comparing `awkward-2.2.3/src/awkward/operations/ak_any.py` & `awkward-2.2.4/src/awkward/operations/ak_any.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("any",)
 import awkward as ak
 from awkward._behavior import behavior_of
 from awkward._connect.numpy import UNSUPPORTED
+from awkward._dispatch import high_level_function
 from awkward._layout import wrap_layout
 from awkward._nplikes.numpylike import NumpyMetadata
 from awkward._regularize import regularize_axis
 
 np = NumpyMetadata.instance()
 
 
+@high_level_function
 def any(
     array,
     axis=None,
     *,
     keepdims=False,
     mask_identity=False,
     highlevel=True,
@@ -47,26 +49,19 @@
     [any](https://docs.scipy.org/doc/numpy/reference/generated/numpy.any.html)
     if all lists at a given dimension have the same length and no None values,
     but it generalizes to cases where they do not.
 
     See #ak.sum for a more complete description of nested list and missing
     value (None) handling in reducers.
     """
-    with ak._errors.OperationErrorContext(
-        "ak.any",
-        {
-            "array": array,
-            "axis": axis,
-            "keepdims": keepdims,
-            "mask_identity": mask_identity,
-            "highlevel": highlevel,
-            "behavior": behavior,
-        },
-    ):
-        return _impl(array, axis, keepdims, mask_identity, highlevel, behavior)
+    # Dispatch
+    yield (array,)
+
+    # Implementation
+    return _impl(array, axis, keepdims, mask_identity, highlevel, behavior)
 
 
 def _impl(array, axis, keepdims, mask_identity, highlevel, behavior):
     axis = regularize_axis(axis)
     layout = ak.operations.to_layout(array, allow_record=False, allow_other=False)
     behavior = behavior_of(array, behavior=behavior)
     reducer = ak._reducers.Any()
```

### Comparing `awkward-2.2.3/src/awkward/operations/ak_argcartesian.py` & `awkward-2.2.4/src/awkward/operations/ak_argcartesian.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("argcartesian",)
+from collections.abc import Mapping
+
 import awkward as ak
 from awkward._backends.dispatch import backend_of
 from awkward._backends.numpy import NumpyBackend
 from awkward._behavior import behavior_of
+from awkward._dispatch import high_level_function
 from awkward._layout import wrap_layout
 from awkward._nplikes.numpylike import NumpyMetadata
 from awkward._regularize import regularize_axis
 
 np = NumpyMetadata.instance()
 cpu = NumpyBackend.instance()
 
 
+@high_level_function
 def argcartesian(
     arrays,
     axis=1,
     *,
     nested=None,
     parameters=None,
     with_name=None,
@@ -84,27 +88,22 @@
         <Array [1.1, 1.1, 2.2, 2.2, 3.3, 3.3] type='6 * float64'>
         >>> two[two_index]
         <Array ['a', 'b', 'a', 'b', 'a', 'b'] type='6 * string'>
 
     All of the parameters for #ak.cartesian apply equally to #ak.argcartesian,
     so see the #ak.cartesian documentation for a more complete description.
     """
-    with ak._errors.OperationErrorContext(
-        "ak.argcartesian",
-        {
-            "arrays": arrays,
-            "axis": axis,
-            "nested": nested,
-            "parameters": parameters,
-            "with_name": with_name,
-            "highlevel": highlevel,
-            "behavior": behavior,
-        },
-    ):
-        return _impl(arrays, axis, nested, parameters, with_name, highlevel, behavior)
+    # Dispatch
+    if isinstance(arrays, Mapping):
+        yield arrays.values()
+    else:
+        yield arrays
+
+    # Implementation
+    return _impl(arrays, axis, nested, parameters, with_name, highlevel, behavior)
 
 
 def _impl(arrays, axis, nested, parameters, with_name, highlevel, behavior):
     axis = regularize_axis(axis)
 
     if isinstance(arrays, dict):
         backend = backend_of(*arrays.values(), default=cpu)
```

### Comparing `awkward-2.2.3/src/awkward/operations/ak_argcombinations.py` & `awkward-2.2.4/src/awkward/operations/ak_argcombinations.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("argcombinations",)
 import awkward as ak
+from awkward._dispatch import high_level_function
 from awkward._layout import wrap_layout
 from awkward._nplikes.numpylike import NumpyMetadata
 from awkward._regularize import regularize_axis
 
 np = NumpyMetadata.instance()
 
 
+@high_level_function
 def argcombinations(
     array,
     n,
     *,
     replacement=False,
     axis=1,
     fields=None,
@@ -50,39 +52,29 @@
     like #ak.combinations, but returning integer indexes for
     #ak.Array.__getitem__.
 
     The motivation and uses of this function are similar to those of
     #ak.argcartesian. See #ak.combinations and #ak.argcartesian for a more
     complete description.
     """
-    with ak._errors.OperationErrorContext(
-        "ak.argcombinations",
-        {
-            "array": array,
-            "n": n,
-            "replacement": replacement,
-            "axis": axis,
-            "fields": fields,
-            "parameters": parameters,
-            "with_name": with_name,
-            "highlevel": highlevel,
-            "behavior": behavior,
-        },
-    ):
-        return _impl(
-            array,
-            n,
-            replacement,
-            axis,
-            fields,
-            parameters,
-            with_name,
-            highlevel,
-            behavior,
-        )
+    # Dispatch
+    yield (array,)
+
+    # Implementation
+    return _impl(
+        array,
+        n,
+        replacement,
+        axis,
+        fields,
+        parameters,
+        with_name,
+        highlevel,
+        behavior,
+    )
 
 
 def _impl(
     array, n, replacement, axis, fields, parameters, with_name, highlevel, behavior
 ):
     axis = regularize_axis(axis)
     if parameters is None:
```

### Comparing `awkward-2.2.3/src/awkward/operations/ak_argmax.py` & `awkward-2.2.4/src/awkward/operations/ak_argmax.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("argmax",)
 import awkward as ak
 from awkward._behavior import behavior_of
 from awkward._connect.numpy import UNSUPPORTED
+from awkward._dispatch import high_level_function
 from awkward._layout import wrap_layout
 from awkward._nplikes.numpylike import NumpyMetadata
 from awkward._regularize import regularize_axis
 
 np = NumpyMetadata.instance()
 
 
+@high_level_function
 def argmax(
     array,
     axis=None,
     *,
     keepdims=False,
     mask_identity=True,
     highlevel=True,
@@ -54,28 +56,22 @@
     but it generalizes to cases where they do not.
 
     See #ak.sum for a more complete description of nested list and missing
     value (None) handling in reducers.
 
     See also #ak.nanargmax.
     """
-    with ak._errors.OperationErrorContext(
-        "ak.argmax",
-        {
-            "array": array,
-            "axis": axis,
-            "keepdims": keepdims,
-            "mask_identity": mask_identity,
-            "highlevel": highlevel,
-            "behavior": behavior,
-        },
-    ):
-        return _impl(array, axis, keepdims, mask_identity, highlevel, behavior)
+    # Dispatch
+    yield (array,)
 
+    # Implementation
+    return _impl(array, axis, keepdims, mask_identity, highlevel, behavior)
 
+
+@high_level_function
 def nanargmax(
     array,
     axis=None,
     *,
     keepdims=False,
     mask_identity=True,
     highlevel=True,
@@ -107,28 +103,26 @@
 
         ak.argmax(ak.nan_to_none(array))
 
     with all other arguments unchanged.
 
     See also #ak.argmax.
     """
-    with ak._errors.OperationErrorContext(
-        "ak.nanargmax",
-        {
-            "array": array,
-            "axis": axis,
-            "keepdims": keepdims,
-            "mask_identity": mask_identity,
-            "highlevel": highlevel,
-            "behavior": behavior,
-        },
-    ):
-        array = ak.operations.ak_nan_to_none._impl(array, False, None)
+    # Dispatch
+    yield (array,)
 
-        return _impl(array, axis, keepdims, mask_identity, highlevel, behavior)
+    # Implementation
+    return _impl(
+        ak.operations.ak_nan_to_none._impl(array, False, None),
+        axis,
+        keepdims,
+        mask_identity,
+        highlevel,
+        behavior,
+    )
 
 
 def _impl(array, axis, keepdims, mask_identity, highlevel, behavior):
     axis = regularize_axis(axis)
     layout = ak.operations.to_layout(array, allow_record=False, allow_other=False)
     behavior = behavior_of(array, behavior=behavior)
     reducer = ak._reducers.ArgMax()
```

### Comparing `awkward-2.2.3/src/awkward/operations/ak_argmin.py` & `awkward-2.2.4/src/awkward/operations/ak_argmin.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("argmin",)
 import awkward as ak
 from awkward._behavior import behavior_of
 from awkward._connect.numpy import UNSUPPORTED
+from awkward._dispatch import high_level_function
 from awkward._layout import wrap_layout
 from awkward._nplikes.numpylike import NumpyMetadata
 from awkward._regularize import regularize_axis
 
 np = NumpyMetadata.instance()
 
 
+@high_level_function
 def argmin(
     array,
     axis=None,
     *,
     keepdims=False,
     mask_identity=True,
     highlevel=True,
@@ -54,28 +56,22 @@
     but it generalizes to cases where they do not.
 
     See #ak.sum for a more complete description of nested list and missing
     value (None) handling in reducers.
 
     See also #ak.nanargmin.
     """
-    with ak._errors.OperationErrorContext(
-        "ak.argmin",
-        {
-            "array": array,
-            "axis": axis,
-            "keepdims": keepdims,
-            "mask_identity": mask_identity,
-            "highlevel": highlevel,
-            "behavior": behavior,
-        },
-    ):
-        return _impl(array, axis, keepdims, mask_identity, highlevel, behavior)
+    # Dispatch
+    yield (array,)
 
+    # Implementation
+    return _impl(array, axis, keepdims, mask_identity, highlevel, behavior)
 
+
+@high_level_function
 def nanargmin(
     array,
     axis=None,
     *,
     keepdims=False,
     mask_identity=True,
     highlevel=True,
@@ -106,28 +102,26 @@
 
         ak.argmin(ak.nan_to_none(array))
 
     with all other arguments unchanged.
 
     See also #ak.argmin.
     """
-    with ak._errors.OperationErrorContext(
-        "ak.nanargmin",
-        {
-            "array": array,
-            "axis": axis,
-            "keepdims": keepdims,
-            "mask_identity": mask_identity,
-            "highlevel": highlevel,
-            "behavior": behavior,
-        },
-    ):
-        array = ak.operations.ak_nan_to_none._impl(array, False, None)
+    # Dispatch
+    yield (array,)
 
-        return _impl(array, axis, keepdims, mask_identity, highlevel, behavior)
+    # Implementation
+    return _impl(
+        ak.operations.ak_nan_to_none._impl(array, False, None),
+        axis,
+        keepdims,
+        mask_identity,
+        highlevel,
+        behavior,
+    )
 
 
 def _impl(array, axis, keepdims, mask_identity, highlevel, behavior):
     axis = regularize_axis(axis)
     layout = ak.operations.to_layout(array, allow_record=False, allow_other=False)
     behavior = behavior_of(array, behavior=behavior)
     reducer = ak._reducers.ArgMin()
```

### Comparing `awkward-2.2.3/src/awkward/operations/ak_argsort.py` & `awkward-2.2.4/src/awkward/operations/ak_argsort.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("argsort",)
 import awkward as ak
 from awkward._connect.numpy import UNSUPPORTED
+from awkward._dispatch import high_level_function
 from awkward._layout import wrap_layout
 from awkward._nplikes.numpylike import NumpyMetadata
 from awkward._regularize import regularize_axis
 
 np = NumpyMetadata.instance()
 
 
+@high_level_function
 def argsort(
     array, axis=-1, *, ascending=True, stable=True, highlevel=True, behavior=None
 ):
     """
     Args:
         array: Array-like data (anything #ak.to_layout recognizes).
         axis (int): The dimension at which this operation is applied. The
@@ -43,26 +45,19 @@
         >>> data = ak.Array([[7, 5, 7], [], [2], [8, 2]])
         >>> index = ak.argsort(data)
         >>> index
         <Array [[1, 0, 2], [], [0], [1, 0]] type='4 * var * int64'>
         >>> data[index]
         <Array [[5, 7, 7], [], [2], [2, 8]] type='4 * var * int64'>
     """
-    with ak._errors.OperationErrorContext(
-        "ak.argsort",
-        {
-            "array": array,
-            "axis": axis,
-            "ascending": ascending,
-            "stable": stable,
-            "highlevel": highlevel,
-            "behavior": behavior,
-        },
-    ):
-        return _impl(array, axis, ascending, stable, highlevel, behavior)
+    # Dispatch
+    yield (array,)
+
+    # Implementation
+    return _impl(array, axis, ascending, stable, highlevel, behavior)
 
 
 def _impl(array, axis, ascending, stable, highlevel, behavior):
     axis = regularize_axis(axis)
     layout = ak.operations.to_layout(array, allow_record=False, allow_other=False)
     out = ak._do.argsort(layout, axis, ascending, stable)
     return wrap_layout(out, behavior, highlevel, like=array)
```

### Comparing `awkward-2.2.3/src/awkward/operations/ak_broadcast_arrays.py` & `awkward-2.2.4/src/awkward/operations/ak_broadcast_arrays.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("broadcast_arrays",)
 import awkward as ak
 from awkward._backends.dispatch import backend_of
 from awkward._backends.numpy import NumpyBackend
 from awkward._behavior import behavior_of
 from awkward._connect.numpy import UNSUPPORTED
+from awkward._dispatch import high_level_function
 from awkward._layout import wrap_layout
 from awkward._nplikes.numpylike import NumpyMetadata
 
 np = NumpyMetadata.instance()
 cpu = NumpyBackend.instance()
 
 
+@high_level_function
 def broadcast_arrays(
     *arrays,
     depth_limit=None,
     broadcast_parameters_rule="one_to_one",
     left_broadcast=True,
     right_broadcast=True,
     highlevel=True,
@@ -172,35 +174,27 @@
          [],
          [[7, 8]]]
         >>> that.show()
         [[[1.1, 2.2], [3.3], [4.4], [5.5]],
          [],
          [[6.6]]]
     """
-    with ak._errors.OperationErrorContext(
-        "ak.broadcast_arrays",
-        {
-            "arrays": arrays,
-            "depth_limit": depth_limit,
-            "broadcast_parameters_rule": broadcast_parameters_rule,
-            "left_broadcast": left_broadcast,
-            "right_broadcast": right_broadcast,
-            "highlevel": highlevel,
-            "behavior": behavior,
-        },
-    ):
-        return _impl(
-            arrays,
-            depth_limit,
-            broadcast_parameters_rule,
-            left_broadcast,
-            right_broadcast,
-            highlevel,
-            behavior,
-        )
+    # Dispatch
+    yield arrays
+
+    # Implementation
+    return _impl(
+        arrays,
+        depth_limit,
+        broadcast_parameters_rule,
+        left_broadcast,
+        right_broadcast,
+        highlevel,
+        behavior,
+    )
 
 
 def _impl(
     arrays,
     depth_limit,
     broadcast_parameters_rule,
     left_broadcast,
```

### Comparing `awkward-2.2.3/src/awkward/operations/ak_broadcast_fields.py` & `awkward-2.2.4/src/awkward/operations/ak_broadcast_fields.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("broadcast_fields",)
 import awkward as ak
 from awkward._backends.dispatch import backend_of
 from awkward._backends.numpy import NumpyBackend
 from awkward._behavior import behavior_of
+from awkward._dispatch import high_level_function
 from awkward._layout import wrap_layout
 
 cpu = NumpyBackend.instance()
 
 
-def broadcast_fields(
-    *arrays,
-    highlevel=True,
-    behavior=None,
-):
+@high_level_function
+def broadcast_fields(*arrays, highlevel=True, behavior=None):
     """
     Args:
         arrays: Array-like data (anything #ak.to_layout recognizes).
         highlevel (bool): If True, return an #ak.Array; otherwise, return
             a low-level #ak.contents.Content subclass.
         behavior (None or dict): Custom #ak.behavior for the output array, if
             high-level.
@@ -46,23 +44,19 @@
                 y: int64,
                 z: ?unknown,
                 w: ?unknown
             }
         }
 
     """
-    with ak._errors.OperationErrorContext(
-        "ak.broadcast_fields",
-        {
-            "arrays": arrays,
-            "highlevel": highlevel,
-            "behavior": behavior,
-        },
-    ):
-        return _impl(arrays, highlevel, behavior)
+    # Dispatch
+    yield arrays
+
+    # Implementation
+    return _impl(arrays, highlevel, behavior)
 
 
 def _impl(arrays, highlevel, behavior):
     backend = backend_of(*arrays, default=cpu)
     layouts = [ak.to_layout(x).to_backend(backend) for x in arrays]
     behavior = behavior_of(*arrays, behavior=behavior)
```

### Comparing `awkward-2.2.3/src/awkward/operations/ak_cartesian.py` & `awkward-2.2.4/src/awkward/operations/ak_cartesian.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("cartesian",)
+from collections.abc import Mapping
+
 import awkward as ak
 from awkward._backends.dispatch import backend_of
 from awkward._backends.numpy import NumpyBackend
 from awkward._behavior import behavior_of
+from awkward._dispatch import high_level_function
 from awkward._errors import AxisError
 from awkward._layout import maybe_posaxis, wrap_layout
 from awkward._nplikes.numpylike import NumpyMetadata
 from awkward._regularize import regularize_axis
 
 np = NumpyMetadata.instance()
 cpu = NumpyBackend.instance()
 
 
+@high_level_function
 def cartesian(
     arrays,
     axis=1,
     *,
     nested=None,
     parameters=None,
     with_name=None,
@@ -188,27 +192,22 @@
     list of strings in #ak.Array.__getitem__.
 
     To get list index positions in the tuples/records, rather than data from
     the original `arrays`, use #ak.argcartesian instead of #ak.cartesian. The
     #ak.argcartesian form can be particularly useful as nested indexing in
     #ak.Array.__getitem__.
     """
-    with ak._errors.OperationErrorContext(
-        "ak.cartesian",
-        {
-            "arrays": arrays,
-            "axis": axis,
-            "nested": nested,
-            "parameters": parameters,
-            "with_name": with_name,
-            "highlevel": highlevel,
-            "behavior": behavior,
-        },
-    ):
-        return _impl(arrays, axis, nested, parameters, with_name, highlevel, behavior)
+    # Dispatch
+    if isinstance(arrays, Mapping):
+        yield arrays.values()
+    else:
+        yield arrays
+
+    # Implementation
+    return _impl(arrays, axis, nested, parameters, with_name, highlevel, behavior)
 
 
 def _impl(arrays, axis, nested, parameters, with_name, highlevel, behavior):
     axis = regularize_axis(axis)
     if isinstance(arrays, dict):
         backend = backend_of(*arrays.values(), default=cpu)
         behavior = behavior_of(*arrays.values(), behavior=behavior)
```

### Comparing `awkward-2.2.3/src/awkward/operations/ak_categories.py` & `awkward-2.2.4/src/awkward/operations/ak_categories.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("categories",)
 import awkward as ak
 from awkward._behavior import behavior_of
+from awkward._dispatch import high_level_function
 from awkward._layout import wrap_layout
 
 
+@high_level_function
 def categories(array, highlevel=True):
     """
     Args:
         array: Array-like data (anything #ak.to_layout recognizes).
         highlevel (bool): If True, return an #ak.Array; otherwise, return
             a low-level #ak.contents.Content subclass.
 
     If the `array` is categorical (contains #ak.contents.IndexedArray or
     #ak.contents.IndexedOptionArray labeled with parameter
     `"__array__" = "categorical"`), then this function returns its categories.
 
     See also #ak.is_categorical, #ak.to_categorical, #ak.from_categorical.
     """
-    with ak._errors.OperationErrorContext(
-        "ak.categories",
-        {"array": array, "highlevel": highlevel},
-    ):
-        return _impl(array, highlevel)
+    # Dispatch
+    yield (array,)
+
+    # Implementation
+    return _impl(array, highlevel)
 
 
 def _impl(array, highlevel):
     output = [None]
 
     def action(layout, **kwargs):
         if layout.parameter("__array__") == "categorical":
```

### Comparing `awkward-2.2.3/src/awkward/operations/ak_combinations.py` & `awkward-2.2.4/src/awkward/operations/ak_combinations.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("combinations",)
 import awkward as ak
+from awkward._dispatch import high_level_function
 from awkward._layout import wrap_layout
 from awkward._nplikes.numpylike import NumpyMetadata
 from awkward._regularize import regularize_axis
 
 np = NumpyMetadata.instance()
 
 
+@high_level_function
 def combinations(
     array,
     n,
     *,
     replacement=False,
     axis=1,
     fields=None,
@@ -171,39 +173,29 @@
     indexes to `keep` (above) gets increasingly complicated for large `n`.
 
     To get list index positions in the tuples/records, rather than data from
     the original `array`, use #ak.argcombinations instead of #ak.combinations.
     The #ak.argcombinations form can be particularly useful as nested indexing
     in #ak.Array.__getitem__.
     """
-    with ak._errors.OperationErrorContext(
-        "ak.combinations",
-        {
-            "array": array,
-            "n": n,
-            "replacement": replacement,
-            "axis": axis,
-            "fields": fields,
-            "parameters": parameters,
-            "with_name": with_name,
-            "highlevel": highlevel,
-            "behavior": behavior,
-        },
-    ):
-        return _impl(
-            array,
-            n,
-            replacement,
-            axis,
-            fields,
-            parameters,
-            with_name,
-            highlevel,
-            behavior,
-        )
+    # Dispatch
+    yield (array,)
+
+    # Implementation
+    return _impl(
+        array,
+        n,
+        replacement,
+        axis,
+        fields,
+        parameters,
+        with_name,
+        highlevel,
+        behavior,
+    )
 
 
 def _impl(
     array, n, replacement, axis, fields, parameters, with_name, highlevel, behavior
 ):
     axis = regularize_axis(axis)
     if parameters is None:
```

### Comparing `awkward-2.2.3/src/awkward/operations/ak_concatenate.py` & `awkward-2.2.4/src/awkward/operations/ak_concatenate.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("concatenate",)
 import awkward as ak
 from awkward._backends.dispatch import backend_of
 from awkward._backends.numpy import NumpyBackend
 from awkward._behavior import behavior_of
+from awkward._dispatch import high_level_function
 from awkward._layout import maybe_posaxis, wrap_layout
 from awkward._nplikes.numpylike import NumpyMetadata
 from awkward._nplikes.shape import unknown_length
 from awkward._regularize import regularize_axis
 from awkward._typing import Sequence
 from awkward.contents import Content
 from awkward.operations.ak_fill_none import fill_none
 
 np = NumpyMetadata.instance()
 cpu = NumpyBackend.instance()
 
 
-@ak._connect.numpy.implements("concatenate")
+@high_level_function
 def concatenate(arrays, axis=0, *, mergebool=True, highlevel=True, behavior=None):
     """
     Args:
         arrays: Array-like data (anything #ak.to_layout recognizes).
         axis (int): The dimension at which this operation is applied. The
             outermost dimension is `0`, followed by `1`, etc., and negative
             values count backward from the innermost: `-1` is the innermost
@@ -35,25 +36,26 @@
             high-level.
 
     Returns an array with `arrays` concatenated. For `axis=0`, this means that
     one whole array follows another. For `axis=1`, it means that the `arrays`
     must have the same lengths and nested lists are each concatenated,
     element for element, and similarly for deeper levels.
     """
-    with ak._errors.OperationErrorContext(
-        "ak.concatenate",
-        {
-            "arrays": arrays,
-            "axis": axis,
-            "mergebool": mergebool,
-            "highlevel": highlevel,
-            "behavior": behavior,
-        },
+    # Dispatch
+    if (
+        # Is an array with a known backend
+        backend_of(arrays, default=None)
+        is not None
     ):
-        return _impl(arrays, axis, mergebool, highlevel, behavior)
+        yield (arrays,)
+    else:
+        yield arrays
+
+    # Implementation
+    return _impl(arrays, axis, mergebool, highlevel, behavior)
 
 
 def _impl(arrays, axis, mergebool, highlevel, behavior):
     axis = regularize_axis(axis)
     # Simple single-array, axis=0 fast-path
     backend = backend_of(*arrays, default=cpu)
     behavior = behavior_of(*arrays, behavior=behavior)
```

### Comparing `awkward-2.2.3/src/awkward/operations/ak_copy.py` & `awkward-2.2.4/src/awkward/operations/ak_copy.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("copy",)
-
 import copy as _copy
 
 import awkward as ak
 from awkward._connect.numpy import UNSUPPORTED
+from awkward._dispatch import high_level_function
 from awkward._nplikes.numpylike import NumpyMetadata
 
 np = NumpyMetadata.instance()
 
 
+@high_level_function
 def copy(array):
     """
     Args:
         array: Array-like data (anything #ak.to_layout recognizes).
 
     Returns a deep copy of the array (no memory shared with original).
 
@@ -54,19 +55,19 @@
 
     This is key to Awkward Array's efficiency (memory and speed): operations that
     only change part of a structure re-use pieces from the original ("structural
     sharing"). Changing data in-place would result in many surprising long-distance
     changes, so we don't support it. However, an #ak.Array's data might come from
     a mutable third-party library, so this function allows you to make a true copy.
     """
-    with ak._errors.OperationErrorContext(
-        "ak.fill_none",
-        {"array": array},
-    ):
-        return _impl(array)
+    # Dispatch
+    yield (array,)
+
+    # Implementation
+    return _impl(array)
 
 
 def _impl(array):
     return _copy.deepcopy(array)
 
 
 @ak._connect.numpy.implements("copy")
```

### Comparing `awkward-2.2.3/src/awkward/operations/ak_corr.py` & `awkward-2.2.4/src/awkward/operations/ak_corr.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,21 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("corr",)
 import awkward as ak
 from awkward._behavior import behavior_of
+from awkward._dispatch import high_level_function
 from awkward._nplikes import ufuncs
 from awkward._nplikes.numpylike import NumpyMetadata
 from awkward._regularize import regularize_axis
 
 np = NumpyMetadata.instance()
 
 
-def corr(
-    x,
-    y,
-    weight=None,
-    axis=None,
-    *,
-    keepdims=False,
-    mask_identity=False,
-):
+@high_level_function
+def corr(x, y, weight=None, axis=None, *, keepdims=False, mask_identity=False):
     """
     Args:
         x: One coordinate to use in the correlation (anything #ak.to_layout recognizes).
         y: The other coordinate to use in the correlation (anything #ak.to_layout recognizes).
         weight: Data that can be broadcasted to `x` and `y` to give each point
             a weight. Weighting points equally is the same as no weights;
             weighting some points higher increases the significance of those
@@ -53,26 +47,19 @@
             / np.sqrt(ak.sum((x - ak.mean(x))**2))
             / np.sqrt(ak.sum((y - ak.mean(y))**2))
 
     See #ak.sum for a complete description of handling nested lists and
     missing values (None) in reducers, and #ak.mean for an example with another
     non-reducer.
     """
-    with ak._errors.OperationErrorContext(
-        "ak.corr",
-        {
-            "x": x,
-            "y": y,
-            "weight": weight,
-            "axis": axis,
-            "keepdims": keepdims,
-            "mask_identity": mask_identity,
-        },
-    ):
-        return _impl(x, y, weight, axis, keepdims, mask_identity)
+    # Dispatch
+    yield x, y, weight
+
+    # Implementation
+    return _impl(x, y, weight, axis, keepdims, mask_identity)
 
 
 def _impl(x, y, weight, axis, keepdims, mask_identity):
     axis = regularize_axis(axis)
     behavior = behavior_of(x, y, weight)
     x = ak.highlevel.Array(
         ak.operations.to_layout(x, allow_record=False, allow_other=False),
```

### Comparing `awkward-2.2.3/src/awkward/operations/ak_count.py` & `awkward-2.2.4/src/awkward/operations/ak_count.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("count",)
 import awkward as ak
 from awkward._behavior import behavior_of
+from awkward._dispatch import high_level_function
 from awkward._layout import wrap_layout
 from awkward._nplikes.numpylike import NumpyMetadata
 from awkward._regularize import regularize_axis
 
 np = NumpyMetadata.instance()
 
 
+@high_level_function
 def count(
     array,
     axis=None,
     *,
     keepdims=False,
     mask_identity=False,
     highlevel=True,
@@ -89,26 +91,19 @@
 
     If it is desirable to include None values in #ak.count, use #ak.fill_none
     to turn the None values into something that would be counted.
 
     If it is desirable to exclude NaN ("not a number") values from #ak.count,
     use #ak.nan_to_none to turn them into None, which are not counted.
     """
-    with ak._errors.OperationErrorContext(
-        "ak.count",
-        {
-            "array": array,
-            "axis": axis,
-            "keepdims": keepdims,
-            "mask_identity": mask_identity,
-            "highlevel": highlevel,
-            "behavior": behavior,
-        },
-    ):
-        return _impl(array, axis, keepdims, mask_identity, highlevel, behavior)
+    # Dispatch
+    yield (array,)
+
+    # Implementation
+    return _impl(array, axis, keepdims, mask_identity, highlevel, behavior)
 
 
 def _impl(array, axis, keepdims, mask_identity, highlevel, behavior):
     axis = regularize_axis(axis)
     layout = ak.operations.to_layout(array, allow_record=False, allow_other=False)
     behavior = behavior_of(array, behavior=behavior)
     reducer = ak._reducers.Count()
```

### Comparing `awkward-2.2.3/src/awkward/operations/ak_count_nonzero.py` & `awkward-2.2.4/src/awkward/operations/ak_count_nonzero.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("count_nonzero",)
 import awkward as ak
 from awkward._behavior import behavior_of
+from awkward._dispatch import high_level_function
 from awkward._layout import wrap_layout
 from awkward._nplikes.numpylike import NumpyMetadata
 from awkward._regularize import regularize_axis
 
 np = NumpyMetadata.instance()
 
 
+@high_level_function
 def count_nonzero(
     array,
     axis=None,
     *,
     keepdims=False,
     mask_identity=False,
     highlevel=True,
@@ -48,26 +50,19 @@
     See #ak.sum for a more complete description of nested list and missing
     value (None) handling in reducers.
 
     Following the same rules as other reducers, #ak.count_nonzero does not
     count None values. If it is desirable to count them, use #ak.fill_none
     to turn them into something that would be counted.
     """
-    with ak._errors.OperationErrorContext(
-        "ak.count_nonzero",
-        {
-            "array": array,
-            "axis": axis,
-            "keepdims": keepdims,
-            "mask_identity": mask_identity,
-            "highlevel": highlevel,
-            "behavior": behavior,
-        },
-    ):
-        return _impl(array, axis, keepdims, mask_identity, highlevel, behavior)
+    # Dispatch
+    yield (array,)
+
+    # Implementation
+    return _impl(array, axis, keepdims, mask_identity, highlevel, behavior)
 
 
 def _impl(array, axis, keepdims, mask_identity, highlevel, behavior):
     axis = regularize_axis(axis)
     layout = ak.operations.to_layout(array, allow_record=False, allow_other=False)
     behavior = behavior_of(array, behavior=behavior)
     reducer = ak._reducers.CountNonzero()
```

### Comparing `awkward-2.2.3/src/awkward/operations/ak_covar.py` & `awkward-2.2.4/src/awkward/operations/ak_covar.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,20 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("covar",)
 import awkward as ak
 from awkward._behavior import behavior_of
+from awkward._dispatch import high_level_function
 from awkward._nplikes.numpylike import NumpyMetadata
 from awkward._regularize import regularize_axis
 
 np = NumpyMetadata.instance()
 
 
-def covar(
-    x,
-    y,
-    weight=None,
-    axis=None,
-    *,
-    keepdims=False,
-    mask_identity=False,
-):
+@high_level_function
+def covar(x, y, weight=None, axis=None, *, keepdims=False, mask_identity=False):
     """
     Args:
         x: One coordinate to use in the covariance calculation (anything #ak.to_layout recognizes).
         y: The other coordinate to use in the covariance calculation (anything #ak.to_layout recognizes).
         weight: Data that can be broadcasted to `x` and `y` to give each point
             a weight. Weighting points equally is the same as no weights;
             weighting some points higher increases the significance of those
@@ -50,26 +44,19 @@
 
         ak.sum((x - ak.mean(x))*(y - ak.mean(y))*weight) / ak.sum(weight)
 
     See #ak.sum for a complete description of handling nested lists and
     missing values (None) in reducers, and #ak.mean for an example with another
     non-reducer.
     """
-    with ak._errors.OperationErrorContext(
-        "ak.covar",
-        {
-            "x": x,
-            "y": y,
-            "weight": weight,
-            "axis": axis,
-            "keepdims": keepdims,
-            "mask_identity": mask_identity,
-        },
-    ):
-        return _impl(x, y, weight, axis, keepdims, mask_identity)
+    # Dispatch
+    yield x, y, weight
+
+    # Implementation
+    return _impl(x, y, weight, axis, keepdims, mask_identity)
 
 
 def _impl(x, y, weight, axis, keepdims, mask_identity):
     axis = regularize_axis(axis)
     behavior = behavior_of(x, y, weight)
     x = ak.highlevel.Array(
         ak.operations.to_layout(x, allow_record=False, allow_other=False),
```

### Comparing `awkward-2.2.3/src/awkward/operations/ak_drop_none.py` & `awkward-2.2.4/src/awkward/operations/ak_drop_none.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("drop_none",)
 import awkward as ak
+from awkward._dispatch import high_level_function
 from awkward._errors import AxisError
 from awkward._layout import maybe_posaxis, wrap_layout
 from awkward._nplikes.numpylike import NumpyMetadata
 from awkward._regularize import regularize_axis
 
 np = NumpyMetadata.instance()
 
 
+@high_level_function
 def drop_none(array, axis=None, highlevel=True, behavior=None):
     """
     Args:
         array: Data in which to remove Nones.
         axis (None or int): If None, the operation drops Nones at all levels of
             nesting, returning an array of the same dimension, but without Nones.
             Otherwise, it drops Nones at a specified depth.
@@ -37,19 +39,19 @@
 
     The default axis is None, however an axis can be specified:
 
         >>> ak.drop_none(array, axis=1)
         <Array [[[0]], [[None]], [[1]], [[2, None]]] type='4 * var * var * ?int64'>
 
     """
-    with ak._errors.OperationErrorContext(
-        "ak.drop_none",
-        {"array": array, "axis": axis, "highlevel": highlevel, "behavior": behavior},
-    ):
-        return _impl(array, axis, highlevel, behavior)
+    # Dispatch
+    yield (array,)
+
+    # Implementation
+    return _impl(array, axis, highlevel, behavior)
 
 
 def _impl(array, axis, highlevel, behavior):
     axis = regularize_axis(axis)
     layout = ak.operations.to_layout(array, allow_record=False, allow_other=False)
 
     def drop_nones(layout, **kwargs):
```

### Comparing `awkward-2.2.3/src/awkward/operations/ak_enforce_type.py` & `awkward-2.2.4/src/awkward/operations/ak_enforce_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,34 +1,28 @@
 from __future__ import annotations
 
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 # ruff: noqa: B023
 __all__ = ("enforce_type",)
-
-
 from itertools import permutations
 
 import awkward as ak
+from awkward._dispatch import high_level_function
 from awkward._layout import wrap_layout
 from awkward._nplikes.numpylike import NumpyMetadata
 from awkward._nplikes.shape import unknown_length
 from awkward._parameters import type_parameters_equal
 from awkward._typing import NamedTuple
 from awkward.types.numpytype import primitive_to_dtype
 
 np = NumpyMetadata.instance()
 
 
-def enforce_type(
-    array,
-    type,
-    *,
-    highlevel=True,
-    behavior=None,
-):
+@high_level_function
+def enforce_type(array, type, *, highlevel=True, behavior=None):
     """
     Args:
         array: Array-like data (anything #ak.to_layout recognizes).
         type (#ak.types.Type, or str): The type that `array` will be enforced to.
         highlevel (bool): If True, return an #ak.Array; otherwise, return
             a low-level #ak.contents.Content subclass.
         behavior (None or dict): Custom #ak.behavior for the output array, if
@@ -223,24 +217,19 @@
       >>> b.type.show()
       3 * ?unknown
 
     The conversion rules outlined above are not data-dependent; the appropriate rule is chosen from the layout and the
     given type value. If the conversion is not possible given the layout data, e.g. a conversion from an irregular list
     to a regular type, it will fail.
     """
-    with ak._errors.OperationErrorContext(
-        "ak.enforce_type",
-        {
-            "array": array,
-            "type": type,
-            "highlevel": highlevel,
-            "behavior": behavior,
-        },
-    ):
-        return _impl(array, type, highlevel, behavior)
+    # Dispatch
+    yield (array,)
+
+    # Implementation
+    return _impl(array, type, highlevel, behavior)
 
 
 def _impl(array, type_, highlevel, behavior):
     layout = ak.to_layout(array, allow_record=True)
 
     if isinstance(type_, str):
         type_ = ak.types.from_datashape(type_, highlevel=False)
```

### Comparing `awkward-2.2.3/src/awkward/operations/ak_fields.py` & `awkward-2.2.4/src/awkward/operations/ak_fields.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("fields",)
-
 import awkward as ak
+from awkward._dispatch import high_level_function
 from awkward._nplikes.numpylike import NumpyMetadata
 
 np = NumpyMetadata.instance()
 
 
+@high_level_function
 def fields(array):
     """
     Args:
         array: Array-like data (anything #ak.to_layout recognizes).
 
     Extracts record fields or tuple slot numbers from `array` (many types
     supported, including all Awkward Arrays and Records).
@@ -19,17 +20,17 @@
     queried. If it contains tuples instead of records, this function outputs
     string representations of integers, such as `"0"`, `"1"`, `"2"`, etc.
     The records or tuples may be within multiple layers of nested lists.
 
     If the array contains neither tuples nor records, this returns an empty
     list.
     """
-    with ak._errors.OperationErrorContext(
-        "ak.fields",
-        {"array": array},
-    ):
-        return _impl(array)
+    # Dispatch
+    yield (array,)
+
+    # Implementation
+    return _impl(array)
 
 
 def _impl(array):
     layout = ak.operations.to_layout(array, allow_record=True, allow_other=False)
     return layout.fields.copy()
```

### Comparing `awkward-2.2.3/src/awkward/operations/ak_fill_none.py` & `awkward-2.2.4/src/awkward/operations/ak_fill_none.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,23 +2,25 @@
 __all__ = ("fill_none",)
 import numbers
 
 import awkward as ak
 from awkward._backends.dispatch import backend_of
 from awkward._backends.numpy import NumpyBackend
 from awkward._behavior import behavior_of
+from awkward._dispatch import high_level_function
 from awkward._errors import AxisError
 from awkward._layout import maybe_posaxis, wrap_layout
 from awkward._nplikes.numpylike import NumpyMetadata
 from awkward._regularize import is_sized_iterable, regularize_axis
 
 np = NumpyMetadata.instance()
 cpu = NumpyBackend.instance()
 
 
+@high_level_function
 def fill_none(array, value, axis=-1, *, highlevel=True, behavior=None):
     """
     Args:
         array: Array-like data (anything #ak.to_layout recognizes).
         value: Data with which to replace None.
         axis (None or int): If None, replace all None values in the array
             with the given value; if an int, The dimension at which this
@@ -55,25 +57,19 @@
         3 * var * union[
             float64,
             string
         ]
 
     The values could be floating-point numbers or strings.
     """
-    with ak._errors.OperationErrorContext(
-        "ak.fill_none",
-        {
-            "array": array,
-            "value": value,
-            "axis": axis,
-            "highlevel": highlevel,
-            "behavior": behavior,
-        },
-    ):
-        return _impl(array, value, axis, highlevel, behavior)
+    # Dispatch
+    yield array, value
+
+    # Implementation
+    return _impl(array, value, axis, highlevel, behavior)
 
 
 def _impl(array, value, axis, highlevel, behavior):
     axis = regularize_axis(axis)
     arraylayout = ak.operations.to_layout(array, allow_record=True, allow_other=False)
     behavior = behavior_of(array, value, behavior=behavior)
     backend = backend_of(arraylayout, default=cpu)
```

### Comparing `awkward-2.2.3/src/awkward/operations/ak_firsts.py` & `awkward-2.2.4/src/awkward/operations/ak_firsts.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("firsts",)
 import awkward as ak
 from awkward._behavior import behavior_of
+from awkward._dispatch import high_level_function
 from awkward._errors import AxisError
 from awkward._layout import maybe_posaxis, wrap_layout
 from awkward._nplikes.numpylike import NumpyMetadata
 from awkward._regularize import is_integer, regularize_axis
 
 np = NumpyMetadata.instance()
 
 
+@high_level_function
 def firsts(array, axis=1, *, highlevel=True, behavior=None):
     """
     Args:
         array: Array-like data (anything #ak.to_layout recognizes).
         axis (int): The dimension at which this operation is applied. The
             outermost dimension is `0`, followed by `1`, etc., and negative
             values count backward from the innermost: `-1` is the innermost
@@ -37,19 +39,19 @@
          None,
          None,
          4.4,
          5.5]
 
     See #ak.singletons to invert this function.
     """
-    with ak._errors.OperationErrorContext(
-        "ak.firsts",
-        {"array": array, "axis": axis, "highlevel": highlevel, "behavior": behavior},
-    ):
-        return _impl(array, axis, highlevel, behavior)
+    # Dispatch
+    yield (array,)
+
+    # Implementation
+    return _impl(array, axis, highlevel, behavior)
 
 
 def _impl(array, axis, highlevel, behavior):
     axis = regularize_axis(axis)
     layout = ak.operations.to_layout(array)
     behavior = behavior_of(array, behavior=behavior)
```

### Comparing `awkward-2.2.3/src/awkward/operations/ak_flatten.py` & `awkward-2.2.4/src/awkward/operations/ak_flatten.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("flatten",)
 import awkward as ak
+from awkward._dispatch import high_level_function
 from awkward._layout import maybe_posaxis, wrap_layout
 from awkward._nplikes.numpylike import NumpyMetadata
 from awkward._regularize import regularize_axis
 
 np = NumpyMetadata.instance()
 
 
+@high_level_function
 def flatten(array, axis=1, *, highlevel=True, behavior=None):
     """
     Args:
         array: Array-like data (anything #ak.to_layout recognizes).
         axis (None or int): If None, the operation flattens all levels of
             nesting, returning a 1-dimensional array. Otherwise, it flattens
             at a specified depth. The outermost dimension is `0`, followed
@@ -153,19 +155,19 @@
          999,
          5.5,
          0,
          1.1,
          2.2,
          999]
     """
-    with ak._errors.OperationErrorContext(
-        "ak.flatten",
-        {"array": array, "axis": axis, "highlevel": highlevel, "behavior": behavior},
-    ):
-        return _impl(array, axis, highlevel, behavior)
+    # Dispatch
+    yield (array,)
+
+    # Implementation
+    return _impl(array, axis, highlevel, behavior)
 
 
 def _impl(array, axis, highlevel, behavior):
     axis = regularize_axis(axis)
     layout = ak.operations.to_layout(array, allow_record=False, allow_other=False)
 
     if axis is None:
```

### Comparing `awkward-2.2.3/src/awkward/operations/ak_from_arrow.py` & `awkward-2.2.4/src/awkward/operations/ak_from_arrow.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("from_arrow",)
 import awkward as ak
+from awkward._dispatch import high_level_function
 from awkward._layout import wrap_layout
 from awkward._nplikes.numpylike import NumpyMetadata
 
 np = NumpyMetadata.instance()
 
 
+@high_level_function
 def from_arrow(array, *, generate_bitmasks=False, highlevel=True, behavior=None):
     """
     Args:
         array (`pyarrow.Array`, `pyarrow.ChunkedArray`, `pyarrow.RecordBatch`, or `pyarrow.Table`):
             Apache Arrow array to convert into an  Awkward Array.
         generate_bitmasks (bool): If enabled and Arrow/Parquet does not have Awkward
             metadata, `generate_bitmasks=True` creates empty bitmasks for nullable
@@ -28,24 +30,15 @@
     `to_pylist` method. If #ak.to_arrow was invoked with `extensionarray=True`, this
     function also preserves the data type (high-level #ak.types.Type, though not the
     low-level #ak.forms.Form), even through Parquet, making Parquet a good way to save
     Awkward Arrays for later use.
 
     See also #ak.to_arrow, #ak.to_arrow_table, #ak.from_parquet, #ak.from_arrow_schema.
     """
-    with ak._errors.OperationErrorContext(
-        "ak.from_arrow",
-        {
-            "array": array,
-            "generate_bitmasks": generate_bitmasks,
-            "highlevel": highlevel,
-            "behavior": behavior,
-        },
-    ):
-        return _impl(array, generate_bitmasks, highlevel, behavior)
+    return _impl(array, generate_bitmasks, highlevel, behavior)
 
 
 def _impl(array, generate_bitmasks, highlevel, behavior):
     import awkward._connect.pyarrow
 
     pyarrow = awkward._connect.pyarrow.pyarrow
```

### Comparing `awkward-2.2.3/src/awkward/operations/ak_from_arrow_schema.py` & `awkward-2.2.4/src/awkward/operations/ak_from_arrow_schema.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,25 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("from_arrow_schema",)
-
-import awkward as ak
+from awkward._dispatch import high_level_function
 from awkward._nplikes.numpylike import NumpyMetadata
 
 np = NumpyMetadata.instance()
 
 
+@high_level_function
 def from_arrow_schema(schema):
     """
     Args:
         schema (`pyarrow.Schema`): Apache Arrow schema to convert into an Awkward Form.
 
     Converts an Apache Arrow schema into an Awkward Form.
 
     See also #ak.to_arrow, #ak.to_arrow_table, #ak.from_arrow, #ak.to_parquet, #ak.from_parquet.
     """
-    with ak._errors.OperationErrorContext(
-        "ak.from_arrow_schema",
-        {"schema": schema},
-    ):
-        return _impl(schema)
+    return _impl(schema)
 
 
 def _impl(schema):
     import awkward._connect.pyarrow
 
     return awkward._connect.pyarrow.form_handle_arrow(schema, pass_empty_field=True)
```

### Comparing `awkward-2.2.3/src/awkward/operations/ak_from_avro_file.py` & `awkward-2.2.4/src/awkward/operations/ak_from_avro_file.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("from_avro_file",)
 
 from os import PathLike, fsdecode
 
 import awkward as ak
+from awkward._dispatch import high_level_function
 from awkward._nplikes.numpylike import NumpyMetadata
 
 np = NumpyMetadata.instance()
 
 
+@high_level_function
 def from_avro_file(
     file, limit_entries=None, *, debug_forth=False, highlevel=True, behavior=None
 ):
     """
     Args:
         file (path-like or file-like object): Avro file to be read as Awkward Array.
         limit_entries (int): The number of rows of the Avro file to be read into the Awkward Array.
@@ -25,44 +27,32 @@
     Reads Avro files as Awkward Arrays.
 
     Internally this function uses AwkwardForth DSL. The function recursively parses the Avro schema, generates
     Awkward form and Forth code for that specific Avro file and then reads it.
     """
     import awkward._connect.avro
 
-    with ak._errors.OperationErrorContext(
-        "ak.from_avro_file",
-        {
-            "file": file,
-            "highlevel": highlevel,
-            "behavior": behavior,
-            "limit_entries": limit_entries,
-            "debug_forth": debug_forth,
-        },
-    ):
-        if isinstance(file, (str, bytes, PathLike)):
-            file = fsdecode(file)
-
-        if isinstance(file, str):
-            with open(file, "rb") as opened_file:
-                form, length, container = awkward._connect.avro.ReadAvroFT(
-                    opened_file, limit_entries, debug_forth
-                ).outcontents
-                return _impl(form, length, container, highlevel, behavior)
-
+    if isinstance(file, (str, bytes, PathLike)):
+        file = fsdecode(file)
+        with open(file, "rb") as opened_file:
+            form, length, container = awkward._connect.avro.ReadAvroFT(
+                opened_file, limit_entries, debug_forth
+            ).outcontents
+            return _impl(form, length, container, highlevel, behavior)
+
+    else:
+        if not hasattr(file, "read") or not hasattr(file, "seek"):
+            raise TypeError(
+                "'file' must either be a filename string or be a file-like object with 'read' and 'seek' methods"
+            )
         else:
-            if not hasattr(file, "read") or not hasattr(file, "seek"):
-                raise TypeError(
-                    "'file' must either be a filename string or be a file-like object with 'read' and 'seek' methods"
-                )
-            else:
-                form, length, container = awkward._connect.avro.ReadAvroFT(
-                    file, limit_entries, debug_forth
-                ).outarr
-                return _impl(form, length, container, highlevel, behavior)
+            form, length, container = awkward._connect.avro.ReadAvroFT(
+                file, limit_entries, debug_forth
+            ).outarr
+            return _impl(form, length, container, highlevel, behavior)
 
 
 def _impl(form, length, container, highlevel, behavior):
     return ak.operations.ak_from_buffers._impl(
         form=form,
         length=length,
         container=container,
```

### Comparing `awkward-2.2.3/src/awkward/operations/ak_from_buffers.py` & `awkward-2.2.4/src/awkward/operations/ak_from_buffers.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,40 +1,41 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 from __future__ import annotations
 
 __all__ = ("from_buffers",)
-
 import math
 
 import awkward as ak
 from awkward._backends.dispatch import regularize_backend
+from awkward._dispatch import high_level_function
 from awkward._layout import wrap_layout
 from awkward._nplikes.numpy import Numpy
 from awkward._nplikes.numpylike import NumpyMetadata
 from awkward._regularize import is_integer
 
 np = NumpyMetadata.instance()
 numpy = Numpy.instance()
 
 
+@high_level_function
 def from_buffers(
     form,
     length,
     container,
     buffer_key="{form_key}-{attribute}",
     *,
     backend="cpu",
     byteorder="<",
     highlevel=True,
     behavior=None,
 ):
     """
     Args:
         form (#ak.forms.Form or str/dict equivalent): The form of the Awkward
-            Array to reconstitute from named buffers.
+            Array to _reconstitute from named buffers.
         length (int): Length of the array. (The output of this function is always
             single-partition.)
         container (Mapping, such as dict): The str \u2192 Python buffers that
             represent the decomposed Awkward Array. This `container` is only
             assumed to have a `__getitem__` method that accepts strings as keys.
         buffer_key (str or callable): Python format string containing
             `"{form_key}"` and/or `"{attribute}"` or a function that takes these
@@ -69,38 +70,25 @@
     If the values of `container` are recognised as arrays by the given backend,
     a view over their existing data will be used, where possible.
 
     The `buffer_key` should be the same as the one used in #ak.to_buffers.
 
     See #ak.to_buffers for examples.
     """
-    with ak._errors.OperationErrorContext(
-        "ak.from_buffers",
-        {
-            "form": form,
-            "length": length,
-            "container": container,
-            "buffer_key": buffer_key,
-            "backend": backend,
-            "byteorder": byteorder,
-            "highlevel": highlevel,
-            "behavior": behavior,
-        },
-    ):
-        return _impl(
-            form,
-            length,
-            container,
-            buffer_key,
-            backend,
-            byteorder,
-            highlevel,
-            behavior,
-            False,
-        )
+    return _impl(
+        form,
+        length,
+        container,
+        buffer_key,
+        backend,
+        byteorder,
+        highlevel,
+        behavior,
+        False,
+    )
 
 
 def _impl(
     form,
     length,
     container,
     buffer_key,
@@ -139,15 +127,15 @@
             return buffer_key(form_key=form.form_key, attribute=attribute, form=form)
 
     else:
         raise TypeError(
             f"buffer_key must be a string or a callable, not {type(buffer_key)}"
         )
 
-    out = reconstitute(form, length, container, getkey, backend, byteorder, simplify)
+    out = _reconstitute(form, length, container, getkey, backend, byteorder, simplify)
     return wrap_layout(out, behavior, highlevel)
 
 
 _index_to_dtype = {
     "i8": np.dtype("<i1"),
     "u8": np.dtype("<u1"),
     "i32": np.dtype("<i4"),
@@ -171,15 +159,15 @@
         array = nplike.frombuffer(buffer, dtype=dtype, count=count)
         if byteorder != ak._util.native_byteorder:
             return array.byteswap(inplace=False)
         else:
             return array
 
 
-def reconstitute(form, length, container, getkey, backend, byteorder, simplify):
+def _reconstitute(form, length, container, getkey, backend, byteorder, simplify):
     if isinstance(form, ak.forms.EmptyForm):
         if length != 0:
             raise ValueError(f"EmptyForm node, but the expected length is {length}")
         return ak.contents.EmptyArray()
 
     elif isinstance(form, ak.forms.NumpyForm):
         dtype = ak.types.numpytype.primitive_to_dtype(form.primitive)
@@ -200,15 +188,15 @@
             else:
                 data = backend.nplike.reshape(data, (-1, *form.inner_shape))
         return ak.contents.NumpyArray(
             data, parameters=form._parameters, backend=backend
         )
 
     elif isinstance(form, ak.forms.UnmaskedForm):
-        content = reconstitute(
+        content = _reconstitute(
             form.content, length, container, getkey, backend, byteorder, simplify
         )
         if simplify:
             make = ak.contents.UnmaskedArray.simplified
         else:
             make = ak.contents.UnmaskedArray
         return make(content, parameters=form._parameters)
@@ -219,15 +207,15 @@
         mask = _from_buffer(
             backend.index_nplike,
             raw_array,
             dtype=_index_to_dtype[form.mask],
             count=excess_length,
             byteorder=byteorder,
         )
-        content = reconstitute(
+        content = _reconstitute(
             form.content, length, container, getkey, backend, byteorder, simplify
         )
         if simplify:
             make = ak.contents.BitMaskedArray.simplified
         else:
             make = ak.contents.BitMaskedArray
         return make(
@@ -244,15 +232,15 @@
         mask = _from_buffer(
             backend.index_nplike,
             raw_array,
             dtype=_index_to_dtype[form.mask],
             count=length,
             byteorder=byteorder,
         )
-        content = reconstitute(
+        content = _reconstitute(
             form.content, length, container, getkey, backend, byteorder, simplify
         )
         if simplify:
             make = ak.contents.ByteMaskedArray.simplified
         else:
             make = ak.contents.ByteMaskedArray
         return make(
@@ -270,15 +258,15 @@
             dtype=_index_to_dtype[form.index],
             count=length,
             byteorder=byteorder,
         )
         next_length = (
             0 if len(index) == 0 else max(0, backend.index_nplike.max(index) + 1)
         )
-        content = reconstitute(
+        content = _reconstitute(
             form.content, next_length, container, getkey, backend, byteorder, simplify
         )
         if simplify:
             make = ak.contents.IndexedOptionArray.simplified
         else:
             make = ak.contents.IndexedOptionArray
         return make(
@@ -299,15 +287,15 @@
         next_length = (
             0
             if len(index) == 0
             else backend.index_nplike.index_as_shape_item(
                 backend.index_nplike.max(index) + 1
             )
         )
-        content = reconstitute(
+        content = _reconstitute(
             form.content, next_length, container, getkey, backend, byteorder, simplify
         )
         if simplify:
             make = ak.contents.IndexedArray.simplified
         else:
             make = ak.contents.IndexedArray
         return make(
@@ -331,15 +319,15 @@
             raw_array2,
             dtype=_index_to_dtype[form.stops],
             count=length,
             byteorder=byteorder,
         )
         reduced_stops = stops[starts != stops]
         next_length = 0 if len(starts) == 0 else backend.index_nplike.max(reduced_stops)
-        content = reconstitute(
+        content = _reconstitute(
             form.content, next_length, container, getkey, backend, byteorder, simplify
         )
         return ak.contents.ListArray(
             ak.index.Index(starts),
             ak.index.Index(stops),
             content,
             parameters=form._parameters,
@@ -351,38 +339,38 @@
             backend.index_nplike,
             raw_array,
             dtype=_index_to_dtype[form.offsets],
             count=length + 1,
             byteorder=byteorder,
         )
         next_length = 0 if len(offsets) == 1 else offsets[-1]
-        content = reconstitute(
+        content = _reconstitute(
             form.content, next_length, container, getkey, backend, byteorder, simplify
         )
         return ak.contents.ListOffsetArray(
             ak.index.Index(offsets),
             content,
             parameters=form._parameters,
         )
 
     elif isinstance(form, ak.forms.RegularForm):
         next_length = length * form.size
-        content = reconstitute(
+        content = _reconstitute(
             form.content, next_length, container, getkey, backend, byteorder, simplify
         )
         return ak.contents.RegularArray(
             content,
             form.size,
             length,
             parameters=form._parameters,
         )
 
     elif isinstance(form, ak.forms.RecordForm):
         contents = [
-            reconstitute(
+            _reconstitute(
                 content, length, container, getkey, backend, byteorder, simplify
             )
             for content in form.contents
         ]
         return ak.contents.RecordArray(
             contents,
             None if form.is_tuple else form.fields,
@@ -411,15 +399,15 @@
         for tag in range(len(form.contents)):
             selected_index = index[tags == tag]
             if len(selected_index) == 0:
                 lengths.append(0)
             else:
                 lengths.append(backend.index_nplike.max(selected_index) + 1)
         contents = [
-            reconstitute(
+            _reconstitute(
                 content, lengths[i], container, getkey, backend, byteorder, simplify
             )
             for i, content in enumerate(form.contents)
         ]
         if simplify:
             make = ak.contents.UnionArray.simplified
         else:
```

### Comparing `awkward-2.2.3/src/awkward/operations/ak_from_categorical.py` & `awkward-2.2.4/src/awkward/operations/ak_from_categorical.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("from_categorical",)
 import awkward as ak
 from awkward._behavior import behavior_of
+from awkward._dispatch import high_level_function
 from awkward._layout import wrap_layout
 
 
+@high_level_function
 def from_categorical(array, *, highlevel=True, behavior=None):
     """
     Args:
         array: Array-like data (anything #ak.to_layout recognizes).
         highlevel (bool): If True, return an #ak.Array; otherwise, return
             a low-level #ak.contents.Content subclass.
         behavior (None or dict): Custom #ak.behavior for the output array, if
@@ -20,19 +22,19 @@
     This is a metadata-only operation; the running time does not scale with the
     size of the dataset. (Conversion to categorical is expensive; conversion
     from categorical is cheap.)
 
     See also #ak.is_categorical, #ak.categories, #ak.to_categorical,
     #ak.from_categorical.
     """
-    with ak._errors.OperationErrorContext(
-        "ak.from_categorical",
-        {"array": array, "highlevel": highlevel, "behavior": behavior},
-    ):
-        return _impl(array, highlevel, behavior)
+    # Dispatch
+    yield (array,)
+
+    # Implementation
+    return _impl(array, highlevel, behavior)
 
 
 def _impl(array, highlevel, behavior):
     def action(layout, **kwargs):
         if layout.parameter("__array__") == "categorical":
             out = ak.operations.with_parameter(
                 layout, "__array__", None, highlevel=False
```

### Comparing `awkward-2.2.3/src/awkward/operations/ak_from_cupy.py` & `awkward-2.2.4/src/awkward/operations/ak_from_jax.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,44 +1,38 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
-__all__ = ("from_cupy",)
-import awkward as ak
+__all__ = ("from_jax",)
+from awkward import jax
+from awkward._dispatch import high_level_function
 from awkward._layout import from_arraylib, wrap_layout
 
 
-def from_cupy(array, *, regulararray=False, highlevel=True, behavior=None):
+@high_level_function
+def from_jax(array, *, regulararray=False, highlevel=True, behavior=None):
     """
     Args:
-        array (cp.ndarray): The CuPy array to convert into an Awkward Array.
+        array (jax.numpy.DeviceArray): The JAX DeviceArray to convert into an Awkward Array.
         regulararray (bool): If True and the array is multidimensional,
             the dimensions are represented by nested #ak.contents.RegularArray
             nodes; if False and the array is multidimensional, the dimensions
             are represented by a multivalued #ak.contents.NumpyArray.shape.
             If the array is one-dimensional, this has no effect.
         highlevel (bool): If True, return an #ak.Array; otherwise, return
             a low-level #ak.contents.Content subclass.
         behavior (None or dict): Custom #ak.behavior for the output array, if
             high-level.
 
-    Converts a CuPy array into an Awkward Array.
+    Converts a JAX DeviceArray array into an Awkward Array.
 
     The resulting layout may involve the following #ak.contents.Content types
     (only):
 
     * #ak.contents.NumpyArray
     * #ak.contents.RegularArray if `regulararray=True`.
 
-    See also #ak.to_cupy, #ak.from_numpy and #ak.from_jax.
+    See also #ak.to_jax, #ak.from_numpy and #ak.from_jax.
     """
-    with ak._errors.OperationErrorContext(
-        "ak.from_cupy",
-        {
-            "array": array,
-            "regulararray": regulararray,
-            "highlevel": highlevel,
-            "behavior": behavior,
-        },
-    ):
-        return wrap_layout(
-            from_arraylib(array, regulararray, False),
-            highlevel=highlevel,
-            behavior=behavior,
-        )
+    jax.assert_registered()
+    return wrap_layout(
+        from_arraylib(array, regulararray, False),
+        highlevel=highlevel,
+        behavior=behavior,
+    )
```

### Comparing `awkward-2.2.3/src/awkward/operations/ak_from_iter.py` & `awkward-2.2.4/src/awkward/operations/ak_from_iter.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("from_iter",)
-
 from collections.abc import Iterable
 
 from awkward_cpp.lib import _ext
 
 import awkward as ak
+from awkward._dispatch import high_level_function
 from awkward._nplikes.numpylike import NumpyMetadata
 
 np = NumpyMetadata.instance()
 
 
+@high_level_function
 def from_iter(
     iterable,
     *,
     allow_record=True,
     highlevel=True,
     behavior=None,
     initial=1024,
@@ -55,26 +56,15 @@
     * dict: converted into #ak.contents.RecordArray with field names
       (i.e. homogeneously typed records with the same sets of fields).
     * iterable, including np.ndarray: converted into
       #ak.contents.ListOffsetArray.
 
     See also #ak.to_list.
     """
-    with ak._errors.OperationErrorContext(
-        "ak.from_iter",
-        {
-            "iterable": iterable,
-            "allow_record": allow_record,
-            "highlevel": highlevel,
-            "behavior": behavior,
-            "initial": initial,
-            "resize": resize,
-        },
-    ):
-        return _impl(iterable, highlevel, behavior, allow_record, initial, resize)
+    return _impl(iterable, highlevel, behavior, allow_record, initial, resize)
 
 
 def _impl(iterable, highlevel, behavior, allow_record, initial, resize):
     if not isinstance(iterable, Iterable):
         raise TypeError(
             f"cannot produce an array from a non-iterable object ({type(iterable)!r})"
         )
```

### Comparing `awkward-2.2.3/src/awkward/operations/ak_from_json.py` & `awkward-2.2.4/src/awkward/operations/ak_from_json.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,23 +4,25 @@
 import pathlib
 from collections.abc import Iterable, Sized
 from urllib.parse import urlparse
 
 from awkward_cpp.lib import _ext
 
 import awkward as ak
+from awkward._dispatch import high_level_function
 from awkward._layout import wrap_layout
 from awkward._nplikes.numpy import Numpy
 from awkward._nplikes.numpylike import NumpyMetadata
 from awkward._regularize import is_integer
 
 np = NumpyMetadata.instance()
 numpy = Numpy.instance()
 
 
+@high_level_function
 def from_json(
     source,
     *,
     line_delimited=False,
     schema=None,
     nan_string=None,
     posinf_string=None,
@@ -315,61 +317,44 @@
         ...         },
         ...     },
         ... )
         <Array [1+1.1j, 2+2.2j] type='2 * complex128'>
 
     See also #ak.to_json.
     """
-    with ak._errors.OperationErrorContext(
-        "ak.from_json",
-        {
-            "source": source,
-            "line_delimited": line_delimited,
-            "schema": schema,
-            "nan_string": nan_string,
-            "posinf_string": posinf_string,
-            "neginf_string": neginf_string,
-            "complex_record_fields": complex_record_fields,
-            "buffersize": buffersize,
-            "initial": initial,
-            "resize": resize,
-            "highlevel": highlevel,
-            "behavior": behavior,
-        },
-    ):
-        if schema is None:
-            return _no_schema(
-                source,
-                line_delimited,
-                nan_string,
-                posinf_string,
-                neginf_string,
-                complex_record_fields,
-                buffersize,
-                initial,
-                resize,
-                highlevel,
-                behavior,
-            )
+    if schema is None:
+        return _no_schema(
+            source,
+            line_delimited,
+            nan_string,
+            posinf_string,
+            neginf_string,
+            complex_record_fields,
+            buffersize,
+            initial,
+            resize,
+            highlevel,
+            behavior,
+        )
 
-        else:
-            return _yes_schema(
-                source,
-                line_delimited,
-                schema,
-                nan_string,
-                posinf_string,
-                neginf_string,
-                complex_record_fields,
-                buffersize,
-                initial,
-                resize,
-                highlevel,
-                behavior,
-            )
+    else:
+        return _yes_schema(
+            source,
+            line_delimited,
+            schema,
+            nan_string,
+            posinf_string,
+            neginf_string,
+            complex_record_fields,
+            buffersize,
+            initial,
+            resize,
+            highlevel,
+            behavior,
+        )
 
 
 class _BytesReader:
     __slots__ = ("data", "current")
 
     def __init__(self, data):
         self.data = data
@@ -531,19 +516,19 @@
     instructions = []
 
     if schema.get("type") == "array":
         if "items" not in schema:
             raise TypeError("JSONSchema type is not concrete: array without items")
 
         instructions.append(["TopLevelArray"])
-        form = build_assembly(schema["items"], container, instructions)
+        form = _build_assembly(schema["items"], container, instructions)
         is_record = False
 
     elif schema.get("type") == "object":
-        form = build_assembly(schema, container, instructions)
+        form = _build_assembly(schema, container, instructions)
         is_record = True
 
     else:
         raise TypeError(
             "only 'array' and 'object' types supported at the JSONSchema root"
         )
 
@@ -576,15 +561,15 @@
 
     if highlevel and isinstance(layout, (ak.contents.Content, ak.record.Record)):
         return wrap_layout(layout, behavior, highlevel)
     else:
         return layout
 
 
-def build_assembly(schema, container, instructions):
+def _build_assembly(schema, container, instructions):
     if not isinstance(schema, dict):
         raise TypeError(f"unrecognized JSONSchema: expected dict, got {schema!r}")
 
     if "type" not in schema is None:
         raise TypeError(f"unrecognized JSONSchema: no 'type' in {schema!r}")
 
     tpe = schema["type"]
@@ -722,15 +707,15 @@
                 container[mask + "-index"] = None
                 instructions.append(
                     ["FillIndexedOptionArray", mask + "-index", "int64"]
                 )
 
             instructions.append(["FixedLengthList", schema.get("minItems")])
 
-            content = build_assembly(schema["items"], container, instructions)
+            content = _build_assembly(schema["items"], container, instructions)
 
             out = ak.forms.RegularForm(content, size=schema.get("minItems"))
             if is_optional:
                 return ak.forms.IndexedOptionForm("i64", out, form_key=mask)
             else:
                 return out
 
@@ -740,15 +725,15 @@
                 container[mask + "-mask"] = None
                 instructions.append(["FillByteMaskedArray", mask + "-mask", "int8"])
 
             offsets = f"node{len(container)}"
             container[offsets + "-offsets"] = None
             instructions.append(["VarLengthList", offsets + "-offsets", "int64"])
 
-            content = build_assembly(schema["items"], container, instructions)
+            content = _build_assembly(schema["items"], container, instructions)
 
             out = ak.forms.ListOffsetForm("i64", content, form_key=offsets)
             if is_optional:
                 return ak.forms.ByteMaskedForm(
                     "i8", out, valid_when=True, form_key=mask
                 )
             else:
@@ -779,15 +764,15 @@
         for name in names:
             instructions.append(["KeyTableItem", name, None])
 
         contents = []
         for keyindex, subschema in enumerate(subschemas):
             # set the "jump_to" instruction position in the KeyTable
             instructions[startkeys + keyindex][2] = len(instructions)
-            contents.append(build_assembly(subschema, container, instructions))
+            contents.append(_build_assembly(subschema, container, instructions))
 
         out = ak.forms.RecordForm(contents, names)
         if is_optional:
             return ak.forms.IndexedOptionForm("i64", out, form_key=mask)
         else:
             return out
```

### Comparing `awkward-2.2.3/src/awkward/operations/ak_from_numpy.py` & `awkward-2.2.4/src/awkward/operations/ak_from_numpy.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("from_numpy",)
-import awkward as ak
+from awkward._dispatch import high_level_function
 from awkward._layout import from_arraylib, wrap_layout
 
 
+@high_level_function
 def from_numpy(
     array, *, regulararray=False, recordarray=True, highlevel=True, behavior=None
 ):
     """
     Args:
         array (np.ndarray): The NumPy array to convert into an Awkward Array.
             This array can be a np.ma.MaskedArray.
@@ -34,22 +35,12 @@
     * #ak.contents.ByteMaskedArray or #ak.contents.UnmaskedArray if the
       `array` is an np.ma.MaskedArray.
     * #ak.contents.RegularArray if `regulararray=True`.
     * #ak.contents.RecordArray if `recordarray=True`.
 
     See also #ak.to_numpy and #ak.from_cupy.
     """
-    with ak._errors.OperationErrorContext(
-        "ak.from_numpy",
-        {
-            "array": array,
-            "regulararray": regulararray,
-            "recordarray": recordarray,
-            "highlevel": highlevel,
-            "behavior": behavior,
-        },
-    ):
-        return wrap_layout(
-            from_arraylib(array, regulararray, recordarray),
-            highlevel=highlevel,
-            behavior=behavior,
-        )
+    return wrap_layout(
+        from_arraylib(array, regulararray, recordarray),
+        highlevel=highlevel,
+        behavior=behavior,
+    )
```

### Comparing `awkward-2.2.3/src/awkward/operations/ak_from_parquet.py` & `awkward-2.2.4/src/awkward/operations/ak_from_parquet.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("from_parquet",)
 import awkward as ak
+from awkward._dispatch import high_level_function
 from awkward._layout import wrap_layout
 from awkward._regularize import is_integer
 
 
+@high_level_function
 def from_parquet(
     path,
     *,
     columns=None,
     row_groups=None,
     storage_options=None,
     max_gap=64_000,
@@ -47,52 +49,38 @@
     The data are eagerly (not lazily) read and must fit into memory. Use `columns`
     and/or `row_groups` to select and filter manageable subsets of the data, and
     use #ak.metadata_from_parquet to find column names and the range of row groups
     that a dataset has.
 
     See also #ak.to_parquet, #ak.metadata_from_parquet.
     """
-    with ak._errors.OperationErrorContext(
-        "ak.from_parquet",
-        {
-            "path": path,
-            "columns": columns,
-            "row_groups": row_groups,
-            "storage_options": storage_options,
-            "max_gap": max_gap,
-            "max_block": max_block,
-            "footer_sample_size": footer_sample_size,
-            "generate_bitmasks": generate_bitmasks,
-            "highlevel": highlevel,
-            "behavior": behavior,
-        },
-    ):
-        import awkward._connect.pyarrow  # noqa: F401
-
-        parquet_columns, subform, actual_paths, fs, subrg, row_counts, meta = metadata(
-            path,
-            storage_options,
-            row_groups,
-            columns,
-        )
-        return _load(
-            actual_paths,
-            parquet_columns if columns is not None else None,
-            subrg,
-            max_gap,
-            max_block,
-            footer_sample_size,
-            generate_bitmasks,
-            subform,
-            highlevel,
-            behavior,
-            fs,
-        )
+    import awkward._connect.pyarrow  # noqa: F401
 
+    parquet_columns, subform, actual_paths, fs, subrg, row_counts, meta = metadata(
+        path,
+        storage_options,
+        row_groups,
+        columns,
+    )
+    return _load(
+        actual_paths,
+        parquet_columns if columns is not None else None,
+        subrg,
+        max_gap,
+        max_block,
+        footer_sample_size,
+        generate_bitmasks,
+        subform,
+        highlevel,
+        behavior,
+        fs,
+    )
 
+
+@high_level_function
 def metadata(
     path,
     storage_options=None,
     row_groups=None,
     columns=None,
     ignore_metadata=False,
     scan_files=True,
```

### Comparing `awkward-2.2.3/src/awkward/operations/ak_from_rdataframe.py` & `awkward-2.2.4/src/awkward/operations/ak_from_rdataframe.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("from_rdataframe",)
-
 import awkward as ak
+from awkward._dispatch import high_level_function
 from awkward._nplikes.numpylike import NumpyMetadata
 
 np = NumpyMetadata.instance()
 
 
+@high_level_function
 def from_rdataframe(
     rdf,
     columns,
     *,
     keep_order=False,
     offsets_type="int64",
     with_name=None,
@@ -41,29 +42,15 @@
     If `columns` is any other iterable, the return value is a record array, in which
     each field corresponds to an RDataFrame column. In particular, if the `columns`
     iterable contains only one string, it is still a record array, which has only
     one field.
 
     See also #ak.to_rdataframe.
     """
-    with ak._errors.OperationErrorContext(
-        "ak.from_rdataframe",
-        {
-            "rdf": rdf,
-            "columns": columns,
-            "keep_order": keep_order,
-            "offsets_type": offsets_type,
-            "with_name": with_name,
-            "highlevel": highlevel,
-            "behavior": behavior,
-        },
-    ):
-        return _impl(
-            rdf, columns, highlevel, behavior, with_name, offsets_type, keep_order
-        )
+    return _impl(rdf, columns, highlevel, behavior, with_name, offsets_type, keep_order)
 
 
 def _impl(
     data_frame, columns, highlevel, behavior, with_name, offsets_type, keep_order
 ):
     import awkward._connect.rdataframe.from_rdataframe  # noqa: F401
```

### Comparing `awkward-2.2.3/src/awkward/operations/ak_from_regular.py` & `awkward-2.2.4/src/awkward/operations/ak_from_regular.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("from_regular",)
 import awkward as ak
 from awkward._behavior import behavior_of
+from awkward._dispatch import high_level_function
 from awkward._errors import AxisError
 from awkward._layout import maybe_posaxis, wrap_layout
 from awkward._nplikes.numpylike import NumpyMetadata
 from awkward._regularize import regularize_axis
 
 np = NumpyMetadata.instance()
 
 
+@high_level_function
 def from_regular(array, axis=1, *, highlevel=True, behavior=None):
     """
     Args:
         array: Array-like data (anything #ak.to_layout recognizes).
         axis (int or None): The dimension at which this operation is applied.
             The outermost dimension is `0`, followed by `1`, etc., and negative
             values count backward from the innermost: `-1` is the innermost
@@ -34,19 +36,19 @@
         >>> ak.from_regular(regular, axis=2).type.show()
         2 * 3 * var * int64
         >>> ak.from_regular(regular, axis=-1).type.show()
         2 * 3 * var * int64
 
     See also #ak.to_regular.
     """
-    with ak._errors.OperationErrorContext(
-        "ak.from_regular",
-        {"array": array, "axis": axis, "highlevel": highlevel, "behavior": behavior},
-    ):
-        return _impl(array, axis, highlevel, behavior)
+    # Dispatch
+    yield (array,)
+
+    # Implementation
+    return _impl(array, axis, highlevel, behavior)
 
 
 def _impl(array, axis, highlevel, behavior):
     axis = regularize_axis(axis)
     layout = ak.operations.to_layout(array)
     behavior = behavior_of(array, behavior=behavior)
```

### Comparing `awkward-2.2.3/src/awkward/operations/ak_full_like.py` & `awkward-2.2.4/src/awkward/operations/ak_full_like.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("full_like",)
 import awkward as ak
 from awkward._behavior import behavior_of
 from awkward._connect.numpy import UNSUPPORTED
+from awkward._dispatch import high_level_function
 from awkward._layout import wrap_layout
 from awkward._nplikes.numpylike import NumpyMetadata
 from awkward._nplikes.typetracer import ensure_known_scalar
 from awkward.operations.ak_zeros_like import _ZEROS
 
 np = NumpyMetadata.instance()
 
 
+@high_level_function
 def full_like(
     array,
     fill_value,
     *,
     dtype=None,
     including_unknown=False,
     highlevel=True,
@@ -74,26 +76,19 @@
     `array`. (To fill them in, use #ak.fill_none.)
 
     See also #ak.zeros_like and #ak.ones_like.
 
     (There is no equivalent of NumPy's `np.empty_like` because Awkward Arrays
     are immutable.)
     """
-    with ak._errors.OperationErrorContext(
-        "ak.full_like",
-        {
-            "array": array,
-            "fill_value": fill_value,
-            "dtype": dtype,
-            "including_unknown": including_unknown,
-            "highlevel": highlevel,
-            "behavior": behavior,
-        },
-    ):
-        return _impl(array, fill_value, highlevel, behavior, dtype, including_unknown)
+    # Dispatch
+    yield array, fill_value
+
+    # Implementation
+    return _impl(array, fill_value, highlevel, behavior, dtype, including_unknown)
 
 
 def _impl(array, fill_value, highlevel, behavior, dtype, including_unknown):
     behavior = behavior_of(array, behavior=behavior)
     layout = ak.operations.to_layout(array, allow_record=True, allow_other=False)
 
     if dtype is not None:
```

### Comparing `awkward-2.2.3/src/awkward/operations/ak_is_categorical.py` & `awkward-2.2.4/src/awkward/operations/ak_is_categorical.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("is_categorical",)
-
 import awkward as ak
+from awkward._dispatch import high_level_function
 
 
+@high_level_function
 def is_categorical(array):
     """
     Args:
         array: Array-like data (anything #ak.to_layout recognizes).
 
     If the `array` is categorical (contains #ak.contents.IndexedArray or
     #ak.contents.IndexedOptionArray labeled with parameter
     `"__array__" = "categorical"`), then this function returns True;
     otherwise, it returns False.
 
     See also #ak.categories, #ak.to_categorical, #ak.from_categorical.
     """
-    with ak._errors.OperationErrorContext(
-        "ak.is_categorical",
-        {"array": array},
-    ):
-        return _impl(array)
+    # Dispatch
+    yield (array,)
+
+    # Implementation
+    return _impl(array)
 
 
 def _impl(array):
     layout = ak.operations.to_layout(array, allow_record=False, allow_other=False)
     return layout.purelist_parameter("__array__") == "categorical"
```

### Comparing `awkward-2.2.3/src/awkward/operations/ak_is_none.py` & `awkward-2.2.4/src/awkward/operations/ak_is_none.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("is_none",)
 import awkward as ak
 from awkward._behavior import behavior_of
+from awkward._dispatch import high_level_function
 from awkward._errors import AxisError
 from awkward._layout import maybe_posaxis, wrap_layout
 from awkward._nplikes.numpylike import NumpyMetadata
 from awkward._regularize import is_integer, regularize_axis
 
 np = NumpyMetadata.instance()
 
 
+@high_level_function
 def is_none(array, axis=0, *, highlevel=True, behavior=None):
     """
     Args:
         array: Array-like data (anything #ak.to_layout recognizes).
         axis (int): The dimension at which this operation is applied. The
             outermost dimension is `0`, followed by `1`, etc., and negative
             values count backward from the innermost: `-1` is the innermost
@@ -22,19 +24,19 @@
             a low-level #ak.contents.Content subclass.
         behavior (None or dict): Custom #ak.behavior for the output array, if
             high-level.
 
     Returns an array whose value is True where an element of `array` is None;
     False otherwise (at a given `axis` depth).
     """
-    with ak._errors.OperationErrorContext(
-        "ak.is_none",
-        {"array": array, "axis": axis, "highlevel": highlevel, "behavior": behavior},
-    ):
-        return _impl(array, axis, highlevel, behavior)
+    # Dispatch
+    yield (array,)
+
+    # Implementation
+    return _impl(array, axis, highlevel, behavior)
 
 
 def _impl(array, axis, highlevel, behavior):
     axis = regularize_axis(axis)
     layout = ak.operations.to_layout(array)
     behavior = behavior_of(array, behavior=behavior)
```

### Comparing `awkward-2.2.3/src/awkward/operations/ak_is_valid.py` & `awkward-2.2.4/src/awkward/operations/ak_validity_error.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,30 +1,37 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
-__all__ = ("is_valid",)
-
+__all__ = ("validity_error",)
 import awkward as ak
+from awkward._dispatch import high_level_function
 
 
-def is_valid(array, *, exception=False):
+@high_level_function
+def validity_error(array, *, exception=False):
     """
     Args:
         array: Array-like data (anything #ak.to_layout recognizes).
         exception (bool): If True, validity errors raise exceptions.
 
-    Returns True if there are no errors and False if there is an error.
+    Returns an empty string if there are no errors and a str containing the error message
+    if there are.
 
     Checks for errors in the structure of the array, such as indexes that run
     beyond the length of a node's `content`, etc. Either an error is raised or
-    the function returns a boolean.
+    a string describing the error is returned.
 
-    See also #ak.validity_error.
+    See also #ak.is_valid.
     """
-    with ak._errors.OperationErrorContext(
-        "ak.is_valid",
-        {"array": array, "exception": exception},
-    ):
-        return _impl(array, exception)
+    # Dispatch
+    yield (array,)
+
+    # Implementation
+    return _impl(array, exception)
 
 
 def _impl(array, exception):
-    out = ak.operations.validity_error(array, exception=exception)
-    return out in (None, "")
+    layout = ak.operations.to_layout(array, allow_record=False, allow_other=False)
+    out = ak._do.validity_error(layout, path="highlevel")
+
+    if out not in (None, "") and exception:
+        raise ValueError(out)
+    else:
+        return out
```

### Comparing `awkward-2.2.3/src/awkward/operations/ak_isclose.py` & `awkward-2.2.4/src/awkward/operations/ak_isclose.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("isclose",)
 import awkward as ak
 from awkward._behavior import behavior_of
+from awkward._dispatch import high_level_function
 from awkward._layout import wrap_layout
 from awkward._nplikes.numpylike import NumpyMetadata
 
 np = NumpyMetadata.instance()
 
 
+@high_level_function
 def isclose(
     a, b, rtol=1e-05, atol=1e-08, equal_nan=False, *, highlevel=True, behavior=None
 ):
     """
     Args:
         a: Array-like data (anything #ak.to_layout recognizes).
         b: Array-like data (anything #ak.to_layout recognizes).
@@ -23,27 +25,19 @@
             a low-level #ak.contents.Content subclass.
         behavior (None or dict): Custom #ak.behavior for the output array, if
             high-level.
 
     Implements [np.isclose](https://numpy.org/doc/stable/reference/generated/numpy.isclose.html)
     for Awkward Arrays.
     """
-    with ak._errors.OperationErrorContext(
-        "ak.isclose",
-        {
-            "a": a,
-            "b": b,
-            "rtol": rtol,
-            "atol": atol,
-            "equal_nan": equal_nan,
-            "highlevel": highlevel,
-            "behavior": behavior,
-        },
-    ):
-        return _impl(a, b, rtol, atol, equal_nan, highlevel, behavior)
+    # Dispatch
+    yield a, b
+
+    # Implementation
+    return _impl(a, b, rtol, atol, equal_nan, highlevel, behavior)
 
 
 def _impl(a, b, rtol, atol, equal_nan, highlevel, behavior):
     one = ak.operations.to_layout(a)
     two = ak.operations.to_layout(b)
 
     def action(inputs, backend, **kwargs):
```

### Comparing `awkward-2.2.3/src/awkward/operations/ak_linear_fit.py` & `awkward-2.2.4/src/awkward/operations/ak_linear_fit.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,23 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("linear_fit",)
 import awkward as ak
 from awkward._backends.dispatch import backend_of
 from awkward._behavior import behavior_of
+from awkward._dispatch import high_level_function
 from awkward._layout import wrap_layout
 from awkward._nplikes import ufuncs
 from awkward._nplikes.numpylike import NumpyMetadata
 from awkward._regularize import regularize_axis
 
 np = NumpyMetadata.instance()
 
 
-def linear_fit(
-    x,
-    y,
-    weight=None,
-    axis=None,
-    *,
-    keepdims=False,
-    mask_identity=False,
-):
+@high_level_function
+def linear_fit(x, y, weight=None, axis=None, *, keepdims=False, mask_identity=False):
     """
     Args:
         x: One coordinate to use in the linear fit (anything #ak.to_layout recognizes).
         y: The other coordinate to use in the linear fit (anything #ak.to_layout recognizes).
         weight: Data that can be broadcasted to `x` and `y` to give each point
             a weight. Weighting points equally is the same as no weights;
             weighting some points higher increases the significance of those
@@ -68,26 +62,19 @@
     might be arrays or even nested arrays; they match the structure of `x` and
     `y`.
 
     See #ak.sum for a complete description of handling nested lists and
     missing values (None) in reducers, and #ak.mean for an example with another
     non-reducer.
     """
-    with ak._errors.OperationErrorContext(
-        "ak.linear_fit",
-        {
-            "x": x,
-            "y": y,
-            "weight": weight,
-            "axis": axis,
-            "keepdims": keepdims,
-            "mask_identity": mask_identity,
-        },
-    ):
-        return _impl(x, y, weight, axis, keepdims, mask_identity)
+    # Dispatch
+    yield x, y, weight
+
+    # Implementation
+    return _impl(x, y, weight, axis, keepdims, mask_identity)
 
 
 def _impl(x, y, weight, axis, keepdims, mask_identity):
     axis = regularize_axis(axis)
     behavior = behavior_of(x, y, weight)
     x = ak.highlevel.Array(
         ak.operations.to_layout(x, allow_record=False, allow_other=False),
```

### Comparing `awkward-2.2.3/src/awkward/operations/ak_local_index.py` & `awkward-2.2.4/src/awkward/operations/ak_local_index.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("local_index",)
 import awkward as ak
+from awkward._dispatch import high_level_function
 from awkward._layout import wrap_layout
 from awkward._nplikes.numpylike import NumpyMetadata
 from awkward._regularize import regularize_axis
 
 np = NumpyMetadata.instance()
 
 
+@high_level_function
 def local_index(array, axis=-1, *, highlevel=True, behavior=None):
     """
     Args:
         array: Array-like data (anything #ak.to_layout recognizes).
         axis (int): The dimension at which this operation is applied. The
             outermost dimension is `0`, followed by `1`, etc., and negative
             values count backward from the innermost: `-1` is the innermost
@@ -68,19 +70,19 @@
                        1               4.4
         3     0        0               5.5
               2        0               6.6
                        1               7.7
                        2               8.8
                        3               9.9
     """
-    with ak._errors.OperationErrorContext(
-        "ak.local_index",
-        {"array": array, "axis": axis, "highlevel": highlevel, "behavior": behavior},
-    ):
-        return _impl(array, axis, highlevel, behavior)
+    # Dispatch
+    yield (array,)
+
+    # Implementation
+    return _impl(array, axis, highlevel, behavior)
 
 
 def _impl(array, axis, highlevel, behavior):
     axis = regularize_axis(axis)
     layout = ak.operations.to_layout(array, allow_record=True, allow_other=False)
     out = ak._do.local_index(layout, axis)
     return wrap_layout(out, behavior, highlevel, like=array)
```

### Comparing `awkward-2.2.3/src/awkward/operations/ak_mask.py` & `awkward-2.2.4/src/awkward/operations/ak_mask.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("mask",)
 import awkward as ak
 from awkward._behavior import behavior_of
+from awkward._dispatch import high_level_function
 from awkward._layout import wrap_layout
 from awkward._nplikes.numpylike import NumpyMetadata
 
 np = NumpyMetadata.instance()
 
 
+@high_level_function
 def mask(array, mask, *, valid_when=True, highlevel=True, behavior=None):
     """
     Args:
         array: Array-like data (anything #ak.to_layout recognizes).
         mask (array of booleans): The mask that overlays elements in the
             `array` with None. Must have the same length as `array`.
         valid_when (bool): If True, True values in `mask` are considered
@@ -84,25 +86,19 @@
 
     is
 
         array.mask[array_of_booleans]
 
     (which is 5 characters away from simply filtering the `array`).
     """
-    with ak._errors.OperationErrorContext(
-        "ak.mask",
-        {
-            "array": array,
-            "mask": mask,
-            "valid_when": valid_when,
-            "highlevel": highlevel,
-            "behavior": behavior,
-        },
-    ):
-        return _impl(array, mask, valid_when, highlevel, behavior)
+    # Dispatch
+    yield array, mask
+
+    # Implementation
+    return _impl(array, mask, valid_when, highlevel, behavior)
 
 
 def _impl(array, mask, valid_when, highlevel, behavior):
     def action(inputs, backend, **kwargs):
         layoutarray, layoutmask = inputs
         if isinstance(layoutmask, ak.contents.NumpyArray):
             m = backend.nplike.asarray(layoutmask)
```

### Comparing `awkward-2.2.3/src/awkward/operations/ak_max.py` & `awkward-2.2.4/src/awkward/operations/ak_max.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("max",)
 import awkward as ak
 from awkward._behavior import behavior_of
 from awkward._connect.numpy import UNSUPPORTED
+from awkward._dispatch import high_level_function
 from awkward._layout import wrap_layout
 from awkward._nplikes.numpylike import NumpyMetadata
 from awkward._regularize import regularize_axis
 
 np = NumpyMetadata.instance()
 
 
+@high_level_function
 def max(
     array,
     axis=None,
     *,
     keepdims=False,
     initial=None,
     mask_identity=True,
@@ -55,37 +57,30 @@
     but it generalizes to cases where they do not.
 
     See #ak.sum for a more complete description of nested list and missing
     value (None) handling in reducers.
 
     See also #ak.nanmax.
     """
-    with ak._errors.OperationErrorContext(
-        "ak.max",
-        {
-            "array": array,
-            "axis": axis,
-            "keepdims": keepdims,
-            "initial": initial,
-            "mask_identity": mask_identity,
-            "highlevel": highlevel,
-            "behavior": behavior,
-        },
-    ):
-        return _impl(
-            array,
-            axis,
-            keepdims,
-            initial,
-            mask_identity,
-            highlevel,
-            behavior,
-        )
+    # Dispatch
+    yield (array,)
 
+    # Implementation
+    return _impl(
+        array,
+        axis,
+        keepdims,
+        initial,
+        mask_identity,
+        highlevel,
+        behavior,
+    )
 
+
+@high_level_function
 def nanmax(
     array,
     axis=None,
     *,
     keepdims=False,
     initial=None,
     mask_identity=True,
@@ -118,37 +113,27 @@
 
         ak.max(ak.nan_to_none(array))
 
     with all other arguments unchanged.
 
     See also #ak.max.
     """
-    with ak._errors.OperationErrorContext(
-        "ak.nanmax",
-        {
-            "array": array,
-            "axis": axis,
-            "keepdims": keepdims,
-            "initial": initial,
-            "mask_identity": mask_identity,
-            "highlevel": highlevel,
-            "behavior": behavior,
-        },
-    ):
-        array = ak.operations.ak_nan_to_none._impl(array, False, None)
-
-        return _impl(
-            array,
-            axis,
-            keepdims,
-            initial,
-            mask_identity,
-            highlevel,
-            behavior,
-        )
+    # Dispatch
+    yield (array,)
+
+    # Implementation
+    return _impl(
+        ak.operations.ak_nan_to_none._impl(array, False, None),
+        axis,
+        keepdims,
+        initial,
+        mask_identity,
+        highlevel,
+        behavior,
+    )
 
 
 def _impl(array, axis, keepdims, initial, mask_identity, highlevel, behavior):
     axis = regularize_axis(axis)
     layout = ak.operations.to_layout(array, allow_record=False, allow_other=False)
     behavior = behavior_of(array, behavior=behavior)
     reducer = ak._reducers.Max(initial)
```

### Comparing `awkward-2.2.3/src/awkward/operations/ak_mean.py` & `awkward-2.2.4/src/awkward/operations/ak_mean.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,22 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("mean",)
 import awkward as ak
 from awkward._behavior import behavior_of
 from awkward._connect.numpy import UNSUPPORTED
+from awkward._dispatch import high_level_function
 from awkward._layout import maybe_posaxis
 from awkward._nplikes.numpylike import NumpyMetadata
 from awkward._regularize import regularize_axis
 
 np = NumpyMetadata.instance()
 
 
-def mean(
-    x,
-    weight=None,
-    axis=None,
-    *,
-    keepdims=False,
-    mask_identity=False,
-):
+@high_level_function
+def mean(x, weight=None, axis=None, *, keepdims=False, mask_identity=False):
     """
     Args:
         x: The data on which to compute the mean (anything #ak.to_layout recognizes).
         weight: Data that can be broadcasted to `x` to give each value a
             weight. Weighting values equally is the same as no weights;
             weighting some values higher increases the significance of those
             values. Weights can be zero or negative.
@@ -76,35 +71,23 @@
     behavior as reducers.
 
     See #ak.sum for a complete description of handling nested lists and
     missing values (None) in reducers.
 
     See also #ak.nanmean.
     """
-    with ak._errors.OperationErrorContext(
-        "ak.mean",
-        {
-            "x": x,
-            "weight": weight,
-            "axis": axis,
-            "keepdims": keepdims,
-            "mask_identity": mask_identity,
-        },
-    ):
-        return _impl(x, weight, axis, keepdims, mask_identity)
-
-
-def nanmean(
-    x,
-    weight=None,
-    axis=None,
-    *,
-    keepdims=False,
-    mask_identity=True,
-):
+    # Dispatch
+    yield x, weight
+
+    # Implementation
+    return _impl(x, weight, axis, keepdims, mask_identity)
+
+
+@high_level_function
+def nanmean(x, weight=None, axis=None, *, keepdims=False, mask_identity=True):
     """
     Args:
         x: The data on which to compute the mean (anything #ak.to_layout recognizes).
         weight: Data that can be broadcasted to `x` to give each value a
             weight. Weighting values equally is the same as no weights;
             weighting some values higher increases the significance of those
             values. Weights can be zero or negative.
@@ -128,29 +111,27 @@
 
         ak.mean(ak.nan_to_none(array))
 
     with all other arguments unchanged.
 
     See also #ak.mean.
     """
-    with ak._errors.OperationErrorContext(
-        "ak.nanmean",
-        {
-            "x": x,
-            "weight": weight,
-            "axis": axis,
-            "keepdims": keepdims,
-            "mask_identity": mask_identity,
-        },
-    ):
-        x = ak.operations.ak_nan_to_none._impl(x, False, None)
-        if weight is not None:
-            weight = ak.operations.ak_nan_to_none._impl(weight, False, None)
+    # Dispatch
+    yield x, weight
+
+    if weight is not None:
+        weight = ak.operations.ak_nan_to_none._impl(weight, False, None)
 
-        return _impl(x, weight, axis, keepdims, mask_identity)
+    return _impl(
+        ak.operations.ak_nan_to_none._impl(x, False, None),
+        weight,
+        axis,
+        keepdims,
+        mask_identity,
+    )
 
 
 def _impl(x, weight, axis, keepdims, mask_identity):
     axis = regularize_axis(axis)
     behavior = behavior_of(x, weight)
     x = ak.highlevel.Array(
         ak.operations.to_layout(x, allow_record=False, allow_other=False),
```

### Comparing `awkward-2.2.3/src/awkward/operations/ak_merge_option_of_records.py` & `awkward-2.2.4/src/awkward/operations/ak_merge_option_of_records.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("merge_option_of_records",)
 import awkward as ak
 from awkward._backends.numpy import NumpyBackend
 from awkward._behavior import behavior_of
+from awkward._dispatch import high_level_function
 from awkward._errors import AxisError
 from awkward._layout import maybe_posaxis, wrap_layout
 from awkward._nplikes.numpylike import NumpyMetadata
 from awkward._regularize import regularize_axis
 
 np = NumpyMetadata.instance()
 cpu = NumpyBackend.instance()
 
 
+@high_level_function
 def merge_option_of_records(array, axis=-1, *, highlevel=True, behavior=None):
     """
     Args:
         array: Array-like data (anything #ak.to_layout recognizes).
         axis (int): The dimension at which this operation is applied.
             The outermost dimension is `0`, followed by `1`, etc., and negative
             values count backward from the  innermost: `-1` is the innermost
@@ -30,19 +32,19 @@
         >>> array = ak.Array([None, {"a": 1}, {"a": 2}])
 
     into records of options, i.e.
 
         >>> ak.merge_option_of_records(array)
         <Array [{a: None}, {a: 1}, {a: 2}] type='3 * {a: ?int64}'>
     """
-    with ak._errors.OperationErrorContext(
-        "ak.merge_option_of_records",
-        {"array": array, "axis": axis, "highlevel": highlevel, "behavior": behavior},
-    ):
-        return _impl(array, axis, highlevel, behavior)
+    # Dispatch
+    yield (array,)
+
+    # Implementation
+    return _impl(array, axis, highlevel, behavior)
 
 
 def _impl(array, axis, highlevel, behavior):
     axis = regularize_axis(axis)
     behavior = behavior_of(array, behavior=behavior)
     layout = ak.to_layout(array, allow_record=False)
```

### Comparing `awkward-2.2.3/src/awkward/operations/ak_merge_union_of_records.py` & `awkward-2.2.4/src/awkward/operations/ak_merge_union_of_records.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("merge_union_of_records",)
 import awkward as ak
 from awkward._backends.numpy import NumpyBackend
 from awkward._behavior import behavior_of
+from awkward._dispatch import high_level_function
 from awkward._errors import AxisError
 from awkward._layout import maybe_posaxis, wrap_layout
 from awkward._nplikes.numpylike import ArrayLike, NumpyMetadata
 from awkward._regularize import regularize_axis
 
 np = NumpyMetadata.instance()
 cpu = NumpyBackend.instance()
 
 
+@high_level_function
 def merge_union_of_records(array, axis=-1, *, highlevel=True, behavior=None):
     """
     Args:
         array: Array-like data (anything #ak.to_layout recognizes).
         axis (int): The dimension at which this operation is applied.
             The outermost dimension is `0`, followed by `1`, etc., and negative
             values count backward from the  innermost: `-1` is the innermost
@@ -40,19 +42,19 @@
 
         >>> array = ak.concatenate(([{"a": 1}], [{"b": 2}, None]))
         >>> array
         <Array [{a: 1}, {b: 2}, None] type='3 * union[{a: int64}, ?{b: int64}]'>
         >>> ak.merge_union_of_records(array)
         <Array [{a: 1, b: None}, {...}, None] type='3 * ?{a: ?int64, b: ?int64}'>
     """
-    with ak._errors.OperationErrorContext(
-        "ak.merge_union_of_records",
-        {"array": array, "axis": axis, "highlevel": highlevel, "behavior": behavior},
-    ):
-        return _impl(array, axis, highlevel, behavior)
+    # Dispatch
+    yield (array,)
+
+    # Implementation
+    return _impl(array, axis, highlevel, behavior)
 
 
 def _impl(array, axis, highlevel, behavior):
     axis = regularize_axis(axis)
     behavior = behavior_of(array, behavior=behavior)
     layout = ak.to_layout(array, allow_record=False)
```

### Comparing `awkward-2.2.3/src/awkward/operations/ak_metadata_from_parquet.py` & `awkward-2.2.4/src/awkward/operations/ak_metadata_from_parquet.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("metadata_from_parquet",)
-
 import collections
 
 import awkward as ak
+from awkward._dispatch import high_level_function
 from awkward._nplikes.numpylike import NumpyMetadata
 
 np = NumpyMetadata.instance()
 
 
 ParquetMetadata = collections.namedtuple(
     "ParquetMetadata",
     ["form", "fs", "paths", "metadata"],
 )
 
 
+@high_level_function
 def metadata_from_parquet(
     path,
     *,
     storage_options=None,
     row_groups=None,
     ignore_metadata=False,
     scan_files=True,
@@ -55,28 +56,21 @@
     * `num_row_groups`: the units that can be filtered (for the #ak.from_parquet `row_groups`
       argument).
 
     See also #ak.from_parquet, #ak.to_parquet.
     """
     import awkward._connect.pyarrow  # noqa: F401
 
-    with ak._errors.OperationErrorContext(
-        "ak.metadata_from_parquet",
-        {
-            "path": path,
-            "storage_options": storage_options,
-        },
-    ):
-        return _impl(
-            path,
-            storage_options,
-            row_groups=row_groups,
-            ignore_metadata=ignore_metadata,
-            scan_files=scan_files,
-        )
+    return _impl(
+        path,
+        storage_options,
+        row_groups=row_groups,
+        ignore_metadata=ignore_metadata,
+        scan_files=scan_files,
+    )
 
 
 def _impl(
     path, storage_options, row_groups=None, ignore_metadata=False, scan_files=True
 ):
     results = ak.operations.ak_from_parquet.metadata(
         path, storage_options, row_groups, None, ignore_metadata, scan_files
```

### Comparing `awkward-2.2.3/src/awkward/operations/ak_min.py` & `awkward-2.2.4/src/awkward/operations/ak_min.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("min",)
 import awkward as ak
 from awkward._behavior import behavior_of
 from awkward._connect.numpy import UNSUPPORTED
+from awkward._dispatch import high_level_function
 from awkward._layout import wrap_layout
 from awkward._nplikes.numpylike import NumpyMetadata
 from awkward._regularize import regularize_axis
 
 np = NumpyMetadata.instance()
 
 
+@high_level_function
 def min(
     array,
     axis=None,
     *,
     keepdims=False,
     initial=None,
     mask_identity=True,
@@ -55,35 +57,30 @@
     but it generalizes to cases where they do not.
 
     See #ak.sum for a more complete description of nested list and missing
     value (None) handling in reducers.
 
     See also #ak.nanmin.
     """
-    with ak._errors.OperationErrorContext(
-        "ak.min",
-        {
-            "array": array,
-            "axis": axis,
-            "keepdims": keepdims,
-            "initial": initial,
-            "mask_identity": mask_identity,
-        },
-    ):
-        return _impl(
-            array,
-            axis,
-            keepdims,
-            initial,
-            mask_identity,
-            highlevel,
-            behavior,
-        )
+    # Dispatch
+    yield (array,)
 
+    # Implementation
+    return _impl(
+        array,
+        axis,
+        keepdims,
+        initial,
+        mask_identity,
+        highlevel,
+        behavior,
+    )
 
+
+@high_level_function
 def nanmin(
     array,
     axis=None,
     *,
     keepdims=False,
     initial=None,
     mask_identity=True,
@@ -116,37 +113,27 @@
 
         ak.min(ak.nan_to_none(array))
 
     with all other arguments unchanged.
 
     See also #ak.min.
     """
-    with ak._errors.OperationErrorContext(
-        "ak.nanmin",
-        {
-            "array": array,
-            "axis": axis,
-            "keepdims": keepdims,
-            "initial": initial,
-            "mask_identity": mask_identity,
-            "highlevel": highlevel,
-            "behavior": behavior,
-        },
-    ):
-        array = ak.operations.ak_nan_to_none._impl(array, False, None)
-
-        return _impl(
-            array,
-            axis,
-            keepdims,
-            initial,
-            mask_identity,
-            highlevel,
-            behavior,
-        )
+    # Dispatch
+    yield (array,)
+
+    # Implementation
+    return _impl(
+        ak.operations.ak_nan_to_none._impl(array, False, None),
+        axis,
+        keepdims,
+        initial,
+        mask_identity,
+        highlevel,
+        behavior,
+    )
 
 
 def _impl(array, axis, keepdims, initial, mask_identity, highlevel, behavior):
     axis = regularize_axis(axis)
     layout = ak.operations.to_layout(array, allow_record=False, allow_other=False)
     behavior = behavior_of(array, behavior=behavior)
     reducer = ak._reducers.Min(initial)
```

### Comparing `awkward-2.2.3/src/awkward/operations/ak_moment.py` & `awkward-2.2.4/src/awkward/operations/ak_moment.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,20 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("moment",)
 import awkward as ak
 from awkward._behavior import behavior_of
+from awkward._dispatch import high_level_function
 from awkward._nplikes.numpylike import NumpyMetadata
 from awkward._regularize import regularize_axis
 
 np = NumpyMetadata.instance()
 
 
-def moment(
-    x,
-    n,
-    weight=None,
-    axis=None,
-    *,
-    keepdims=False,
-    mask_identity=False,
-):
+@high_level_function
+def moment(x, n, weight=None, axis=None, *, keepdims=False, mask_identity=False):
     """
     Args:
         x: The data on which to compute the moment (anything #ak.to_layout recognizes).
         n (int): The choice of moment: `0` is a sum of weights, `1` is
             #ak.mean, `2` is #ak.var without subtracting the mean, etc.
         weight: Data that can be broadcasted to `x` to give each value a
             weight. Weighting values equally is the same as no weights;
@@ -54,26 +48,19 @@
     The `n=2` moment differs from #ak.var in that #ak.var also subtracts the
     mean (the `n=1` moment).
 
     See #ak.sum for a complete description of handling nested lists and
     missing values (None) in reducers, and #ak.mean for an example with another
     non-reducer.
     """
-    with ak._errors.OperationErrorContext(
-        "ak.moment",
-        {
-            "x": x,
-            "n": n,
-            "weight": weight,
-            "axis": axis,
-            "keepdims": keepdims,
-            "mask_identity": mask_identity,
-        },
-    ):
-        return _impl(x, n, weight, axis, keepdims, mask_identity)
+    # Dispatch
+    yield x, weight
+
+    # Implementation
+    return _impl(x, n, weight, axis, keepdims, mask_identity)
 
 
 def _impl(x, n, weight, axis, keepdims, mask_identity):
     axis = regularize_axis(axis)
     behavior = behavior_of(x, weight)
     x = ak.highlevel.Array(
         ak.operations.to_layout(x, allow_record=False, allow_other=False),
```

### Comparing `awkward-2.2.3/src/awkward/operations/ak_nan_to_none.py` & `awkward-2.2.4/src/awkward/operations/ak_nan_to_none.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,39 +1,37 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("nan_to_none",)
 import awkward as ak
 from awkward._behavior import behavior_of
+from awkward._dispatch import high_level_function
 from awkward._layout import wrap_layout
 from awkward._nplikes.numpylike import NumpyMetadata
 
 np = NumpyMetadata.instance()
 
 
+@high_level_function
 def nan_to_none(array, *, highlevel=True, behavior=None):
     """
     Args:
         array: Array-like data (anything #ak.to_layout recognizes).
         highlevel (bool): If True, return an #ak.Array; otherwise, return
             a low-level #ak.contents.Content subclass.
         behavior (None or dict): Custom #ak.behavior for the output array, if
             high-level.
 
     Converts NaN ("not a number") into None, i.e. missing values with option-type.
 
     See also #ak.nan_to_num to convert NaN or infinity to specified values.
     """
-    with ak._errors.OperationErrorContext(
-        "ak.nan_to_none",
-        {
-            "array": array,
-            "highlevel": highlevel,
-            "behavior": behavior,
-        },
-    ):
-        return _impl(array, highlevel, behavior)
+    # Dispatch
+    yield (array,)
+
+    # Implementation
+    return _impl(array, highlevel, behavior)
 
 
 def _impl(array, highlevel, behavior):
     def action(layout, continuation, **kwargs):
         if isinstance(layout, ak.contents.NumpyArray) and issubclass(
             layout.dtype.type, np.floating
         ):
```

### Comparing `awkward-2.2.3/src/awkward/operations/ak_nan_to_num.py` & `awkward-2.2.4/src/awkward/operations/ak_nan_to_num.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("nan_to_num",)
 import awkward as ak
 from awkward._behavior import behavior_of
+from awkward._dispatch import high_level_function
 from awkward._layout import wrap_layout
 from awkward._nplikes.numpylike import NumpyMetadata
 
 np = NumpyMetadata.instance()
 
 
+@high_level_function
 def nan_to_num(
     array,
     copy=True,
     nan=0.0,
     posinf=None,
     neginf=None,
     *,
@@ -33,27 +35,19 @@
             high-level.
 
     Implements [np.nan_to_num](https://numpy.org/doc/stable/reference/generated/numpy.nan_to_num.html)
     for Awkward Arrays, which replaces NaN ("not a number") or infinity with specified values.
 
     See also #ak.nan_to_none to convert NaN to None, i.e. missing values with option-type.
     """
-    with ak._errors.OperationErrorContext(
-        "ak.nan_to_num",
-        {
-            "array": array,
-            "copy": copy,
-            "nan": nan,
-            "posinf": posinf,
-            "neginf": neginf,
-            "highlevel": highlevel,
-            "behavior": behavior,
-        },
-    ):
-        return _impl(array, copy, nan, posinf, neginf, highlevel, behavior)
+    # Dispatch
+    yield (array,)
+
+    # Implementation
+    return _impl(array, copy, nan, posinf, neginf, highlevel, behavior)
 
 
 def _impl(array, copy, nan, posinf, neginf, highlevel, behavior):
     behavior = behavior_of(array, behavior=behavior)
 
     broadcasting_ids = {}
     broadcasting = []
```

### Comparing `awkward-2.2.3/src/awkward/operations/ak_num.py` & `awkward-2.2.4/src/awkward/operations/ak_num.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("num",)
 import awkward as ak
 from awkward._behavior import behavior_of
+from awkward._dispatch import high_level_function
 from awkward._errors import AxisError
 from awkward._layout import maybe_posaxis, wrap_layout
 from awkward._nplikes.numpylike import NumpyMetadata
 from awkward._regularize import is_integer, regularize_axis
 
 np = NumpyMetadata.instance()
 
 
+@high_level_function
 def num(array, axis=1, *, highlevel=True, behavior=None):
     """
     Args:
         array: Array-like data (anything #ak.to_layout recognizes).
         axis (int): The dimension at which this operation is applied. The
             outermost dimension is `0`, followed by `1`, etc., and negative
             values count backward from the innermost: `-1` is the innermost
@@ -65,19 +67,19 @@
 
     To keep a placeholder (None) in each place we do not want to select,
     consider using #ak.mask instead of a #ak.Array.__getitem__.
 
         >>> array.mask[ak.num(array) > 0][:, 0]
         <Array [[1.1, 2.2, 3.3], None, [7.7]] type='3 * option[var * float64]'>
     """
-    with ak._errors.OperationErrorContext(
-        "ak.num",
-        {"array": array, "axis": axis, "highlevel": highlevel, "behavior": behavior},
-    ):
-        return _impl(array, axis, highlevel, behavior)
+    # Dispatch
+    yield (array,)
+
+    # Implementation
+    return _impl(array, axis, highlevel, behavior)
 
 
 def _impl(array, axis, highlevel, behavior):
     axis = regularize_axis(axis)
     layout = ak.operations.to_layout(array)
     behavior = behavior_of(array, behavior=behavior)
```

### Comparing `awkward-2.2.3/src/awkward/operations/ak_ones_like.py` & `awkward-2.2.4/src/awkward/operations/ak_ones_like.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("ones_like",)
-
 import awkward as ak
 from awkward._connect.numpy import UNSUPPORTED
+from awkward._dispatch import high_level_function
 from awkward._nplikes.numpylike import NumpyMetadata
 
 np = NumpyMetadata.instance()
 
 
+@high_level_function
 def ones_like(
     array, *, dtype=None, including_unknown=False, highlevel=True, behavior=None
 ):
     """
     Args:
         array: Array-like data (anything #ak.to_layout recognizes).
         dtype (None or NumPy dtype): Overrides the data type of the result.
@@ -26,25 +27,19 @@
     This is the equivalent of NumPy's `np.ones_like` for Awkward Arrays.
 
     See #ak.full_like for details, and see also #ak.zeros_like.
 
     (There is no equivalent of NumPy's `np.empty_like` because Awkward Arrays
     are immutable.)
     """
-    with ak._errors.OperationErrorContext(
-        "ak.ones_like",
-        {
-            "array": array,
-            "dtype": dtype,
-            "including_unknown": including_unknown,
-            "highlevel": highlevel,
-            "behavior": behavior,
-        },
-    ):
-        return _impl(array, highlevel, behavior, dtype, including_unknown)
+    # Dispatch
+    yield (array,)
+
+    # Implementation
+    return _impl(array, highlevel, behavior, dtype, including_unknown)
 
 
 def _impl(array, highlevel, behavior, dtype, including_unknown):
     return ak.operations.ak_full_like._impl(
         array, 1, highlevel, behavior, dtype, including_unknown
     )
```

### Comparing `awkward-2.2.3/src/awkward/operations/ak_pad_none.py` & `awkward-2.2.4/src/awkward/operations/ak_pad_none.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("pad_none",)
 import awkward as ak
+from awkward._dispatch import high_level_function
 from awkward._layout import wrap_layout
 from awkward._nplikes.numpylike import NumpyMetadata
 from awkward._regularize import regularize_axis
 
 np = NumpyMetadata.instance()
 
 
+@high_level_function
 def pad_none(array, target, axis=1, *, clip=False, highlevel=True, behavior=None):
     """
     Args:
         array: Array-like data (anything #ak.to_layout recognizes).
         target (int): The intended length of the lists. If `clip=True`,
             the output lists will have exactly this length; otherwise,
             they will have *at least* this length.
@@ -91,26 +93,19 @@
     in the distinction between the following types.
 
         >>> ak.pad_none(array, 2, axis=2).type.show()
         3 * var * var * ?float64
         >>> ak.pad_none(array, 2, axis=2, clip=True).type.show()
         3 * var *   2 * ?float64
     """
-    with ak._errors.OperationErrorContext(
-        "ak.pad_none",
-        {
-            "array": array,
-            "target": target,
-            "axis": axis,
-            "clip": clip,
-            "highlevel": highlevel,
-            "behavior": behavior,
-        },
-    ):
-        return _impl(array, target, axis, clip, highlevel, behavior)
+    # Dispatch
+    yield (array,)
+
+    # Implementation
+    return _impl(array, target, axis, clip, highlevel, behavior)
 
 
 def _impl(array, target, axis, clip, highlevel, behavior):
     axis = regularize_axis(axis)
     layout = ak.operations.to_layout(array, allow_record=False, allow_other=False)
     out = ak._do.pad_none(layout, target, axis, clip=clip)
```

### Comparing `awkward-2.2.3/src/awkward/operations/ak_parameters.py` & `awkward-2.2.4/src/awkward/operations/ak_parameters.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("parameters",)
-
 import copy
 import numbers
 
 from awkward_cpp.lib import _ext
 
 import awkward as ak
+from awkward._dispatch import high_level_function
 from awkward._nplikes.numpylike import NumpyMetadata
 
 np = NumpyMetadata.instance()
 
 
+@high_level_function
 def parameters(array):
     """
     Args:
         array: Array-like data (anything #ak.to_layout recognizes).
 
     Extracts parameters from the outermost array node of `array` (many types
     supported, including all Awkward Arrays and Records).
@@ -24,19 +25,19 @@
     Every #ak.contents.Content node has a different set of parameters. Some
     key names are special, such as `"__record__"` and `"__array__"` that name
     particular records and arrays as capable of supporting special behaviors.
 
     See #ak.Array and #ak.behavior for a more complete description of
     behaviors.
     """
-    with ak._errors.OperationErrorContext(
-        "ak.parameters",
-        {"array": array},
-    ):
-        return _impl(array)
+    # Dispatch
+    yield (array,)
+
+    # Implementation
+    return _impl(array)
 
 
 def _impl(array):
     if isinstance(array, (ak.highlevel.Array, ak.highlevel.Record)):
         return _copy(array.layout.parameters)
 
     elif isinstance(
```

### Comparing `awkward-2.2.3/src/awkward/operations/ak_prod.py` & `awkward-2.2.4/src/awkward/operations/ak_prod.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("prod",)
 import awkward as ak
 from awkward._behavior import behavior_of
 from awkward._connect.numpy import UNSUPPORTED
+from awkward._dispatch import high_level_function
 from awkward._layout import wrap_layout
 from awkward._nplikes.numpylike import NumpyMetadata
 from awkward._regularize import regularize_axis
 
 np = NumpyMetadata.instance()
 
 
+@high_level_function
 def prod(
     array,
     axis=None,
     *,
     keepdims=False,
     mask_identity=False,
     highlevel=True,
@@ -47,28 +49,22 @@
     but it generalizes to cases where they do not.
 
     See #ak.sum for a more complete description of nested list and missing
     value (None) handling in reducers.
 
     See also #ak.nanprod.
     """
-    with ak._errors.OperationErrorContext(
-        "ak.prod",
-        {
-            "array": array,
-            "axis": axis,
-            "keepdims": keepdims,
-            "mask_identity": mask_identity,
-            "highlevel": highlevel,
-            "behavior": behavior,
-        },
-    ):
-        return _impl(array, axis, keepdims, mask_identity, highlevel, behavior)
+    # Dispatch
+    yield (array,)
 
+    # Implementation
+    return _impl(array, axis, keepdims, mask_identity, highlevel, behavior)
 
+
+@high_level_function
 def nanprod(
     array,
     axis=None,
     *,
     keepdims=False,
     mask_identity=False,
     highlevel=True,
@@ -96,28 +92,26 @@
 
         ak.prod(ak.nan_to_none(array))
 
     with all other arguments unchanged.
 
     See also #ak.prod.
     """
-    with ak._errors.OperationErrorContext(
-        "ak.nanprod",
-        {
-            "array": array,
-            "axis": axis,
-            "keepdims": keepdims,
-            "mask_identity": mask_identity,
-            "highlevel": highlevel,
-            "behavior": behavior,
-        },
-    ):
-        array = ak.operations.ak_nan_to_none._impl(array, False, None)
+    # Dispatch
+    yield (array,)
 
-        return _impl(array, axis, keepdims, mask_identity, highlevel, behavior)
+    # Implementation
+    return _impl(
+        ak.operations.ak_nan_to_none._impl(array, False, None),
+        axis,
+        keepdims,
+        mask_identity,
+        highlevel,
+        behavior,
+    )
 
 
 def _impl(array, axis, keepdims, mask_identity, highlevel, behavior):
     axis = regularize_axis(axis)
     layout = ak.operations.to_layout(array, allow_record=False, allow_other=False)
     behavior = behavior_of(array, behavior=behavior)
     reducer = ak._reducers.Prod()
```

### Comparing `awkward-2.2.3/src/awkward/operations/ak_ptp.py` & `awkward-2.2.4/src/awkward/operations/ak_ptp.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("ptp",)
 import awkward as ak
 from awkward._behavior import behavior_of
 from awkward._connect.numpy import UNSUPPORTED
+from awkward._dispatch import high_level_function
 from awkward._layout import maybe_posaxis
 from awkward._nplikes.numpylike import NumpyMetadata
 from awkward._regularize import regularize_axis
 
 np = NumpyMetadata.instance()
 
 
+@high_level_function
 def ptp(array, axis=None, *, keepdims=False, mask_identity=True):
     """
     Args:
         array: Array-like data (anything #ak.to_layout recognizes).
         axis (None or int): If None, combine all values from the array into
             a single scalar result; if an int, group by that axis: `0` is the
             outermost, `1` is the first level of nested lists, etc., and
@@ -53,24 +55,19 @@
         <Array [3, 0, 1] type='3 * float64'>
 
     The second value is `0` because the list is empty.
 
     See #ak.sum for a more complete description of nested list and missing
     value (None) handling in reducers.
     """
-    with ak._errors.OperationErrorContext(
-        "ak.ptp",
-        {
-            "array": array,
-            "axis": axis,
-            "keepdims": keepdims,
-            "mask_identity": mask_identity,
-        },
-    ):
-        return _impl(array, axis, keepdims, mask_identity)
+    # Dispatch
+    yield (array,)
+
+    # Implementation
+    return _impl(array, axis, keepdims, mask_identity)
 
 
 def _impl(array, axis, keepdims, mask_identity):
     axis = regularize_axis(axis)
     behavior = behavior_of(array)
     layout = ak.operations.to_layout(array, allow_record=False, allow_other=False)
```

### Comparing `awkward-2.2.3/src/awkward/operations/ak_ravel.py` & `awkward-2.2.4/src/awkward/operations/ak_ravel.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("ravel",)
 import awkward as ak
 from awkward._connect.numpy import UNSUPPORTED
+from awkward._dispatch import high_level_function
 from awkward._layout import wrap_layout
 from awkward._nplikes.numpylike import NumpyMetadata
 
 np = NumpyMetadata.instance()
 
 
+@high_level_function
 def ravel(array, *, highlevel=True, behavior=None):
     """
     Args:
         array: Array-like data (anything #ak.to_layout recognizes).
         highlevel (bool): If True, return an #ak.Array; otherwise, return
             a low-level #ak.contents.Content subclass.
         behavior (None or dict): Custom #ak.behavior for the output array, if
@@ -45,19 +47,19 @@
          7.7,
          8.8,
          9.9]
 
     Missing values are not eliminated by flattening. See #ak.flatten with
     `axis=None` for an equivalent function that eliminates the option type.
     """
-    with ak._errors.OperationErrorContext(
-        "ak.ravel",
-        {"array": array, "highlevel": highlevel, "behavior": behavior},
-    ):
-        return _impl(array, highlevel, behavior)
+    # Dispatch
+    yield (array,)
+
+    # Implementation
+    return _impl(array, highlevel, behavior)
 
 
 def _impl(array, highlevel, behavior):
     layout = ak.operations.to_layout(array, allow_record=False, allow_other=False)
 
     out = ak._do.remove_structure(layout, function_name="ak.ravel", drop_nones=False)
     assert isinstance(out, tuple) and all(
```

### Comparing `awkward-2.2.3/src/awkward/operations/ak_run_lengths.py` & `awkward-2.2.4/src/awkward/operations/ak_run_lengths.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("run_lengths",)
 import awkward as ak
 from awkward._backends.dispatch import backend_of
 from awkward._backends.numpy import NumpyBackend
 from awkward._behavior import behavior_of
+from awkward._dispatch import high_level_function
 from awkward._layout import wrap_layout
 from awkward._nplikes.numpylike import NumpyMetadata
 from awkward._nplikes.shape import unknown_length
 
 np = NumpyMetadata.instance()
 cpu = NumpyBackend.instance()
 
 
+@high_level_function
 def run_lengths(array, *, highlevel=True, behavior=None):
     """
     Args:
         array: Array-like data (anything #ak.to_layout recognizes).
         highlevel (bool): If True, return an #ak.Array; otherwise, return
             a low-level #ak.contents.Content subclass.
         behavior (None or dict): Custom #ak.behavior for the output array, if
@@ -82,23 +84,19 @@
         >>> counts = ak.flatten(ak.run_lengths(sorted.x), axis=None)
         >>> ak.unflatten(sorted, counts, axis=-1).show()
         [[[{x: 1, y: 1.1}, {x: 1, y: 1.1}], [{x: 2, y: 2.2}]],
          [[{x: 1, y: 1.1}], [{x: 2, y: 2.2}], [{x: 3, y: 3.3}]]]
 
     See also #ak.num, #ak.argsort, #ak.unflatten.
     """
-    with ak._errors.OperationErrorContext(
-        "ak.run_lengths",
-        {
-            "array": array,
-            "highlevel": highlevel,
-            "behavior": behavior,
-        },
-    ):
-        return _impl(array, highlevel, behavior)
+    # Dispatch
+    yield (array,)
+
+    # Implementation
+    return _impl(array, highlevel, behavior)
 
 
 def _impl(array, highlevel, behavior):
     backend = backend_of(array, default=cpu)
 
     def lengths_of(data, offsets):
         if backend.nplike.is_own_array(data):
```

### Comparing `awkward-2.2.3/src/awkward/operations/ak_singletons.py` & `awkward-2.2.4/src/awkward/operations/ak_singletons.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("singletons",)
 import awkward as ak
 from awkward._behavior import behavior_of
+from awkward._dispatch import high_level_function
 from awkward._errors import AxisError
 from awkward._layout import maybe_posaxis, wrap_layout
 from awkward._nplikes.numpylike import NumpyMetadata
 from awkward._regularize import is_integer, regularize_axis
 
 np = NumpyMetadata.instance()
 
 
+@high_level_function
 def singletons(array, axis=0, *, highlevel=True, behavior=None):
     """
     Args:
         array: Array-like data (anything #ak.to_layout recognizes).
         axis (int): The dimension at which this operation is applied. The
             outermost dimension is `0`, followed by `1`, etc., and negative
             values count backward from the innermost: `-1` is the innermost
@@ -37,19 +39,19 @@
          [],
          [],
          [4.4],
          [5.5]]
 
     See #ak.firsts to invert this function.
     """
-    with ak._errors.OperationErrorContext(
-        "ak.singletons",
-        {"array": array, "axis": axis, "highlevel": highlevel, "behavior": behavior},
-    ):
-        return _impl(array, axis, highlevel, behavior)
+    # Dispatch
+    yield (array,)
+
+    # Implementation
+    return _impl(array, axis, highlevel, behavior)
 
 
 def _impl(array, axis, highlevel, behavior):
     axis = regularize_axis(axis)
     layout = ak.operations.to_layout(array)
     behavior = behavior_of(array, behavior=behavior)
```

### Comparing `awkward-2.2.3/src/awkward/operations/ak_softmax.py` & `awkward-2.2.4/src/awkward/operations/ak_softmax.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("softmax",)
 import awkward as ak
 from awkward._behavior import behavior_of
+from awkward._dispatch import high_level_function
 from awkward._nplikes import ufuncs
 from awkward._nplikes.numpylike import NumpyMetadata
 from awkward._regularize import regularize_axis
 
 np = NumpyMetadata.instance()
 
 
+@high_level_function
 def softmax(x, axis=None, *, keepdims=False, mask_identity=False):
     """
     Args:
         x: The data on which to compute the softmax (anything #ak.to_layout recognizes).
         axis (None or int): If None, combine all values from the array into
             a single scalar result; if an int, group by that axis: `0` is the
             outermost, `1` is the first level of nested lists, etc., and
@@ -38,24 +40,19 @@
 
         np.exp(x) / ak.sum(np.exp(x))
 
     See #ak.sum for a complete description of handling nested lists and
     missing values (None) in reducers, and #ak.mean for an example with another
     non-reducer.
     """
-    with ak._errors.OperationErrorContext(
-        "ak.softmax",
-        {
-            "x": x,
-            "axis": axis,
-            "keepdims": keepdims,
-            "mask_identity": mask_identity,
-        },
-    ):
-        return _impl(x, axis, keepdims, mask_identity)
+    # Dispatch
+    yield (x,)
+
+    # Implementation
+    return _impl(x, axis, keepdims, mask_identity)
 
 
 def _impl(x, axis, keepdims, mask_identity):
     axis = regularize_axis(axis)
     behavior = behavior_of(x)
     x = ak.highlevel.Array(
         ak.operations.to_layout(x, allow_record=False, allow_other=False),
```

### Comparing `awkward-2.2.3/src/awkward/operations/ak_sort.py` & `awkward-2.2.4/src/awkward/operations/ak_sort.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("sort",)
 import awkward as ak
 from awkward._connect.numpy import UNSUPPORTED
+from awkward._dispatch import high_level_function
 from awkward._layout import wrap_layout
 from awkward._nplikes.numpylike import NumpyMetadata
 from awkward._regularize import regularize_axis
 
 np = NumpyMetadata.instance()
 
 
+@high_level_function
 def sort(array, axis=-1, *, ascending=True, stable=True, highlevel=True, behavior=None):
     """
     Args:
         array: Array-like data (anything #ak.to_layout recognizes).
         axis (int): The dimension at which this operation is applied. The
             outermost dimension is `0`, followed by `1`, etc., and negative
             values count backward from the innermost: `-1` is the innermost
@@ -30,26 +32,19 @@
     Returns a sorted array.
 
     For example,
 
         >>> ak.sort(ak.Array([[7, 5, 7], [], [2], [8, 2]]))
         <Array [[5, 7, 7], [], [2], [2, 8]] type='4 * var * int64'>
     """
-    with ak._errors.OperationErrorContext(
-        "ak.sort",
-        {
-            "array": array,
-            "axis": axis,
-            "ascending": ascending,
-            "stable": stable,
-            "highlevel": highlevel,
-            "behavior": behavior,
-        },
-    ):
-        return _impl(array, axis, ascending, stable, highlevel, behavior)
+    # Dispatch
+    yield (array,)
+
+    # Implementation
+    return _impl(array, axis, ascending, stable, highlevel, behavior)
 
 
 def _impl(array, axis, ascending, stable, highlevel, behavior):
     axis = regularize_axis(axis)
     layout = ak.operations.to_layout(array, allow_record=False, allow_other=False)
     out = ak._do.sort(layout, axis, ascending, stable)
     return wrap_layout(out, behavior, highlevel, like=array)
```

### Comparing `awkward-2.2.3/src/awkward/operations/ak_std.py` & `awkward-2.2.4/src/awkward/operations/ak_std.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,23 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("std",)
 import awkward as ak
 from awkward._behavior import behavior_of
 from awkward._connect.numpy import UNSUPPORTED
+from awkward._dispatch import high_level_function
 from awkward._layout import maybe_posaxis
 from awkward._nplikes import ufuncs
 from awkward._nplikes.numpylike import NumpyMetadata
 from awkward._regularize import regularize_axis
 
 np = NumpyMetadata.instance()
 
 
-def std(
-    x,
-    weight=None,
-    ddof=0,
-    axis=None,
-    *,
-    keepdims=False,
-    mask_identity=False,
-):
+@high_level_function
+def std(x, weight=None, ddof=0, axis=None, *, keepdims=False, mask_identity=False):
     """
     Args:
         x: The data on which to compute the standard deviation (anything #ak.to_layout recognizes).
         weight: Data that can be broadcasted to `x` to give each value a
             weight. Weighting values equally is the same as no weights;
             weighting some values higher increases the significance of those
             values. Weights can be zero or negative.
@@ -59,37 +53,23 @@
 
     See #ak.sum for a complete description of handling nested lists and
     missing values (None) in reducers, and #ak.mean for an example with another
     non-reducer.
 
     See also #ak.nanstd.
     """
-    with ak._errors.OperationErrorContext(
-        "ak.std",
-        {
-            "x": x,
-            "weight": weight,
-            "ddof": ddof,
-            "axis": axis,
-            "keepdims": keepdims,
-            "mask_identity": mask_identity,
-        },
-    ):
-        return _impl(x, weight, ddof, axis, keepdims, mask_identity)
-
-
-def nanstd(
-    x,
-    weight=None,
-    ddof=0,
-    axis=None,
-    *,
-    keepdims=False,
-    mask_identity=True,
-):
+    # Dispatch
+    yield x, weight
+
+    # Implementation
+    return _impl(x, weight, ddof, axis, keepdims, mask_identity)
+
+
+@high_level_function
+def nanstd(x, weight=None, ddof=0, axis=None, *, keepdims=False, mask_identity=True):
     """
     Args:
         x: The data on which to compute the standard deviation (anything #ak.to_layout recognizes).
         weight: Data that can be broadcasted to `x` to give each value a
             weight. Weighting values equally is the same as no weights;
             weighting some values higher increases the significance of those
             values. Weights can be zero or negative.
@@ -116,30 +96,29 @@
 
         ak.std(ak.nan_to_none(array))
 
     with all other arguments unchanged.
 
     See also #ak.std.
     """
-    with ak._errors.OperationErrorContext(
-        "ak.nanstd",
-        {
-            "x": x,
-            "weight": weight,
-            "ddof": ddof,
-            "axis": axis,
-            "keepdims": keepdims,
-            "mask_identity": mask_identity,
-        },
-    ):
-        x = ak.operations.ak_nan_to_none._impl(x, False, None)
-        if weight is not None:
-            weight = ak.operations.ak_nan_to_none._impl(weight, False, None)
+    # Dispatch
+    yield x, weight
 
-        return _impl(x, weight, ddof, axis, keepdims, mask_identity)
+    # Implementation
+    if weight is not None:
+        weight = ak.operations.ak_nan_to_none._impl(weight, False, None)
+
+    return _impl(
+        ak.operations.ak_nan_to_none._impl(x, False, None),
+        weight,
+        ddof,
+        axis,
+        keepdims,
+        mask_identity,
+    )
 
 
 def _impl(x, weight, ddof, axis, keepdims, mask_identity):
     axis = regularize_axis(axis)
     behavior = behavior_of(x, weight)
     x = ak.highlevel.Array(
         ak.operations.to_layout(x, allow_record=False, allow_other=False),
```

### Comparing `awkward-2.2.3/src/awkward/operations/ak_strings_astype.py` & `awkward-2.2.4/src/awkward/operations/ak_with_name.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,81 +1,73 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
-__all__ = ("strings_astype",)
+__all__ = ("with_name",)
 import awkward as ak
 from awkward._behavior import behavior_of
+from awkward._dispatch import high_level_function
 from awkward._layout import wrap_layout
-from awkward._nplikes.numpy import Numpy
 from awkward._nplikes.numpylike import NumpyMetadata
 
 np = NumpyMetadata.instance()
-numpy = Numpy.instance()
 
 
-def strings_astype(array, to, *, highlevel=True, behavior=None):
+@high_level_function
+def with_name(array, name, *, highlevel=True, behavior=None):
     """
     Args:
         array: Array-like data (anything #ak.to_layout recognizes).
-        to (dtype or dtype specifier): Type to convert the strings into.
+        name (str or None): Name to give to the records or tuples; this assigns
+            the `"__record__"` parameter. If None, any existing name is unset.
         highlevel (bool): If True, return an #ak.Array; otherwise, return
             a low-level #ak.contents.Content subclass.
         behavior (None or dict): Custom #ak.behavior for the output array, if
             high-level.
 
-    Converts all strings in the array to a new type, leaving the structure
-    untouched.
-
-    For example,
+    Returns an #ak.Array or #ak.Record (or low-level equivalent, if
+    `highlevel=False`) with a new name. This function does not change the
+    array in-place. If the new name is None, then an array without a name is
+    returned.
+
+    The records or tuples may be nested within multiple levels of nested lists.
+    If records are nested within records, only the outermost are affected.
+
+    Setting the `"__record__"` parameter makes it possible to add behaviors
+    to the data; see #ak.Array and #ak.behavior for a more complete
+    description.
+    """
+    # Dispatch
+    yield (array,)
 
-        >>> array = ak.Array(["1", "2", "    3    ", "00004", "-5"])
-        >>> ak.strings_astype(array, np.int32)
-        <Array [1, 2, 3, 4, -5] type='5 * int32'>
+    # Implementation
+    return _impl(array, name, highlevel, behavior)
 
-    and
 
-        >>> array = ak.Array(["1.1", "2.2", "    3.3    ", "00004.4", "-5.5"])
-        >>> ak.strings_astype(array, np.float64)
-        <Array [1.1, 2.2, 3.3, 4.4, -5.5] type='5 * float64'>
+def _impl(array, name, highlevel, behavior):
+    behavior = behavior_of(array, behavior=behavior)
+    layout = ak.operations.to_layout(array)
 
-    and finally,
+    def action(layout, **ignore):
+        if isinstance(layout, ak.contents.RecordArray):
+            return ak.contents.RecordArray(
+                layout._contents,
+                layout._fields,
+                layout._length,
+                parameters={**layout.parameters, "__record__": name},
+            )
+        else:
+            return None
 
-        >>> array = ak.Array([["1.1", "2.2", "    3.3    "], [], ["00004.4", "-5.5"]])
-        >>> ak.strings_astype(array, np.float64)
-        <Array [[1.1, 2.2, 3.3], [], [4.4, -5.5]] type='3 * var * float64'>
+    out = ak._do.recursively_apply(layout, action, behavior)
 
-    See also #ak.numbers_astype.
-    """
-    with ak._errors.OperationErrorContext(
-        "ak.strings_astype",
-        {"array": array, "to": to, "highlevel": highlevel, "behavior": behavior},
-    ):
-        return _impl(array, to, highlevel, behavior)
-
-
-def _impl(array, to, highlevel, behavior):
-    to_dtype = np.dtype(to)
-
-    def action(layout, **kwargs):
-        if layout.is_list and (
-            layout.parameter("__array__") == "string"
-            or layout.parameter("__array__") == "bytestring"
-        ):
-            layout = ak.operations.without_parameters(
-                layout, highlevel=False, behavior=behavior
-            )
-            max_length = ak.operations.max(ak.operations.num(layout, behavior=behavior))
-            regulararray = ak._do.pad_none(layout, max_length, 1)
-            maskedarray = ak.operations.to_numpy(regulararray, allow_missing=True)
-            npstrings = maskedarray.data
-            if maskedarray.mask is not False:
-                npstrings[maskedarray.mask] = 0
-            npnumbers = numpy.astype(
-                numpy.reshape(npstrings, (-1,)).view("<S" + str(max_length)),
-                dtype=to_dtype,
+    def action2(layout, **ignore):
+        if layout.is_union:
+            return ak.contents.UnionArray.simplified(
+                layout._tags,
+                layout._index,
+                layout._contents,
+                parameters=layout._parameters,
             )
-            return ak.contents.NumpyArray(npnumbers)
         else:
             return None
 
-    layout = ak.operations.to_layout(array, allow_record=False, allow_other=False)
-    behavior = behavior_of(array, behavior=behavior)
-    out = ak._do.recursively_apply(layout, action, behavior)
-    return wrap_layout(out, behavior, highlevel)
+    out2 = ak._do.recursively_apply(out, action2, behavior)
+
+    return wrap_layout(out2, behavior, highlevel)
```

### Comparing `awkward-2.2.3/src/awkward/operations/ak_sum.py` & `awkward-2.2.4/src/awkward/operations/ak_sum.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("sum",)
 import awkward as ak
 from awkward._behavior import behavior_of
 from awkward._connect.numpy import UNSUPPORTED
+from awkward._dispatch import high_level_function
 from awkward._layout import wrap_layout
 from awkward._nplikes.numpylike import NumpyMetadata
 from awkward._regularize import regularize_axis
 
 np = NumpyMetadata.instance()
 
 
+@high_level_function
 def sum(
     array,
     axis=None,
     *,
     keepdims=False,
     mask_identity=False,
     highlevel=True,
@@ -191,28 +193,22 @@
 
     The third list is reduced to `0` if `mask_identity=False` because `0` is
     the identity of addition, but it is reduced to None if
     `mask_identity=True`.
 
     See also #ak.nansum.
     """
-    with ak._errors.OperationErrorContext(
-        "ak.sum",
-        {
-            "array": array,
-            "axis": axis,
-            "keepdims": keepdims,
-            "mask_identity": mask_identity,
-            "highlevel": highlevel,
-            "behavior": behavior,
-        },
-    ):
-        return _impl(array, axis, keepdims, mask_identity, highlevel, behavior)
+    # Dispatch
+    yield (array,)
 
+    # Implementation
+    return _impl(array, axis, keepdims, mask_identity, highlevel, behavior)
 
+
+@high_level_function
 def nansum(
     array,
     axis=None,
     *,
     keepdims=False,
     mask_identity=False,
     highlevel=True,
@@ -244,28 +240,26 @@
 
         ak.sum(ak.nan_to_none(array))
 
     with all other arguments unchanged.
 
     See also #ak.sum.
     """
-    with ak._errors.OperationErrorContext(
-        "ak.nansum",
-        {
-            "array": array,
-            "axis": axis,
-            "keepdims": keepdims,
-            "mask_identity": mask_identity,
-            "highlevel": highlevel,
-            "behavior": behavior,
-        },
-    ):
-        array = ak.operations.ak_nan_to_none._impl(array, False, None)
+    # Dispatch
+    yield (array,)
 
-        return _impl(array, axis, keepdims, mask_identity, highlevel, behavior)
+    # Implementation
+    return _impl(
+        ak.operations.ak_nan_to_none._impl(array, False, None),
+        axis,
+        keepdims,
+        mask_identity,
+        highlevel,
+        behavior,
+    )
 
 
 def _impl(array, axis, keepdims, mask_identity, highlevel, behavior):
     axis = regularize_axis(axis)
     layout = ak.operations.to_layout(array, allow_record=False, allow_other=False)
     behavior = behavior_of(array, behavior=behavior)
     reducer = ak._reducers.Sum()
```

### Comparing `awkward-2.2.3/src/awkward/operations/ak_to_arrow.py` & `awkward-2.2.4/src/awkward/operations/ak_to_arrow.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("to_arrow",)
-
 import awkward as ak
+from awkward._dispatch import high_level_function
 from awkward._nplikes.numpylike import NumpyMetadata
 
 np = NumpyMetadata.instance()
 
 
+@high_level_function
 def to_arrow(
     array,
     *,
     list_to32=False,
     string_to32=False,
     bytestring_to32=False,
     emptyarray_to=None,
@@ -60,37 +61,28 @@
     data type (high-level #ak.types.Type, though not the low-level #ak.forms.Form),
     even through Parquet, making Parquet a good way to save Awkward Arrays for later
     use. If any third-party tools don't recognize Arrow's extension arrays, set this
     option to False for plain Arrow arrays.
 
     See also #ak.from_arrow, #ak.to_arrow_table, #ak.to_parquet, #ak.from_arrow_schema.
     """
-    with ak._errors.OperationErrorContext(
-        "ak.to_arrow",
-        {
-            "array": array,
-            "list_to32": list_to32,
-            "string_to32": string_to32,
-            "bytestring_to32": bytestring_to32,
-            "emptyarray_to": emptyarray_to,
-            "categorical_as_dictionary": categorical_as_dictionary,
-            "extensionarray": extensionarray,
-            "count_nulls": count_nulls,
-        },
-    ):
-        return _impl(
-            array,
-            list_to32,
-            string_to32,
-            bytestring_to32,
-            emptyarray_to,
-            categorical_as_dictionary,
-            extensionarray,
-            count_nulls,
-        )
+    # Dispatch
+    yield (array,)
+
+    # Implementation
+    return _impl(
+        array,
+        list_to32,
+        string_to32,
+        bytestring_to32,
+        emptyarray_to,
+        categorical_as_dictionary,
+        extensionarray,
+        count_nulls,
+    )
 
 
 def _impl(
     array,
     list_to32,
     string_to32,
     bytestring_to32,
```

### Comparing `awkward-2.2.3/src/awkward/operations/ak_to_arrow_table.py` & `awkward-2.2.4/src/awkward/operations/ak_to_arrow_table.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("to_arrow_table",)
-
 import json
 
 import awkward as ak
+from awkward._dispatch import high_level_function
 from awkward._nplikes.numpylike import NumpyMetadata
 
 np = NumpyMetadata.instance()
 
 
+@high_level_function
 def to_arrow_table(
     array,
     *,
     list_to32=False,
     string_to32=False,
     bytestring_to32=False,
     emptyarray_to=None,
@@ -61,37 +62,28 @@
     data type (high-level #ak.types.Type, though not the low-level #ak.forms.Form),
     even through Parquet, making Parquet a good way to save Awkward Arrays for later
     use. If any third-party tools don't recognize Arrow's extension arrays, set this
     option to False for plain Arrow arrays.
 
     See also #ak.from_arrow, #ak.to_arrow, #ak.to_parquet.
     """
-    with ak._errors.OperationErrorContext(
-        "ak.to_arrow_table",
-        {
-            "array": array,
-            "list_to32": list_to32,
-            "string_to32": string_to32,
-            "bytestring_to32": bytestring_to32,
-            "emptyarray_to": emptyarray_to,
-            "categorical_as_dictionary": categorical_as_dictionary,
-            "extensionarray": extensionarray,
-            "count_nulls": count_nulls,
-        },
-    ):
-        return _impl(
-            array,
-            list_to32,
-            string_to32,
-            bytestring_to32,
-            emptyarray_to,
-            categorical_as_dictionary,
-            extensionarray,
-            count_nulls,
-        )
+    # Dispatch
+    yield (array,)
+
+    # Implementation
+    return _impl(
+        array,
+        list_to32,
+        string_to32,
+        bytestring_to32,
+        emptyarray_to,
+        categorical_as_dictionary,
+        extensionarray,
+        count_nulls,
+    )
 
 
 def _impl(
     array,
     list_to32,
     string_to32,
     bytestring_to32,
```

### Comparing `awkward-2.2.3/src/awkward/operations/ak_to_backend.py` & `awkward-2.2.4/src/awkward/operations/ak_to_backend.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("to_backend",)
 import awkward as ak
 from awkward._backends.dispatch import regularize_backend
 from awkward._behavior import behavior_of
+from awkward._dispatch import high_level_function
 from awkward._layout import wrap_layout
 from awkward._nplikes.numpylike import NumpyMetadata
 
 np = NumpyMetadata.instance()
 
 
+@high_level_function
 def to_backend(array, backend, *, highlevel=True, behavior=None):
     """
     Args:
         array: Array-like data (anything #ak.to_layout recognizes).
         backend (`"cpu"`, `"cuda"`, or `"jax"`): If `"cpu"`, the array structure is
             recursively copied (if need be) to main memory for use with
             the default Numpy backend; if `"cuda"`, the structure is copied
@@ -44,24 +46,19 @@
 
     or
 
         conda install -c conda-forge jax
 
     See #ak.kernels.
     """
-    with ak._errors.OperationErrorContext(
-        "ak.to_backend",
-        {
-            "array": array,
-            "backend": backend,
-            "highlevel": highlevel,
-            "behavior": behavior,
-        },
-    ):
-        return _impl(array, backend, highlevel, behavior)
+    # Dispatch
+    yield (array,)
+
+    # Implementation
+    return _impl(array, backend, highlevel, behavior)
 
 
 def _impl(array, backend, highlevel, behavior):
     layout = ak.operations.to_layout(
         array,
         allow_record=True,
         allow_other=True,
```

### Comparing `awkward-2.2.3/src/awkward/operations/ak_to_buffers.py` & `awkward-2.2.4/src/awkward/operations/ak_to_buffers.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("to_buffers",)
-
 import awkward as ak
 from awkward._backends.dispatch import regularize_backend
+from awkward._dispatch import high_level_function
 from awkward._nplikes.numpylike import NumpyMetadata
 
 np = NumpyMetadata.instance()
 
 
+@high_level_function
 def to_buffers(
     array,
     container=None,
     buffer_key="{form_key}-{attribute}",
     form_key="node{id}",
     *,
     id_start=0,
@@ -115,29 +116,19 @@
         <Array [[1, 2, 3], [], [4, 5]] type='3 * var * int64'>
 
     If you intend to use this function for saving data, you may want to pack it
     first with #ak.to_packed.
 
     See also #ak.from_buffers and #ak.to_packed.
     """
-    with ak._errors.OperationErrorContext(
-        "ak.to_buffers",
-        {
-            "array": array,
-            "container": container,
-            "buffer_key": buffer_key,
-            "form_key": form_key,
-            "id_start": id_start,
-            "backend": backend,
-            "byteorder": byteorder,
-        },
-    ):
-        return _impl(
-            array, container, buffer_key, form_key, id_start, backend, byteorder
-        )
+    # Dispatch
+    yield (array,)
+
+    # Implementation
+    return _impl(array, container, buffer_key, form_key, id_start, backend, byteorder)
 
 
 def _impl(array, container, buffer_key, form_key, id_start, backend, byteorder):
     layout = ak.operations.to_layout(array, allow_record=False, allow_other=False)
 
     if backend is not None:
         backend = regularize_backend(backend)
```

### Comparing `awkward-2.2.3/src/awkward/operations/ak_to_categorical.py` & `awkward-2.2.4/src/awkward/operations/ak_to_categorical.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("to_categorical",)
 import awkward as ak
 from awkward._behavior import behavior_of
+from awkward._dispatch import high_level_function
 from awkward._layout import wrap_layout
 from awkward._nplikes.numpy import Numpy
 from awkward._nplikes.numpylike import NumpyMetadata
 
 np = NumpyMetadata.instance()
 numpy = Numpy.instance()
 
 
+@high_level_function
 def to_categorical(array, *, highlevel=True, behavior=None):
     """
     Args:
         array: Array-like data (anything #ak.to_layout recognizes).
         highlevel (bool): If True, return an #ak.Array; otherwise, return
             a low-level #ak.contents.Content subclass.
         behavior (None or dict): Custom #ak.behavior for the output array, if
@@ -77,19 +79,19 @@
 
     The check for uniqueness is currently implemented in a Python loop, so
     conversion to categorical should be regarded as expensive. (This can
     change, but it would always be an _n log(n)_ operation.)
 
     See also #ak.is_categorical, #ak.categories, #ak.from_categorical.
     """
-    with ak._errors.OperationErrorContext(
-        "ak.to_categorical",
-        {"array": array, "highlevel": highlevel, "behavior": behavior},
-    ):
-        return _impl(array, highlevel, behavior)
+    # Dispatch
+    yield (array,)
+
+    # Implementation
+    return _impl(array, highlevel, behavior)
 
 
 def _impl(array, highlevel, behavior):
     def action(layout, **kwargs):
         if layout.purelist_depth == 1:
             if layout.is_indexed and layout.is_option:
                 content = layout.content
```

### Comparing `awkward-2.2.3/src/awkward/operations/ak_to_cupy.py` & `awkward-2.2.4/src/awkward/operations/ak_to_cupy.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("to_cupy",)
-
 import awkward as ak
 from awkward._backends.cupy import CupyBackend
+from awkward._dispatch import high_level_function
 
 
+@high_level_function
 def to_cupy(array):
     """
     Args:
         array: Array-like data (anything #ak.to_layout recognizes).
 
     Converts `array` (many types supported) into a CuPy array, if possible.
 
@@ -18,19 +19,19 @@
 
     Otherwise, the function raises an error.
 
     If `array` is a scalar, it is converted into a CuPy scalar.
 
     See also #ak.from_cupy and #ak.to_numpy.
     """
-    with ak._errors.OperationErrorContext(
-        "ak.to_cupy",
-        {"array": array},
-    ):
-        return _impl(array)
+    # Dispatch
+    yield (array,)
+
+    # Implementation
+    return _impl(array)
 
 
 def _impl(array):
     layout = ak.to_layout(array, allow_record=False)
 
     backend = CupyBackend.instance()
     cupy_layout = layout.to_backend(backend)
```

### Comparing `awkward-2.2.3/src/awkward/operations/ak_to_dataframe.py` & `awkward-2.2.4/src/awkward/operations/ak_to_dataframe.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("to_dataframe",)
-
 import awkward as ak
+from awkward._dispatch import high_level_function
 from awkward._nplikes.numpy import Numpy
 from awkward._nplikes.numpylike import NumpyMetadata
 
 numpy = Numpy.instance()
 np = NumpyMetadata.instance()
 
 
+def _default_levelname(index: int) -> str:
+    return "sub" * index + "entry"
+
+
+@high_level_function
 def to_dataframe(
-    array, *, how="inner", levelname=lambda i: "sub" * i + "entry", anonymous="values"
+    array, *, how="inner", levelname=_default_levelname, anonymous="values"
 ):
     """
     Args:
         array: Array-like data (anything #ak.to_layout recognizes).
         how (None or str): Passed to
             [pd.merge](https://pandas.pydata.org/pandas-docs/version/1.0.3/reference/api/pandas.merge.html)
             to combine DataFrames for each multiplicity into one DataFrame. If
@@ -118,24 +123,19 @@
               1         2.0  NaN
               2         3.0  NaN
         4     0         1.0  NaN
               1         2.0  NaN
               2         3.0  NaN
               3         4.0  NaN
     """
-    with ak._errors.OperationErrorContext(
-        "ak.to_dataframe",
-        {
-            "array": array,
-            "how": how,
-            "levelname": levelname,
-            "anonymous": anonymous,
-        },
-    ):
-        return _impl(array, how, levelname, anonymous)
+    # Dispatch
+    yield (array,)
+
+    # Implementation
+    return _impl(array, how, levelname, anonymous)
 
 
 def _impl(array, how, levelname, anonymous):
     try:
         import pandas
     except ImportError as err:
         raise ImportError(
```

### Comparing `awkward-2.2.3/src/awkward/operations/ak_to_jax.py` & `awkward-2.2.4/src/awkward/operations/ak_to_jax.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("to_jax",)
-
 import awkward as ak
 from awkward._backends.jax import JaxBackend
+from awkward._dispatch import high_level_function
 
 
+@high_level_function
 def to_jax(array):
     """
     Args:
         array: Array-like data (anything #ak.to_layout recognizes).
 
     Converts `array` (many types supported) into a JAX Device Array, if possible.
 
@@ -18,19 +19,19 @@
 
     Otherwise, the function raises an error.
 
     If `array` is a scalar, it is converted into a JAX scalar.
 
     See also #ak.from_jax and #ak.to_numpy.
     """
-    with ak._errors.OperationErrorContext(
-        "ak.to_jax",
-        {"array": array},
-    ):
-        return _impl(array)
+    # Dispatch
+    yield (array,)
+
+    # Implementation
+    return _impl(array)
 
 
 def _impl(array):
     layout = ak.to_layout(array, allow_record=False)
 
     backend = JaxBackend.instance()
     numpy_layout = layout.to_backend(backend)
```

### Comparing `awkward-2.2.3/src/awkward/operations/ak_to_json.py` & `awkward-2.2.4/src/awkward/operations/ak_to_json.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,21 +5,23 @@
 from os import PathLike, fsdecode
 from urllib.parse import urlparse
 
 from awkward_cpp.lib import _ext
 
 import awkward as ak
 from awkward._behavior import behavior_of
+from awkward._dispatch import high_level_function
 from awkward._nplikes.numpy import Numpy
 from awkward._nplikes.numpylike import NumpyMetadata
 
 np = NumpyMetadata.instance()
 numpy = Numpy.instance()
 
 
+@high_level_function
 def to_json(
     array,
     file=None,
     *,
     line_delimited=False,
     num_indent_spaces=None,
     num_readability_spaces=0,
@@ -107,43 +109,31 @@
 
     Other non-serializable types are only possible through custom behaviors that
     override `__getitem__` (which might return arbitrary Python objects). Use
     `convert_other` to detect these types and convert them.
 
     See also #ak.from_json.
     """
-    with ak._errors.OperationErrorContext(
-        "ak.to_json",
-        {
-            "array": array,
-            "file": file,
-            "line_delimited": line_delimited,
-            "num_indent_spaces": num_indent_spaces,
-            "num_readability_spaces": num_readability_spaces,
-            "nan_string": nan_string,
-            "posinf_string": posinf_string,
-            "neginf_string": neginf_string,
-            "complex_record_fields": complex_record_fields,
-            "convert_bytes": convert_bytes,
-            "convert_other": convert_other,
-        },
-    ):
-        return _impl(
-            array,
-            file,
-            line_delimited,
-            num_indent_spaces,
-            num_readability_spaces,
-            nan_string,
-            posinf_string,
-            neginf_string,
-            complex_record_fields,
-            convert_bytes,
-            convert_other,
-        )
+    # Dispatch
+    yield (array,)
+
+    # Implementation
+    return _impl(
+        array,
+        file,
+        line_delimited,
+        num_indent_spaces,
+        num_readability_spaces,
+        nan_string,
+        posinf_string,
+        neginf_string,
+        complex_record_fields,
+        convert_bytes,
+        convert_other,
+    )
 
 
 def _impl(
     array,
     file,
     line_delimited,
     num_indent_spaces,
```

### Comparing `awkward-2.2.3/src/awkward/operations/ak_to_layout.py` & `awkward-2.2.4/src/awkward/operations/ak_to_layout.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("to_layout",)
-
 from collections.abc import Iterable
 
 from awkward_cpp.lib import _ext
 
 import awkward as ak
-from awkward import _errors
 from awkward._backends.typetracer import TypeTracerBackend
+from awkward._dispatch import high_level_function
 from awkward._nplikes.cupy import Cupy
 from awkward._nplikes.jax import Jax
 from awkward._nplikes.numpy import Numpy
 from awkward._nplikes.numpylike import NumpyMetadata
 from awkward._nplikes.typetracer import TypeTracer
 
 np = NumpyMetadata.instance()
 numpy = Numpy.instance()
 
 
+@high_level_function
 def to_layout(array, *, allow_record=True, allow_other=False, regulararray=True):
     """
     Args:
         array: Array-like data. May be a high level #ak.Array, #ak.Record (if `allow_record`),
             #ak.ArrayBuilder, or low-level #ak.contents.Content, #ak.record.Record (if `allow_record`),
             or a supported backend array (NumPy `ndarray`, CuPy `ndarray`,
             JAX DeviceArray), data-less TypeTracer, Arrow object, or an arbitrary Python
@@ -37,24 +37,19 @@
     Records) into a #ak.contents.Content and maybe #ak.record.Record or
     other types.
 
     This function is usually used to sanitize inputs for other functions; it
     would rarely be used in a data analysis because #ak.contents.Content and
     #ak.record.Record are lower-level than #ak.Array.
     """
-    with _errors.OperationErrorContext(
-        "ak.to_layout",
-        {
-            "array": array,
-            "allow_record": allow_record,
-            "allow_other": allow_other,
-            "regulararray": regulararray,
-        },
-    ):
-        return _impl(array, allow_record, allow_other, regulararray=regulararray)
+    # Dispatch
+    yield (array,)
+
+    # Implementation
+    return _impl(array, allow_record, allow_other, regulararray=regulararray)
 
 
 def _impl(array, allow_record, allow_other, regulararray):
     if isinstance(array, ak.contents.Content):
         return array
 
     elif isinstance(array, ak.record.Record):
```

### Comparing `awkward-2.2.3/src/awkward/operations/ak_to_list.py` & `awkward-2.2.4/src/awkward/operations/ak_to_list.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("to_list",)
-
 from collections.abc import Iterable, Mapping
 
 from awkward_cpp.lib import _ext
 
 import awkward as ak
+from awkward._dispatch import high_level_function
 from awkward._nplikes.numpylike import NumpyMetadata
 
 np = NumpyMetadata.instance()
 
 
+@high_level_function
 def to_list(array):
     """
     Args:
         array: Array-like data (anything #ak.to_layout recognizes).
 
     Converts `array` (many types supported, including all Awkward Arrays and
     Records) into Python objects. If `array` is not recognized as an array, it
@@ -34,19 +35,19 @@
       `"__string__"`: converted into str.
     * #ak.types.RecordArray without field names: converted into tuple.
     * #ak.types.RecordArray with field names: converted into dict.
     * #ak.types.UnionArray: Python data are naturally heterogeneous.
 
     See also #ak.from_iter and #ak.Array.tolist.
     """
-    with ak._errors.OperationErrorContext(
-        "ak.to_list",
-        {"array": array},
-    ):
-        return _impl(array)
+    # Dispatch
+    yield (array,)
+
+    # Implementation
+    return _impl(array)
 
 
 def _impl(array):
     if isinstance(
         array,
         (
             ak.highlevel.Array,
```

### Comparing `awkward-2.2.3/src/awkward/operations/ak_to_numpy.py` & `awkward-2.2.4/src/awkward/operations/ak_to_numpy.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("to_numpy",)
 import awkward as ak
 from awkward._backends.numpy import NumpyBackend
+from awkward._dispatch import high_level_function
 
 
+@high_level_function
 def to_numpy(array, *, allow_missing=True):
     """
     Args:
         array: Array-like data (anything #ak.to_layout recognizes).
         allow_missing (bool): allow missing (None) values.
 
     Converts `array` (many types supported, including all Awkward Arrays and
@@ -31,19 +33,19 @@
     If `allow_missing` is True; NumPy
     [masked arrays](https://docs.scipy.org/doc/numpy/reference/maskedarray.html)
     are a possible result; otherwise, missing values (None) cause this
     function to raise an error.
 
     See also #ak.from_numpy and #ak.to_cupy.
     """
-    with ak._errors.OperationErrorContext(
-        "ak.to_numpy",
-        {"array": array, "allow_missing": allow_missing},
-    ):
-        return _impl(array, allow_missing)
+    # Dispatch
+    yield (array,)
+
+    # Implementation
+    return _impl(array, allow_missing)
 
 
 def _impl(array, allow_missing):
     import numpy  # noqa: TID251
 
     with numpy.errstate(invalid="ignore"):
         layout = ak.to_layout(array, allow_record=False)
```

### Comparing `awkward-2.2.3/src/awkward/operations/ak_to_packed.py` & `awkward-2.2.4/src/awkward/operations/ak_to_packed.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("to_packed",)
 import awkward as ak
+from awkward._dispatch import high_level_function
 from awkward._layout import wrap_layout
 from awkward._nplikes.numpylike import NumpyMetadata
 
 np = NumpyMetadata.instance()
 
 
+@high_level_function
 def to_packed(array, *, highlevel=True, behavior=None):
     """
     Args:
         array: Array-like data (anything #ak.to_layout recognizes).
         highlevel (bool): If True, return an #ak.Array; otherwise, return
             a low-level #ak.contents.Content subclass.
         behavior (None or dict): Custom #ak.behavior for the output array, if
@@ -61,18 +63,18 @@
 
     Performing these operations will minimize the output size of data sent to
     #ak.to_buffers (though conversions through Arrow, #ak.to_arrow and
     #ak.to_parquet, do not need this because packing is part of that conversion).
 
     See also #ak.to_buffers.
     """
-    with ak._errors.OperationErrorContext(
-        "ak.to_packed",
-        {"array": array, "highlevel": highlevel, "behavior": behavior},
-    ):
-        return _impl(array, highlevel, behavior)
+    # Dispatch
+    yield (array,)
+
+    # Implementation
+    return _impl(array, highlevel, behavior)
 
 
 def _impl(array, highlevel, behavior):
     layout = ak.operations.to_layout(array, allow_record=True, allow_other=False)
     out = layout.to_packed()
     return wrap_layout(out, behavior, highlevel, like=array)
```

### Comparing `awkward-2.2.3/src/awkward/operations/ak_to_parquet.py` & `awkward-2.2.4/src/awkward/operations/ak_to_parquet.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("to_parquet",)
-
 from collections.abc import Mapping, Sequence
 from os import fsdecode
 
 import awkward as ak
+from awkward._dispatch import high_level_function
 from awkward._nplikes.numpylike import NumpyMetadata
 
 metadata = NumpyMetadata.instance()
 
 
+@high_level_function
 def to_parquet(
     array,
     destination,
     *,
     list_to32=False,
     string_to32=True,
     bytestring_to32=True,
@@ -166,14 +167,18 @@
     Parquet files can maintain the distinction between "option-type but no elements are
     missing" and "not option-type" at all levels, including the top level. However,
     there is no distinction between `?union[X, Y, Z]]` type and `union[?X, ?Y, ?Z]` type.
     Be aware of these type distinctions when passing data through Arrow or Parquet.
 
     See also #ak.to_arrow, which is used as an intermediate step.
     """
+    # Dispatch
+    yield (array,)
+
+    # Implementation
     import awkward._connect.pyarrow
 
     data = array
 
     pyarrow_parquet = awkward._connect.pyarrow.import_pyarrow_parquet("ak.to_parquet")
     fsspec = awkward._connect.pyarrow.import_fsspec("ak.to_parquet")
```

### Comparing `awkward-2.2.3/src/awkward/operations/ak_to_rdataframe.py` & `awkward-2.2.4/src/awkward/operations/ak_to_rdataframe.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("to_rdataframe",)
 from collections.abc import Mapping
 
 import awkward as ak
 from awkward._backends.numpy import NumpyBackend
+from awkward._dispatch import high_level_function
 
 cpu = NumpyBackend.instance()
 
 
+@high_level_function
 def to_rdataframe(arrays, *, flatlist_as_rvec=True):
     """
     Args:
         arrays (dict of arrays): Each value in this dict can be any array-like data
             that #ak.to_layout recognizes, but they must all have the same length.
         flatlist_as_rvec (bool): If True, lists of primitive types (numbers, booleans, etc.)
             are presented to C++ as `ROOT::RVec<primitive>`, but all other types use
@@ -36,22 +38,22 @@
         {'z': ndarray([ 8.7,  4.2, 16.2])}
 
         >>> ak.sum(x, axis=-1) + y.a + y.b[:, 0]
         <Array [8.7, 4.2, 16.2] type='3 * float64'>
 
     See also #ak.from_rdataframe.
     """
-    with ak._errors.OperationErrorContext(
-        "ak.to_rdataframe",
-        {"arrays": arrays},
-    ):
-        return _impl(
-            arrays,
-            flatlist_as_rvec=flatlist_as_rvec,
-        )
+    # Dispatch
+    yield arrays.values()
+
+    # Implementation
+    return _impl(
+        arrays,
+        flatlist_as_rvec=flatlist_as_rvec,
+    )
 
 
 def _impl(
     arrays,
     flatlist_as_rvec,
 ):
     import awkward._connect.rdataframe.to_rdataframe  # noqa: F401
```

### Comparing `awkward-2.2.3/src/awkward/operations/ak_to_regular.py` & `awkward-2.2.4/src/awkward/operations/ak_to_regular.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("to_regular",)
 import awkward as ak
 from awkward._behavior import behavior_of
+from awkward._dispatch import high_level_function
 from awkward._errors import AxisError
 from awkward._layout import maybe_posaxis, wrap_layout
 from awkward._nplikes.numpylike import NumpyMetadata
 from awkward._regularize import regularize_axis
 
 np = NumpyMetadata.instance()
 
 
+@high_level_function
 def to_regular(array, axis=1, *, highlevel=True, behavior=None):
     """
     Args:
         array: Array-like data (anything #ak.to_layout recognizes).
         axis (int or None): The dimension at which this operation is applied.
             The outermost dimension is `0`, followed by `1`, etc., and negative
             values count backward from the innermost: `-1` is the innermost
@@ -47,19 +49,19 @@
                 highlevel = True
                 behavior = None
             )
         Error details: cannot convert to RegularArray because subarray lengths are not regular
 
     See also #ak.from_regular.
     """
-    with ak._errors.OperationErrorContext(
-        "ak.to_regular",
-        {"array": array, "axis": axis, "highlevel": highlevel, "behavior": behavior},
-    ):
-        return _impl(array, axis, highlevel, behavior)
+    # Dispatch
+    yield (array,)
+
+    # Implementation
+    return _impl(array, axis, highlevel, behavior)
 
 
 def _impl(array, axis, highlevel, behavior):
     axis = regularize_axis(axis)
     layout = ak.operations.to_layout(array)
     behavior = behavior_of(array, behavior=behavior)
```

### Comparing `awkward-2.2.3/src/awkward/operations/ak_transform.py` & `awkward-2.2.4/src/awkward/operations/ak_transform.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,19 +2,21 @@
 __all__ = ("transform",)
 import copy
 
 import awkward as ak
 from awkward._backends.dispatch import backend_of
 from awkward._backends.numpy import NumpyBackend
 from awkward._behavior import behavior_of
+from awkward._dispatch import high_level_function
 from awkward._layout import wrap_layout
 
 cpu = NumpyBackend.instance()
 
 
+@high_level_function
 def transform(
     transformation,
     array,
     *more_arrays,
     depth_context=None,
     lateral_context=None,
     allow_records=True,
@@ -405,49 +407,34 @@
 
     `"none"`
         The output arrays will not be given parameters.
 
     See also: #ak.is_valid and #ak.valid_when to check the validity of transformed
     outputs.
     """
-    with ak._errors.OperationErrorContext(
-        "ak.transform",
-        {
-            "transformation": transformation,
-            "array": array,
-            "more_arrays": more_arrays,
-            "depth_context": depth_context,
-            "lateral_context": lateral_context,
-            "allow_records": allow_records,
-            "broadcast_parameters_rule": broadcast_parameters_rule,
-            "left_broadcast": left_broadcast,
-            "right_broadcast": right_broadcast,
-            "numpy_to_regular": numpy_to_regular,
-            "regular_to_jagged": regular_to_jagged,
-            "return_value": return_value,
-            "behavior": behavior,
-            "highlevel": highlevel,
-        },
-    ):
-        return _impl(
-            transformation,
-            array,
-            more_arrays,
-            depth_context,
-            lateral_context,
-            allow_records,
-            broadcast_parameters_rule,
-            left_broadcast,
-            right_broadcast,
-            numpy_to_regular,
-            regular_to_jagged,
-            return_value,
-            behavior,
-            highlevel,
-        )
+    # Dispatch
+    yield (array, *more_arrays)
+
+    # Implementation
+    return _impl(
+        transformation,
+        array,
+        more_arrays,
+        depth_context,
+        lateral_context,
+        allow_records,
+        broadcast_parameters_rule,
+        left_broadcast,
+        right_broadcast,
+        numpy_to_regular,
+        regular_to_jagged,
+        return_value,
+        behavior,
+        highlevel,
+    )
 
 
 def _impl(
     transformation,
     array,
     more_arrays,
     depth_context,
```

### Comparing `awkward-2.2.3/src/awkward/operations/ak_type.py` & `awkward-2.2.4/src/awkward/operations/ak_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,19 +3,21 @@
 import numbers
 from datetime import datetime, timedelta
 
 from awkward_cpp.lib import _ext
 
 import awkward as ak
 from awkward._behavior import behavior_of
+from awkward._dispatch import high_level_function
 from awkward._nplikes.numpylike import NumpyMetadata
 
 np = NumpyMetadata.instance()
 
 
+@high_level_function
 def type(array, *, behavior=None):
     """
     Args:
         array: Array-like data (anything #ak.to_layout recognizes).
         behavior (None or dict): Custom #ak.behavior for the output type, if
             high-level.
 
@@ -69,19 +71,19 @@
             var * int64
         ]
 
     but "union" is not a Datashape type-constructor. (Its syntax is
     similar to existing type-constructors, so it's a plausible addition
     to the language.)
     """
-    with ak._errors.OperationErrorContext(
-        "ak.type",
-        {"array": array, "behavior": behavior},
-    ):
-        return _impl(array, behavior)
+    # Dispatch
+    yield (array,)
+
+    # Implementation
+    return _impl(array, behavior)
 
 
 def _impl(array, behavior):
     behavior = behavior_of(array, behavior=behavior)
 
     if isinstance(array, _ext.ArrayBuilder):
         form = ak.forms.from_json(array.form())
```

### Comparing `awkward-2.2.3/src/awkward/operations/ak_unflatten.py` & `awkward-2.2.4/src/awkward/operations/ak_unflatten.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("unflatten",)
 import awkward as ak
 from awkward._behavior import behavior_of
+from awkward._dispatch import high_level_function
 from awkward._layout import maybe_posaxis, wrap_layout
 from awkward._nplikes.numpylike import NumpyMetadata
 from awkward._nplikes.shape import unknown_length
 from awkward._nplikes.typetracer import is_unknown_scalar
 from awkward._regularize import is_integer_like, regularize_axis
 
 np = NumpyMetadata.instance()
 
 
+@high_level_function
 def unflatten(array, counts, axis=0, *, highlevel=True, behavior=None):
     """
     Args:
         array: Array-like data (anything #ak.to_layout recognizes).
         counts (int or array): Number of elements the new level should have.
             If an integer, the new level will be regularly sized; otherwise,
             it will consist of variable-length lists with the given lengths.
@@ -70,25 +72,19 @@
         Error details: structure imposed by 'counts' does not fit in the array or partition at axis=1
 
     Also note that new lists created by this function cannot cross partitions
     (which is only possible at `axis=0`, anyway).
 
     See also #ak.num and #ak.flatten.
     """
-    with ak._errors.OperationErrorContext(
-        "ak.unflatten",
-        {
-            "array": array,
-            "counts": counts,
-            "axis": axis,
-            "highlevel": highlevel,
-            "behavior": behavior,
-        },
-    ):
-        return _impl(array, counts, axis, highlevel, behavior)
+    # Dispatch
+    yield (array,)
+
+    # Implementation
+    return _impl(array, counts, axis, highlevel, behavior)
 
 
 def _impl(array, counts, axis, highlevel, behavior):
     axis = regularize_axis(axis)
     layout = ak.operations.to_layout(
         array, allow_record=False, allow_other=False
     ).to_packed()
```

### Comparing `awkward-2.2.3/src/awkward/operations/ak_unzip.py` & `awkward-2.2.4/src/awkward/operations/ak_unzip.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("unzip",)
 import awkward as ak
 from awkward._behavior import behavior_of
+from awkward._dispatch import high_level_function
 from awkward._layout import wrap_layout
 from awkward._nplikes.numpylike import NumpyMetadata
 
 np = NumpyMetadata.instance()
 
 
+@high_level_function
 def unzip(array, *, highlevel=True, behavior=None):
     """
     Args:
         array: Array-like data (anything #ak.to_layout recognizes).
         highlevel (bool): If True, return an #ak.Array; otherwise, return
             a low-level #ak.contents.Content subclass.
         behavior (None or dict): Custom #ak.behavior for the output array, if
@@ -30,19 +32,19 @@
         ...                   {"x": 3.3, "y": [3, 3, 3]}])
         >>> x, y = ak.unzip(array)
         >>> x
         <Array [1.1, 2.2, 3.3] type='3 * float64'>
         >>> y
         <Array [[1], [2, 2], [3, 3, 3]] type='3 * var * int64'>
     """
-    with ak._errors.OperationErrorContext(
-        "ak.unzip",
-        {"array": array, "highlevel": highlevel, "behavior": behavior},
-    ):
-        return _impl(array, highlevel, behavior)
+    # Dispatch
+    yield (array,)
+
+    # Implementation
+    return _impl(array, highlevel, behavior)
 
 
 def _impl(array, highlevel, behavior):
     behavior = behavior_of(array, behavior=behavior)
     layout = ak.operations.to_layout(array, allow_record=True, allow_other=False)
     fields = ak.operations.fields(layout)
```

### Comparing `awkward-2.2.3/src/awkward/operations/ak_values_astype.py` & `awkward-2.2.4/src/awkward/operations/ak_values_astype.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("values_astype",)
 import awkward as ak
+from awkward._dispatch import high_level_function
 from awkward._layout import wrap_layout
 from awkward._nplikes.numpylike import NumpyMetadata
 
 np = NumpyMetadata.instance()
 
 
+@high_level_function
 def values_astype(array, to, *, including_unknown=False, highlevel=True, behavior=None):
     """
     Args:
         array: Array-like data (anything #ak.to_layout recognizes).
         to (dtype or dtype specifier): Type to convert the numbers into.
         including_unknown (bool): If True, the `unknown` type is considered
             a value type and is converted to the specified dtype; if False,
@@ -48,25 +50,19 @@
 
         >>> array = ak.Array([1567416600000])
         >>> ak.values_astype(array, np.dtype("M8[ms]"))
         <Array [2019-09-02T09:30:00.000] type='1 * datetime64[ms]['>
 
     See also #ak.strings_astype.
     """
-    with ak._errors.OperationErrorContext(
-        "ak.values_astype",
-        {
-            "array": array,
-            "to": to,
-            "including_unknown": including_unknown,
-            "highlevel": highlevel,
-            "behavior": behavior,
-        },
-    ):
-        return _impl(array, to, including_unknown, highlevel, behavior)
+    # Dispatch
+    yield (array,)
+
+    # Implementation
+    return _impl(array, to, including_unknown, highlevel, behavior)
 
 
 def _impl(array, to, including_unknown, highlevel, behavior):
     to_dtype = np.dtype(to)
     to_str = ak.types.numpytype.dtype_to_primitive(to_dtype)
     layout = ak.operations.to_layout(array, allow_record=False, allow_other=False)
     out = ak._do.numbers_to_type(layout, to_str, including_unknown)
```

### Comparing `awkward-2.2.3/src/awkward/operations/ak_var.py` & `awkward-2.2.4/src/awkward/operations/ak_var.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,22 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("var",)
 import awkward as ak
 from awkward._behavior import behavior_of
 from awkward._connect.numpy import UNSUPPORTED
+from awkward._dispatch import high_level_function
 from awkward._layout import maybe_posaxis
 from awkward._nplikes.numpylike import NumpyMetadata
 from awkward._regularize import regularize_axis
 
 np = NumpyMetadata.instance()
 
 
-def var(
-    x,
-    weight=None,
-    ddof=0,
-    axis=None,
-    *,
-    keepdims=False,
-    mask_identity=False,
-):
+@high_level_function
+def var(x, weight=None, ddof=0, axis=None, *, keepdims=False, mask_identity=False):
     """
     Args:
         x: The data on which to compute the variance (anything #ak.to_layout recognizes).
         weight: Data that can be broadcasted to `x` to give each value a
             weight. Weighting values equally is the same as no weights;
             weighting some values higher increases the significance of those
             values. Weights can be zero or negative.
@@ -64,37 +58,23 @@
 
     See #ak.sum for a complete description of handling nested lists and
     missing values (None) in reducers, and #ak.mean for an example with another
     non-reducer.
 
     See also #ak.nanvar.
     """
-    with ak._errors.OperationErrorContext(
-        "ak.var",
-        {
-            "x": x,
-            "weight": weight,
-            "ddof": ddof,
-            "axis": axis,
-            "keepdims": keepdims,
-            "mask_identity": mask_identity,
-        },
-    ):
-        return _impl(x, weight, ddof, axis, keepdims, mask_identity)
-
-
-def nanvar(
-    x,
-    weight=None,
-    ddof=0,
-    axis=None,
-    *,
-    keepdims=False,
-    mask_identity=True,
-):
+    # Dispatch
+    yield x, weight
+
+    # Implementation
+    return _impl(x, weight, ddof, axis, keepdims, mask_identity)
+
+
+@high_level_function
+def nanvar(x, weight=None, ddof=0, axis=None, *, keepdims=False, mask_identity=True):
     """
     Args:
         x: The data on which to compute the variance (anything #ak.to_layout recognizes).
         weight: Data that can be broadcasted to `x` to give each value a
             weight. Weighting values equally is the same as no weights;
             weighting some values higher increases the significance of those
             values. Weights can be zero or negative.
@@ -121,30 +101,29 @@
 
         ak.var(ak.nan_to_none(array))
 
     with all other arguments unchanged.
 
     See also #ak.var.
     """
-    with ak._errors.OperationErrorContext(
-        "ak.nanvar",
-        {
-            "x": x,
-            "weight": weight,
-            "ddof": ddof,
-            "axis": axis,
-            "keepdims": keepdims,
-            "mask_identity": mask_identity,
-        },
-    ):
-        x = ak.operations.ak_nan_to_none._impl(x, False, None)
-        if weight is not None:
-            weight = ak.operations.ak_nan_to_none._impl(weight, False, None)
+    # Dispatch
+    yield x, weight
 
-        return _impl(x, weight, ddof, axis, keepdims, mask_identity)
+    # Implementation
+    if weight is not None:
+        weight = ak.operations.ak_nan_to_none._impl(weight, False, None)
+
+    return _impl(
+        ak.operations.ak_nan_to_none._impl(x, False, None),
+        weight,
+        ddof,
+        axis,
+        keepdims,
+        mask_identity,
+    )
 
 
 def _impl(x, weight, ddof, axis, keepdims, mask_identity):
     axis = regularize_axis(axis)
     behavior = behavior_of(x, weight)
     x = ak.highlevel.Array(
         ak.operations.to_layout(x, allow_record=False, allow_other=False),
```

### Comparing `awkward-2.2.3/src/awkward/operations/ak_where.py` & `awkward-2.2.4/src/awkward/operations/ak_where.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("where",)
 import awkward as ak
 from awkward._backends.dispatch import backend_of
 from awkward._backends.numpy import NumpyBackend
 from awkward._behavior import behavior_of
+from awkward._dispatch import high_level_function
 from awkward._layout import wrap_layout
 from awkward._nplikes.numpylike import NumpyMetadata
 
 np = NumpyMetadata.instance()
 cpu = NumpyBackend.instance()
 
 
-@ak._connect.numpy.implements("where")
+@high_level_function
 def where(condition, *args, mergebool=True, highlevel=True, behavior=None):
     """
     Args:
         condition: Array-like data (anything #ak.to_layout recognizes) of booleans.
         x: Optional array-like data (anything #ak.to_layout recognizes) with the same
             length as `condition`.
         y: Optional array-like data (anything #ak.to_layout recognizes) with the same
@@ -39,37 +40,27 @@
     `condition`, `x`, and `y` must all have the same length and
 
         output[i] = x[i] if condition[i] else y[i]
 
     for all `i`. The structure of `x` and `y` do not need to be the same; if
     they are incompatible types, the output will have #ak.type.UnionType.
     """
+    # Dispatch
+    yield (*args, condition)
+
+    # Implementation
     if len(args) == 0:
-        with ak._errors.OperationErrorContext(
-            "ak.where",
-            {"condition": condition, "mergebool": mergebool, "highlevel": highlevel},
-        ):
-            return _impl1(condition, mergebool, highlevel, behavior)
+        return _impl1(condition, mergebool, highlevel, behavior)
 
     elif len(args) == 1:
         raise ValueError("either both or neither of x and y should be given")
 
     elif len(args) == 2:
         x, y = args
-        with ak._errors.OperationErrorContext(
-            "ak.where",
-            {
-                "condition": condition,
-                "x": x,
-                "y": y,
-                "mergebool": mergebool,
-                "highlevel": highlevel,
-            },
-        ):
-            return _impl3(condition, x, y, mergebool, highlevel, behavior)
+        return _impl3(condition, x, y, mergebool, highlevel, behavior)
 
     else:
         raise TypeError(
             "where() takes from 1 to 3 positional arguments but {} were "
             "given".format(len(args) + 1)
         )
```

### Comparing `awkward-2.2.3/src/awkward/operations/ak_with_field.py` & `awkward-2.2.4/src/awkward/operations/ak_with_field.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,24 +2,26 @@
 __all__ = ("with_field",)
 import copy
 
 import awkward as ak
 from awkward._backends.dispatch import backend_of
 from awkward._backends.numpy import NumpyBackend
 from awkward._behavior import behavior_of
+from awkward._dispatch import high_level_function
 from awkward._layout import wrap_layout
 from awkward._nplikes.numpylike import NumpyMetadata
 from awkward._regularize import is_non_string_like_sequence
 
 np = NumpyMetadata.instance()
 
 
 cpu = NumpyBackend.instance()
 
 
+@high_level_function
 def with_field(array, what, where=None, *, highlevel=True, behavior=None):
     """
     Args:
         array: Array-like data (anything #ak.to_layout recognizes).
         what: Array-like data (anything #ak.to_layout recognizes) to add as a new field.
         where (None or str or non-empy sequence of str): If None, the new field
             has no name (can be accessed as an integer slot number in a
@@ -35,25 +37,19 @@
     change the array in-place.
 
     See #ak.Array.__setitem__ and #ak.Record.__setitem__ for a variant that
     changes the high-level object in-place. (These methods internally use
     #ak.with_field, so performance is not a factor in choosing one over the
     other.)
     """
-    with ak._errors.OperationErrorContext(
-        "ak.with_field",
-        {
-            "array": array,
-            "what": what,
-            "where": where,
-            "highlevel": highlevel,
-            "behavior": behavior,
-        },
-    ):
-        return _impl(array, what, where, highlevel, behavior)
+    # Dispatch
+    yield array, what
+
+    # Implementation
+    return _impl(array, what, where, highlevel, behavior)
 
 
 def _impl(base, what, where, highlevel, behavior):
     if not (
         where is None
         or isinstance(where, str)
         or (
```

### Comparing `awkward-2.2.3/src/awkward/operations/ak_with_parameter.py` & `awkward-2.2.4/src/awkward/operations/ak_with_parameter.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("with_parameter",)
 import awkward as ak
 from awkward._behavior import behavior_of
+from awkward._dispatch import high_level_function
 from awkward._layout import wrap_layout
 from awkward._nplikes.numpylike import NumpyMetadata
 
 np = NumpyMetadata.instance()
 
 
+@high_level_function
 def with_parameter(array, parameter, value, *, highlevel=True, behavior=None):
     """
     Args:
         array: Array-like data (anything #ak.to_layout recognizes).
         parameter (str): Name of the parameter to set on that array.
         value (JSON): Value of the parameter to set on that array.
         highlevel (bool): If True, return an #ak.Array; otherwise, return
@@ -24,25 +26,19 @@
 
     Note that a "new array" is a lightweight shallow copy, not a duplication
     of large data buffers.
 
     You can also remove a single parameter with this function, since setting
     a parameter to None is equivalent to removing it.
     """
-    with ak._errors.OperationErrorContext(
-        "ak.with_parameter",
-        {
-            "array": array,
-            "parameter": parameter,
-            "value": value,
-            "highlevel": highlevel,
-            "behavior": behavior,
-        },
-    ):
-        return _impl(array, parameter, value, highlevel, behavior)
+    # Dispatch
+    yield (array,)
+
+    # Implementation
+    return _impl(array, parameter, value, highlevel, behavior)
 
 
 def _impl(array, parameter, value, highlevel, behavior):
     behavior = behavior_of(array, behavior=behavior)
     layout = ak.operations.to_layout(array, allow_record=True, allow_other=False)
 
     out = layout.with_parameter(parameter, value)
```

### Comparing `awkward-2.2.3/src/awkward/operations/ak_without_field.py` & `awkward-2.2.4/src/awkward/operations/ak_without_field.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("without_field",)
 from collections.abc import Sequence
 
 import awkward as ak
 from awkward._behavior import behavior_of
+from awkward._dispatch import high_level_function
 from awkward._layout import wrap_layout
 from awkward._nplikes.numpylike import NumpyMetadata
 
 np = NumpyMetadata.instance()
 
 
+@high_level_function
 def without_field(array, where, *, highlevel=True, behavior=None):
     """
     Args:
         array: Array-like data (anything #ak.to_layout recognizes).
         where (str or non-empy sequence of str): If str, the name of the field
             to be removed. If a sequence, it is interpreted as a path where to
             remove the field in a nested record.
@@ -27,19 +29,19 @@
     change the array in-place.
 
     See #ak.Array.__delitem__ and #ak.Record.__delitem__ for a variant that
     changes the high-level object in-place. (These methods internally use
     #ak.without_field, so performance is not a factor in choosing one over the
     other.)
     """
-    with ak._errors.OperationErrorContext(
-        "ak.without_field",
-        {"array": array, "where": where, "highlevel": highlevel, "behavior": behavior},
-    ):
-        return _impl(array, where, highlevel, behavior)
+    # Dispatch
+    yield (array,)
+
+    # Implementation
+    return _impl(array, where, highlevel, behavior)
 
 
 def _impl(base, where, highlevel, behavior):
     if isinstance(where, str):
         where = [where]
     elif not (isinstance(where, Sequence) and all(isinstance(x, str) for x in where)):
         raise TypeError(
```

### Comparing `awkward-2.2.3/src/awkward/operations/ak_without_parameters.py` & `awkward-2.2.4/src/awkward/operations/ak_without_parameters.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("without_parameters",)
 import awkward as ak
 from awkward._behavior import behavior_of
+from awkward._dispatch import high_level_function
 from awkward._layout import wrap_layout
 from awkward._nplikes.numpylike import NumpyMetadata
 
 np = NumpyMetadata.instance()
 
 
+@high_level_function
 def without_parameters(array, *, highlevel=True, behavior=None):
     """
     Args:
         array: Array-like data (anything #ak.to_layout recognizes).
         highlevel (bool): If True, return an #ak.Array; otherwise, return
             a low-level #ak.contents.Content subclass.
         behavior (None or dict): Custom #ak.behavior for the output array, if
@@ -19,19 +21,19 @@
 
     This function returns a new array without any parameters in its
     #ak.Array.layout, on nodes of any level of depth.
 
     Note that a "new array" is a lightweight shallow copy, not a duplication
     of large data buffers.
     """
-    with ak._errors.OperationErrorContext(
-        "ak.without_parameters",
-        {"array": array, "highlevel": highlevel, "behavior": behavior},
-    ):
-        return _impl(array, highlevel, behavior)
+    # Dispatch
+    yield (array,)
+
+    # Implementation
+    return _impl(array, highlevel, behavior)
 
 
 def _impl(array, highlevel, behavior):
     behavior = behavior_of(array, behavior=behavior)
     layout = ak.operations.to_layout(array, allow_record=True, allow_other=False)
 
     out = ak._do.recursively_apply(
```

### Comparing `awkward-2.2.3/src/awkward/operations/ak_zeros_like.py` & `awkward-2.2.4/src/awkward/operations/ak_zeros_like.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("zeros_like",)
-
 import awkward as ak
 from awkward._connect.numpy import UNSUPPORTED
+from awkward._dispatch import high_level_function
 from awkward._nplikes.numpylike import NumpyMetadata
 
 np = NumpyMetadata.instance()
 
 
 _ZEROS = object()
 
 
+@high_level_function
 def zeros_like(
     array, *, dtype=None, including_unknown=False, highlevel=True, behavior=None
 ):
     """
     Args:
         array: Array-like data (anything #ak.to_layout recognizes).
         dtype (None or NumPy dtype): Overrides the data type of the result.
@@ -29,25 +30,19 @@
     This is the equivalent of NumPy's `np.zeros_like` for Awkward Arrays.
 
     See #ak.full_like for details, and see also #ak.ones_like.
 
     (There is no equivalent of NumPy's `np.empty_like` because Awkward Arrays
     are immutable.)
     """
-    with ak._errors.OperationErrorContext(
-        "ak.zeros_like",
-        {
-            "array": array,
-            "dtype": dtype,
-            "including_unknown": including_unknown,
-            "highlevel": highlevel,
-            "behavior": behavior,
-        },
-    ):
-        return _impl(array, highlevel, behavior, dtype, including_unknown)
+    # Dispatch
+    yield (array,)
+
+    # Implementation
+    return _impl(array, highlevel, behavior, dtype, including_unknown)
 
 
 def _impl(array, highlevel, behavior, dtype, including_unknown):
     if dtype is not None:
         return ak.operations.ak_full_like._impl(
             array, 0, highlevel, behavior, dtype, including_unknown
         )
```

### Comparing `awkward-2.2.3/src/awkward/operations/ak_zip.py` & `awkward-2.2.4/src/awkward/operations/ak_zip.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("zip",)
+from collections.abc import Mapping
+
 import awkward as ak
 from awkward._behavior import behavior_of
+from awkward._dispatch import high_level_function
 from awkward._layout import wrap_layout
 from awkward._nplikes.numpylike import NumpyMetadata
 
 np = NumpyMetadata.instance()
 
 
+@high_level_function
 def zip(
     arrays,
     depth_limit=None,
     *,
     parameters=None,
     with_name=None,
     right_broadcast=False,
@@ -127,37 +131,31 @@
     If the `optiontype_outside_record` option is set to `True`, Awkward will continue to
     broadcast the arrays together at the depth_limit until it reaches non-option
     types. This effectively takes the union of the option mask:
 
         >>> ak.zip([one, two], optiontype_outside_record=True)
         <Array [None, (2, 5), None] type='3 * ?(int64, int64)'>
     """
-    with ak._errors.OperationErrorContext(
-        "ak.zip",
-        {
-            "arrays": arrays,
-            "depth_limit": depth_limit,
-            "parameters": parameters,
-            "with_name": with_name,
-            "right_broadcast": right_broadcast,
-            "optiontype_outside_record": optiontype_outside_record,
-            "highlevel": highlevel,
-            "behavior": behavior,
-        },
-    ):
-        return _impl(
-            arrays,
-            depth_limit,
-            parameters,
-            with_name,
-            right_broadcast,
-            optiontype_outside_record,
-            highlevel,
-            behavior,
-        )
+    # Dispatch
+    if isinstance(arrays, Mapping):
+        yield arrays.values()
+    else:
+        yield arrays
+
+    # Implementation
+    return _impl(
+        arrays,
+        depth_limit,
+        parameters,
+        with_name,
+        right_broadcast,
+        optiontype_outside_record,
+        highlevel,
+        behavior,
+    )
 
 
 def _impl(
     arrays,
     depth_limit,
     parameters,
     with_name,
```

### Comparing `awkward-2.2.3/src/awkward/types/__init__.py` & `awkward-2.2.4/src/awkward/types/__init__.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/types/_awkward_datashape_parser.py` & `awkward-2.2.4/src/awkward/types/_awkward_datashape_parser.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/types/arraytype.py` & `awkward-2.2.4/src/awkward/types/arraytype.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/types/listtype.py` & `awkward-2.2.4/src/awkward/types/listtype.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/types/numpytype.py` & `awkward-2.2.4/src/awkward/types/numpytype.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/types/optiontype.py` & `awkward-2.2.4/src/awkward/types/optiontype.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/types/recordtype.py` & `awkward-2.2.4/src/awkward/types/recordtype.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/types/regulartype.py` & `awkward-2.2.4/src/awkward/types/regulartype.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/types/scalartype.py` & `awkward-2.2.4/src/awkward/types/scalartype.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/types/type.py` & `awkward-2.2.4/src/awkward/types/type.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/types/uniontype.py` & `awkward-2.2.4/src/awkward/types/uniontype.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/src/awkward/types/unknowntype.py` & `awkward-2.2.4/src/awkward/types/unknowntype.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0002_minimal_listarray.py` & `awkward-2.2.4/tests/test_0002_minimal_listarray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0008_slices_and_getitem.py` & `awkward-2.2.4/tests/test_0008_slices_and_getitem.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0011_listarray.py` & `awkward-2.2.4/tests/test_0011_listarray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0013_error_handling_struct.py` & `awkward-2.2.4/tests/test_0013_error_handling_struct.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0014_finish_up_getitem.py` & `awkward-2.2.4/tests/test_0014_finish_up_getitem.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0018_fromiter_fillable.py` & `awkward-2.2.4/tests/test_0018_fromiter_fillable.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0019_use_json_library.py` & `awkward-2.2.4/tests/test_0019_use_json_library.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0020_support_unsigned_indexes.py` & `awkward-2.2.4/tests/test_0020_support_unsigned_indexes.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0021_emptyarray.py` & `awkward-2.2.4/tests/test_0021_emptyarray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0023_regular_array.py` & `awkward-2.2.4/tests/test_0023_regular_array.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0024_use_regular_array.py` & `awkward-2.2.4/tests/test_0024_use_regular_array.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0025_record_array.py` & `awkward-2.2.4/tests/test_0025_record_array.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0028_add_dressed_types.py` & `awkward-2.2.4/tests/test_0028_add_dressed_types.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0032_replace_dressedtype.py` & `awkward-2.2.4/tests/test_0032_replace_dressedtype.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0046_start_indexedarray.py` & `awkward-2.2.4/tests/test_0046_start_indexedarray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0049_distinguish_record_and_recordarray_behaviors.py` & `awkward-2.2.4/tests/test_0049_distinguish_record_and_recordarray_behaviors.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0057_introducing_forms.py` & `awkward-2.2.4/tests/test_0057_introducing_forms.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0070_argmin_and_argmax.py` & `awkward-2.2.4/tests/test_0070_argmin_and_argmax.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0072_fillna_operation.py` & `awkward-2.2.4/tests/test_0072_fillna_operation.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0074_argsort_and_sort.py` & `awkward-2.2.4/tests/test_0074_argsort_and_sort.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0077_zip_operation.py` & `awkward-2.2.4/tests/test_0077_zip_operation.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0078_argcross_and_cross.py` & `awkward-2.2.4/tests/test_0078_argcross_and_cross.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0079_argchoose_and_choose.py` & `awkward-2.2.4/tests/test_0079_argchoose_and_choose.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0080_flatpandas_multiindex_rows_and_columns.py` & `awkward-2.2.4/tests/test_0080_flatpandas_multiindex_rows_and_columns.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0084_start_unionarray.py` & `awkward-2.2.4/tests/test_0084_start_unionarray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0086_nep13_ufunc.py` & `awkward-2.2.4/tests/test_0086_nep13_ufunc.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0089_numpy_functions.py` & `awkward-2.2.4/tests/test_0089_numpy_functions.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0093_simplify_uniontypes_and_optiontypes.py` & `awkward-2.2.4/tests/test_0093_simplify_uniontypes_and_optiontypes.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0107_assign_fields_to_records.py` & `awkward-2.2.4/tests/test_0107_assign_fields_to_records.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0111_jagged_and_masked_getitem.py` & `awkward-2.2.4/tests/test_0111_jagged_and_masked_getitem.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0115_generic_reducer_operation.py` & `awkward-2.2.4/tests/test_0115_generic_reducer_operation.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0118_numba_cpointers.py` & `awkward-2.2.4/tests/test_0118_numba_cpointers.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0119_numexpr_and_broadcast_arrays.py` & `awkward-2.2.4/tests/test_0119_numexpr_and_broadcast_arrays.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0124_strings_in_numba.py` & `awkward-2.2.4/tests/test_0124_strings_in_numba.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0127_tomask_operation.py` & `awkward-2.2.4/tests/test_0127_tomask_operation.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0127b_tomask_operation_numba.py` & `awkward-2.2.4/tests/test_0127b_tomask_operation_numba.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0138_emptyarray_type.py` & `awkward-2.2.4/tests/test_0138_emptyarray_type.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0150_flatten.py` & `awkward-2.2.4/tests/test_0150_flatten.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0163_negative_axis_wrap.py` & `awkward-2.2.4/tests/test_0163_negative_axis_wrap.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0166_0167_0170_random_issues.py` & `awkward-2.2.4/tests/test_0166_0167_0170_random_issues.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0173_astype_operation.py` & `awkward-2.2.4/tests/test_0173_astype_operation.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0184_concatenate_operation.py` & `awkward-2.2.4/tests/test_0184_concatenate_operation.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0193_is_none_axis_parameter.py` & `awkward-2.2.4/tests/test_0193_is_none_axis_parameter.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0198_tutorial_documentation_1.py` & `awkward-2.2.4/tests/test_0198_tutorial_documentation_1.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0222_count_with_axis0.py` & `awkward-2.2.4/tests/test_0222_count_with_axis0.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0224_arrow_to_awkward.py` & `awkward-2.2.4/tests/test_0224_arrow_to_awkward.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0264_reduce_last_empty.py` & `awkward-2.2.4/tests/test_0264_reduce_last_empty.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0273_path_for_with_field.py` & `awkward-2.2.4/tests/test_0273_path_for_with_field.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0286_broadcast_single_value_with_field.py` & `awkward-2.2.4/tests/test_0286_broadcast_single_value_with_field.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0290_bug_fixes_for_hats.py` & `awkward-2.2.4/tests/test_0290_bug_fixes_for_hats.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0315_integerindex.py` & `awkward-2.2.4/tests/test_0315_integerindex.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0331_pandas_indexedarray.py` & `awkward-2.2.4/tests/test_0331_pandas_indexedarray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0334_fully_broadcastable_where.py` & `awkward-2.2.4/tests/test_0334_fully_broadcastable_where.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0339_highlevel_sorting_function.py` & `awkward-2.2.4/tests/test_0339_highlevel_sorting_function.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0348_form_keys.py` & `awkward-2.2.4/tests/test_0348_form_keys.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0355_mixins.py` & `awkward-2.2.4/tests/test_0355_mixins.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0395_complex_type_arrays.py` & `awkward-2.2.4/tests/test_0395_complex_type_arrays.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0395_fix_numba_indexedarray.py` & `awkward-2.2.4/tests/test_0395_fix_numba_indexedarray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0397_arrays_as_constants_in_numba.py` & `awkward-2.2.4/tests/test_0397_arrays_as_constants_in_numba.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0401_add_categorical_type_for_arrow_dictionary.py` & `awkward-2.2.4/tests/test_0401_add_categorical_type_for_arrow_dictionary.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0404_array_validity_check.py` & `awkward-2.2.4/tests/test_0404_array_validity_check.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0410_fix_argminmax_positions_for_missing_values.py` & `awkward-2.2.4/tests/test_0410_fix_argminmax_positions_for_missing_values.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0437_stream_of_many_json_files.py` & `awkward-2.2.4/tests/test_0437_stream_of_many_json_files.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0447_preserve_regularness_in_reduce.py` & `awkward-2.2.4/tests/test_0447_preserve_regularness_in_reduce.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0449_merge_many_arrays_in_one_pass.py` & `awkward-2.2.4/tests/test_0449_merge_many_arrays_in_one_pass.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0493_zeros_ones_full_like.py` & `awkward-2.2.4/tests/test_0493_zeros_ones_full_like.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0496_provide_local_index.py` & `awkward-2.2.4/tests/test_0496_provide_local_index.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0499_getitem_indexedarray_bug.py` & `awkward-2.2.4/tests/test_0499_getitem_indexedarray_bug.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0504_block_ufuncs_for_strings.py` & `awkward-2.2.4/tests/test_0504_block_ufuncs_for_strings.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0511_copy_and_deepcopy.py` & `awkward-2.2.4/tests/test_0511_copy_and_deepcopy.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0527_fix_unionarray_ufuncs_and_parameters_in_merging.py` & `awkward-2.2.4/tests/test_0527_fix_unionarray_ufuncs_and_parameters_in_merging.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0549_numba_array_asarray.py` & `awkward-2.2.4/tests/test_0549_numba_array_asarray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0557_min_max_initial_argument.py` & `awkward-2.2.4/tests/test_0557_min_max_initial_argument.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0559_fix_booleans_in_numba.py` & `awkward-2.2.4/tests/test_0559_fix_booleans_in_numba.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0572_numba_array_ndim.py` & `awkward-2.2.4/tests/test_0572_numba_array_ndim.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0582_propagate_context_in_broadcast_and_apply.py` & `awkward-2.2.4/tests/test_0582_propagate_context_in_broadcast_and_apply.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0583_implement_unflatten_function.py` & `awkward-2.2.4/tests/test_0583_implement_unflatten_function.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0590_allow_regulararray_size_zero.py` & `awkward-2.2.4/tests/test_0590_allow_regulararray_size_zero.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0593_preserve_nullability_in_arrow_and_parquet.py` & `awkward-2.2.4/tests/test_0593_preserve_nullability_in_arrow_and_parquet.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0652_tests_of_complex_numbers.py` & `awkward-2.2.4/tests/test_0652_tests_of_complex_numbers.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0674_categorical_validation.py` & `awkward-2.2.4/tests/test_0674_categorical_validation.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0713_getitem_field_should_simplify_optiontype.py` & `awkward-2.2.4/tests/test_0713_getitem_field_should_simplify_optiontype.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0723_ensure_that_jagged_slice_fits_array_length.py` & `awkward-2.2.4/tests/test_0723_ensure_that_jagged_slice_fits_array_length.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0730_unflatten_axis_parameter.py` & `awkward-2.2.4/tests/test_0730_unflatten_axis_parameter.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0733_run_lengths.py` & `awkward-2.2.4/tests/test_0733_run_lengths.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0736_implement_argsort_for_strings.py` & `awkward-2.2.4/tests/test_0736_implement_argsort_for_strings.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0766_prevent_combinations_of_characters.py` & `awkward-2.2.4/tests/test_0766_prevent_combinations_of_characters.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0773_typeparser.py` & `awkward-2.2.4/tests/test_0773_typeparser.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0788_indexedarray_carrying_recordarray_parameters.py` & `awkward-2.2.4/tests/test_0788_indexedarray_carrying_recordarray_parameters.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0794_ak_cartesian_on_empty_array.py` & `awkward-2.2.4/tests/test_0794_ak_cartesian_on_empty_array.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0803_argsort_fix_type.py` & `awkward-2.2.4/tests/test_0803_argsort_fix_type.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0806_empty_lists_cartesian_fix.py` & `awkward-2.2.4/tests/test_0806_empty_lists_cartesian_fix.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0813_full_like_dtype_arg.py` & `awkward-2.2.4/tests/test_0813_full_like_dtype_arg.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0815_broadcast_union_types_to_all_possibilities.py` & `awkward-2.2.4/tests/test_0815_broadcast_union_types_to_all_possibilities.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0828_arrow_datatype_null.py` & `awkward-2.2.4/tests/test_0828_arrow_datatype_null.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0835_datetime_type.py` & `awkward-2.2.4/tests/test_0835_datetime_type.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0835_datetime_type_pandas.py` & `awkward-2.2.4/tests/test_0835_datetime_type_pandas.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0835_datetime_type_pyarrow.py` & `awkward-2.2.4/tests/test_0835_datetime_type_pyarrow.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0850_argsort_mask_array.py` & `awkward-2.2.4/tests/test_0850_argsort_mask_array.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0866_getitem_field_and_flatten_unions.py` & `awkward-2.2.4/tests/test_0866_getitem_field_and_flatten_unions.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0875_arrow_null_type.py` & `awkward-2.2.4/tests/test_0875_arrow_null_type.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0879_non_primitive_with_field.py` & `awkward-2.2.4/tests/test_0879_non_primitive_with_field.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0884_index_and_identifier_refactoring.py` & `awkward-2.2.4/tests/test_0884_index_and_identifier_refactoring.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0889_ptp.py` & `awkward-2.2.4/tests/test_0889_ptp.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0896_content_classes_refactoring.py` & `awkward-2.2.4/tests/test_0896_content_classes_refactoring.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0898_unzip_heterogeneous_records.py` & `awkward-2.2.4/tests/test_0898_unzip_heterogeneous_records.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0905_leading_zeros_in_unflatten.py` & `awkward-2.2.4/tests/test_0905_leading_zeros_in_unflatten.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0906_arrow_fixed_size_list_type.py` & `awkward-2.2.4/tests/test_0906_arrow_fixed_size_list_type.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0910_unflatten_counts_relation.py` & `awkward-2.2.4/tests/test_0910_unflatten_counts_relation.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0912_packed.py` & `awkward-2.2.4/tests/test_0912_packed.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0914_types_and_forms.py` & `awkward-2.2.4/tests/test_0914_types_and_forms.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0916_datetime_values_astype.py` & `awkward-2.2.4/tests/test_0916_datetime_values_astype.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0927_numpy_array_nbytes.py` & `awkward-2.2.4/tests/test_0927_numpy_array_nbytes.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0930_bug_in_unionarray_purelist_parameter.py` & `awkward-2.2.4/tests/test_0930_bug_in_unionarray_purelist_parameter.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0945_argsort_sort_nan_array.py` & `awkward-2.2.4/tests/test_0945_argsort_sort_nan_array.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0958_new_forms_must_accept_old_form_json.py` & `awkward-2.2.4/tests/test_0958_new_forms_must_accept_old_form_json.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0959__getitem_array_implementation.py` & `awkward-2.2.4/tests/test_0959__getitem_array_implementation.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0975_mask_multidimensional_numpy_array.py` & `awkward-2.2.4/tests/test_0975_mask_multidimensional_numpy_array.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0979_where_multidimentional_numpy_array.py` & `awkward-2.2.4/tests/test_0979_where_multidimentional_numpy_array.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0982_missing_case_in_nonlocal_reducers.py` & `awkward-2.2.4/tests/test_0982_missing_case_in_nonlocal_reducers.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0984_ravel.py` & `awkward-2.2.4/tests/test_0984_ravel.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_0992_correct_ptp_unmasking.py` & `awkward-2.2.4/tests/test_0992_correct_ptp_unmasking.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_1000_fixes_argmax_for_ListOffsetArray_with_nonzero_start.py` & `awkward-2.2.4/tests/test_1000_fixes_argmax_for_ListOffsetArray_with_nonzero_start.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_1017_numpyarray_broadcast.py` & `awkward-2.2.4/tests/test_1017_numpyarray_broadcast.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_1030_mixin_class_name.py` & `awkward-2.2.4/tests/test_1030_mixin_class_name.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_1031_start_getitem_next.py` & `awkward-2.2.4/tests/test_1031_start_getitem_next.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_1031b_start_getitem_next_specialized.py` & `awkward-2.2.4/tests/test_1031b_start_getitem_next_specialized.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_1049_concatenate_single_array.py` & `awkward-2.2.4/tests/test_1049_concatenate_single_array.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_1055_fill_none_numpy_dimension.py` & `awkward-2.2.4/tests/test_1055_fill_none_numpy_dimension.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_1059_localindex.py` & `awkward-2.2.4/tests/test_1059_localindex.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_1066_to_numpy_masked_structured_array.py` & `awkward-2.2.4/tests/test_1066_to_numpy_masked_structured_array.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_1071_mask_identity_false_should_not_return_option_type.py` & `awkward-2.2.4/tests/test_1071_mask_identity_false_should_not_return_option_type.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_1072_sort.py` & `awkward-2.2.4/tests/test_1072_sort.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_1074_combinations.py` & `awkward-2.2.4/tests/test_1074_combinations.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_1075_validityerror.py` & `awkward-2.2.4/tests/test_1075_validityerror.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_1110_type_tracer_1.py` & `awkward-2.2.4/tests/test_1110_type_tracer_1.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_1116_project_maskedarrays.py` & `awkward-2.2.4/tests/test_1116_project_maskedarrays.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_1125_to_arrow_from_arrow.py` & `awkward-2.2.4/tests/test_1125_to_arrow_from_arrow.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 
 import os
 
 import numpy as np
 import pytest
+from packaging.version import parse as parse_version
 
 import awkward as ak
 
 pyarrow = pytest.importorskip("pyarrow")
 pyarrow_parquet = pytest.importorskip("pyarrow.parquet")
 
 to_list = ak.operations.to_list
@@ -567,15 +568,16 @@
     paarray = akarray.to_arrow(extensionarray=extensionarray)
     if not is_tuple or extensionarray:
         arrow_round_trip(akarray, paarray, extensionarray)
         parquet_round_trip(akarray, paarray, extensionarray, tmp_path)
 
 
 @pytest.mark.skipif(
-    not ak._util.numpy_at_least("1.20"), reason="NumPy >= 1.20 required for dates"
+    parse_version(np.__version__) < parse_version("1.20.0"),
+    reason="NumPy >= 1.20 required for dates",
 )
 @pytest.mark.parametrize("extensionarray", [False, True])
 def test_numpyarray_datetime(tmp_path, extensionarray):
     # pyarrow doesn't yet support datetime/duration conversions to Parquet.
     # (FIXME: find or create a JIRA ticket.)
 
     akarray = ak.contents.NumpyArray(
```

### Comparing `awkward-2.2.3/tests/test_1132_utility_methods_for_highlevel_functions.py` & `awkward-2.2.4/tests/test_1132_utility_methods_for_highlevel_functions.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_1134_from_buffers_to_buffers.py` & `awkward-2.2.4/tests/test_1134_from_buffers_to_buffers.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_1135_rpad_operation.py` & `awkward-2.2.4/tests/test_1135_rpad_operation.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_1136_regulararray_zeros_in_shape.py` & `awkward-2.2.4/tests/test_1136_regulararray_zeros_in_shape.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_1137_num.py` & `awkward-2.2.4/tests/test_1137_num.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_1142_numbers_to_type.py` & `awkward-2.2.4/tests/test_1142_numbers_to_type.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_1149_datetime_sort.py` & `awkward-2.2.4/tests/test_1149_datetime_sort.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_1154_arrow_tables_should_preserve_parameters.py` & `awkward-2.2.4/tests/test_1154_arrow_tables_should_preserve_parameters.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_1162_ak_from_json_schema.py` & `awkward-2.2.4/tests/test_1162_ak_from_json_schema.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_1183_bugs_found_by_dask_project_2.py` & `awkward-2.2.4/tests/test_1183_bugs_found_by_dask_project_2.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_1189_fix_singletons_for_non_optional_data.py` & `awkward-2.2.4/tests/test_1189_fix_singletons_for_non_optional_data.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_1192_iterables_in___array_function__.py` & `awkward-2.2.4/tests/test_1192_iterables_in___array_function__.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_1193_is_none_nested_option.py` & `awkward-2.2.4/tests/test_1193_is_none_nested_option.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_1233_ak_with_name.py` & `awkward-2.2.4/tests/test_1233_ak_with_name.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_1240_v2_implementation_of_numba_1.py` & `awkward-2.2.4/tests/test_1240_v2_implementation_of_numba_1.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_1259_simplify_optiontype.py` & `awkward-2.2.4/tests/test_1259_simplify_optiontype.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_1260_simplify_masked_option_types.py` & `awkward-2.2.4/tests/test_1260_simplify_masked_option_types.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_1271_fix_4D_reducers.py` & `awkward-2.2.4/tests/test_1271_fix_4D_reducers.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_1294_to_and_from_parquet.py` & `awkward-2.2.4/tests/test_1294_to_and_from_parquet.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 
 import os.path
 
 import numpy as np
 import pytest
+from packaging.version import parse as parse_version
 
 import awkward as ak
 
 pyarrow_parquet = pytest.importorskip("pyarrow.parquet")
+fsspec = pytest.importorskip("fsspec")
 
 
 def through_arrow(
     akarray,
     extensionarray,
     tmp_path,
     list_to32=False,
@@ -670,15 +672,16 @@
     predicted_form = ak._connect.pyarrow.form_handle_arrow(
         schema_arrow, pass_empty_field=True
     )
     assert predicted_form == array_form
 
 
 @pytest.mark.skipif(
-    not ak._util.numpy_at_least("1.20"), reason="NumPy >= 1.20 required for dates"
+    parse_version(np.__version__) < parse_version("1.20.0"),
+    reason="NumPy >= 1.20 required for dates",
 )
 @pytest.mark.parametrize("through", [through_arrow, through_parquet])
 @pytest.mark.parametrize("extensionarray", [False, True])
 def test_numpyarray_datetime(tmp_path, through, extensionarray):
     # pyarrow doesn't yet support datetime/duration conversions to Parquet.
     # (FIXME: find or create a JIRA ticket.)
 
@@ -844,16 +847,14 @@
 #  - directory without _metadata but with _common_metadata
 #  - directory with only data files, scanned
 #  - directory with only data files, not scanned
 
 
 @pytest.fixture()
 def generate_datafiles(tmp_path):
-    import fsspec
-
     fs = fsspec.filesystem("file")
     data1 = ak.from_iter([[1, 2, 3], [4, 5]])
     data2 = data1 + 1
     md1 = ak.to_parquet(data1, os.path.join(tmp_path, "data1.parq"))
     md2 = ak.to_parquet(data2, os.path.join(tmp_path, "data2.parq"))
     return str(tmp_path), [md1, md2], fs
```

### Comparing `awkward-2.2.3/tests/test_1298_allow_nan_to_num_arguments_to_be_arrays.py` & `awkward-2.2.4/tests/test_1298_allow_nan_to_num_arguments_to_be_arrays.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_1300_awkward_to_cpp_converter_with_cling.py` & `awkward-2.2.4/tests/test_1300_awkward_to_cpp_converter_with_cling.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_1300b_same_for_numba.py` & `awkward-2.2.4/tests/test_1300b_same_for_numba.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_1308_zip_after_option.py` & `awkward-2.2.4/tests/test_1308_zip_after_option.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_1318_array_function_types.py` & `awkward-2.2.4/tests/test_1318_array_function_types.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_1320_mask_identity_defaults.py` & `awkward-2.2.4/tests/test_1320_mask_identity_defaults.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_1344_broadcast_arrays_depth_limit.py` & `awkward-2.2.4/tests/test_1344_broadcast_arrays_depth_limit.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_1345_avro_reader.py` & `awkward-2.2.4/tests/test_1345_avro_reader.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_1351_is_tuple.py` & `awkward-2.2.4/tests/test_1351_is_tuple.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_1374_to_rdataframe.py` & `awkward-2.2.4/tests/test_1374_to_rdataframe.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_1377_ravel_string.py` & `awkward-2.2.4/tests/test_1377_ravel_string.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_1379_reducers_with_axis_None_and_typetracers.py` & `awkward-2.2.4/tests/test_1379_reducers_with_axis_None_and_typetracers.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_1399_from_jax.py` & `awkward-2.2.4/tests/test_1399_from_jax.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_1399_to_jax.py` & `awkward-2.2.4/tests/test_1399_to_jax.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_1405_slicing_untested_cases.py` & `awkward-2.2.4/tests/test_1405_slicing_untested_cases.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_1415_behaviour_forwarding.py` & `awkward-2.2.4/tests/test_1415_behaviour_forwarding.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_1440_start_v2_to_parquet.py` & `awkward-2.2.4/tests/test_1440_start_v2_to_parquet.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import numpy as np
 import pytest
 
 import awkward as ak
 
 pyarrow = pytest.importorskip("pyarrow")
 pyarrow_parquet = pytest.importorskip("pyarrow.parquet")
+fsspec = pytest.importorskip("fsspec")
 
 to_list = ak.operations.to_list
 
 
 def parquet_round_trip(
     akarray, extensionarray, tmp_path, categorical_as_dictionary=False
 ):
```

### Comparing `awkward-2.2.3/tests/test_1447_jax_autodiff_slices_ufuncs.py` & `awkward-2.2.4/tests/test_1447_jax_autodiff_slices_ufuncs.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_1449_v2_to_json_from_json_functions.py` & `awkward-2.2.4/tests/test_1449_v2_to_json_from_json_functions.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_1453_write_single_records_to_parquet.py` & `awkward-2.2.4/tests/test_1453_write_single_records_to_parquet.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_1473_from_rdataframe.py` & `awkward-2.2.4/tests/test_1473_from_rdataframe.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_1477_generator_entry_type_as_rvec.py` & `awkward-2.2.4/tests/test_1477_generator_entry_type_as_rvec.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_1490_jax_reducers_combinations.py` & `awkward-2.2.4/tests/test_1490_jax_reducers_combinations.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_1502_getitem_jagged_issue1406.py` & `awkward-2.2.4/tests/test_1502_getitem_jagged_issue1406.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_1504_typetracer_like.py` & `awkward-2.2.4/tests/test_1504_typetracer_like.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_1508_awkward_from_rdataframe.py` & `awkward-2.2.4/tests/test_1508_awkward_from_rdataframe.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_1511_set_attribute.py` & `awkward-2.2.4/tests/test_1511_set_attribute.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_1539_isnone_axis_check_issue1417.py` & `awkward-2.2.4/tests/test_1539_isnone_axis_check_issue1417.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_1559_fix_ufuncs_records_1439.py` & `awkward-2.2.4/tests/test_1559_fix_ufuncs_records_1439.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_1565_axis_wrap_if_negative_record.py` & `awkward-2.2.4/tests/test_1565_axis_wrap_if_negative_record.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_1567_fix_longlong_in_Index.py` & `awkward-2.2.4/tests/test_1567_fix_longlong_in_Index.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_1568_fix_lengths_empty_regular_slices.py` & `awkward-2.2.4/tests/test_1568_fix_lengths_empty_regular_slices.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_1586_concatenate_should_preserve_regulararray.py` & `awkward-2.2.4/tests/test_1586_concatenate_should_preserve_regulararray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_1604_preserve_form_in_concatenate.py` & `awkward-2.2.4/tests/test_1604_preserve_form_in_concatenate.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_1607_no_reducers_on_records.py` & `awkward-2.2.4/tests/test_1607_no_reducers_on_records.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_1613_generator_tolayout_records.py` & `awkward-2.2.4/tests/test_1613_generator_tolayout_records.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_1619_from_parquet_empty_field.py` & `awkward-2.2.4/tests/test_1619_from_parquet_empty_field.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 import numpy as np  # noqa: F401
 import pytest
 
 import awkward as ak
 
 pytest.importorskip("pyarrow.parquet")
+pytest.importorskip("fsspec")
 
 
 def test_no_extension(tmp_path):
     array = ak.Array(
         [
             [
                 {"x": 1, "y": 1.1},
```

### Comparing `awkward-2.2.3/tests/test_1620_layout_builders.py` & `awkward-2.2.4/tests/test_1620_layout_builders.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_1625_multiple_columns_from_rdataframe.py` & `awkward-2.2.4/tests/test_1625_multiple_columns_from_rdataframe.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_1642_from_iter_of_tuples.py` & `awkward-2.2.4/tests/test_1642_from_iter_of_tuples.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_1650_Record_to_list_should_listify_itself.py` & `awkward-2.2.4/tests/test_1650_Record_to_list_should_listify_itself.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_1671_categorical_type.py` & `awkward-2.2.4/tests/test_1671_categorical_type.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_1672_broadcast_parameters.py` & `awkward-2.2.4/tests/test_1672_broadcast_parameters.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_1677_array_builder_in_numba.py` & `awkward-2.2.4/tests/test_1677_array_builder_in_numba.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_1685_IndexedArray_project_parameters.py` & `awkward-2.2.4/tests/test_1685_IndexedArray_project_parameters.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_1686_UnionArray_simplified_preserve_parameters.py` & `awkward-2.2.4/tests/test_1686_UnionArray_simplified_preserve_parameters.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_1688_pack_categorical.py` & `awkward-2.2.4/tests/test_1688_pack_categorical.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_1703_fill_none_typetracer.py` & `awkward-2.2.4/tests/test_1703_fill_none_typetracer.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_1707_broadcast_parameters_ufunc.py` & `awkward-2.2.4/tests/test_1707_broadcast_parameters_ufunc.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_1709_ak_array_constructor_behavior.py` & `awkward-2.2.4/tests/test_1709_ak_array_constructor_behavior.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_1747_bytemaskedarray_mergemany.py` & `awkward-2.2.4/tests/test_1747_bytemaskedarray_mergemany.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_1753_indexedarray_merge_kernel.py` & `awkward-2.2.4/tests/test_1753_indexedarray_merge_kernel.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_1762_jax_behavior_support.py` & `awkward-2.2.4/tests/test_1762_jax_behavior_support.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_1764_jax_jacobian.py` & `awkward-2.2.4/tests/test_1764_jax_jacobian.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_1765_add_ioanas_test_of_to_arraylib.py` & `awkward-2.2.4/tests/test_1765_add_ioanas_test_of_to_arraylib.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_1766_record_form_fields.py` & `awkward-2.2.4/tests/test_1766_record_form_fields.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_1781_rdataframe_snapshot.py` & `awkward-2.2.4/tests/test_1781_rdataframe_snapshot.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_1784_reduce_leading_sublist.py` & `awkward-2.2.4/tests/test_1784_reduce_leading_sublist.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_1790_reduce_regulararray.py` & `awkward-2.2.4/tests/test_1790_reduce_regulararray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_1791_reduce_trailing_sublist.py` & `awkward-2.2.4/tests/test_1791_reduce_trailing_sublist.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_1794_run_lengths_empty_sublist.py` & `awkward-2.2.4/tests/test_1794_run_lengths_empty_sublist.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_1829_to_from_rdataframe_bool.py` & `awkward-2.2.4/tests/test_1829_to_from_rdataframe_bool.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_1840_ak_type_to_handle_ndarray_dtype_and_nptypes.py` & `awkward-2.2.4/tests/test_1840_ak_type_to_handle_ndarray_dtype_and_nptypes.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_1847_numpy_array_contiguous.py` & `awkward-2.2.4/tests/test_1847_numpy_array_contiguous.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_1850_bytemasked_array_to_bytemaskedarray.py` & `awkward-2.2.4/tests/test_1850_bytemasked_array_to_bytemaskedarray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_1867_pass_behavior_through_combinations.py` & `awkward-2.2.4/tests/test_1867_pass_behavior_through_combinations.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_1904_drop_none.py` & `awkward-2.2.4/tests/test_1904_drop_none.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_1914_improved_axis_to_posaxis.py` & `awkward-2.2.4/tests/test_1914_improved_axis_to_posaxis.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_1928_replace_simplify_method_with_classmethod_constructor.py` & `awkward-2.2.4/tests/test_1928_replace_simplify_method_with_classmethod_constructor.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_1930_unflatten_counts_checks.py` & `awkward-2.2.4/tests/test_1930_unflatten_counts_checks.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_1936_with_field_broadcasting.py` & `awkward-2.2.4/tests/test_1936_with_field_broadcasting.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_1940_ak_backend.py` & `awkward-2.2.4/tests/test_1940_ak_backend.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_1943_regular_indexing.py` & `awkward-2.2.4/tests/test_1943_regular_indexing.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_1960_awkward_from_rdataframe.py` & `awkward-2.2.4/tests/test_1960_awkward_from_rdataframe.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_1961_ak_without_field.py` & `awkward-2.2.4/tests/test_1961_ak_without_field.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_2020_reduce_axis_none.py` & `awkward-2.2.4/tests/test_2020_reduce_axis_none.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_2021_check_TypeTracerArray_in_ak_where.py` & `awkward-2.2.4/tests/test_2021_check_TypeTracerArray_in_ak_where.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_2023_from_rdataframe.py` & `awkward-2.2.4/tests/test_2023_from_rdataframe.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_2027_add_data_touch_reporting_to_TypeTracerArray.py` & `awkward-2.2.4/tests/test_2027_add_data_touch_reporting_to_TypeTracerArray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_2047_ak_transform_regular_to_jagged.py` & `awkward-2.2.4/tests/test_2047_ak_transform_regular_to_jagged.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_2055_array_builder_check.py` & `awkward-2.2.4/tests/test_2055_array_builder_check.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_2058_merge_numpy_array.py` & `awkward-2.2.4/tests/test_2058_merge_numpy_array.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_2064_fill_none_record.py` & `awkward-2.2.4/tests/test_2064_fill_none_record.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_2067_to_buffers_byteorder.py` & `awkward-2.2.4/tests/test_2067_to_buffers_byteorder.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_2070_to_layout_string.py` & `awkward-2.2.4/tests/test_2070_to_layout_string.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_2071_unflatten_non_packed_counts.py` & `awkward-2.2.4/tests/test_2071_unflatten_non_packed_counts.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_2078_array_function_wrap.py` & `awkward-2.2.4/tests/test_2078_array_function_wrap.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_2082_broadcast_zero_size.py` & `awkward-2.2.4/tests/test_2082_broadcast_zero_size.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_2085_empty_if_typetracer.py` & `awkward-2.2.4/tests/test_2085_empty_if_typetracer.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_2096_ak_scalar_type.py` & `awkward-2.2.4/tests/test_2096_ak_scalar_type.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_2101_pickle_behavior_class.py` & `awkward-2.2.4/tests/test_2101_pickle_behavior_class.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_2104_numpy_merge_option.py` & `awkward-2.2.4/tests/test_2104_numpy_merge_option.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_2106_pickle_class.py` & `awkward-2.2.4/tests/test_2106_pickle_class.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_2108_fill_none_indexed.py` & `awkward-2.2.4/tests/test_2108_fill_none_indexed.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_2115_fix_up_typetracers.py` & `awkward-2.2.4/tests/test_2115_fix_up_typetracers.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_2125_type_of_scalar.py` & `awkward-2.2.4/tests/test_2125_type_of_scalar.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_2150_typetracer_high_level_ufunc.py` & `awkward-2.2.4/tests/test_2150_typetracer_high_level_ufunc.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_2179_parameter_merging_rules.py` & `awkward-2.2.4/tests/test_2179_parameter_merging_rules.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_2185_merge_union_of_records.py` & `awkward-2.2.4/tests/test_2185_merge_union_of_records.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_2188_values_astype_turns_EmptyArray_into_NumpyArray.py` & `awkward-2.2.4/tests/test_2188_values_astype_turns_EmptyArray_into_NumpyArray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_2198_almost_equal.py` & `awkward-2.2.4/tests/test_2198_almost_equal.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_2202_filter_multiple_columns_from_rdataframe.py` & `awkward-2.2.4/tests/test_2202_filter_multiple_columns_from_rdataframe.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_2214_offset_bool_index.py` & `awkward-2.2.4/tests/test_2214_offset_bool_index.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_2226_slice_regulararray_typetracer.py` & `awkward-2.2.4/tests/test_2226_slice_regulararray_typetracer.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_2229_getitem_range_slice.py` & `awkward-2.2.4/tests/test_2229_getitem_range_slice.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_2234_from_rdataframe_keep_order.py` & `awkward-2.2.4/tests/test_2234_from_rdataframe_keep_order.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_2236_merge_union_of_records_option.py` & `awkward-2.2.4/tests/test_2236_merge_union_of_records_option.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_2240_simplify_merge_as_union.py` & `awkward-2.2.4/tests/test_2240_simplify_merge_as_union.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_2246_slice_not_packed.py` & `awkward-2.2.4/tests/test_2246_slice_not_packed.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_2250_full_like_bool.py` & `awkward-2.2.4/tests/test_2250_full_like_bool.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_2258_from_rdataframe_with_arguments.py` & `awkward-2.2.4/tests/test_2258_from_rdataframe_with_arguments.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_2263_to_packed_list.py` & `awkward-2.2.4/tests/test_2263_to_packed_list.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_2267_broadcast_fields.py` & `awkward-2.2.4/tests/test_2267_broadcast_fields.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_2293_unflatten_typetracer.py` & `awkward-2.2.4/tests/test_2293_unflatten_typetracer.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_2296_duplicate_field.py` & `awkward-2.2.4/tests/test_2296_duplicate_field.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_2297_common_backend.py` & `awkward-2.2.4/tests/test_2297_common_backend.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_2305_nep_18_lazy_conversion.py` & `awkward-2.2.4/tests/test_2305_nep_18_lazy_conversion.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_2306_cppyy_git.py` & `awkward-2.2.4/tests/test_2306_cppyy_git.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_2319_from_buffers_array.py` & `awkward-2.2.4/tests/test_2319_from_buffers_array.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_2327_array_interface.py` & `awkward-2.2.4/tests/test_2327_array_interface.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_2329_cartesian_broadcasting_fixes.py` & `awkward-2.2.4/tests/test_2329_cartesian_broadcasting_fixes.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_2349_growablebuffer_in_numba.py` & `awkward-2.2.4/tests/test_2349_growablebuffer_in_numba.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_2354_ufunc_same_backend.py` & `awkward-2.2.4/tests/test_2354_ufunc_same_backend.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_2355_to_backend_record.py` & `awkward-2.2.4/tests/test_2355_to_backend_record.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_2361_typetracer_asarray_nd.py` & `awkward-2.2.4/tests/test_2361_typetracer_asarray_nd.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_2364_empty_list_of_string.py` & `awkward-2.2.4/tests/test_2364_empty_list_of_string.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_2365_enforce_type.py` & `awkward-2.2.4/tests/test_2365_enforce_type.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_2368_type_is_equal.py` & `awkward-2.2.4/tests/test_2368_type_is_equal.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_2373_unzip_touching.py` & `awkward-2.2.4/tests/test_2373_unzip_touching.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_2374_cartesian_touching.py` & `awkward-2.2.4/tests/test_2374_cartesian_touching.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_2385_with_field_empty_record.py` & `awkward-2.2.4/tests/test_2385_with_field_empty_record.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_2395_copy_asarray_touch.py` & `awkward-2.2.4/tests/test_2395_copy_asarray_touch.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_2410_string_broadcast.py` & `awkward-2.2.4/tests/test_2410_string_broadcast.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_2411_cartesian_axis_validation.py` & `awkward-2.2.4/tests/test_2411_cartesian_axis_validation.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_2417_bytemasked_singletons.py` & `awkward-2.2.4/tests/test_2417_bytemasked_singletons.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_2424_almost_equal_union_record.py` & `awkward-2.2.4/tests/test_2424_almost_equal_union_record.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_2425_forms_from_type.py` & `awkward-2.2.4/tests/test_2425_forms_from_type.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_2426_is_equal_to.py` & `awkward-2.2.4/tests/test_2426_is_equal_to.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_2471_flatten_string.py` & `awkward-2.2.4/tests/test_2471_flatten_string.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_2484_reduce_starts_empty.py` & `awkward-2.2.4/tests/test_2484_reduce_starts_empty.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_2487_broadcast_list_offsets.py` & `awkward-2.2.4/tests/test_2487_broadcast_list_offsets.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_2490_reduce_regulararray_positional.py` & `awkward-2.2.4/tests/test_2490_reduce_regulararray_positional.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_2495_concatenate_typetracer.py` & `awkward-2.2.4/tests/test_2495_concatenate_typetracer.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_2501_positional_record_reducer.py` & `awkward-2.2.4/tests/test_2501_positional_record_reducer.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_2503_deprecate_to_numpyform.py` & `awkward-2.2.4/tests/test_2503_deprecate_to_numpyform.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_2512_record_array_carry.py` & `awkward-2.2.4/tests/test_2512_record_array_carry.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/test_2518_datetime_units_as_parameter.py` & `awkward-2.2.4/tests/test_2518_datetime_units_as_parameter.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/samples/list-depths-records-list.parquet` & `awkward-2.2.4/tests/samples/list-depths-records-list.parquet`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/samples/list-depths-records.parquet` & `awkward-2.2.4/tests/samples/list-depths-records.parquet`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/samples/list-depths-strings.parquet` & `awkward-2.2.4/tests/samples/list-depths-strings.parquet`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/samples/list-depths.parquet` & `awkward-2.2.4/tests/samples/list-depths.parquet`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/samples/nonnullable-depths.parquet` & `awkward-2.2.4/tests/samples/nonnullable-depths.parquet`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/samples/nullable-depths.parquet` & `awkward-2.2.4/tests/samples/nullable-depths.parquet`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/samples/nullable-levels.parquet` & `awkward-2.2.4/tests/samples/nullable-levels.parquet`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/samples/nullable-list-depths-records-list.parquet` & `awkward-2.2.4/tests/samples/nullable-list-depths-records-list.parquet`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/samples/nullable-list-depths-records.parquet` & `awkward-2.2.4/tests/samples/nullable-list-depths-records.parquet`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/samples/nullable-list-depths-strings.parquet` & `awkward-2.2.4/tests/samples/nullable-list-depths-strings.parquet`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/samples/nullable-list-depths.parquet` & `awkward-2.2.4/tests/samples/nullable-list-depths.parquet`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/samples/nullable-record-primitives.parquet` & `awkward-2.2.4/tests/samples/nullable-record-primitives.parquet`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/samples/record-primitives.parquet` & `awkward-2.2.4/tests/samples/record-primitives.parquet`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/samples/test-nan-inf.json` & `awkward-2.2.4/tests/samples/test-nan-inf.json`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/samples/test-two-arrays.json` & `awkward-2.2.4/tests/samples/test-two-arrays.json`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests/samples/test.json` & `awkward-2.2.4/tests/samples/test.json`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests-cuda/test_1276_cuda_num.py` & `awkward-2.2.4/tests-cuda/test_1276_cuda_num.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests-cuda/test_1276_cuda_transfers.py` & `awkward-2.2.4/tests-cuda/test_1276_cuda_transfers.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests-cuda/test_1276_cupy_interop.py` & `awkward-2.2.4/tests-cuda/test_1276_cupy_interop.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests-cuda/test_1276_from_cupy.py` & `awkward-2.2.4/tests-cuda/test_1276_from_cupy.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests-cuda/test_1300_same_for_numba_cuda.py` & `awkward-2.2.4/tests-cuda/test_1300_same_for_numba_cuda.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests-cuda/test_1381_check_errors.py` & `awkward-2.2.4/tests-cuda/test_1381_check_errors.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/tests-cuda/test_1809_array_cuda_jit.py` & `awkward-2.2.4/tests-cuda/test_1809_array_cuda_jit.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/.gitignore` & `awkward-2.2.4/.gitignore`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/LICENSE` & `awkward-2.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `awkward-2.2.3/pyproject.toml` & `awkward-2.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "hatchling>=1.10.0",
     "hatch-fancy-pypi-readme"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "awkward"
-version = "2.2.3"
+version = "2.2.4"
 description = "Manipulate JSON-like data with NumPy-like idioms."
 license = { text = "BSD-3-Clause" }
 requires-python = ">=3.7"
 authors = [
     { name = "Jim Pivarski", email = "pivarski@princeton.edu" },
 ]
 classifiers = [
@@ -304,13 +304,14 @@
 
 [tool.ruff.per-file-ignores]
 "dev/*" = ["T20", "TID251"]
 "src/awkward/_connect/*" = ["TID251"]
 "src/awkward/__init__.py" = ["E402", "F401", "F403", "I001"]
 "src/awkward/operations/__init__.py" = ["F403"]
 "src/awkward/_nplikes/*" = ["TID251"]
+"src/awkward/_operators.py" = ["TID251"]
 "tests*/*" = ["T20", "TID251"]
 
 [tool.ruff.flake8-tidy-imports.banned-api]
 "numpy".msg = "Use `numpy = ak._nplikes.Numpy.instance()` instead"
 "jax".msg = "Use `jax = ak._nplikes.Jax.instance()` instead"
 "cupy".msg = "Use `cupy = ak._nplikes.Cupy.instance()` instead"
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 [build-system] requires = [ "hatchling>=1.10.0", "hatch-fancy-pypi-readme" ]
-build-backend = "hatchling.build" [project] name = "awkward" version = "2.2.3"
+build-backend = "hatchling.build" [project] name = "awkward" version = "2.2.4"
 description = "Manipulate JSON-like data with NumPy-like idioms." license =
 { text = "BSD-3-Clause" } requires-python = ">=3.7" authors = [ { name = "Jim
 Pivarski", email = "pivarski@princeton.edu" }, ] classifiers = [ "Development
 Status :: 5 - Production/Stable", "Intended Audience :: Developers", "Intended
 Audience :: Information Technology", "Intended Audience :: Science/Research",
 "License :: OSI Approved :: BSD License", "Operating System :: MacOS :: MacOS
 X", "Operating System :: Microsoft :: Windows", "Operating System :: POSIX ::
@@ -89,12 +89,13 @@
 assignment target "PLW0603", # Using the global statement to update is
 discouraged "PLC1901", # x == "" can be simplified to not x (empty string is
 falsey) ] target-version = "py37" typing-modules = ["awkward._typing"] src =
 ["src"] unfixable = [ "T20", # Removes print statements "F841", # Removes
 unused variables ] external = [] mccabe.max-complexity = 100 [tool.ruff.per-
 file-ignores] "dev/*" = ["T20", "TID251"] "src/awkward/_connect/*" = ["TID251"]
 "src/awkward/__init__.py" = ["E402", "F401", "F403", "I001"] "src/awkward/
-operations/__init__.py" = ["F403"] "src/awkward/_nplikes/*" = ["TID251"]
-"tests*/*" = ["T20", "TID251"] [tool.ruff.flake8-tidy-imports.banned-api]
-"numpy".msg = "Use `numpy = ak._nplikes.Numpy.instance()` instead" "jax".msg =
-"Use `jax = ak._nplikes.Jax.instance()` instead" "cupy".msg = "Use `cupy =
+operations/__init__.py" = ["F403"] "src/awkward/_nplikes/*" = ["TID251"] "src/
+awkward/_operators.py" = ["TID251"] "tests*/*" = ["T20", "TID251"]
+[tool.ruff.flake8-tidy-imports.banned-api] "numpy".msg = "Use `numpy =
+ak._nplikes.Numpy.instance()` instead" "jax".msg = "Use `jax =
+ak._nplikes.Jax.instance()` instead" "cupy".msg = "Use `cupy =
 ak._nplikes.Cupy.instance()` instead"
```

### Comparing `awkward-2.2.3/PKG-INFO` & `awkward-2.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awkward
-Version: 2.2.3
+Version: 2.2.4
 Summary: Manipulate JSON-like data with NumPy-like idioms.
 Project-URL: Bug Tracker, https://github.com/scikit-hep/awkward-1.0/issues
 Project-URL: Chat, https://gitter.im/Scikit-HEP/awkward-array
 Project-URL: Discussions, https://github.com/scikit-hep/awkward-1.0/discussions
 Project-URL: Documentation, https://awkward-array.org
 Project-URL: Homepage, https://github.com/scikit-hep/awkward-1.0
 Project-URL: Releases, https://github.com/scikit-hep/awkward-1.0/releases
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: awkward Version: 2.2.3 Summary: Manipulate JSON-
+Metadata-Version: 2.1 Name: awkward Version: 2.2.4 Summary: Manipulate JSON-
 like data with NumPy-like idioms. Project-URL: Bug Tracker, https://github.com/
 scikit-hep/awkward-1.0/issues Project-URL: Chat, https://gitter.im/Scikit-HEP/
 awkward-array Project-URL: Discussions, https://github.com/scikit-hep/awkward-
 1.0/discussions Project-URL: Documentation, https://awkward-array.org Project-
 URL: Homepage, https://github.com/scikit-hep/awkward-1.0 Project-URL: Releases,
 https://github.com/scikit-hep/awkward-1.0/releases Project-URL: Source Code,
 https://github.com/scikit-hep/awkward-1.0 Author-email: Jim Pivarski
```

