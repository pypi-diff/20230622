# Comparing `tmp/bibat-0.1.6.tar.gz` & `tmp/bibat-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bibat-0.1.6.tar", last modified: Fri Jun  2 14:32:56 2023, max compression
+gzip compressed data, was "bibat-0.1.8.tar", last modified: Thu Jun 22 15:21:46 2023, max compression
```

## Comparing `bibat-0.1.6.tar` & `bibat-0.1.8.tar`

### file list

```diff
@@ -1,136 +1,136 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:32:56.047705 bibat-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-02 14:32:43.000000 bibat-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-02 14:32:43.000000 bibat-0.1.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7753 2023-06-02 14:32:56.047705 bibat-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6840 2023-06-02 14:32:43.000000 bibat-0.1.6/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:32:55.995705 bibat-0.1.6/bibat/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-02 14:32:43.000000 bibat-0.1.6/bibat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-06-02 14:32:43.000000 bibat-0.1.6/bibat/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-06-02 14:32:43.000000 bibat-0.1.6/bibat/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:32:55.991705 bibat-0.1.6/bibat/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:32:55.999705 bibat-0.1.6/bibat/examples/baseball/
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-02 14:32:43.000000 bibat-0.1.6/bibat/examples/baseball/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     5217 2023-06-02 14:32:43.000000 bibat-0.1.6/bibat/examples/baseball/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-06-02 14:32:43.000000 bibat-0.1.6/bibat/examples/baseball/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-06-02 14:32:43.000000 bibat-0.1.6/bibat/examples/baseball/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-06-02 14:32:43.000000 bibat-0.1.6/bibat/examples/baseball/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:32:56.003705 bibat-0.1.6/bibat/examples/baseball/baseball/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-02 14:32:43.000000 bibat-0.1.6/bibat/examples/baseball/baseball/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5891 2023-06-02 14:32:43.000000 bibat-0.1.6/bibat/examples/baseball/baseball/data_preparation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-02 14:32:43.000000 bibat-0.1.6/bibat/examples/baseball/baseball/fetch_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5285 2023-06-02 14:32:43.000000 bibat-0.1.6/bibat/examples/baseball/baseball/fitting_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-06-02 14:32:43.000000 bibat-0.1.6/bibat/examples/baseball/baseball/inference_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)   722180 2023-06-02 14:32:43.000000 bibat-0.1.6/bibat/examples/baseball/baseball/investigate.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-02 14:32:43.000000 bibat-0.1.6/bibat/examples/baseball/baseball/prepare_data.py
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-02 14:32:43.000000 bibat-0.1.6/bibat/examples/baseball/baseball/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-06-02 14:32:43.000000 bibat-0.1.6/bibat/examples/baseball/baseball/sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:32:56.011705 bibat-0.1.6/bibat/examples/baseball/baseball/stan/
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-06-02 14:32:43.000000 bibat-0.1.6/bibat/examples/baseball/baseball/stan/custom_functions.stan
--rwxr-xr-x   0 runner    (1001) docker     (123)  2092164 2023-06-02 14:32:43.000000 bibat-0.1.6/bibat/examples/baseball/baseball/stan/gpareto
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-02 14:32:43.000000 bibat-0.1.6/bibat/examples/baseball/baseball/stan/gpareto.stan
--rwxr-xr-x   0 runner    (1001) docker     (123)  2061251 2023-06-02 14:32:43.000000 bibat-0.1.6/bibat/examples/baseball/baseball/stan/normal
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-06-02 14:32:43.000000 bibat-0.1.6/bibat/examples/baseball/baseball/stan/normal.stan
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-02 14:32:43.000000 bibat-0.1.6/bibat/examples/baseball/baseball/stan/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-06-02 14:32:43.000000 bibat-0.1.6/bibat/examples/baseball/baseball/stan_input_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-06-02 14:32:43.000000 bibat-0.1.6/bibat/examples/baseball/baseball/util.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-02 14:32:43.000000 bibat-0.1.6/bibat/examples/baseball/bibat_version.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:32:55.991705 bibat-0.1.6/bibat/examples/baseball/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:32:56.035705 bibat-0.1.6/bibat/examples/baseball/data/raw/
--rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-06-02 14:32:43.000000 bibat-0.1.6/bibat/examples/baseball/data/raw/2006.csv
--rw-r--r--   0 runner    (1001) docker     (123)  8493039 2023-06-02 14:32:43.000000 bibat-0.1.6/bibat/examples/baseball/data/raw/bdb-apps.csv
--rw-r--r--   0 runner    (1001) docker     (123)  9327402 2023-06-02 14:32:43.000000 bibat-0.1.6/bibat/examples/baseball/data/raw/bdb-main.csv
--rw-r--r--   0 runner    (1001) docker     (123)  1246311 2023-06-02 14:32:43.000000 bibat-0.1.6/bibat/examples/baseball/data/raw/bdb-post.csv
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-02 14:32:43.000000 bibat-0.1.6/bibat/examples/baseball/data/raw/readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:32:56.035705 bibat-0.1.6/bibat/examples/baseball/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-06-02 14:32:43.000000 bibat-0.1.6/bibat/examples/baseball/docs/bibliography.bib
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:32:56.035705 bibat-0.1.6/bibat/examples/baseball/docs/img/
--rw-r--r--   0 runner    (1001) docker     (123)   206003 2023-06-02 14:32:43.000000 bibat-0.1.6/bibat/examples/baseball/docs/img/example.png
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-02 14:32:43.000000 bibat-0.1.6/bibat/examples/baseball/docs/img/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)  1461954 2023-06-02 14:32:43.000000 bibat-0.1.6/bibat/examples/baseball/docs/report.html
--rw-r--r--   0 runner    (1001) docker     (123)    18579 2023-06-02 14:32:43.000000 bibat-0.1.6/bibat/examples/baseball/docs/report.qmd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:32:55.991705 bibat-0.1.6/bibat/examples/baseball/inferences/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:32:56.035705 bibat-0.1.6/bibat/examples/baseball/inferences/gpareto2006/
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-02 14:32:43.000000 bibat-0.1.6/bibat/examples/baseball/inferences/gpareto2006/config.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:32:56.035705 bibat-0.1.6/bibat/examples/baseball/inferences/gparetobdb/
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-02 14:32:43.000000 bibat-0.1.6/bibat/examples/baseball/inferences/gparetobdb/config.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:32:56.035705 bibat-0.1.6/bibat/examples/baseball/inferences/normal2006/
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-06-02 14:32:43.000000 bibat-0.1.6/bibat/examples/baseball/inferences/normal2006/config.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:32:56.035705 bibat-0.1.6/bibat/examples/baseball/inferences/normalbdb/
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-02 14:32:43.000000 bibat-0.1.6/bibat/examples/baseball/inferences/normalbdb/config.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:32:56.039705 bibat-0.1.6/bibat/examples/baseball/plots/
--rw-r--r--   0 runner    (1001) docker     (123)    49023 2023-06-02 14:32:43.000000 bibat-0.1.6/bibat/examples/baseball/plots/posterior_ll_comparison.png
--rw-r--r--   0 runner    (1001) docker     (123)    78042 2023-06-02 14:32:43.000000 bibat-0.1.6/bibat/examples/baseball/plots/posterior_predictive_comparison.png
--rw-r--r--   0 runner    (1001) docker     (123)   140008 2023-06-02 14:32:43.000000 bibat-0.1.6/bibat/examples/baseball/plots/posterior_quantiles.png
--rw-r--r--   0 runner    (1001) docker     (123)   166694 2023-06-02 14:32:43.000000 bibat-0.1.6/bibat/examples/baseball/plots/prior_quantiles.png
--rw-r--r--   0 runner    (1001) docker     (123)    49296 2023-06-02 14:32:43.000000 bibat-0.1.6/bibat/examples/baseball/plots/raw_data.png
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-06-02 14:32:43.000000 bibat-0.1.6/bibat/examples/baseball/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:32:56.039705 bibat-0.1.6/bibat/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-06-02 14:32:43.000000 bibat-0.1.6/bibat/hooks/post_gen_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-06-02 14:32:43.000000 bibat-0.1.6/bibat/wizarding.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:32:56.039705 bibat-0.1.6/bibat/{{cookiecutter.repo_name}}/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:32:55.995705 bibat-0.1.6/bibat/{{cookiecutter.repo_name}}/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:32:56.039705 bibat-0.1.6/bibat/{{cookiecutter.repo_name}}/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-02 14:32:43.000000 bibat-0.1.6/bibat/{{cookiecutter.repo_name}}/.github/workflows/run_pytest.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-02 14:32:43.000000 bibat-0.1.6/bibat/{{cookiecutter.repo_name}}/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-06-02 14:32:43.000000 bibat-0.1.6/bibat/{{cookiecutter.repo_name}}/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-06-02 14:32:43.000000 bibat-0.1.6/bibat/{{cookiecutter.repo_name}}/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-06-02 14:32:43.000000 bibat-0.1.6/bibat/{{cookiecutter.repo_name}}/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-02 14:32:43.000000 bibat-0.1.6/bibat/{{cookiecutter.repo_name}}/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-02 14:32:43.000000 bibat-0.1.6/bibat/{{cookiecutter.repo_name}}/bibat_version.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:32:55.995705 bibat-0.1.6/bibat/{{cookiecutter.repo_name}}/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:32:56.039705 bibat-0.1.6/bibat/{{cookiecutter.repo_name}}/data/raw/
--rw-r--r--   0 runner    (1001) docker     (123)     4887 2023-06-02 14:32:43.000000 bibat-0.1.6/bibat/{{cookiecutter.repo_name}}/data/raw/raw_measurements.csv
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-02 14:32:43.000000 bibat-0.1.6/bibat/{{cookiecutter.repo_name}}/data/raw/readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:32:56.043705 bibat-0.1.6/bibat/{{cookiecutter.repo_name}}/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:32:56.043705 bibat-0.1.6/bibat/{{cookiecutter.repo_name}}/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-02 14:32:43.000000 bibat-0.1.6/bibat/{{cookiecutter.repo_name}}/docs/_static/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-06-02 14:32:43.000000 bibat-0.1.6/bibat/{{cookiecutter.repo_name}}/docs/bibliography.bib
--rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-06-02 14:32:43.000000 bibat-0.1.6/bibat/{{cookiecutter.repo_name}}/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:32:56.043705 bibat-0.1.6/bibat/{{cookiecutter.repo_name}}/docs/img/
--rw-r--r--   0 runner    (1001) docker     (123)   206003 2023-06-02 14:32:43.000000 bibat-0.1.6/bibat/{{cookiecutter.repo_name}}/docs/img/example.png
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-02 14:32:43.000000 bibat-0.1.6/bibat/{{cookiecutter.repo_name}}/docs/img/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-06-02 14:32:43.000000 bibat-0.1.6/bibat/{{cookiecutter.repo_name}}/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    18507 2023-06-02 14:32:43.000000 bibat-0.1.6/bibat/{{cookiecutter.repo_name}}/docs/report.html
--rw-r--r--   0 runner    (1001) docker     (123)   267406 2023-06-02 14:32:43.000000 bibat-0.1.6/bibat/{{cookiecutter.repo_name}}/docs/report.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-06-02 14:32:43.000000 bibat-0.1.6/bibat/{{cookiecutter.repo_name}}/docs/report.qmd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:32:55.995705 bibat-0.1.6/bibat/{{cookiecutter.repo_name}}/inferences/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:32:56.043705 bibat-0.1.6/bibat/{{cookiecutter.repo_name}}/inferences/fake_interaction/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-02 14:32:43.000000 bibat-0.1.6/bibat/{{cookiecutter.repo_name}}/inferences/fake_interaction/config.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:32:56.043705 bibat-0.1.6/bibat/{{cookiecutter.repo_name}}/inferences/interaction/
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-06-02 14:32:43.000000 bibat-0.1.6/bibat/{{cookiecutter.repo_name}}/inferences/interaction/config.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:32:56.043705 bibat-0.1.6/bibat/{{cookiecutter.repo_name}}/inferences/no_interaction/
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-06-02 14:32:43.000000 bibat-0.1.6/bibat/{{cookiecutter.repo_name}}/inferences/no_interaction/config.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:32:56.043705 bibat-0.1.6/bibat/{{cookiecutter.repo_name}}/plots/
--rw-r--r--   0 runner    (1001) docker     (123)    46184 2023-06-02 14:32:43.000000 bibat-0.1.6/bibat/{{cookiecutter.repo_name}}/plots/posterior_ll_comparison.png
--rw-r--r--   0 runner    (1001) docker     (123)    78410 2023-06-02 14:32:43.000000 bibat-0.1.6/bibat/{{cookiecutter.repo_name}}/plots/posterior_predictive_comparison.png
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-06-02 14:32:43.000000 bibat-0.1.6/bibat/{{cookiecutter.repo_name}}/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:32:55.995705 bibat-0.1.6/bibat/{{cookiecutter.repo_name}}/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:32:56.043705 bibat-0.1.6/bibat/{{cookiecutter.repo_name}}/tests/test_integration/
--rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-06-02 14:32:43.000000 bibat-0.1.6/bibat/{{cookiecutter.repo_name}}/tests/test_integration/test_data_preparation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:32:56.043705 bibat-0.1.6/bibat/{{cookiecutter.repo_name}}/tests/test_unit/
--rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-06-02 14:32:43.000000 bibat-0.1.6/bibat/{{cookiecutter.repo_name}}/tests/test_unit/test_inference_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-06-02 14:32:43.000000 bibat-0.1.6/bibat/{{cookiecutter.repo_name}}/tests/test_unit/test_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:32:56.047705 bibat-0.1.6/bibat/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-02 14:32:43.000000 bibat-0.1.6/bibat/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5459 2023-06-02 14:32:43.000000 bibat-0.1.6/bibat/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}/data_preparation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5262 2023-06-02 14:32:43.000000 bibat-0.1.6/bibat/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}/fitting_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     4561 2023-06-02 14:32:43.000000 bibat-0.1.6/bibat/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}/inference_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)   428248 2023-06-02 14:32:43.000000 bibat-0.1.6/bibat/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}/investigate.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-02 14:32:43.000000 bibat-0.1.6/bibat/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}/prepare_data.py
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-02 14:32:43.000000 bibat-0.1.6/bibat/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-06-02 14:32:43.000000 bibat-0.1.6/bibat/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}/sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:32:56.047705 bibat-0.1.6/bibat/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}/stan/
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-02 14:32:43.000000 bibat-0.1.6/bibat/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}/stan/custom_functions.stan
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-06-02 14:32:43.000000 bibat-0.1.6/bibat/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}/stan/multilevel-linear-regression.stan
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-02 14:32:43.000000 bibat-0.1.6/bibat/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}/stan/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-06-02 14:32:43.000000 bibat-0.1.6/bibat/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}/stan_input_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-06-02 14:32:43.000000 bibat-0.1.6/bibat/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:32:55.999705 bibat-0.1.6/bibat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7753 2023-06-02 14:32:55.000000 bibat-0.1.6/bibat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4925 2023-06-02 14:32:55.000000 bibat-0.1.6/bibat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:32:55.000000 bibat-0.1.6/bibat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-02 14:32:55.000000 bibat-0.1.6/bibat.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-02 14:32:55.000000 bibat-0.1.6/bibat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-02 14:32:55.000000 bibat-0.1.6/bibat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-06-02 14:32:43.000000 bibat-0.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 14:32:56.047705 bibat-0.1.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:21:46.798131 bibat-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-22 15:21:31.000000 bibat-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-22 15:21:31.000000 bibat-0.1.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7753 2023-06-22 15:21:46.798131 bibat-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6840 2023-06-22 15:21:31.000000 bibat-0.1.8/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:21:46.750130 bibat-0.1.8/bibat/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-22 15:21:31.000000 bibat-0.1.8/bibat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-06-22 15:21:31.000000 bibat-0.1.8/bibat/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-22 15:21:31.000000 bibat-0.1.8/bibat/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:21:46.742130 bibat-0.1.8/bibat/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:21:46.754130 bibat-0.1.8/bibat/examples/baseball/
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-22 15:21:31.000000 bibat-0.1.8/bibat/examples/baseball/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     5217 2023-06-22 15:21:31.000000 bibat-0.1.8/bibat/examples/baseball/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-06-22 15:21:31.000000 bibat-0.1.8/bibat/examples/baseball/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-06-22 15:21:31.000000 bibat-0.1.8/bibat/examples/baseball/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-06-22 15:21:31.000000 bibat-0.1.8/bibat/examples/baseball/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:21:46.754130 bibat-0.1.8/bibat/examples/baseball/baseball/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-22 15:21:31.000000 bibat-0.1.8/bibat/examples/baseball/baseball/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5891 2023-06-22 15:21:31.000000 bibat-0.1.8/bibat/examples/baseball/baseball/data_preparation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-22 15:21:31.000000 bibat-0.1.8/bibat/examples/baseball/baseball/fetch_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5285 2023-06-22 15:21:31.000000 bibat-0.1.8/bibat/examples/baseball/baseball/fitting_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-06-22 15:21:31.000000 bibat-0.1.8/bibat/examples/baseball/baseball/inference_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)   722180 2023-06-22 15:21:31.000000 bibat-0.1.8/bibat/examples/baseball/baseball/investigate.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-22 15:21:31.000000 bibat-0.1.8/bibat/examples/baseball/baseball/prepare_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-22 15:21:31.000000 bibat-0.1.8/bibat/examples/baseball/baseball/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-06-22 15:21:31.000000 bibat-0.1.8/bibat/examples/baseball/baseball/sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:21:46.762130 bibat-0.1.8/bibat/examples/baseball/baseball/stan/
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-06-22 15:21:31.000000 bibat-0.1.8/bibat/examples/baseball/baseball/stan/custom_functions.stan
+-rwxr-xr-x   0 runner    (1001) docker     (123)  2092164 2023-06-22 15:21:31.000000 bibat-0.1.8/bibat/examples/baseball/baseball/stan/gpareto
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-22 15:21:31.000000 bibat-0.1.8/bibat/examples/baseball/baseball/stan/gpareto.stan
+-rwxr-xr-x   0 runner    (1001) docker     (123)  2061251 2023-06-22 15:21:31.000000 bibat-0.1.8/bibat/examples/baseball/baseball/stan/normal
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-06-22 15:21:31.000000 bibat-0.1.8/bibat/examples/baseball/baseball/stan/normal.stan
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-22 15:21:31.000000 bibat-0.1.8/bibat/examples/baseball/baseball/stan/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-06-22 15:21:31.000000 bibat-0.1.8/bibat/examples/baseball/baseball/stan_input_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-06-22 15:21:31.000000 bibat-0.1.8/bibat/examples/baseball/baseball/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-22 15:21:31.000000 bibat-0.1.8/bibat/examples/baseball/bibat_version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:21:46.742130 bibat-0.1.8/bibat/examples/baseball/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:21:46.782131 bibat-0.1.8/bibat/examples/baseball/data/raw/
+-rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-06-22 15:21:31.000000 bibat-0.1.8/bibat/examples/baseball/data/raw/2006.csv
+-rw-r--r--   0 runner    (1001) docker     (123)  8493039 2023-06-22 15:21:31.000000 bibat-0.1.8/bibat/examples/baseball/data/raw/bdb-apps.csv
+-rw-r--r--   0 runner    (1001) docker     (123)  9327402 2023-06-22 15:21:31.000000 bibat-0.1.8/bibat/examples/baseball/data/raw/bdb-main.csv
+-rw-r--r--   0 runner    (1001) docker     (123)  1246311 2023-06-22 15:21:31.000000 bibat-0.1.8/bibat/examples/baseball/data/raw/bdb-post.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-22 15:21:31.000000 bibat-0.1.8/bibat/examples/baseball/data/raw/readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:21:46.786131 bibat-0.1.8/bibat/examples/baseball/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-06-22 15:21:31.000000 bibat-0.1.8/bibat/examples/baseball/docs/bibliography.bib
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:21:46.786131 bibat-0.1.8/bibat/examples/baseball/docs/img/
+-rw-r--r--   0 runner    (1001) docker     (123)   206003 2023-06-22 15:21:31.000000 bibat-0.1.8/bibat/examples/baseball/docs/img/example.png
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-22 15:21:31.000000 bibat-0.1.8/bibat/examples/baseball/docs/img/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)  1461954 2023-06-22 15:21:31.000000 bibat-0.1.8/bibat/examples/baseball/docs/report.html
+-rw-r--r--   0 runner    (1001) docker     (123)    18579 2023-06-22 15:21:31.000000 bibat-0.1.8/bibat/examples/baseball/docs/report.qmd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:21:46.746130 bibat-0.1.8/bibat/examples/baseball/inferences/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:21:46.786131 bibat-0.1.8/bibat/examples/baseball/inferences/gpareto2006/
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-22 15:21:31.000000 bibat-0.1.8/bibat/examples/baseball/inferences/gpareto2006/config.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:21:46.786131 bibat-0.1.8/bibat/examples/baseball/inferences/gparetobdb/
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-22 15:21:31.000000 bibat-0.1.8/bibat/examples/baseball/inferences/gparetobdb/config.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:21:46.786131 bibat-0.1.8/bibat/examples/baseball/inferences/normal2006/
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-06-22 15:21:31.000000 bibat-0.1.8/bibat/examples/baseball/inferences/normal2006/config.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:21:46.786131 bibat-0.1.8/bibat/examples/baseball/inferences/normalbdb/
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-22 15:21:31.000000 bibat-0.1.8/bibat/examples/baseball/inferences/normalbdb/config.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:21:46.786131 bibat-0.1.8/bibat/examples/baseball/plots/
+-rw-r--r--   0 runner    (1001) docker     (123)    49023 2023-06-22 15:21:31.000000 bibat-0.1.8/bibat/examples/baseball/plots/posterior_ll_comparison.png
+-rw-r--r--   0 runner    (1001) docker     (123)    78042 2023-06-22 15:21:31.000000 bibat-0.1.8/bibat/examples/baseball/plots/posterior_predictive_comparison.png
+-rw-r--r--   0 runner    (1001) docker     (123)   140008 2023-06-22 15:21:31.000000 bibat-0.1.8/bibat/examples/baseball/plots/posterior_quantiles.png
+-rw-r--r--   0 runner    (1001) docker     (123)   166694 2023-06-22 15:21:31.000000 bibat-0.1.8/bibat/examples/baseball/plots/prior_quantiles.png
+-rw-r--r--   0 runner    (1001) docker     (123)    49296 2023-06-22 15:21:31.000000 bibat-0.1.8/bibat/examples/baseball/plots/raw_data.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-06-22 15:21:31.000000 bibat-0.1.8/bibat/examples/baseball/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:21:46.786131 bibat-0.1.8/bibat/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-06-22 15:21:31.000000 bibat-0.1.8/bibat/hooks/post_gen_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-06-22 15:21:31.000000 bibat-0.1.8/bibat/wizarding.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:21:46.790131 bibat-0.1.8/bibat/{{cookiecutter.repo_name}}/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:21:46.746130 bibat-0.1.8/bibat/{{cookiecutter.repo_name}}/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:21:46.790131 bibat-0.1.8/bibat/{{cookiecutter.repo_name}}/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-22 15:21:31.000000 bibat-0.1.8/bibat/{{cookiecutter.repo_name}}/.github/workflows/run_pytest.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-22 15:21:31.000000 bibat-0.1.8/bibat/{{cookiecutter.repo_name}}/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-06-22 15:21:31.000000 bibat-0.1.8/bibat/{{cookiecutter.repo_name}}/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-06-22 15:21:31.000000 bibat-0.1.8/bibat/{{cookiecutter.repo_name}}/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-06-22 15:21:31.000000 bibat-0.1.8/bibat/{{cookiecutter.repo_name}}/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-22 15:21:31.000000 bibat-0.1.8/bibat/{{cookiecutter.repo_name}}/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-22 15:21:31.000000 bibat-0.1.8/bibat/{{cookiecutter.repo_name}}/bibat_version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:21:46.746130 bibat-0.1.8/bibat/{{cookiecutter.repo_name}}/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:21:46.790131 bibat-0.1.8/bibat/{{cookiecutter.repo_name}}/data/raw/
+-rw-r--r--   0 runner    (1001) docker     (123)     4887 2023-06-22 15:21:31.000000 bibat-0.1.8/bibat/{{cookiecutter.repo_name}}/data/raw/raw_measurements.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-22 15:21:31.000000 bibat-0.1.8/bibat/{{cookiecutter.repo_name}}/data/raw/readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:21:46.790131 bibat-0.1.8/bibat/{{cookiecutter.repo_name}}/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:21:46.790131 bibat-0.1.8/bibat/{{cookiecutter.repo_name}}/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-22 15:21:31.000000 bibat-0.1.8/bibat/{{cookiecutter.repo_name}}/docs/_static/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-06-22 15:21:31.000000 bibat-0.1.8/bibat/{{cookiecutter.repo_name}}/docs/bibliography.bib
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-06-22 15:21:31.000000 bibat-0.1.8/bibat/{{cookiecutter.repo_name}}/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:21:46.790131 bibat-0.1.8/bibat/{{cookiecutter.repo_name}}/docs/img/
+-rw-r--r--   0 runner    (1001) docker     (123)   206003 2023-06-22 15:21:31.000000 bibat-0.1.8/bibat/{{cookiecutter.repo_name}}/docs/img/example.png
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-22 15:21:31.000000 bibat-0.1.8/bibat/{{cookiecutter.repo_name}}/docs/img/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-06-22 15:21:31.000000 bibat-0.1.8/bibat/{{cookiecutter.repo_name}}/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    18507 2023-06-22 15:21:31.000000 bibat-0.1.8/bibat/{{cookiecutter.repo_name}}/docs/report.html
+-rw-r--r--   0 runner    (1001) docker     (123)   267406 2023-06-22 15:21:31.000000 bibat-0.1.8/bibat/{{cookiecutter.repo_name}}/docs/report.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-06-22 15:21:31.000000 bibat-0.1.8/bibat/{{cookiecutter.repo_name}}/docs/report.qmd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:21:46.746130 bibat-0.1.8/bibat/{{cookiecutter.repo_name}}/inferences/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:21:46.790131 bibat-0.1.8/bibat/{{cookiecutter.repo_name}}/inferences/fake_interaction/
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-06-22 15:21:31.000000 bibat-0.1.8/bibat/{{cookiecutter.repo_name}}/inferences/fake_interaction/config.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:21:46.790131 bibat-0.1.8/bibat/{{cookiecutter.repo_name}}/inferences/interaction/
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-22 15:21:31.000000 bibat-0.1.8/bibat/{{cookiecutter.repo_name}}/inferences/interaction/config.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:21:46.790131 bibat-0.1.8/bibat/{{cookiecutter.repo_name}}/inferences/no_interaction/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-22 15:21:31.000000 bibat-0.1.8/bibat/{{cookiecutter.repo_name}}/inferences/no_interaction/config.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:21:46.790131 bibat-0.1.8/bibat/{{cookiecutter.repo_name}}/plots/
+-rw-r--r--   0 runner    (1001) docker     (123)    46184 2023-06-22 15:21:31.000000 bibat-0.1.8/bibat/{{cookiecutter.repo_name}}/plots/posterior_ll_comparison.png
+-rw-r--r--   0 runner    (1001) docker     (123)    78410 2023-06-22 15:21:31.000000 bibat-0.1.8/bibat/{{cookiecutter.repo_name}}/plots/posterior_predictive_comparison.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-06-22 15:21:31.000000 bibat-0.1.8/bibat/{{cookiecutter.repo_name}}/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:21:46.746130 bibat-0.1.8/bibat/{{cookiecutter.repo_name}}/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:21:46.794131 bibat-0.1.8/bibat/{{cookiecutter.repo_name}}/tests/test_integration/
+-rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-06-22 15:21:31.000000 bibat-0.1.8/bibat/{{cookiecutter.repo_name}}/tests/test_integration/test_data_preparation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:21:46.794131 bibat-0.1.8/bibat/{{cookiecutter.repo_name}}/tests/test_unit/
+-rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-06-22 15:21:31.000000 bibat-0.1.8/bibat/{{cookiecutter.repo_name}}/tests/test_unit/test_inference_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-06-22 15:21:31.000000 bibat-0.1.8/bibat/{{cookiecutter.repo_name}}/tests/test_unit/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:21:46.794131 bibat-0.1.8/bibat/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-22 15:21:31.000000 bibat-0.1.8/bibat/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5459 2023-06-22 15:21:31.000000 bibat-0.1.8/bibat/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}/data_preparation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5262 2023-06-22 15:21:31.000000 bibat-0.1.8/bibat/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}/fitting_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4561 2023-06-22 15:21:31.000000 bibat-0.1.8/bibat/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}/inference_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)   428248 2023-06-22 15:21:31.000000 bibat-0.1.8/bibat/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}/investigate.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-22 15:21:31.000000 bibat-0.1.8/bibat/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}/prepare_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-22 15:21:31.000000 bibat-0.1.8/bibat/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-06-22 15:21:31.000000 bibat-0.1.8/bibat/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}/sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:21:46.794131 bibat-0.1.8/bibat/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}/stan/
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-22 15:21:31.000000 bibat-0.1.8/bibat/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}/stan/custom_functions.stan
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-06-22 15:21:31.000000 bibat-0.1.8/bibat/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}/stan/multilevel-linear-regression.stan
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-22 15:21:31.000000 bibat-0.1.8/bibat/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}/stan/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-06-22 15:21:31.000000 bibat-0.1.8/bibat/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}/stan_input_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-06-22 15:21:31.000000 bibat-0.1.8/bibat/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:21:46.750130 bibat-0.1.8/bibat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7753 2023-06-22 15:21:46.000000 bibat-0.1.8/bibat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4925 2023-06-22 15:21:46.000000 bibat-0.1.8/bibat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 15:21:46.000000 bibat-0.1.8/bibat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-22 15:21:46.000000 bibat-0.1.8/bibat.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-22 15:21:46.000000 bibat-0.1.8/bibat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-22 15:21:46.000000 bibat-0.1.8/bibat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-06-22 15:21:31.000000 bibat-0.1.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 15:21:46.798131 bibat-0.1.8/setup.cfg
```

### Comparing `bibat-0.1.6/LICENSE` & `bibat-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `bibat-0.1.6/PKG-INFO` & `bibat-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bibat
-Version: 0.1.6
+Version: 0.1.8
 Summary: Batteries-included Bayesian analysis template
 Author-email: Teddy Groves <tedgro@dtu.dk>
 License: GNU General Public License version 3
 Project-URL: homepage, https://github.com/teddygroves/bibat
 Project-URL: download, https://pypi.org/project/bibat
 Project-URL: documentation, https://bibat.readthedocs.io/
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `bibat-0.1.6/README.rst` & `bibat-0.1.8/README.rst`

 * *Files identical despite different names*

### Comparing `bibat-0.1.6/bibat/cli.py` & `bibat-0.1.8/bibat/cli.py`

 * *Files identical despite different names*

### Comparing `bibat-0.1.6/bibat/cookiecutter.json` & `bibat-0.1.8/bibat/cookiecutter.json`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9166666666666666%*

 * *Differences: {"'n_iter_default'": "'1000'"}*

```diff
@@ -7,14 +7,15 @@
     "create_tests_directory": "y",
     "description": "A short description of the project.",
     "docs_format": [
         "Quarto",
         "Sphinx",
         "No docs"
     ],
+    "n_iter_default": "1000",
     "open_source_license": [
         "MIT",
         "BSD-3-Clause",
         "No license file"
     ],
     "project_name": "project_name",
     "repo_name": "{{ cookiecutter.project_name.lower().replace(' ', '_') }}"
```

### Comparing `bibat-0.1.6/bibat/examples/baseball/.gitignore` & `bibat-0.1.8/bibat/examples/baseball/.gitignore`

 * *Files identical despite different names*

### Comparing `bibat-0.1.6/bibat/examples/baseball/CODE_OF_CONDUCT.md` & `bibat-0.1.8/bibat/examples/baseball/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `bibat-0.1.6/bibat/examples/baseball/LICENSE` & `bibat-0.1.8/bibat/examples/baseball/LICENSE`

 * *Files identical despite different names*

### Comparing `bibat-0.1.6/bibat/examples/baseball/Makefile` & `bibat-0.1.8/bibat/examples/baseball/Makefile`

 * *Files identical despite different names*

### Comparing `bibat-0.1.6/bibat/examples/baseball/README.md` & `bibat-0.1.8/bibat/examples/baseball/README.md`

 * *Files identical despite different names*

### Comparing `bibat-0.1.6/bibat/examples/baseball/baseball/data_preparation.py` & `bibat-0.1.8/bibat/examples/baseball/baseball/data_preparation.py`

 * *Files identical despite different names*

### Comparing `bibat-0.1.6/bibat/examples/baseball/baseball/fetch_data.py` & `bibat-0.1.8/bibat/examples/baseball/baseball/fetch_data.py`

 * *Files identical despite different names*

### Comparing `bibat-0.1.6/bibat/examples/baseball/baseball/fitting_mode.py` & `bibat-0.1.8/bibat/examples/baseball/baseball/fitting_mode.py`

 * *Files identical despite different names*

### Comparing `bibat-0.1.6/bibat/examples/baseball/baseball/inference_configuration.py` & `bibat-0.1.8/bibat/examples/baseball/baseball/inference_configuration.py`

 * *Files identical despite different names*

### Comparing `bibat-0.1.6/bibat/examples/baseball/baseball/investigate.ipynb` & `bibat-0.1.8/bibat/examples/baseball/baseball/investigate.ipynb`

 * *Files identical despite different names*

### Comparing `bibat-0.1.6/bibat/examples/baseball/baseball/sample.py` & `bibat-0.1.8/bibat/examples/baseball/baseball/sample.py`

 * *Files identical despite different names*

### Comparing `bibat-0.1.6/bibat/examples/baseball/baseball/stan/custom_functions.stan` & `bibat-0.1.8/bibat/examples/baseball/baseball/stan/custom_functions.stan`

 * *Files identical despite different names*

### Comparing `bibat-0.1.6/bibat/examples/baseball/baseball/stan/gpareto` & `bibat-0.1.8/bibat/examples/baseball/baseball/stan/gpareto`

 * *Files identical despite different names*

### Comparing `bibat-0.1.6/bibat/examples/baseball/baseball/stan/gpareto.stan` & `bibat-0.1.8/bibat/examples/baseball/baseball/stan/gpareto.stan`

 * *Files identical despite different names*

### Comparing `bibat-0.1.6/bibat/examples/baseball/baseball/stan/normal` & `bibat-0.1.8/bibat/examples/baseball/baseball/stan/normal`

 * *Files identical despite different names*

### Comparing `bibat-0.1.6/bibat/examples/baseball/baseball/stan/normal.stan` & `bibat-0.1.8/bibat/examples/baseball/baseball/stan/normal.stan`

 * *Files identical despite different names*

### Comparing `bibat-0.1.6/bibat/examples/baseball/baseball/stan_input_functions.py` & `bibat-0.1.8/bibat/examples/baseball/baseball/stan_input_functions.py`

 * *Files identical despite different names*

### Comparing `bibat-0.1.6/bibat/examples/baseball/baseball/util.py` & `bibat-0.1.8/bibat/examples/baseball/baseball/util.py`

 * *Files identical despite different names*

### Comparing `bibat-0.1.6/bibat/examples/baseball/data/raw/2006.csv` & `bibat-0.1.8/bibat/examples/baseball/data/raw/2006.csv`

 * *Files identical despite different names*

### Comparing `bibat-0.1.6/bibat/examples/baseball/data/raw/bdb-apps.csv` & `bibat-0.1.8/bibat/examples/baseball/data/raw/bdb-apps.csv`

 * *Files identical despite different names*

### Comparing `bibat-0.1.6/bibat/examples/baseball/data/raw/bdb-main.csv` & `bibat-0.1.8/bibat/examples/baseball/data/raw/bdb-main.csv`

 * *Files identical despite different names*

### Comparing `bibat-0.1.6/bibat/examples/baseball/data/raw/bdb-post.csv` & `bibat-0.1.8/bibat/examples/baseball/data/raw/bdb-post.csv`

 * *Files identical despite different names*

### Comparing `bibat-0.1.6/bibat/examples/baseball/docs/bibliography.bib` & `bibat-0.1.8/bibat/examples/baseball/docs/bibliography.bib`

 * *Files identical despite different names*

### Comparing `bibat-0.1.6/bibat/examples/baseball/docs/img/example.png` & `bibat-0.1.8/bibat/examples/baseball/docs/img/example.png`

 * *Files identical despite different names*

### Comparing `bibat-0.1.6/bibat/examples/baseball/docs/report.html` & `bibat-0.1.8/bibat/examples/baseball/docs/report.html`

 * *Files identical despite different names*

### Comparing `bibat-0.1.6/bibat/examples/baseball/docs/report.qmd` & `bibat-0.1.8/bibat/examples/baseball/docs/report.qmd`

 * *Files identical despite different names*

### Comparing `bibat-0.1.6/bibat/examples/baseball/plots/posterior_ll_comparison.png` & `bibat-0.1.8/bibat/examples/baseball/plots/posterior_ll_comparison.png`

 * *Files identical despite different names*

### Comparing `bibat-0.1.6/bibat/examples/baseball/plots/posterior_predictive_comparison.png` & `bibat-0.1.8/bibat/examples/baseball/plots/posterior_predictive_comparison.png`

 * *Files identical despite different names*

### Comparing `bibat-0.1.6/bibat/examples/baseball/plots/posterior_quantiles.png` & `bibat-0.1.8/bibat/examples/baseball/plots/posterior_quantiles.png`

 * *Files identical despite different names*

### Comparing `bibat-0.1.6/bibat/examples/baseball/plots/prior_quantiles.png` & `bibat-0.1.8/bibat/examples/baseball/plots/prior_quantiles.png`

 * *Files identical despite different names*

### Comparing `bibat-0.1.6/bibat/examples/baseball/plots/raw_data.png` & `bibat-0.1.8/bibat/examples/baseball/plots/raw_data.png`

 * *Files identical despite different names*

### Comparing `bibat-0.1.6/bibat/examples/baseball/pyproject.toml` & `bibat-0.1.8/bibat/examples/baseball/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bibat-0.1.6/bibat/hooks/post_gen_project.py` & `bibat-0.1.8/bibat/hooks/post_gen_project.py`

 * *Files identical despite different names*

### Comparing `bibat-0.1.6/bibat/wizarding.py` & `bibat-0.1.8/bibat/wizarding.py`

 * *Files identical despite different names*

### Comparing `bibat-0.1.6/bibat/{{cookiecutter.repo_name}}/.github/workflows/run_pytest.yml` & `bibat-0.1.8/bibat/{{cookiecutter.repo_name}}/.github/workflows/run_pytest.yml`

 * *Files identical despite different names*

### Comparing `bibat-0.1.6/bibat/{{cookiecutter.repo_name}}/.gitignore` & `bibat-0.1.8/bibat/{{cookiecutter.repo_name}}/.gitignore`

 * *Files identical despite different names*

### Comparing `bibat-0.1.6/bibat/{{cookiecutter.repo_name}}/CODE_OF_CONDUCT.md` & `bibat-0.1.8/bibat/{{cookiecutter.repo_name}}/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `bibat-0.1.6/bibat/{{cookiecutter.repo_name}}/LICENSE` & `bibat-0.1.8/bibat/{{cookiecutter.repo_name}}/LICENSE`

 * *Files identical despite different names*

### Comparing `bibat-0.1.6/bibat/{{cookiecutter.repo_name}}/Makefile` & `bibat-0.1.8/bibat/{{cookiecutter.repo_name}}/Makefile`

 * *Files 0% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 ifeq ($(OS),Windows_NT)
 	INSTALL_CMDSTAN_FLAGS = --compiler
 	ACTIVATE_VENV = .venv/Scripts/activate
 else
 	INSTALL_CMDSTAN_FLAGS =
 endif
 
+env: $(ENV_MARKER)
+
 $(ACTIVATE_VENV):
 	python -m venv .venv --prompt={{cookiecutter.repo_name}}
 
 {% if cookiecutter.docs_format == 'Quarto' -%}
 $(QUARTO_EXTENSIONS_FOLDER):
 	cd docs && quarto add quarto-ext/include-code-files && cd -
 {%- endif %}
```

### Comparing `bibat-0.1.6/bibat/{{cookiecutter.repo_name}}/README.md` & `bibat-0.1.8/bibat/{{cookiecutter.repo_name}}/README.md`

 * *Files identical despite different names*

### Comparing `bibat-0.1.6/bibat/{{cookiecutter.repo_name}}/data/raw/raw_measurements.csv` & `bibat-0.1.8/bibat/{{cookiecutter.repo_name}}/data/raw/raw_measurements.csv`

 * *Files identical despite different names*

### Comparing `bibat-0.1.6/bibat/{{cookiecutter.repo_name}}/docs/bibliography.bib` & `bibat-0.1.8/bibat/{{cookiecutter.repo_name}}/docs/bibliography.bib`

 * *Files identical despite different names*

### Comparing `bibat-0.1.6/bibat/{{cookiecutter.repo_name}}/docs/conf.py` & `bibat-0.1.8/bibat/{{cookiecutter.repo_name}}/docs/conf.py`

 * *Files identical despite different names*

### Comparing `bibat-0.1.6/bibat/{{cookiecutter.repo_name}}/docs/img/example.png` & `bibat-0.1.8/bibat/{{cookiecutter.repo_name}}/docs/img/example.png`

 * *Files identical despite different names*

### Comparing `bibat-0.1.6/bibat/{{cookiecutter.repo_name}}/docs/index.rst` & `bibat-0.1.8/bibat/{{cookiecutter.repo_name}}/docs/index.rst`

 * *Files identical despite different names*

### Comparing `bibat-0.1.6/bibat/{{cookiecutter.repo_name}}/docs/report.html` & `bibat-0.1.8/bibat/{{cookiecutter.repo_name}}/docs/report.html`

 * *Files identical despite different names*

### Comparing `bibat-0.1.6/bibat/{{cookiecutter.repo_name}}/docs/report.pdf` & `bibat-0.1.8/bibat/{{cookiecutter.repo_name}}/docs/report.pdf`

 * *Files identical despite different names*

### Comparing `bibat-0.1.6/bibat/{{cookiecutter.repo_name}}/docs/report.qmd` & `bibat-0.1.8/bibat/{{cookiecutter.repo_name}}/docs/report.qmd`

 * *Files identical despite different names*

### Comparing `bibat-0.1.6/bibat/{{cookiecutter.repo_name}}/plots/posterior_ll_comparison.png` & `bibat-0.1.8/bibat/{{cookiecutter.repo_name}}/plots/posterior_ll_comparison.png`

 * *Files identical despite different names*

### Comparing `bibat-0.1.6/bibat/{{cookiecutter.repo_name}}/plots/posterior_predictive_comparison.png` & `bibat-0.1.8/bibat/{{cookiecutter.repo_name}}/plots/posterior_predictive_comparison.png`

 * *Files identical despite different names*

### Comparing `bibat-0.1.6/bibat/{{cookiecutter.repo_name}}/pyproject.toml` & `bibat-0.1.8/bibat/{{cookiecutter.repo_name}}/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bibat-0.1.6/bibat/{{cookiecutter.repo_name}}/tests/test_integration/test_data_preparation.py` & `bibat-0.1.8/bibat/{{cookiecutter.repo_name}}/tests/test_integration/test_data_preparation.py`

 * *Files identical despite different names*

### Comparing `bibat-0.1.6/bibat/{{cookiecutter.repo_name}}/tests/test_unit/test_inference_configuration.py` & `bibat-0.1.8/bibat/{{cookiecutter.repo_name}}/tests/test_unit/test_inference_configuration.py`

 * *Files identical despite different names*

### Comparing `bibat-0.1.6/bibat/{{cookiecutter.repo_name}}/tests/test_unit/test_util.py` & `bibat-0.1.8/bibat/{{cookiecutter.repo_name}}/tests/test_unit/test_util.py`

 * *Files identical despite different names*

### Comparing `bibat-0.1.6/bibat/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}/data_preparation.py` & `bibat-0.1.8/bibat/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}/data_preparation.py`

 * *Files identical despite different names*

### Comparing `bibat-0.1.6/bibat/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}/fitting_mode.py` & `bibat-0.1.8/bibat/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}/fitting_mode.py`

 * *Files identical despite different names*

### Comparing `bibat-0.1.6/bibat/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}/inference_configuration.py` & `bibat-0.1.8/bibat/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}/inference_configuration.py`

 * *Files identical despite different names*

### Comparing `bibat-0.1.6/bibat/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}/investigate.ipynb` & `bibat-0.1.8/bibat/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}/investigate.ipynb`

 * *Files identical despite different names*

### Comparing `bibat-0.1.6/bibat/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}/sample.py` & `bibat-0.1.8/bibat/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}/sample.py`

 * *Files identical despite different names*

### Comparing `bibat-0.1.6/bibat/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}/stan/custom_functions.stan` & `bibat-0.1.8/bibat/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}/stan/custom_functions.stan`

 * *Files identical despite different names*

### Comparing `bibat-0.1.6/bibat/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}/stan/multilevel-linear-regression.stan` & `bibat-0.1.8/bibat/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}/stan/multilevel-linear-regression.stan`

 * *Files identical despite different names*

### Comparing `bibat-0.1.6/bibat/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}/stan_input_functions.py` & `bibat-0.1.8/bibat/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}/stan_input_functions.py`

 * *Files identical despite different names*

### Comparing `bibat-0.1.6/bibat/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}/util.py` & `bibat-0.1.8/bibat/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}/util.py`

 * *Files identical despite different names*

### Comparing `bibat-0.1.6/bibat.egg-info/PKG-INFO` & `bibat-0.1.8/bibat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bibat
-Version: 0.1.6
+Version: 0.1.8
 Summary: Batteries-included Bayesian analysis template
 Author-email: Teddy Groves <tedgro@dtu.dk>
 License: GNU General Public License version 3
 Project-URL: homepage, https://github.com/teddygroves/bibat
 Project-URL: download, https://pypi.org/project/bibat
 Project-URL: documentation, https://bibat.readthedocs.io/
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `bibat-0.1.6/bibat.egg-info/SOURCES.txt` & `bibat-0.1.8/bibat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bibat-0.1.6/pyproject.toml` & `bibat-0.1.8/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "bibat"
 authors = [
     {name = "Teddy Groves", email = "tedgro@dtu.dk"},
 ]
-version = "0.1.6"
+version = "0.1.8"
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Natural Language :: English",
     "Operating System :: MacOS :: MacOS X",
     "Operating System :: Microsoft :: Windows :: Windows 10",
@@ -36,15 +36,15 @@
     "pre-commit",
     "codecov",
     "pytest",
     "pytest-cov",
     "tox",
     "sphinx",
     "sphinx-click",
-    "pydata_sphinx_theme",
+    "furo",
 ]
 [project.urls]
 homepage = "https://github.com/teddygroves/bibat"
 download = "https://pypi.org/project/bibat"
 documentation = "https://bibat.readthedocs.io/"
 
 [tool.setuptools]
```

