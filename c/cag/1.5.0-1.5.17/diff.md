# Comparing `tmp/cag-1.5.0.tar.gz` & `tmp/cag-1.5.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cag-1.5.0.tar", last modified: Thu Mar 30 12:55:12 2023, max compression
+gzip compressed data, was "cag-1.5.17.tar", last modified: Thu Jun 22 14:51:27 2023, max compression
```

## Comparing `cag-1.5.0.tar` & `cag-1.5.17.tar`

### file list

```diff
@@ -1,154 +1,160 @@
--rw-r--r--   0        0        0     1049 2023-03-06 12:31:21.580633 cag-1.5.0/.github/workflows/main.yml
--rw-r--r--   0        0        0      873 2023-03-06 12:31:21.582020 cag-1.5.0/.gitignore
--rw-r--r--   0        0        0      756 2023-02-03 13:44:29.336324 cag-1.5.0/.gitlab-ci.yml
--rw-r--r--   0        0        0     1675 2023-03-27 09:03:13.368135 cag-1.5.0/CITATION.cff
--rw-r--r--   0        0        0      161 2023-03-06 12:31:21.583045 cag-1.5.0/Dockerfile
--rw-r--r--   0        0        0     1089 2023-02-03 13:44:29.336324 cag-1.5.0/LICENSE
--rw-r--r--   0        0        0     4406 2023-03-30 12:16:26.886721 cag-1.5.0/README.md
--rw-r--r--   0        0        0       94 2023-02-03 13:44:29.336324 cag-1.5.0/cag/MANIFETS.in
--rw-r--r--   0        0        0      973 2023-02-16 12:48:56.910640 cag-1.5.0/cag/__init__.py
--rw-r--r--   0        0        0     2163 2023-03-30 12:50:37.927299 cag-1.5.0/cag/cli.py
--rw-r--r--   0        0        0      526 2023-03-30 12:16:26.889131 cag-1.5.0/cag/cookiecutter.json
--rw-r--r--   0        0        0      222 2023-02-15 07:33:42.901109 cag-1.5.0/cag/framework/__init__.py
--rw-r--r--   0        0        0       21 2023-02-15 07:33:42.902128 cag-1.5.0/cag/framework/analyzer/__init__.py
--rw-r--r--   0        0        0     2155 2023-02-15 07:33:42.902128 cag-1.5.0/cag/framework/analyzer/analyzer_base.py
--rw-r--r--   0        0        0        0 2023-02-03 13:44:29.351827 cag-1.5.0/cag/framework/annotator/__init__.py
--rw-r--r--   0        0        0     4528 2023-02-16 10:50:36.680532 cag-1.5.0/cag/framework/annotator/annotator_base.py
--rw-r--r--   0        0        0        0 2023-02-03 13:44:29.351827 cag-1.5.0/cag/framework/annotator/element/__init__.py
--rw-r--r--   0        0        0     4739 2023-02-16 12:48:56.913984 cag-1.5.0/cag/framework/annotator/element/graph_elements.py
--rw-r--r--   0        0        0     5411 2023-02-16 12:48:56.914125 cag-1.5.0/cag/framework/annotator/element/orchestrator.py
--rw-r--r--   0        0        0        0 2023-02-03 13:44:29.351827 cag-1.5.0/cag/framework/annotator/instance/__init__.py
--rw-r--r--   0        0        0      548 2023-02-16 10:50:36.684081 cag-1.5.0/cag/framework/annotator/instance/dummy.py
--rw-r--r--   0        0        0     2715 2023-02-16 12:48:56.915866 cag-1.5.0/cag/framework/annotator/instance/emotion_orchestrator.py
--rw-r--r--   0        0        0     1869 2023-02-16 12:48:56.916206 cag-1.5.0/cag/framework/annotator/instance/empath_orchestrator.py
--rw-r--r--   0        0        0     2197 2023-02-16 12:48:56.917725 cag-1.5.0/cag/framework/annotator/instance/hedge_orchestrator.py
--rw-r--r--   0        0        0     2567 2023-02-16 12:48:56.917906 cag-1.5.0/cag/framework/annotator/instance/mpqa_orchestrator.py
--rw-r--r--   0        0        0     2355 2023-03-29 11:59:20.342906 cag-1.5.0/cag/framework/annotator/instance/ner_orchestrator.py
--rw-r--r--   0        0        0     2441 2023-02-16 12:48:56.920130 cag-1.5.0/cag/framework/annotator/instance/toxicity_orchestrator.py
--rw-r--r--   0        0        0        0 2023-02-03 13:44:29.351827 cag-1.5.0/cag/framework/annotator/pipe/__init__.py
--rw-r--r--   0        0        0        0 2023-02-03 13:44:29.351827 cag-1.5.0/cag/framework/annotator/pipe/linguistic/__init__.py
--rw-r--r--   0        0        0     1255 2023-02-16 12:48:56.921023 cag-1.5.0/cag/framework/annotator/pipe/linguistic/discourse_marker.py
--rw-r--r--   0        0        0     4130 2023-02-16 12:48:56.921213 cag-1.5.0/cag/framework/annotator/pipe/linguistic/emotion.py
--rw-r--r--   0        0        0     3314 2023-02-16 12:48:56.922105 cag-1.5.0/cag/framework/annotator/pipe/linguistic/empath.py
--rw-r--r--   0        0        0     2149 2023-02-16 12:48:56.922793 cag-1.5.0/cag/framework/annotator/pipe/linguistic/hedge.py
--rw-r--r--   0        0        0     1314 2023-02-14 10:46:37.179987 cag-1.5.0/cag/framework/annotator/pipe/linguistic/metadata.py
--rw-r--r--   0        0        0     1975 2023-02-16 12:48:56.923409 cag-1.5.0/cag/framework/annotator/pipe/linguistic/mpqa.py
--rw-r--r--   0        0        0     3946 2023-02-16 10:50:36.685639 cag-1.5.0/cag/framework/annotator/pipe/linguistic/style_features.py
--rw-r--r--   0        0        0     3916 2023-02-16 12:48:56.924462 cag-1.5.0/cag/framework/annotator/pipe/linguistic/toxicity.py
--rw-r--r--   0        0        0     1938 2023-02-16 12:48:56.924875 cag-1.5.0/cag/framework/annotator/pipe/linguistic/typos.py
--rw-r--r--   0        0        0        0 2023-02-03 13:44:29.351827 cag-1.5.0/cag/framework/annotator/pipeline/__init__.py
--rw-r--r--   0        0        0    11452 2023-02-16 12:48:56.925719 cag-1.5.0/cag/framework/annotator/pipeline/pipeline_base.py
--rw-r--r--   0        0        0     6720 2023-02-16 12:48:56.926634 cag-1.5.0/cag/framework/annotator/registered_pipes.py
--rw-r--r--   0        0        0    14104 2023-03-30 12:50:37.928455 cag-1.5.0/cag/framework/component.py
--rw-r--r--   0        0        0        0 2023-02-03 13:44:29.351827 cag-1.5.0/cag/framework/creator/__init__.py
--rw-r--r--   0        0        0     5777 2023-03-30 12:50:37.929471 cag-1.5.0/cag/framework/creator/base_creator.py
--rw-r--r--   0        0        0        0 2023-02-03 13:44:29.351827 cag-1.5.0/cag/graph_elements/__init__.py
--rw-r--r--   0        0        0     4621 2023-03-06 12:32:52.261933 cag-1.5.0/cag/graph_elements/base_graph.py
--rw-r--r--   0        0        0     1797 2023-03-30 12:50:37.929471 cag-1.5.0/cag/graph_elements/nodes.py
--rw-r--r--   0        0        0      765 2023-02-16 12:48:14.930123 cag-1.5.0/cag/graph_elements/relations.py
--rw-r--r--   0        0        0        0 2023-02-03 13:44:29.351827 cag-1.5.0/cag/utils/__init__.py
--rw-r--r--   0        0        0     3441 2023-02-16 12:48:56.929217 cag-1.5.0/cag/utils/config.py
--rw-r--r--   0        0        0     1491 2023-02-14 10:46:37.359709 cag-1.5.0/cag/utils/timer.py
--rw-r--r--   0        0        0     2593 2023-02-16 13:30:00.371942 cag-1.5.0/cag/utils/utils.py
--rw-r--r--   0        0        0        0 2023-02-03 13:44:29.351827 cag-1.5.0/cag/view_wrapper/__init__.py
--rw-r--r--   0        0        0     6939 2023-03-06 12:32:52.293360 cag-1.5.0/cag/view_wrapper/arango_analyzer.py
--rw-r--r--   0        0        0     1748 2023-02-16 10:50:36.697782 cag-1.5.0/cag/view_wrapper/link.py
--rw-r--r--   0        0        0     3027 2023-02-16 10:50:36.699007 cag-1.5.0/cag/view_wrapper/view.py
--rw-r--r--   0        0        0      311 2023-03-30 12:16:26.890100 cag-1.5.0/cag/{{cookiecutter.project_slug}}/.editorconfig
--rw-r--r--   0        0        0     1310 2023-03-30 12:16:26.890100 cag-1.5.0/cag/{{cookiecutter.project_slug}}/.gitignore
--rw-r--r--   0        0        0      191 2023-03-30 12:16:26.893243 cag-1.5.0/cag/{{cookiecutter.project_slug}}/AUTHORS.rst
--rw-r--r--   0        0        0     4141 2023-03-30 12:16:26.894133 cag-1.5.0/cag/{{cookiecutter.project_slug}}/CONTRIBUTING.rst
--rw-r--r--   0        0        0      116 2023-03-30 12:16:26.894133 cag-1.5.0/cag/{{cookiecutter.project_slug}}/HISTORY.rst
--rw-r--r--   0        0        0     6098 2023-03-30 12:16:26.894133 cag-1.5.0/cag/{{cookiecutter.project_slug}}/LICENSE
--rw-r--r--   0        0        0      337 2023-03-30 12:16:26.895131 cag-1.5.0/cag/{{cookiecutter.project_slug}}/MANIFEST.in
--rw-r--r--   0        0        0     2974 2023-03-30 12:16:26.896132 cag-1.5.0/cag/{{cookiecutter.project_slug}}/Makefile
--rw-r--r--   0        0        0     1783 2023-03-30 12:16:26.896611 cag-1.5.0/cag/{{cookiecutter.project_slug}}/README.rst
--rw-r--r--   0        0        0      249 2023-03-30 12:16:26.896611 cag-1.5.0/cag/{{cookiecutter.project_slug}}/docker-compose.yml
--rw-r--r--   0        0        0      652 2023-03-30 12:16:26.897615 cag-1.5.0/cag/{{cookiecutter.project_slug}}/docs/Makefile
--rw-r--r--   0        0        0       29 2023-03-30 12:16:26.897956 cag-1.5.0/cag/{{cookiecutter.project_slug}}/docs/authors.rst
--rw-r--r--   0        0        0     5319 2023-03-30 12:16:26.898456 cag-1.5.0/cag/{{cookiecutter.project_slug}}/docs/conf.py
--rw-r--r--   0        0        0       34 2023-03-30 12:16:26.898784 cag-1.5.0/cag/{{cookiecutter.project_slug}}/docs/contributing.rst
--rw-r--r--   0        0        0       29 2023-03-30 12:16:26.899062 cag-1.5.0/cag/{{cookiecutter.project_slug}}/docs/history.rst
--rw-r--r--   0        0        0      408 2023-03-30 12:16:26.899383 cag-1.5.0/cag/{{cookiecutter.project_slug}}/docs/index.rst
--rw-r--r--   0        0        0     1461 2023-03-30 12:16:26.899383 cag-1.5.0/cag/{{cookiecutter.project_slug}}/docs/installation.rst
--rwxr-xr-x   0        0        0      829 2023-03-30 12:16:26.900107 cag-1.5.0/cag/{{cookiecutter.project_slug}}/docs/make.bat
--rw-r--r--   0        0        0       28 2023-03-30 12:16:26.900567 cag-1.5.0/cag/{{cookiecutter.project_slug}}/docs/readme.rst
--rw-r--r--   0        0        0      124 2023-03-30 12:16:26.900567 cag-1.5.0/cag/{{cookiecutter.project_slug}}/docs/usage.rst
--rw-r--r--   0        0        0      311 2023-03-30 12:16:26.901004 cag-1.5.0/cag/{{cookiecutter.project_slug}}/requirements.txt
--rw-r--r--   0        0        0     2541 2023-03-30 12:16:26.901311 cag-1.5.0/cag/{{cookiecutter.project_slug}}/setup.py
--rw-r--r--   0        0        0       62 2023-03-30 12:16:26.901705 cag-1.5.0/cag/{{cookiecutter.project_slug}}/tests/__init__.py
--rw-r--r--   0        0        0     2390 2023-03-30 12:16:26.901969 cag-1.5.0/cag/{{cookiecutter.project_slug}}/tests/test_{{cookiecutter.project_slug}}.py
--rw-r--r--   0        0        0     3982 2023-03-30 12:50:12.124076 cag-1.5.0/cag/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/MovieEmbeddings.py
--rw-r--r--   0        0        0      415 2023-03-30 12:16:26.903008 cag-1.5.0/cag/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/MovieGraphCreator.py
--rw-r--r--   0        0        0      197 2023-03-30 12:50:12.125072 cag-1.5.0/cag/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/__init__.py
--rw-r--r--   0        0        0     1172 2023-03-30 12:16:26.903008 cag-1.5.0/cag/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/cli.py
--rw-r--r--   0        0        0      782 2023-03-30 12:16:26.903008 cag-1.5.0/cag/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/conf.py
--rw-r--r--   0        0        0     3544 2023-03-30 12:16:26.904098 cag-1.5.0/cag/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/data/sample_data.json
--rw-r--r--   0        0        0      589 2023-03-30 12:50:12.125791 cag-1.5.0/cag/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/edges.py
--rw-r--r--   0        0        0     4684 2023-03-30 12:50:12.125876 cag-1.5.0/cag/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/graph.py
--rw-r--r--   0        0        0     1133 2023-03-30 12:50:12.126550 cag-1.5.0/cag/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/nodes.py
--rw-r--r--   0        0        0      404 2023-03-06 12:31:21.584517 cag-1.5.0/docker-compose.yml
--rw-r--r--   0        0        0      658 2023-03-06 12:31:16.846123 cag-1.5.0/docs/Makefile
--rw-r--r--   0        0        0   188985 2023-02-03 13:44:29.367451 cag-1.5.0/docs/cag.pdf
--rw-r--r--   0        0        0   102584 2023-02-03 13:44:29.367451 cag-1.5.0/docs/cag.png
--rwxr-xr-x   0        0        0      804 2023-03-06 12:31:16.847150 cag-1.5.0/docs/make.bat
--rw-r--r--   0        0        0     1060 2023-03-06 12:31:16.851162 cag-1.5.0/docs/source/conf.py
--rw-r--r--   0        0        0    65268 2023-02-03 13:44:29.367451 cag-1.5.0/docs/source/imgs/data_model.png
--rw-r--r--   0        0        0     1002 2023-02-03 13:44:29.367451 cag-1.5.0/docs/source/index.rst
--rw-r--r--   0        0        0     5260 2023-03-06 12:31:16.853161 cag-1.5.0/docs/source/reference/0_concept.rst
--rw-r--r--   0        0        0     3322 2023-03-06 12:31:16.858673 cag-1.5.0/docs/source/reference/1_get_started.rst
--rw-r--r--   0        0        0     2965 2023-02-03 13:44:29.367451 cag-1.5.0/docs/source/reference/2_annotator.rst
--rw-r--r--   0        0        0     1272 2023-02-03 13:44:29.367451 cag-1.5.0/docs/source/reference/3_analyzers.rst
--rw-r--r--   0        0        0     6442 2023-02-03 13:44:29.367451 cag-1.5.0/docs/source/reference/4_view_management.rst
--rw-r--r--   0        0        0     4587 2023-02-15 07:33:42.906618 cag-1.5.0/examples/0_download_process_data.ipynb
--rw-r--r--   0        0        0    74302 2023-03-29 14:07:05.744044 cag-1.5.0/examples/1_create_graph.ipynb
--rw-r--r--   0        0        0     7639 2023-03-06 12:32:52.781687 cag-1.5.0/examples/2_annotate_graph.ipynb
--rw-r--r--   0        0        0     2271 2023-02-16 10:50:36.703029 cag-1.5.0/examples/annotation_example.py
--rw-r--r--   0        0        0    26159 2023-02-03 13:44:29.367451 cag-1.5.0/examples/data/periodic_wiki_batches/Machine_learning/10Oct2021-12Oct2021/alphago_revisions.parquet
--rw-r--r--   0        0        0    55294 2023-02-03 13:44:29.367451 cag-1.5.0/examples/data/periodic_wiki_batches/Machine_learning/10Oct2021-12Oct2021/conference-on-knowledge-discovery-and-data-mining_revisions.parquet
--rw-r--r--   0        0        0    34689 2023-02-03 13:44:29.367451 cag-1.5.0/examples/data/periodic_wiki_batches/Machine_learning/10Oct2021-12Oct2021/differential-evolution_revisions.parquet
--rw-r--r--   0        0        0    26043 2023-02-03 13:44:29.367451 cag-1.5.0/examples/data/periodic_wiki_batches/Machine_learning/10Oct2021-12Oct2021/feature-engineering_revisions.parquet
--rw-r--r--   0        0        0    11556 2023-02-03 13:44:29.367451 cag-1.5.0/examples/data/periodic_wiki_batches/Machine_learning/10Oct2021-12Oct2021/feature-machine-learning_revisions.parquet
--rw-r--r--   0        0        0   786994 2023-02-03 13:44:29.383103 cag-1.5.0/examples/data/periodic_wiki_batches/Machine_learning/10Oct2021-12Oct2021/gpt-language-model_revisions.parquet
--rw-r--r--   0        0        0    15758 2023-02-03 13:44:29.383103 cag-1.5.0/examples/data/periodic_wiki_batches/Machine_learning/10Oct2021-12Oct2021/gpt3_revisions.parquet
--rw-r--r--   0        0        0    11576 2023-02-03 13:44:29.383103 cag-1.5.0/examples/data/periodic_wiki_batches/Machine_learning/10Oct2021-12Oct2021/gram-matrix_revisions.parquet
--rw-r--r--   0        0        0    33210 2023-02-03 13:44:29.383103 cag-1.5.0/examples/data/periodic_wiki_batches/Machine_learning/10Oct2021-12Oct2021/julia-programming-language_revisions.parquet
--rw-r--r--   0        0        0    34402 2023-02-03 13:44:29.383103 cag-1.5.0/examples/data/periodic_wiki_batches/Machine_learning/10Oct2021-12Oct2021/kaggle_revisions.parquet
--rw-r--r--   0        0        0    19617 2023-02-03 13:44:29.383103 cag-1.5.0/examples/data/periodic_wiki_batches/Machine_learning/10Oct2021-12Oct2021/knearest-neighbors-algorithm_revisions.parquet
--rw-r--r--   0        0        0    41808 2023-02-03 13:44:29.383103 cag-1.5.0/examples/data/periodic_wiki_batches/Machine_learning/10Oct2021-12Oct2021/list-of-datasets-for-machinelearning-research_revisions.parquet
--rw-r--r--   0        0        0    21038 2023-02-03 13:44:29.383103 cag-1.5.0/examples/data/periodic_wiki_batches/Machine_learning/10Oct2021-12Oct2021/machine-learning-in-video-games_revisions.parquet
--rw-r--r--   0        0        0   388941 2023-02-03 13:44:29.383103 cag-1.5.0/examples/data/periodic_wiki_batches/Machine_learning/10Oct2021-12Oct2021/normal-discriminant-analysis_revisions.parquet
--rw-r--r--   0        0        0    26362 2023-02-03 13:44:29.383103 cag-1.5.0/examples/data/periodic_wiki_batches/Machine_learning/10Oct2021-12Oct2021/onnx_revisions.parquet
--rw-r--r--   0        0        0    30444 2023-02-03 13:44:29.383103 cag-1.5.0/examples/data/periodic_wiki_batches/Machine_learning/10Oct2021-12Oct2021/perceiver_revisions.parquet
--rw-r--r--   0        0        0    12820 2023-02-03 13:44:29.383103 cag-1.5.0/examples/data/periodic_wiki_batches/Machine_learning/10Oct2021-12Oct2021/rademacher-complexity_revisions.parquet
--rw-r--r--   0        0        0    27530 2023-02-03 13:44:29.383103 cag-1.5.0/examples/data/periodic_wiki_batches/Machine_learning/10Oct2021-12Oct2021/support-vector-machine_revisions.parquet
--rw-r--r--   0        0        0   120147 2023-02-03 13:44:29.383103 cag-1.5.0/examples/data/periodic_wiki_batches/Machine_learning/10Oct2021-12Oct2021/underfitting_revisions.parquet
--rw-r--r--   0        0        0    15129 2023-02-03 13:44:29.383103 cag-1.5.0/examples/data/periodic_wiki_batches/Machine_learning/10Oct2021-12Oct2021/unsupervised-learning_revisions.parquet
--rw-r--r--   0        0        0   144227 2023-02-03 13:44:29.398699 cag-1.5.0/examples/data/periodic_wiki_batches/Machine_learning/10Oct2021-12Oct2021/validation-set_revisions.parquet
--rw-r--r--   0        0        0    13203 2023-02-03 13:44:29.398699 cag-1.5.0/examples/data/periodic_wiki_batches/Machine_learning/10Oct2021-12Oct2021/weak-supervision_revisions.parquet
--rw-r--r--   0        0        0    35165 2023-02-03 13:44:29.398699 cag-1.5.0/examples/data/periodic_wiki_batches/Machine_learning/10Oct2022-12Oct2022/alex-james-professor_revisions.parquet
--rw-r--r--   0        0        0    15382 2023-02-03 13:44:29.398699 cag-1.5.0/examples/data/periodic_wiki_batches/Machine_learning/10Oct2022-12Oct2022/data-version-control_revisions.parquet
--rw-r--r--   0        0        0    29431 2023-02-03 13:44:29.398699 cag-1.5.0/examples/data/periodic_wiki_batches/Machine_learning/10Oct2022-12Oct2022/deepnude_revisions.parquet
--rw-r--r--   0        0        0    61781 2023-02-03 13:44:29.398699 cag-1.5.0/examples/data/periodic_wiki_batches/Machine_learning/10Oct2022-12Oct2022/facial-recognition-system_revisions.parquet
--rw-r--r--   0        0        0    33859 2023-02-03 13:44:29.398699 cag-1.5.0/examples/data/periodic_wiki_batches/Machine_learning/10Oct2022-12Oct2022/feature-learning_revisions.parquet
--rw-r--r--   0        0        0    36983 2023-02-03 13:44:29.398699 cag-1.5.0/examples/data/periodic_wiki_batches/Machine_learning/10Oct2022-12Oct2022/julia-programming-language_revisions.parquet
--rw-r--r--   0        0        0    20270 2023-02-03 13:44:29.398699 cag-1.5.0/examples/data/periodic_wiki_batches/Machine_learning/10Oct2022-12Oct2022/models-of-dna-evolution_revisions.parquet
--rw-r--r--   0        0        0    85401 2023-02-03 13:44:29.398699 cag-1.5.0/examples/data/periodic_wiki_batches/Machine_learning/10Oct2022-12Oct2022/multipleinstance-learning_revisions.parquet
--rw-r--r--   0        0        0    24168 2023-02-03 13:44:29.398699 cag-1.5.0/examples/data/periodic_wiki_batches/Machine_learning/10Oct2022-12Oct2022/nikiai_revisions.parquet
--rw-r--r--   0        0        0    26362 2023-02-03 13:44:29.398699 cag-1.5.0/examples/data/periodic_wiki_batches/Machine_learning/10Oct2022-12Oct2022/onnx_revisions.parquet
--rw-r--r--   0        0        0    16064 2023-02-03 13:44:29.398699 cag-1.5.0/examples/data/periodic_wiki_batches/Machine_learning/10Oct2022-12Oct2022/overfitting_revisions.parquet
--rw-r--r--   0        0        0    11787 2023-02-03 13:44:29.398699 cag-1.5.0/examples/data/periodic_wiki_batches/Machine_learning/10Oct2022-12Oct2022/pop-music-automation_revisions.parquet
--rw-r--r--   0        0        0    15259 2023-02-03 13:44:29.398699 cag-1.5.0/examples/data/periodic_wiki_batches/Machine_learning/10Oct2022-12Oct2022/prescription-monitoring-program_revisions.parquet
--rw-r--r--   0        0        0   189865 2023-02-03 13:44:29.398699 cag-1.5.0/examples/data/periodic_wiki_batches/Machine_learning/10Oct2022-12Oct2022/squared-error-loss_revisions.parquet
--rw-r--r--   0        0        0    20292 2023-02-03 13:44:29.398699 cag-1.5.0/examples/data/periodic_wiki_batches/Machine_learning/10Oct2022-12Oct2022/stochastic-gradient-descent_revisions.parquet
--rw-r--r--   0        0        0    15014 2023-02-03 13:44:29.398699 cag-1.5.0/examples/data/periodic_wiki_batches/Machine_learning/10Oct2022-12Oct2022/symbolic-regression_revisions.parquet
--rw-r--r--   0        0        0    27282 2023-02-03 13:44:29.398699 cag-1.5.0/examples/data/periodic_wiki_batches/Machine_learning/10Oct2022-12Oct2022/word2vec_revisions.parquet
--rw-r--r--   0        0        0  3919314 2023-02-03 13:44:29.414327 cag-1.5.0/examples/example.html
--rw-r--r--   0        0        0     1963 2023-02-16 10:50:36.703378 cag-1.5.0/examples/view_creation_example.py
--rw-r--r--   0        0        0     1772 2023-03-30 12:50:37.929471 cag-1.5.0/pyproject.toml
--rw-r--r--   0        0        0      339 2023-03-30 12:16:26.905789 cag-1.5.0/requirements.txt
--rw-r--r--   0        0        0      518 2023-03-27 09:03:13.372364 cag-1.5.0/tests/__init__.py
--rw-r--r--   0        0        0    11993 2023-03-27 09:03:13.374364 cag-1.5.0/tests/test_graph_creator.py
--rw-r--r--   0        0        0     3130 2023-03-27 09:03:13.375587 cag-1.5.0/tests/test_graph_creator/test_improve_edge_definitions.py
--rw-r--r--   0        0        0     8316 2023-03-30 12:50:37.930477 cag-1.5.0/tests/test_view.py
--rw-r--r--   0        0        0     5660 1970-01-01 00:00:00.000000 cag-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1049 2023-05-10 08:19:54.003899 cag-1.5.17/.github/workflows/main.yml
+-rw-r--r--   0        0        0      873 2023-05-10 08:19:54.005476 cag-1.5.17/.gitignore
+-rw-r--r--   0        0        0      756 2023-02-03 13:44:29.336324 cag-1.5.17/.gitlab-ci.yml
+-rw-r--r--   0        0        0     1675 2023-05-10 08:19:54.006625 cag-1.5.17/CITATION.cff
+-rw-r--r--   0        0        0      161 2023-05-10 08:19:54.008597 cag-1.5.17/Dockerfile
+-rw-r--r--   0        0        0     1089 2023-02-03 13:44:29.336324 cag-1.5.17/LICENSE
+-rw-r--r--   0        0        0     4586 2023-06-03 13:29:58.418689 cag-1.5.17/README.md
+-rw-r--r--   0        0        0       94 2023-02-03 13:44:29.336324 cag-1.5.17/cag/MANIFETS.in
+-rw-r--r--   0        0        0      973 2023-02-16 12:48:56.910640 cag-1.5.17/cag/__init__.py
+-rw-r--r--   0        0        0     2163 2023-05-10 08:19:54.023008 cag-1.5.17/cag/cli.py
+-rw-r--r--   0        0        0      526 2023-05-10 08:19:54.023629 cag-1.5.17/cag/cookiecutter.json
+-rw-r--r--   0        0        0      222 2023-02-15 07:33:42.901109 cag-1.5.17/cag/framework/__init__.py
+-rw-r--r--   0        0        0       21 2023-02-15 07:33:42.902128 cag-1.5.17/cag/framework/analyzer/__init__.py
+-rw-r--r--   0        0        0     2155 2023-02-15 07:33:42.902128 cag-1.5.17/cag/framework/analyzer/analyzer_base.py
+-rw-r--r--   0        0        0        0 2023-02-03 13:44:29.351827 cag-1.5.17/cag/framework/annotator/__init__.py
+-rw-r--r--   0        0        0     4528 2023-02-16 10:50:36.680532 cag-1.5.17/cag/framework/annotator/annotator_base.py
+-rw-r--r--   0        0        0        0 2023-02-03 13:44:29.351827 cag-1.5.17/cag/framework/annotator/element/__init__.py
+-rw-r--r--   0        0        0     6760 2023-06-22 14:50:45.522656 cag-1.5.17/cag/framework/annotator/element/graph_elements.py
+-rw-r--r--   0        0        0     5411 2023-02-16 12:48:56.914125 cag-1.5.17/cag/framework/annotator/element/orchestrator.py
+-rw-r--r--   0        0        0        0 2023-02-03 13:44:29.351827 cag-1.5.17/cag/framework/annotator/instance/__init__.py
+-rw-r--r--   0        0        0      548 2023-02-16 10:50:36.684081 cag-1.5.17/cag/framework/annotator/instance/dummy.py
+-rw-r--r--   0        0        0     2715 2023-02-16 12:48:56.915866 cag-1.5.17/cag/framework/annotator/instance/emotion_orchestrator.py
+-rw-r--r--   0        0        0     1869 2023-02-16 12:48:56.916206 cag-1.5.17/cag/framework/annotator/instance/empath_orchestrator.py
+-rw-r--r--   0        0        0     2201 2023-05-10 08:29:52.448375 cag-1.5.17/cag/framework/annotator/instance/hedge_orchestrator.py
+-rw-r--r--   0        0        0     1937 2023-06-22 14:50:45.523156 cag-1.5.17/cag/framework/annotator/instance/iptcmedia_topic_orchestrator.py
+-rw-r--r--   0        0        0     1783 2023-06-22 14:50:45.523328 cag-1.5.17/cag/framework/annotator/instance/keyterms_orchestrator.py
+-rw-r--r--   0        0        0     2567 2023-02-16 12:48:56.917906 cag-1.5.17/cag/framework/annotator/instance/mpqa_orchestrator.py
+-rw-r--r--   0        0        0     2355 2023-03-29 11:59:20.342906 cag-1.5.17/cag/framework/annotator/instance/ner_orchestrator.py
+-rw-r--r--   0        0        0     1871 2023-06-22 14:50:45.523695 cag-1.5.17/cag/framework/annotator/instance/openalex_concept_orchestrator.py
+-rw-r--r--   0        0        0     2441 2023-02-16 12:48:56.920130 cag-1.5.17/cag/framework/annotator/instance/toxicity_orchestrator.py
+-rw-r--r--   0        0        0        0 2023-02-03 13:44:29.351827 cag-1.5.17/cag/framework/annotator/pipe/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-03 13:44:29.351827 cag-1.5.17/cag/framework/annotator/pipe/linguistic/__init__.py
+-rw-r--r--   0        0        0     1255 2023-02-16 12:48:56.921023 cag-1.5.17/cag/framework/annotator/pipe/linguistic/discourse_marker.py
+-rw-r--r--   0        0        0     4128 2023-06-22 14:50:45.523695 cag-1.5.17/cag/framework/annotator/pipe/linguistic/emotion.py
+-rw-r--r--   0        0        0     3314 2023-02-16 12:48:56.922105 cag-1.5.17/cag/framework/annotator/pipe/linguistic/empath.py
+-rw-r--r--   0        0        0     2149 2023-02-16 12:48:56.922793 cag-1.5.17/cag/framework/annotator/pipe/linguistic/hedge.py
+-rw-r--r--   0        0        0     3192 2023-06-22 14:50:45.525225 cag-1.5.17/cag/framework/annotator/pipe/linguistic/iptcmedia_topic.py
+-rw-r--r--   0        0        0     2248 2023-06-22 14:50:45.525225 cag-1.5.17/cag/framework/annotator/pipe/linguistic/keyterms.py
+-rw-r--r--   0        0        0     1314 2023-02-14 10:46:37.179987 cag-1.5.17/cag/framework/annotator/pipe/linguistic/metadata.py
+-rw-r--r--   0        0        0     1975 2023-02-16 12:48:56.923409 cag-1.5.17/cag/framework/annotator/pipe/linguistic/mpqa.py
+-rw-r--r--   0        0        0     3235 2023-06-22 14:50:45.525727 cag-1.5.17/cag/framework/annotator/pipe/linguistic/oaconcept.py
+-rw-r--r--   0        0        0     3946 2023-02-16 10:50:36.685639 cag-1.5.17/cag/framework/annotator/pipe/linguistic/style_features.py
+-rw-r--r--   0        0        0     3916 2023-02-16 12:48:56.924462 cag-1.5.17/cag/framework/annotator/pipe/linguistic/toxicity.py
+-rw-r--r--   0        0        0     1938 2023-02-16 12:48:56.924875 cag-1.5.17/cag/framework/annotator/pipe/linguistic/typos.py
+-rw-r--r--   0        0        0        0 2023-02-03 13:44:29.351827 cag-1.5.17/cag/framework/annotator/pipeline/__init__.py
+-rw-r--r--   0        0        0    12243 2023-06-22 14:50:45.526908 cag-1.5.17/cag/framework/annotator/pipeline/pipeline_base.py
+-rw-r--r--   0        0        0     9365 2023-06-22 14:50:45.527093 cag-1.5.17/cag/framework/annotator/registered_pipes.py
+-rw-r--r--   0        0        0    14104 2023-05-10 08:19:54.026630 cag-1.5.17/cag/framework/component.py
+-rw-r--r--   0        0        0        0 2023-02-03 13:44:29.351827 cag-1.5.17/cag/framework/creator/__init__.py
+-rw-r--r--   0        0        0     5777 2023-05-10 08:19:54.032640 cag-1.5.17/cag/framework/creator/base_creator.py
+-rw-r--r--   0        0        0        0 2023-02-03 13:44:29.351827 cag-1.5.17/cag/graph_elements/__init__.py
+-rw-r--r--   0        0        0     4621 2023-05-10 08:19:54.035312 cag-1.5.17/cag/graph_elements/base_graph.py
+-rw-r--r--   0        0        0     1797 2023-05-10 08:19:54.037278 cag-1.5.17/cag/graph_elements/nodes.py
+-rw-r--r--   0        0        0      765 2023-02-16 12:48:14.930123 cag-1.5.17/cag/graph_elements/relations.py
+-rw-r--r--   0        0        0        0 2023-02-03 13:44:29.351827 cag-1.5.17/cag/utils/__init__.py
+-rw-r--r--   0        0        0     3441 2023-02-16 12:48:56.929217 cag-1.5.17/cag/utils/config.py
+-rw-r--r--   0        0        0     1491 2023-02-14 10:46:37.359709 cag-1.5.17/cag/utils/timer.py
+-rw-r--r--   0        0        0     2698 2023-06-22 14:50:45.527093 cag-1.5.17/cag/utils/utils.py
+-rw-r--r--   0        0        0        0 2023-02-03 13:44:29.351827 cag-1.5.17/cag/view_wrapper/__init__.py
+-rw-r--r--   0        0        0     6939 2023-05-10 08:19:54.039338 cag-1.5.17/cag/view_wrapper/arango_analyzer.py
+-rw-r--r--   0        0        0     1748 2023-02-16 10:50:36.697782 cag-1.5.17/cag/view_wrapper/link.py
+-rw-r--r--   0        0        0     3027 2023-02-16 10:50:36.699007 cag-1.5.17/cag/view_wrapper/view.py
+-rw-r--r--   0        0        0      311 2023-05-10 08:19:54.041507 cag-1.5.17/cag/{{cookiecutter.project_slug}}/.editorconfig
+-rw-r--r--   0        0        0     1310 2023-05-10 08:19:54.042008 cag-1.5.17/cag/{{cookiecutter.project_slug}}/.gitignore
+-rw-r--r--   0        0        0      191 2023-05-10 08:19:54.043214 cag-1.5.17/cag/{{cookiecutter.project_slug}}/AUTHORS.rst
+-rw-r--r--   0        0        0     4141 2023-05-10 08:19:54.044007 cag-1.5.17/cag/{{cookiecutter.project_slug}}/CONTRIBUTING.rst
+-rw-r--r--   0        0        0      116 2023-05-10 08:19:54.044804 cag-1.5.17/cag/{{cookiecutter.project_slug}}/HISTORY.rst
+-rw-r--r--   0        0        0     6098 2023-05-10 08:19:54.047464 cag-1.5.17/cag/{{cookiecutter.project_slug}}/LICENSE
+-rw-r--r--   0        0        0      337 2023-05-10 08:19:54.048348 cag-1.5.17/cag/{{cookiecutter.project_slug}}/MANIFEST.in
+-rw-r--r--   0        0        0     2974 2023-05-10 08:19:54.049243 cag-1.5.17/cag/{{cookiecutter.project_slug}}/Makefile
+-rw-r--r--   0        0        0     1783 2023-05-10 08:19:54.050824 cag-1.5.17/cag/{{cookiecutter.project_slug}}/README.rst
+-rw-r--r--   0        0        0      249 2023-05-10 08:19:54.051323 cag-1.5.17/cag/{{cookiecutter.project_slug}}/docker-compose.yml
+-rw-r--r--   0        0        0      652 2023-05-10 08:19:54.053911 cag-1.5.17/cag/{{cookiecutter.project_slug}}/docs/Makefile
+-rw-r--r--   0        0        0       29 2023-05-10 08:19:54.054413 cag-1.5.17/cag/{{cookiecutter.project_slug}}/docs/authors.rst
+-rw-r--r--   0        0        0     5319 2023-05-10 08:19:54.061228 cag-1.5.17/cag/{{cookiecutter.project_slug}}/docs/conf.py
+-rw-r--r--   0        0        0       34 2023-05-10 08:19:54.064526 cag-1.5.17/cag/{{cookiecutter.project_slug}}/docs/contributing.rst
+-rw-r--r--   0        0        0       29 2023-05-10 08:19:54.068696 cag-1.5.17/cag/{{cookiecutter.project_slug}}/docs/history.rst
+-rw-r--r--   0        0        0      408 2023-05-10 08:19:54.080902 cag-1.5.17/cag/{{cookiecutter.project_slug}}/docs/index.rst
+-rw-r--r--   0        0        0     1461 2023-05-10 08:19:54.082915 cag-1.5.17/cag/{{cookiecutter.project_slug}}/docs/installation.rst
+-rwxr-xr-x   0        0        0      829 2023-05-10 08:19:54.083675 cag-1.5.17/cag/{{cookiecutter.project_slug}}/docs/make.bat
+-rw-r--r--   0        0        0       28 2023-05-10 08:19:54.084676 cag-1.5.17/cag/{{cookiecutter.project_slug}}/docs/readme.rst
+-rw-r--r--   0        0        0      124 2023-05-10 08:19:54.085705 cag-1.5.17/cag/{{cookiecutter.project_slug}}/docs/usage.rst
+-rw-r--r--   0        0        0      311 2023-05-10 08:19:54.085705 cag-1.5.17/cag/{{cookiecutter.project_slug}}/requirements.txt
+-rw-r--r--   0        0        0     2541 2023-05-10 08:19:54.087339 cag-1.5.17/cag/{{cookiecutter.project_slug}}/setup.py
+-rw-r--r--   0        0        0       62 2023-05-10 08:19:54.088943 cag-1.5.17/cag/{{cookiecutter.project_slug}}/tests/__init__.py
+-rw-r--r--   0        0        0     2390 2023-05-10 08:19:54.094396 cag-1.5.17/cag/{{cookiecutter.project_slug}}/tests/test_{{cookiecutter.project_slug}}.py
+-rw-r--r--   0        0        0     3982 2023-05-10 08:33:52.062832 cag-1.5.17/cag/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/MovieEmbeddings.py
+-rw-r--r--   0        0        0      415 2023-05-10 08:19:54.097863 cag-1.5.17/cag/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/MovieGraphCreator.py
+-rw-r--r--   0        0        0      197 2023-05-10 08:33:51.529146 cag-1.5.17/cag/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/__init__.py
+-rw-r--r--   0        0        0     1172 2023-05-10 08:19:54.103931 cag-1.5.17/cag/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/cli.py
+-rw-r--r--   0        0        0      782 2023-05-10 08:19:54.104432 cag-1.5.17/cag/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/conf.py
+-rw-r--r--   0        0        0     3544 2023-05-10 08:19:54.111344 cag-1.5.17/cag/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/data/sample_data.json
+-rw-r--r--   0        0        0      593 2023-05-10 08:33:51.738927 cag-1.5.17/cag/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/edges.py
+-rw-r--r--   0        0        0     4794 2023-05-10 08:33:52.323338 cag-1.5.17/cag/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/graph.py
+-rw-r--r--   0        0        0     1141 2023-05-10 08:33:51.881068 cag-1.5.17/cag/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/nodes.py
+-rw-r--r--   0        0        0      404 2023-05-10 08:19:54.116709 cag-1.5.17/docker-compose.yml
+-rw-r--r--   0        0        0      658 2023-05-10 08:19:54.118208 cag-1.5.17/docs/Makefile
+-rw-r--r--   0        0        0   188985 2023-02-03 13:44:29.367451 cag-1.5.17/docs/cag.pdf
+-rw-r--r--   0        0        0   102584 2023-02-03 13:44:29.367451 cag-1.5.17/docs/cag.png
+-rwxr-xr-x   0        0        0      804 2023-05-10 08:19:54.119709 cag-1.5.17/docs/make.bat
+-rw-r--r--   0        0        0     1060 2023-05-10 08:19:54.128820 cag-1.5.17/docs/source/conf.py
+-rw-r--r--   0        0        0    65268 2023-02-03 13:44:29.367451 cag-1.5.17/docs/source/imgs/data_model.png
+-rw-r--r--   0        0        0     1002 2023-05-10 08:19:54.130545 cag-1.5.17/docs/source/index.rst
+-rw-r--r--   0        0        0     5260 2023-05-10 08:19:54.132741 cag-1.5.17/docs/source/reference/0_concept.rst
+-rw-r--r--   0        0        0     3322 2023-05-10 08:19:54.133916 cag-1.5.17/docs/source/reference/1_get_started.rst
+-rw-r--r--   0        0        0     2965 2023-05-10 08:19:54.135019 cag-1.5.17/docs/source/reference/2_annotator.rst
+-rw-r--r--   0        0        0     1272 2023-05-10 08:19:54.135926 cag-1.5.17/docs/source/reference/3_analyzers.rst
+-rw-r--r--   0        0        0     6442 2023-05-10 08:19:54.141188 cag-1.5.17/docs/source/reference/4_view_management.rst
+-rw-r--r--   0        0        0     4587 2023-02-15 07:33:42.906618 cag-1.5.17/examples/0_download_process_data.ipynb
+-rw-r--r--   0        0        0    74302 2023-05-02 13:38:54.354473 cag-1.5.17/examples/1_create_graph.ipynb
+-rw-r--r--   0        0        0     7894 2023-05-10 08:19:54.144410 cag-1.5.17/examples/2_annotate_graph.ipynb
+-rw-r--r--   0        0        0     2271 2023-02-16 10:50:36.703029 cag-1.5.17/examples/annotation_example.py
+-rw-r--r--   0        0        0    26159 2023-02-03 13:44:29.367451 cag-1.5.17/examples/data/periodic_wiki_batches/Machine_learning/10Oct2021-12Oct2021/alphago_revisions.parquet
+-rw-r--r--   0        0        0    55294 2023-02-03 13:44:29.367451 cag-1.5.17/examples/data/periodic_wiki_batches/Machine_learning/10Oct2021-12Oct2021/conference-on-knowledge-discovery-and-data-mining_revisions.parquet
+-rw-r--r--   0        0        0    34689 2023-02-03 13:44:29.367451 cag-1.5.17/examples/data/periodic_wiki_batches/Machine_learning/10Oct2021-12Oct2021/differential-evolution_revisions.parquet
+-rw-r--r--   0        0        0    26043 2023-02-03 13:44:29.367451 cag-1.5.17/examples/data/periodic_wiki_batches/Machine_learning/10Oct2021-12Oct2021/feature-engineering_revisions.parquet
+-rw-r--r--   0        0        0    11556 2023-02-03 13:44:29.367451 cag-1.5.17/examples/data/periodic_wiki_batches/Machine_learning/10Oct2021-12Oct2021/feature-machine-learning_revisions.parquet
+-rw-r--r--   0        0        0   786994 2023-02-03 13:44:29.383103 cag-1.5.17/examples/data/periodic_wiki_batches/Machine_learning/10Oct2021-12Oct2021/gpt-language-model_revisions.parquet
+-rw-r--r--   0        0        0    15758 2023-02-03 13:44:29.383103 cag-1.5.17/examples/data/periodic_wiki_batches/Machine_learning/10Oct2021-12Oct2021/gpt3_revisions.parquet
+-rw-r--r--   0        0        0    11576 2023-02-03 13:44:29.383103 cag-1.5.17/examples/data/periodic_wiki_batches/Machine_learning/10Oct2021-12Oct2021/gram-matrix_revisions.parquet
+-rw-r--r--   0        0        0    33210 2023-02-03 13:44:29.383103 cag-1.5.17/examples/data/periodic_wiki_batches/Machine_learning/10Oct2021-12Oct2021/julia-programming-language_revisions.parquet
+-rw-r--r--   0        0        0    34402 2023-02-03 13:44:29.383103 cag-1.5.17/examples/data/periodic_wiki_batches/Machine_learning/10Oct2021-12Oct2021/kaggle_revisions.parquet
+-rw-r--r--   0        0        0    19617 2023-02-03 13:44:29.383103 cag-1.5.17/examples/data/periodic_wiki_batches/Machine_learning/10Oct2021-12Oct2021/knearest-neighbors-algorithm_revisions.parquet
+-rw-r--r--   0        0        0    41808 2023-02-03 13:44:29.383103 cag-1.5.17/examples/data/periodic_wiki_batches/Machine_learning/10Oct2021-12Oct2021/list-of-datasets-for-machinelearning-research_revisions.parquet
+-rw-r--r--   0        0        0    21038 2023-02-03 13:44:29.383103 cag-1.5.17/examples/data/periodic_wiki_batches/Machine_learning/10Oct2021-12Oct2021/machine-learning-in-video-games_revisions.parquet
+-rw-r--r--   0        0        0   388941 2023-02-03 13:44:29.383103 cag-1.5.17/examples/data/periodic_wiki_batches/Machine_learning/10Oct2021-12Oct2021/normal-discriminant-analysis_revisions.parquet
+-rw-r--r--   0        0        0    26362 2023-02-03 13:44:29.383103 cag-1.5.17/examples/data/periodic_wiki_batches/Machine_learning/10Oct2021-12Oct2021/onnx_revisions.parquet
+-rw-r--r--   0        0        0    30444 2023-02-03 13:44:29.383103 cag-1.5.17/examples/data/periodic_wiki_batches/Machine_learning/10Oct2021-12Oct2021/perceiver_revisions.parquet
+-rw-r--r--   0        0        0    12820 2023-02-03 13:44:29.383103 cag-1.5.17/examples/data/periodic_wiki_batches/Machine_learning/10Oct2021-12Oct2021/rademacher-complexity_revisions.parquet
+-rw-r--r--   0        0        0    27530 2023-02-03 13:44:29.383103 cag-1.5.17/examples/data/periodic_wiki_batches/Machine_learning/10Oct2021-12Oct2021/support-vector-machine_revisions.parquet
+-rw-r--r--   0        0        0   120147 2023-02-03 13:44:29.383103 cag-1.5.17/examples/data/periodic_wiki_batches/Machine_learning/10Oct2021-12Oct2021/underfitting_revisions.parquet
+-rw-r--r--   0        0        0    15129 2023-02-03 13:44:29.383103 cag-1.5.17/examples/data/periodic_wiki_batches/Machine_learning/10Oct2021-12Oct2021/unsupervised-learning_revisions.parquet
+-rw-r--r--   0        0        0   144227 2023-02-03 13:44:29.398699 cag-1.5.17/examples/data/periodic_wiki_batches/Machine_learning/10Oct2021-12Oct2021/validation-set_revisions.parquet
+-rw-r--r--   0        0        0    13203 2023-02-03 13:44:29.398699 cag-1.5.17/examples/data/periodic_wiki_batches/Machine_learning/10Oct2021-12Oct2021/weak-supervision_revisions.parquet
+-rw-r--r--   0        0        0    35165 2023-02-03 13:44:29.398699 cag-1.5.17/examples/data/periodic_wiki_batches/Machine_learning/10Oct2022-12Oct2022/alex-james-professor_revisions.parquet
+-rw-r--r--   0        0        0    15382 2023-02-03 13:44:29.398699 cag-1.5.17/examples/data/periodic_wiki_batches/Machine_learning/10Oct2022-12Oct2022/data-version-control_revisions.parquet
+-rw-r--r--   0        0        0    29431 2023-02-03 13:44:29.398699 cag-1.5.17/examples/data/periodic_wiki_batches/Machine_learning/10Oct2022-12Oct2022/deepnude_revisions.parquet
+-rw-r--r--   0        0        0    61781 2023-02-03 13:44:29.398699 cag-1.5.17/examples/data/periodic_wiki_batches/Machine_learning/10Oct2022-12Oct2022/facial-recognition-system_revisions.parquet
+-rw-r--r--   0        0        0    33859 2023-02-03 13:44:29.398699 cag-1.5.17/examples/data/periodic_wiki_batches/Machine_learning/10Oct2022-12Oct2022/feature-learning_revisions.parquet
+-rw-r--r--   0        0        0    36983 2023-02-03 13:44:29.398699 cag-1.5.17/examples/data/periodic_wiki_batches/Machine_learning/10Oct2022-12Oct2022/julia-programming-language_revisions.parquet
+-rw-r--r--   0        0        0    20270 2023-02-03 13:44:29.398699 cag-1.5.17/examples/data/periodic_wiki_batches/Machine_learning/10Oct2022-12Oct2022/models-of-dna-evolution_revisions.parquet
+-rw-r--r--   0        0        0    85401 2023-02-03 13:44:29.398699 cag-1.5.17/examples/data/periodic_wiki_batches/Machine_learning/10Oct2022-12Oct2022/multipleinstance-learning_revisions.parquet
+-rw-r--r--   0        0        0    24168 2023-02-03 13:44:29.398699 cag-1.5.17/examples/data/periodic_wiki_batches/Machine_learning/10Oct2022-12Oct2022/nikiai_revisions.parquet
+-rw-r--r--   0        0        0    26362 2023-02-03 13:44:29.398699 cag-1.5.17/examples/data/periodic_wiki_batches/Machine_learning/10Oct2022-12Oct2022/onnx_revisions.parquet
+-rw-r--r--   0        0        0    16064 2023-02-03 13:44:29.398699 cag-1.5.17/examples/data/periodic_wiki_batches/Machine_learning/10Oct2022-12Oct2022/overfitting_revisions.parquet
+-rw-r--r--   0        0        0    11787 2023-02-03 13:44:29.398699 cag-1.5.17/examples/data/periodic_wiki_batches/Machine_learning/10Oct2022-12Oct2022/pop-music-automation_revisions.parquet
+-rw-r--r--   0        0        0    15259 2023-02-03 13:44:29.398699 cag-1.5.17/examples/data/periodic_wiki_batches/Machine_learning/10Oct2022-12Oct2022/prescription-monitoring-program_revisions.parquet
+-rw-r--r--   0        0        0   189865 2023-02-03 13:44:29.398699 cag-1.5.17/examples/data/periodic_wiki_batches/Machine_learning/10Oct2022-12Oct2022/squared-error-loss_revisions.parquet
+-rw-r--r--   0        0        0    20292 2023-02-03 13:44:29.398699 cag-1.5.17/examples/data/periodic_wiki_batches/Machine_learning/10Oct2022-12Oct2022/stochastic-gradient-descent_revisions.parquet
+-rw-r--r--   0        0        0    15014 2023-02-03 13:44:29.398699 cag-1.5.17/examples/data/periodic_wiki_batches/Machine_learning/10Oct2022-12Oct2022/symbolic-regression_revisions.parquet
+-rw-r--r--   0        0        0    27282 2023-02-03 13:44:29.398699 cag-1.5.17/examples/data/periodic_wiki_batches/Machine_learning/10Oct2022-12Oct2022/word2vec_revisions.parquet
+-rw-r--r--   0        0        0  3919314 2023-02-03 13:44:29.414327 cag-1.5.17/examples/example.html
+-rw-r--r--   0        0        0     1963 2023-06-04 21:32:13.424631 cag-1.5.17/examples/view_creation_example.py
+-rw-r--r--   0        0        0     1458 2023-06-22 14:50:45.528118 cag-1.5.17/pyproject.toml
+-rw-r--r--   0        0        0      361 2023-06-22 14:50:45.528118 cag-1.5.17/requirements.txt
+-rw-r--r--   0        0        0      518 2023-05-10 08:19:54.150201 cag-1.5.17/tests/__init__.py
+-rw-r--r--   0        0        0    11993 2023-05-10 08:19:54.151939 cag-1.5.17/tests/test_graph_creator.py
+-rw-r--r--   0        0        0     3130 2023-05-10 08:19:54.156776 cag-1.5.17/tests/test_graph_creator/test_improve_edge_definitions.py
+-rw-r--r--   0        0        0     8316 2023-05-10 08:19:54.158278 cag-1.5.17/tests/test_view.py
+-rw-r--r--   0        0        0     5830 1970-01-01 00:00:00.000000 cag-1.5.17/PKG-INFO
```

### Comparing `cag-1.5.0/.github/workflows/main.yml` & `cag-1.5.17/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `cag-1.5.0/.gitignore` & `cag-1.5.17/.gitignore`

 * *Files identical despite different names*

### Comparing `cag-1.5.0/.gitlab-ci.yml` & `cag-1.5.17/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `cag-1.5.0/CITATION.cff` & `cag-1.5.17/CITATION.cff`

 * *Files identical despite different names*

### Comparing `cag-1.5.0/LICENSE` & `cag-1.5.17/LICENSE`

 * *Files identical despite different names*

### Comparing `cag-1.5.0/README.md` & `cag-1.5.17/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 > `cag` is a Python Library offering an architectural framework to employ the build-annotate pattern when building Graphs.
 
 ---
 
 
 
-[Paper video](https://drive.google.com/drive/folders/1KE4NT2NQyfj4VYsAdQAE8WoBpGWA33O0?usp=sharing).
+[Official Documentation](https://cagraph.info/).
 
 **Corpus Annotation Graph builder (CAG)**  is an *architectural framework* that employs the *build-and-annotate* pattern for creating a graph. CAG is built on top of [ArangoDB](https://www.arangodb.com) and its Python drivers ([PyArango](https://pyarango.readthedocs.io/en/latest/)). The *build-and-annotate* pattern consists of two phases (see Figure below): (1) data is collected from different sources (e.g., publication databases, online encyclopedias, news feeds, web portals, electronic libraries, repositories, media platforms) and preprocessed to build the core nodes, which we call *Objects of Interest*. The component responsible for this phase is the **Graph-Creator**. (2) Annotations are extracted from the OOIs, and corresponding annotation nodes are created and linked to the core nodes. The component dealing with this phase is the **Graph-Annotator**.
 
 
 ![cag](https://github.com/DLR-SC/corpus-annotation-graph-builder/blob/main/docs/cag.png?raw=true)
 
 
@@ -53,30 +53,41 @@
 
 ### Manual cloning
 Clone the repository, go to the root folder and then run:
 
 ```
 pip install -e .
 ```
+
+## Citation
+Please cite us in case you use CAG
+
+    @inproceedings{el-baff-etal-2023-corpus,
+      title = "Corpus Annotation Graph Builder ({CAG}): An Architectural Framework to Create and Annotate a Multi-source Graph",
+      author = "El Baff, Roxanne  and
+        Hecking, Tobias  and
+        Hamm, Andreas  and
+        Korte, Jasper W.  and
+        Bartsch, Sabine",
+      booktitle = "Proceedings of the 17th Conference of the European Chapter of the Association for Computational Linguistics: System Demonstrations",
+      month = may,
+      year = "2023",
+      address = "Dubrovnik, Croatia",
+      publisher = "Association for Computational Linguistics",
+      url = "https://aclanthology.org/2023.eacl-demo.28",
+      pages = "248--255"
+    }
+
+
 ## Usage
 * After the installation, a project scaffold can be created with the command `cag start-project`
 * Graph Creation [[jupyter notebook](https://github.com/DLR-SC/corpus-annotation-graph-builder/blob/main/examples/1_create_graph.ipynb)]
 * Graph Annotation [[jupyter notebook](https://github.com/DLR-SC/corpus-annotation-graph-builder/blob/main/examples/2_annotate_graph.ipynb)]
 
 
-## Citation
-Please cite us in case you use CAG
 
-      @InProceedings{elbaffdemo:2023,
-        author =  {Roxanne {El Baff} and Tobias Hecking and Andreas Hamm and Jasper W. Korte and Sabine Bartsch},
-        title     = {Corpus {A}nnotation {G}raph Builder ({CAG}):  An Architectural Framework to Create and Annotate a Multi-source Graph},
-        booktitle = {The 17th Conference of the European Chapter of the Association for Computational Linguistics (EACL 2023): : System Demonstrations },
-        month = "may",
-        year = "2023"
-        address = "Dubrovnik, Croatia",
-        publisher = "Association for Computational Linguistics",
-        }
+## Zenodo refs
 
+* v1.5.0 [![DOI](https://zenodo.org/badge/572124344.svg)](https://zenodo.org/badge/latestdoi/572124344)
+* v1.4.0 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7701921.svg)](https://doi.org/10.5281/zenodo.7701921)
 
-## Zenodo refs
-v1.4.0 [![DOI](https://zenodo.org/badge/572124344.svg)](https://zenodo.org/badge/latestdoi/572124344)
```

#### html2text {}

```diff
@@ -1,40 +1,43 @@
       ****** Welcome to the Corpus Annotation Graph Builder (CAG) ******
 [Badge:_PyPI_version] [Badge:_Made_with_Python] [Badge:_Open_in_VSCode] [Badge:
               Black] [DOI] [License:_MIT] [Twitter:_DLR_Software]
 > `cag` is a Python Library offering an architectural framework to employ the
-build-annotate pattern when building Graphs. --- [Paper video](https://
-drive.google.com/drive/folders/1KE4NT2NQyfj4VYsAdQAE8WoBpGWA33O0?usp=sharing).
-**Corpus Annotation Graph builder (CAG)** is an *architectural framework* that
-employs the *build-and-annotate* pattern for creating a graph. CAG is built on
-top of [ArangoDB](https://www.arangodb.com) and its Python drivers ([PyArango]
-(https://pyarango.readthedocs.io/en/latest/)). The *build-and-annotate* pattern
-consists of two phases (see Figure below): (1) data is collected from different
-sources (e.g., publication databases, online encyclopedias, news feeds, web
-portals, electronic libraries, repositories, media platforms) and preprocessed
-to build the core nodes, which we call *Objects of Interest*. The component
-responsible for this phase is the **Graph-Creator**. (2) Annotations are
-extracted from the OOIs, and corresponding annotation nodes are created and
-linked to the core nodes. The component dealing with this phase is the **Graph-
-Annotator**. ![cag](https://github.com/DLR-SC/corpus-annotation-graph-builder/
-blob/main/docs/cag.png?raw=true) This framework aims to offer researchers a
-flexible but unified and reproducible way of organizing and maintaining their
-interlinked document collections in a Corpus Annotation Graph. ## Installation
-### Direct install via pip The package can also be installed directly via pip.
-``` pip install cag ``` This will allow you to use the module **`cag`** from
-any python script locally. The two main packages are **`cag.framework`** and
+build-annotate pattern when building Graphs. --- [Official Documentation]
+(https://cagraph.info/). **Corpus Annotation Graph builder (CAG)** is an
+*architectural framework* that employs the *build-and-annotate* pattern for
+creating a graph. CAG is built on top of [ArangoDB](https://www.arangodb.com)
+and its Python drivers ([PyArango](https://pyarango.readthedocs.io/en/latest/
+)). The *build-and-annotate* pattern consists of two phases (see Figure below):
+(1) data is collected from different sources (e.g., publication databases,
+online encyclopedias, news feeds, web portals, electronic libraries,
+repositories, media platforms) and preprocessed to build the core nodes, which
+we call *Objects of Interest*. The component responsible for this phase is the
+**Graph-Creator**. (2) Annotations are extracted from the OOIs, and
+corresponding annotation nodes are created and linked to the core nodes. The
+component dealing with this phase is the **Graph-Annotator**. ![cag](https://
+github.com/DLR-SC/corpus-annotation-graph-builder/blob/main/docs/
+cag.png?raw=true) This framework aims to offer researchers a flexible but
+unified and reproducible way of organizing and maintaining their interlinked
+document collections in a Corpus Annotation Graph. ## Installation ### Direct
+install via pip The package can also be installed directly via pip. ``` pip
+install cag ``` This will allow you to use the module **`cag`** from any python
+script locally. The two main packages are **`cag.framework`** and
 **`cag.view_wrapper`**. ### Manual cloning Clone the repository, go to the root
-folder and then run: ``` pip install -e . ``` ## Usage * After the
-installation, a project scaffold can be created with the command `cag start-
-project` * Graph Creation [[jupyter notebook](https://github.com/DLR-SC/corpus-
-annotation-graph-builder/blob/main/examples/1_create_graph.ipynb)] * Graph
-Annotation [[jupyter notebook](https://github.com/DLR-SC/corpus-annotation-
-graph-builder/blob/main/examples/2_annotate_graph.ipynb)] ## Citation Please
-cite us in case you use CAG @InProceedings{elbaffdemo:2023, author = {Roxanne
-{El Baff} and Tobias Hecking and Andreas Hamm and Jasper W. Korte and Sabine
-Bartsch}, title = {Corpus {A}nnotation {G}raph Builder ({CAG}): An
-Architectural Framework to Create and Annotate a Multi-source Graph}, booktitle
-= {The 17th Conference of the European Chapter of the Association for
-Computational Linguistics (EACL 2023): : System Demonstrations }, month =
-"may", year = "2023" address = "Dubrovnik, Croatia", publisher = "Association
-for Computational Linguistics", } ## Zenodo refs v1.4.0 [![DOI](https://
-zenodo.org/badge/572124344.svg)](https://zenodo.org/badge/latestdoi/572124344)
+folder and then run: ``` pip install -e . ``` ## Citation Please cite us in
+case you use CAG @inproceedings{el-baff-etal-2023-corpus, title = "Corpus
+Annotation Graph Builder ({CAG}): An Architectural Framework to Create and
+Annotate a Multi-source Graph", author = "El Baff, Roxanne and Hecking, Tobias
+and Hamm, Andreas and Korte, Jasper W. and Bartsch, Sabine", booktitle =
+"Proceedings of the 17th Conference of the European Chapter of the Association
+for Computational Linguistics: System Demonstrations", month = may, year =
+"2023", address = "Dubrovnik, Croatia", publisher = "Association for
+Computational Linguistics", url = "https://aclanthology.org/2023.eacl-demo.28",
+pages = "248--255" } ## Usage * After the installation, a project scaffold can
+be created with the command `cag start-project` * Graph Creation [[jupyter
+notebook](https://github.com/DLR-SC/corpus-annotation-graph-builder/blob/main/
+examples/1_create_graph.ipynb)] * Graph Annotation [[jupyter notebook](https://
+github.com/DLR-SC/corpus-annotation-graph-builder/blob/main/examples/
+2_annotate_graph.ipynb)] ## Zenodo refs * v1.5.0 [![DOI](https://zenodo.org/
+badge/572124344.svg)](https://zenodo.org/badge/latestdoi/572124344) * v1.4.0 [!
+[DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7701921.svg)](https://
+doi.org/10.5281/zenodo.7701921)
```

### Comparing `cag-1.5.0/cag/__init__.py` & `cag-1.5.17/cag/__init__.py`

 * *Files identical despite different names*

### Comparing `cag-1.5.0/cag/cli.py` & `cag-1.5.17/cag/cli.py`

 * *Files identical despite different names*

### Comparing `cag-1.5.0/cag/cookiecutter.json` & `cag-1.5.17/cag/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `cag-1.5.0/cag/framework/analyzer/analyzer_base.py` & `cag-1.5.17/cag/framework/analyzer/analyzer_base.py`

 * *Files identical despite different names*

### Comparing `cag-1.5.0/cag/framework/annotator/annotator_base.py` & `cag-1.5.17/cag/framework/annotator/annotator_base.py`

 * *Files identical despite different names*

### Comparing `cag-1.5.0/cag/framework/annotator/element/graph_elements.py` & `cag-1.5.17/cag/framework/annotator/element/graph_elements.py`

 * *Files 23% similar despite different names*

```diff
@@ -60,14 +60,53 @@
 
 class HedgeAnnotationNode(GenericAnnotationNode):
     """A class to define a Hedge node in arangodb - This is used by pyarango to create the Collection"""
 
     _fields = GenericAnnotationNode._fields
 
 
+class OAConceptAnnotationNode(parent_nodes.GenericNode):
+    """A class to define a Named Entity node in arangodb - This is used by pyarango to create the Collection"""
+
+    _fields = {
+        "oa_id": parent_nodes.Field(),
+        "name": parent_nodes.Field(),
+    }
+
+    def __init__(self, database, jsonData):
+        super().__init__(database, jsonData)
+        self.ensureFulltextIndex([ "name"], name="fti_annotator_oaconcept")
+        self.ensurePersistentIndex(["oa_id", "name"], unique=True)
+
+class MediaTopicAnnotationNode(parent_nodes.GenericNode):
+    """A class to define a Named Entity node in arangodb - This is used by pyarango to create the Collection"""
+
+    _fields = {
+        "mediatopic_id": parent_nodes.Field(),
+        "name": parent_nodes.Field(),
+    }
+
+    def __init__(self, database, jsonData):
+        super().__init__(database, jsonData)
+        self.ensureFulltextIndex([ "name"], name="fti_annotator_mediatopic")
+        self.ensurePersistentIndex(["mediatopic_id", "name"], unique=True)
+
+
+class KeyTermAnnotationNode(parent_nodes.GenericNode):
+    """A class to define a Named Entity node in arangodb - This is used by pyarango to create the Collection"""
+
+    _fields = {
+        "name": parent_nodes.Field(),
+    }
+
+    def __init__(self, database, jsonData):
+        super().__init__(database, jsonData)
+        self.ensureFulltextIndex(["name"], name="fti_annotator_keyterm")
+        self.ensurePersistentIndex(["name"], unique=True)
+
 ##############
 #    EDGES   #
 ##############
 class GenericAnnotationEdge(GenericEdge):
     """A class to define an annotation edge in arangodb - This is used by pyarango to create the Collection"""
 
     _fields = {
@@ -143,7 +182,33 @@
         "sentence_index_w_highest_score": Field(default=-1),
         "highest_score": Field(),
     }
 
 
 class HasMpqaAnnotation(GenericAnnotationEdge):
     _fields = GenericAnnotationEdge._fields
+
+
+class HasOAConceptAnnotation(GenericEdge):
+    _fields = {
+        **GenericEdge._fields,
+        "level": Field(),
+        "metadata": Field()
+    }
+
+
+class HasMediaTopicAnnotation(GenericEdge):
+    _fields = {
+        **GenericEdge._fields,
+        "level": Field(),
+        "metadata": Field()
+    }
+
+
+class HasKeyTermAnnotation(GenericEdge):
+    _fields = {
+        **GenericEdge._fields,
+        "rank": Field(),
+        "score": Field(),
+        "metadata": Field()
+
+    }
```

### Comparing `cag-1.5.0/cag/framework/annotator/element/orchestrator.py` & `cag-1.5.17/cag/framework/annotator/element/orchestrator.py`

 * *Files identical despite different names*

### Comparing `cag-1.5.0/cag/framework/annotator/instance/dummy.py` & `cag-1.5.17/cag/framework/annotator/instance/dummy.py`

 * *Files identical despite different names*

### Comparing `cag-1.5.0/cag/framework/annotator/instance/emotion_orchestrator.py` & `cag-1.5.17/cag/framework/annotator/instance/emotion_orchestrator.py`

 * *Files identical despite different names*

### Comparing `cag-1.5.0/cag/framework/annotator/instance/empath_orchestrator.py` & `cag-1.5.17/cag/framework/annotator/instance/empath_orchestrator.py`

 * *Files identical despite different names*

### Comparing `cag-1.5.0/cag/framework/annotator/instance/hedge_orchestrator.py` & `cag-1.5.17/cag/framework/annotator/instance/hedge_orchestrator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from pyArango.document import Document
 from cag.framework.annotator.element.orchestrator import PipeOrchestrator
 import pandas as pd
 
 from cag.framework.annotator.pipe.linguistic.hedge import HedgeFactory
 
 
-class HedgeOrchestrator(PipeOrchestrator):
+class HedgePipeOrchestrator(PipeOrchestrator):
     def create_node(self, hedge_label: str) -> Document:
         data = {"label": hedge_label}
         return self.upsert_node(self.node_name, data, alt_key=["label"])
 
     def create_edge(
         self, _from: Document, _to: Document, hedge_attrs
     ) -> Document:
```

### Comparing `cag-1.5.0/cag/framework/annotator/instance/mpqa_orchestrator.py` & `cag-1.5.17/cag/framework/annotator/instance/mpqa_orchestrator.py`

 * *Files identical despite different names*

### Comparing `cag-1.5.0/cag/framework/annotator/instance/ner_orchestrator.py` & `cag-1.5.17/cag/framework/annotator/instance/ner_orchestrator.py`

 * *Files identical despite different names*

### Comparing `cag-1.5.0/cag/framework/annotator/instance/toxicity_orchestrator.py` & `cag-1.5.17/cag/framework/annotator/instance/toxicity_orchestrator.py`

 * *Files identical despite different names*

### Comparing `cag-1.5.0/cag/framework/annotator/pipe/linguistic/discourse_marker.py` & `cag-1.5.17/cag/framework/annotator/pipe/linguistic/discourse_marker.py`

 * *Files identical despite different names*

### Comparing `cag-1.5.0/cag/framework/annotator/pipe/linguistic/emotion.py` & `cag-1.5.17/cag/framework/annotator/pipe/linguistic/emotion.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,23 +72,23 @@
                 label = sent_emotion_score["label"]
                 score = sent_emotion_score["score"]
 
                 all_scores[label].append(score)
 
                 sentence._.set(f"emotion_{label}", score)
             dominant_lbl = res_df.iloc[res_df["score"].argmax()]["label"]
-            sentence._.set(f"emotion_dominant {dominant_lbl}")
+            sentence._.set("emotion_dominant", dominant_lbl)
             logger.debug("appending")
             sentence_lbls.append(dominant_lbl)
 
         doc_mean_df = pd.DataFrame(
             [
                 {
                     "label": x,
-                    "score_mean": mean(y) if len(y) > 0 else 0.0,
+                    "mean_score": mean(y) if len(y) > 0 else 0.0,
                     "highest_score": max(y),
                     "sentence_index_w_highest_score": np.asarray(y).argmax()
                     if max(y) > 0.0
                     else -1,
                 }
                 for x, y in all_scores.items()
             ]
```

### Comparing `cag-1.5.0/cag/framework/annotator/pipe/linguistic/empath.py` & `cag-1.5.17/cag/framework/annotator/pipe/linguistic/empath.py`

 * *Files identical despite different names*

### Comparing `cag-1.5.0/cag/framework/annotator/pipe/linguistic/hedge.py` & `cag-1.5.17/cag/framework/annotator/pipe/linguistic/hedge.py`

 * *Files identical despite different names*

### Comparing `cag-1.5.0/cag/framework/annotator/pipe/linguistic/metadata.py` & `cag-1.5.17/cag/framework/annotator/pipe/linguistic/metadata.py`

 * *Files identical despite different names*

### Comparing `cag-1.5.0/cag/framework/annotator/pipe/linguistic/mpqa.py` & `cag-1.5.17/cag/framework/annotator/pipe/linguistic/mpqa.py`

 * *Files identical despite different names*

### Comparing `cag-1.5.0/cag/framework/annotator/pipe/linguistic/style_features.py` & `cag-1.5.17/cag/framework/annotator/pipe/linguistic/style_features.py`

 * *Files identical despite different names*

### Comparing `cag-1.5.0/cag/framework/annotator/pipe/linguistic/toxicity.py` & `cag-1.5.17/cag/framework/annotator/pipe/linguistic/toxicity.py`

 * *Files identical despite different names*

### Comparing `cag-1.5.0/cag/framework/annotator/pipe/linguistic/typos.py` & `cag-1.5.17/cag/framework/annotator/pipe/linguistic/typos.py`

 * *Files identical despite different names*

### Comparing `cag-1.5.0/cag/framework/annotator/pipeline/pipeline_base.py` & `cag-1.5.17/cag/framework/annotator/pipeline/pipeline_base.py`

 * *Files 14% similar despite different names*

```diff
@@ -165,16 +165,32 @@
                         self.out_df = self.out_df.merge(
                             _df,
                             how="outer",
                             left_on="text_key",
                             right_on="text_key",
                         )
         if self.out_path is not None and self.out_path != "":
-            logger.debug("Saving to parquet..")
-            self.out_df.to_parquet(self.out_path)
+            try:
+                utils.create_folder(self.out_path)
+                name_format= self.out_path.split('.')
+                format = "csv"
+                if len(name_format) > 1:
+                    format = name_format[-1]
+                else: self.out_path = self.out_path + ".csv"
+                
+                if format == "parquet":
+                    logger.info(f"Saving to parquet: {self.out_path}")
+                    self.out_df.to_parquet(self.out_path)
+                elif format ==  "csv":
+                    logger.info(f"Saving to csv: {self.out_path}")
+                    self.out_df.to_csv(self.out_path)
+                else:
+                    logger.info("your out_path should end with .parquet or .csv")
+            except:
+                logger.warning(f"Failed to save file {self.out_path}")
         logger.debug("saved annotations")
 
     ####################################
     #           SETTERS                #
     ####################################
     def reset_input_output(self):
         self.set_input(None)
@@ -293,14 +309,15 @@
                     "parser",
                     "attribute_ruler",
                     "lemmatizer",
                     "ner",
                 ],
             )
         )
+        nlp.max_length=1500000
         for pipe in subpipeline:
             if not nlp.has_pipe(pipe.pipe_id_or_func):
                 if pipe.pipe_id_or_func in nlp.disabled:
                     nlp.enable_pipe(pipe.pipe_id_or_func)
                 else:
                     nlp.add_pipe(pipe.pipe_id_or_func)  # , **kargs)
             else:
```

### Comparing `cag-1.5.0/cag/framework/annotator/registered_pipes.py` & `cag-1.5.17/cag/framework/annotator/registered_pipes.py`

 * *Files 15% similar despite different names*

```diff
@@ -92,14 +92,50 @@
     PipeConfigKeys._level: "node",  # node or set
     PipeConfigKeys._data_type: "text",  # for now we support text - later url, image
     PipeConfigKeys._annotated_node_name: "TextNode",
     PipeConfigKeys._node_class: "cag.framework.annotator.element.graph_elements.ToxicityAnnotationNode",
     PipeConfigKeys._edge_class: "cag.framework.annotator.element.graph_elements.HasToxicityAnnotation",
 }
 
+_dict["OpenAlexConcept"] = {
+    PipeConfigKeys._orchestrator_class: "cag.framework.annotator.instance.openalex_concept_orchestrator.OAConceptPipeOrchestrator",
+    PipeConfigKeys._pipe_id_or_func: "openalex_concept_component",  # id in case of space, function name otherwise
+    PipeConfigKeys._pipe_path: "cag.framework.annotator.pipe.linguistic.oaconcept",  # leave empty if the pipe is a spacy native pipe, otherwise provide the path of where the pipe_id_or_func exists
+    PipeConfigKeys._level: "node",  # node or set
+    PipeConfigKeys._data_type: "text",  # for now we support text - later url, image
+    PipeConfigKeys._annotated_node_name: "TextNode",
+    PipeConfigKeys._node_class: "cag.framework.annotator.element.graph_elements.OAConceptAnnotationNode",
+    PipeConfigKeys._edge_class: "cag.framework.annotator.element.graph_elements.HasOAConceptAnnotation",
+}
+
+
+_dict["IPTCMediaTopic"] = {
+    PipeConfigKeys._orchestrator_class: "cag.framework.annotator.instance.iptcmedia_topic_orchestrator.MediaTopicPipeOrchestrator",
+    PipeConfigKeys._pipe_id_or_func: "iptc_media_topic_component",  # id in case of space, function name otherwise
+    PipeConfigKeys._pipe_path: "cag.framework.annotator.pipe.linguistic.iptcmedia_topic",  # leave empty if the pipe is a spacy native pipe, otherwise provide the path of where the pipe_id_or_func exists
+    PipeConfigKeys._level: "node",  # node or set
+    PipeConfigKeys._data_type: "text",  # for now we support text - later url, image
+    PipeConfigKeys._annotated_node_name: "TextNode",
+    PipeConfigKeys._node_class: "cag.framework.annotator.element.graph_elements.MediaTopicAnnotationNode",
+    PipeConfigKeys._edge_class: "cag.framework.annotator.element.graph_elements.HasMediaTopicAnnotation",
+}
+
+_dict["Keyterms"] = {
+    PipeConfigKeys._orchestrator_class: "cag.framework.annotator.instance.keyterms_orchestrator.KeyTermsPipeOrchestrator",
+    PipeConfigKeys._pipe_id_or_func: "keyterms_component",  # id in case of space, function name otherwise
+    PipeConfigKeys._pipe_path: "cag.framework.annotator.pipe.linguistic.keyterms",  # leave empty if the pipe is a spacy native pipe, otherwise provide the path of where the pipe_id_or_func exists
+    PipeConfigKeys._level: "node",  # node or set
+    PipeConfigKeys._data_type: "text",  # for now we support text - later url, image
+    PipeConfigKeys._annotated_node_name: "TextNode",
+    PipeConfigKeys._node_class: "cag.framework.annotator.element.graph_elements.KeyTermAnnotationNode",
+    PipeConfigKeys._edge_class: "cag.framework.annotator.element.graph_elements.HasKeyTermAnnotation",
+}
+
+
+
 _dict["DummyPipeOrchestrator"] = {
     PipeConfigKeys._orchestrator_class: "cag.framework.annotator.instance.dummy.DummyPipeOrchestrator",
     PipeConfigKeys._pipe_id_or_func: "customized_pipe_func",  # id in case of space, function name otherwise
     PipeConfigKeys._pipe_path: "cag.framework.annotator.instance.dummy",  # leave empty if the pipe is a spacy native pipe, otherwise provide the path of where the pipe_id_or_func exists
     PipeConfigKeys._level: "node",  # node or set
     PipeConfigKeys._data_type: "text",  # for now we support text - later url, image
     PipeConfigKeys._annotated_node_name: "TextNode",
```

### Comparing `cag-1.5.0/cag/framework/component.py` & `cag-1.5.17/cag/framework/component.py`

 * *Files identical despite different names*

### Comparing `cag-1.5.0/cag/framework/creator/base_creator.py` & `cag-1.5.17/cag/framework/creator/base_creator.py`

 * *Files 0% similar despite different names*

```diff
@@ -164,15 +164,15 @@
             "uri": uri,
             "description": description,
             "name": name,
             "timestamp": timestamp,
             "copyright": copyright,
         }
 
-        video = self.upsert_node(IFrameNode.__name__, dict_, alt_key="url")
+        video = self.upsert_node(IFrameNode.__name__, dict_, alt_key="uri")
         return video
 
     def create_author_node(self, author_name, timestamp=None):
         dict_ = {"name": author_name, "timestamp": timestamp}
 
         author = self.upsert_node(
             GraphCreatorBase._AUTHOR_NODE_NAME, dict_, alt_key="name"
```

### Comparing `cag-1.5.0/cag/graph_elements/base_graph.py` & `cag-1.5.17/cag/graph_elements/base_graph.py`

 * *Files identical despite different names*

### Comparing `cag-1.5.0/cag/graph_elements/nodes.py` & `cag-1.5.17/cag/graph_elements/nodes.py`

 * *Files identical despite different names*

### Comparing `cag-1.5.0/cag/graph_elements/relations.py` & `cag-1.5.17/cag/graph_elements/relations.py`

 * *Files identical despite different names*

### Comparing `cag-1.5.0/cag/utils/config.py` & `cag-1.5.17/cag/utils/config.py`

 * *Files identical despite different names*

### Comparing `cag-1.5.0/cag/utils/timer.py` & `cag-1.5.17/cag/utils/timer.py`

 * *Files identical despite different names*

### Comparing `cag-1.5.0/cag/utils/utils.py` & `cag-1.5.17/cag/utils/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import hashlib
 import importlib
 import json
 import pkgutil
 import urllib
 from re import sub
 
+from pathlib import Path
 
 def get_hash_from_str(str: str) -> str:
     """generate a sha256-16 byte int from your string to use as a key
 
     :param str: the string to hash
     :type str: str
     :return: the hasehed string
@@ -91,7 +92,10 @@
     # print(f"prefix {prefix}")
     for importer, modname, ispkg in pkgutil.iter_modules(
         package.__path__, prefix
     ):
         # print(f"Found submodule {modname} (is a package: {ispkg})" )
         _ = load_module(modname)
         # print (f"Imported {module}")
+
+def create_folder(path):
+    Path(path).mkdir(parents=True, exist_ok=True)
```

### Comparing `cag-1.5.0/cag/view_wrapper/arango_analyzer.py` & `cag-1.5.17/cag/view_wrapper/arango_analyzer.py`

 * *Files identical despite different names*

### Comparing `cag-1.5.0/cag/view_wrapper/link.py` & `cag-1.5.17/cag/view_wrapper/link.py`

 * *Files identical despite different names*

### Comparing `cag-1.5.0/cag/view_wrapper/view.py` & `cag-1.5.17/cag/view_wrapper/view.py`

 * *Files identical despite different names*

### Comparing `cag-1.5.0/cag/{{cookiecutter.project_slug}}/.gitignore` & `cag-1.5.17/cag/{{cookiecutter.project_slug}}/.gitignore`

 * *Files identical despite different names*

### Comparing `cag-1.5.0/cag/{{cookiecutter.project_slug}}/CONTRIBUTING.rst` & `cag-1.5.17/cag/{{cookiecutter.project_slug}}/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `cag-1.5.0/cag/{{cookiecutter.project_slug}}/LICENSE` & `cag-1.5.17/cag/{{cookiecutter.project_slug}}/LICENSE`

 * *Files identical despite different names*

### Comparing `cag-1.5.0/cag/{{cookiecutter.project_slug}}/Makefile` & `cag-1.5.17/cag/{{cookiecutter.project_slug}}/Makefile`

 * *Files identical despite different names*

### Comparing `cag-1.5.0/cag/{{cookiecutter.project_slug}}/README.rst` & `cag-1.5.17/cag/{{cookiecutter.project_slug}}/README.rst`

 * *Files identical despite different names*

### Comparing `cag-1.5.0/cag/{{cookiecutter.project_slug}}/docs/Makefile` & `cag-1.5.17/cag/{{cookiecutter.project_slug}}/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cag-1.5.0/cag/{{cookiecutter.project_slug}}/docs/conf.py` & `cag-1.5.17/cag/{{cookiecutter.project_slug}}/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cag-1.5.0/cag/{{cookiecutter.project_slug}}/docs/installation.rst` & `cag-1.5.17/cag/{{cookiecutter.project_slug}}/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `cag-1.5.0/cag/{{cookiecutter.project_slug}}/docs/make.bat` & `cag-1.5.17/cag/{{cookiecutter.project_slug}}/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cag-1.5.0/cag/{{cookiecutter.project_slug}}/setup.py` & `cag-1.5.17/cag/{{cookiecutter.project_slug}}/setup.py`

 * *Files identical despite different names*

### Comparing `cag-1.5.0/cag/{{cookiecutter.project_slug}}/tests/test_{{cookiecutter.project_slug}}.py` & `cag-1.5.17/cag/{{cookiecutter.project_slug}}/tests/test_{{cookiecutter.project_slug}}.py`

 * *Files identical despite different names*

### Comparing `cag-1.5.0/cag/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/MovieEmbeddings.py` & `cag-1.5.17/cag/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/MovieEmbeddings.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,17 +80,17 @@
             description_batch = datasets_df_batch.description.tolist()
 
             title_embs = self.generate_fake_embedding(title_batch)
             ab_embs = self.generate_fake_embedding(description_batch)
 
             datasets_df_batch.loc[:, "title_emb"] = list(title_embs)
             datasets_df_batch.loc[:, "description_emb"] = list(ab_embs)
-            datasets_df_batch["title_emb"] = datasets_df_batch["title_emb"].apply(
-                lambda x: x.squeeze().tolist()
-            )
+            datasets_df_batch["title_emb"] = datasets_df_batch[
+                "title_emb"
+            ].apply(lambda x: x.squeeze().tolist())
             datasets_df_batch["description_emb"] = datasets_df_batch[
                 "description_emb"
             ].apply(lambda x: x.squeeze().tolist())
             update_batch = datasets_df_batch.loc[
                 :, ["_id", "title_emb", "description_emb"]
             ].to_dict("records")
             ds_collection.update_many(update_batch)
```

### Comparing `cag-1.5.0/cag/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/cli.py` & `cag-1.5.17/cag/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/cli.py`

 * *Files identical despite different names*

### Comparing `cag-1.5.0/cag/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/conf.py` & `cag-1.5.17/cag/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/conf.py`

 * *Files identical despite different names*

### Comparing `cag-1.5.0/cag/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/data/sample_data.json` & `cag-1.5.17/cag/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/data/sample_data.json`

 * *Files identical despite different names*

### Comparing `cag-1.5.0/cag/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/edges.py` & `cag-1.5.17/cag/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/edges.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,17 +7,19 @@
     A class representing a 'played in' edge in a graph.
 
     Inherits from GenericEdge class.
 
     Attributes:
         _fields (dict): A dictionary containing the fields and their respective types for the 'played in' edge.
     """
+
     _fields = {"rating": Field(), **GenericEdge._fields}
 
 
 class Directed(GenericEdge):
     """
     A class representing a 'directed' edge in a graph.
 
     Inherits from GenericEdge class.
     """
+
     ...
```

### Comparing `cag-1.5.0/cag/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/graph.py` & `cag-1.5.17/cag/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/graph.py`

 * *Files 3% similar despite different names*

```diff
@@ -59,26 +59,30 @@
                     "year": entry["year"],
                     "genre": entry["genre"],
                     "description": entry["description"],
                 },
             )
             for actor in entry["actors"]:
                 actor_node = self.upsert_node(
-                    "Actor", {"name": actor["name"], "birthdate": actor["birthdate"]}
+                    "Actor",
+                    {"name": actor["name"], "birthdate": actor["birthdate"]},
                 )
                 self.upsert_edge(
                     "PlayedIn",
                     actor_node,
                     movie_node,
                     edge_attrs={"rating": actor["rating"]},
                 )
             for director in entry["directors"]:
                 director_node = self.upsert_node(
                     "Director",
-                    {"name": director["name"], "birthdate": director["birthdate"]},
+                    {
+                        "name": director["name"],
+                        "birthdate": director["birthdate"],
+                    },
                 )
                 self.upsert_edge("Directed", director_node, movie_node)
 
     def create_view(self):
         """
         Creates a view for the movies collection with fuzzy search and tokenization analyzers.
 
@@ -105,15 +109,16 @@
         link_analyzers = AnalyzerList(["fuzzy_search_bigram", "en_tokenizer"])
         link.analyzers = link_analyzers
 
         title_field = ViewField(
             "title", AnalyzerList(["fuzzy_search_bigram", "en_tokenizer"])
         )
         description_field = ViewField(
-            "description", AnalyzerList(["fuzzy_search_bigram", "en_tokenizer"])
+            "description",
+            AnalyzerList(["fuzzy_search_bigram", "en_tokenizer"]),
         )
 
         title_emb_field = ViewField("title_emb")
         description_emb_field = ViewField("description_emb")
         id_field = ViewField("_id")
 
         link.add_field(title_field)
```

### Comparing `cag-1.5.0/cag/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/nodes.py` & `cag-1.5.17/cag/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/nodes.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     A class representing a movie node in a graph.
 
     Attributes:
         _name (str): The name of the movie node.
         _fields (dict): A dictionary containing the fields and their respective types for the movie node.
 
     """
+
     _name = "Movie"
     _fields = {
         "name": Field(),
         "year": Field(),
         "genre": Field(),
         "description": Field(),
         **GenericOOSNode._fields,
@@ -24,26 +25,29 @@
     """
     A class representing a person node in a graph.
 
     Attributes:
         _fields (dict): A dictionary containing the fields and their respective types for the person node.
 
     """
+
     _fields = {"name": Field(), "birthdate": Field(), **GenericOOSNode._fields}
 
 
 class Actor(Person):
     """
     A class representing an actor node in a graph.
 
     Inherits from Person class.
     """
+
     ...
 
 
 class Director(Person):
     """
     A class representing a director node in a graph.
 
     Inherits from Person class.
     """
+
     ...
```

### Comparing `cag-1.5.0/docs/Makefile` & `cag-1.5.17/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cag-1.5.0/docs/cag.pdf` & `cag-1.5.17/docs/cag.pdf`

 * *Files identical despite different names*

### Comparing `cag-1.5.0/docs/cag.png` & `cag-1.5.17/docs/cag.png`

 * *Files identical despite different names*

### Comparing `cag-1.5.0/docs/make.bat` & `cag-1.5.17/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cag-1.5.0/docs/source/conf.py` & `cag-1.5.17/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `cag-1.5.0/docs/source/imgs/data_model.png` & `cag-1.5.17/docs/source/imgs/data_model.png`

 * *Files identical despite different names*

### Comparing `cag-1.5.0/docs/source/index.rst` & `cag-1.5.17/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `cag-1.5.0/docs/source/reference/0_concept.rst` & `cag-1.5.17/docs/source/reference/0_concept.rst`

 * *Files identical despite different names*

### Comparing `cag-1.5.0/docs/source/reference/1_get_started.rst` & `cag-1.5.17/docs/source/reference/1_get_started.rst`

 * *Files identical despite different names*

### Comparing `cag-1.5.0/docs/source/reference/2_annotator.rst` & `cag-1.5.17/docs/source/reference/2_annotator.rst`

 * *Files identical despite different names*

### Comparing `cag-1.5.0/docs/source/reference/3_analyzers.rst` & `cag-1.5.17/docs/source/reference/3_analyzers.rst`

 * *Files identical despite different names*

### Comparing `cag-1.5.0/docs/source/reference/4_view_management.rst` & `cag-1.5.17/docs/source/reference/4_view_management.rst`

 * *Files identical despite different names*

### Comparing `cag-1.5.0/examples/0_download_process_data.ipynb` & `cag-1.5.17/examples/0_download_process_data.ipynb`

 * *Files identical despite different names*

### Comparing `cag-1.5.0/examples/1_create_graph.ipynb` & `cag-1.5.17/examples/1_create_graph.ipynb`

 * *Files identical despite different names*

### Comparing `cag-1.5.0/examples/2_annotate_graph.ipynb` & `cag-1.5.17/examples/2_annotate_graph.ipynb`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 25% similar despite different names*

```diff
@@ -1,478 +1,494 @@
-00000000: 7b0a 2022 6365 6c6c 7322 3a20 5b0a 2020  {. "cells": [.  
-00000010: 7b0a 2020 2022 6365 6c6c 5f74 7970 6522  {.   "cell_type"
-00000020: 3a20 2263 6f64 6522 2c0a 2020 2022 6578  : "code",.   "ex
-00000030: 6563 7574 696f 6e5f 636f 756e 7422 3a20  ecution_count": 
-00000040: 6e75 6c6c 2c0a 2020 2022 6964 223a 2022  null,.   "id": "
-00000050: 3662 3463 3234 3833 222c 0a20 2020 226d  6b4c2483",.   "m
-00000060: 6574 6164 6174 6122 3a20 7b7d 2c0a 2020  etadata": {},.  
-00000070: 2022 6f75 7470 7574 7322 3a20 5b5d 2c0a   "outputs": [],.
-00000080: 2020 2022 736f 7572 6365 223a 205b 0a20     "source": [. 
-00000090: 2020 2022 2320 2570 6970 2069 6e73 7461     "# %pip insta
-000000a0: 6c6c 202d 6520 2e2e 2f22 0a20 2020 5d0a  ll -e ../".   ].
-000000b0: 2020 7d2c 0a20 207b 0a20 2020 2263 656c    },.  {.   "cel
-000000c0: 6c5f 7479 7065 223a 2022 636f 6465 222c  l_type": "code",
-000000d0: 0a20 2020 2265 7865 6375 7469 6f6e 5f63  .   "execution_c
-000000e0: 6f75 6e74 223a 206e 756c 6c2c 0a20 2020  ount": null,.   
-000000f0: 2269 6422 3a20 2261 6539 3161 3762 6122  "id": "ae91a7ba"
-00000100: 2c0a 2020 2022 6d65 7461 6461 7461 223a  ,.   "metadata":
-00000110: 207b 7d2c 0a20 2020 226f 7574 7075 7473   {},.   "outputs
-00000120: 223a 205b 5d2c 0a20 2020 2273 6f75 7263  ": [],.   "sourc
-00000130: 6522 3a20 5b0a 2020 2020 2225 7069 7020  e": [.    "%pip 
-00000140: 7368 6f77 2063 6167 220a 2020 205d 0a20  show cag".   ]. 
-00000150: 207d 2c0a 2020 7b0a 2020 2022 6365 6c6c   },.  {.   "cell
-00000160: 5f74 7970 6522 3a20 2263 6f64 6522 2c0a  _type": "code",.
-00000170: 2020 2022 6578 6563 7574 696f 6e5f 636f     "execution_co
-00000180: 756e 7422 3a20 6e75 6c6c 2c0a 2020 2022  unt": null,.   "
-00000190: 6964 223a 2022 6231 6163 6163 6637 222c  id": "b1acacf7",
-000001a0: 0a20 2020 226d 6574 6164 6174 6122 3a20  .   "metadata": 
-000001b0: 7b7d 2c0a 2020 2022 6f75 7470 7574 7322  {},.   "outputs"
-000001c0: 3a20 5b5d 2c0a 2020 2022 736f 7572 6365  : [],.   "source
-000001d0: 223a 205b 0a20 2020 2022 6672 6f6d 2063  ": [.    "from c
-000001e0: 6167 2e66 7261 6d65 776f 726b 2e61 6e6e  ag.framework.ann
-000001f0: 6f74 6174 6f72 2e70 6970 656c 696e 652e  otator.pipeline.
-00000200: 7069 7065 6c69 6e65 5f62 6173 6520 696d  pipeline_base im
-00000210: 706f 7274 2050 6970 656c 696e 655c 6e22  port Pipeline\n"
-00000220: 2c0a 2020 2020 2266 726f 6d20 6361 672e  ,.    "from cag.
-00000230: 7574 696c 732e 636f 6e66 6967 2069 6d70  utils.config imp
-00000240: 6f72 7420 436f 6e66 6967 5c6e 222c 0a20  ort Config\n",. 
-00000250: 2020 2022 6672 6f6d 2074 7164 6d20 696d     "from tqdm im
-00000260: 706f 7274 2074 7164 6d22 0a20 2020 5d0a  port tqdm".   ].
-00000270: 2020 7d2c 0a20 207b 0a20 2020 2263 656c    },.  {.   "cel
-00000280: 6c5f 7479 7065 223a 2022 636f 6465 222c  l_type": "code",
-00000290: 0a20 2020 2265 7865 6375 7469 6f6e 5f63  .   "execution_c
-000002a0: 6f75 6e74 223a 206e 756c 6c2c 0a20 2020  ount": null,.   
-000002b0: 2269 6422 3a20 2238 3537 3036 3661 3222  "id": "857066a2"
-000002c0: 2c0a 2020 2022 6d65 7461 6461 7461 223a  ,.   "metadata":
-000002d0: 207b 7d2c 0a20 2020 226f 7574 7075 7473   {},.   "outputs
-000002e0: 223a 205b 5d2c 0a20 2020 2273 6f75 7263  ": [],.   "sourc
-000002f0: 6522 3a20 5b0a 2020 2020 2223 206d 616b  e": [.    "# mak
-00000300: 6520 7375 7265 2061 7261 6e67 6f64 6220  e sure arangodb 
-00000310: 6973 2075 7020 616e 6420 7275 6e6e 696e  is up and runnin
-00000320: 6720 2d20 456e 7465 7220 796f 7572 2063  g - Enter your c
-00000330: 7265 6465 6e74 6961 6c73 2062 656c 6f77  redentials below
-00000340: 5c6e 222c 0a20 2020 2022 6d79 5f63 6f6e  \n",.    "my_con
-00000350: 6669 6720 3d20 436f 6e66 6967 285c 6e22  fig = Config(\n"
-00000360: 2c0a 2020 2020 2220 2020 2075 726c 3d5c  ,.    "    url=\
-00000370: 2268 7474 703a 2f2f 3132 372e 302e 302e  "http://127.0.0.
-00000380: 313a 3835 3239 5c22 2c5c 6e22 2c0a 2020  1:8529\",\n",.  
-00000390: 2020 2220 2020 2075 7365 723d 5c22 726f    "    user=\"ro
-000003a0: 6f74 5c22 2c5c 6e22 2c0a 2020 2020 2220  ot\",\n",.    " 
-000003b0: 2020 2070 6173 7377 6f72 643d 5c22 726f     password=\"ro
-000003c0: 6f74 5c22 2c5c 6e22 2c0a 2020 2020 2220  ot\",\n",.    " 
-000003d0: 2020 2064 6174 6162 6173 653d 5c22 5f73     database=\"_s
-000003e0: 7973 7465 6d5c 222c 5c6e 222c 0a20 2020  ystem\",\n",.   
-000003f0: 2022 2020 2020 6772 6170 683d 5c22 4d79   "    graph=\"My
-00000400: 4361 6747 7261 7068 5c22 2c5c 6e22 2c0a  CagGraph\",\n",.
-00000410: 2020 2020 2229 220a 2020 205d 0a20 207d      ")".   ].  }
-00000420: 2c0a 2020 7b0a 2020 2022 6174 7461 6368  ,.  {.   "attach
-00000430: 6d65 6e74 7322 3a20 7b7d 2c0a 2020 2022  ments": {},.   "
-00000440: 6365 6c6c 5f74 7970 6522 3a20 226d 6172  cell_type": "mar
-00000450: 6b64 6f77 6e22 2c0a 2020 2022 6964 223a  kdown",.   "id":
-00000460: 2022 6363 3335 6566 6130 222c 0a20 2020   "cc35efa0",.   
-00000470: 226d 6574 6164 6174 6122 3a20 7b7d 2c0a  "metadata": {},.
-00000480: 2020 2022 736f 7572 6365 223a 205b 0a20     "source": [. 
-00000490: 2020 2022 2323 2043 7265 6174 6520 796f     "## Create yo
-000004a0: 7572 2066 6972 7374 2043 4147 2041 6e6e  ur first CAG Ann
-000004b0: 6f74 6174 696f 6e20 5069 7065 6c69 6e65  otation Pipeline
-000004c0: 220a 2020 205d 0a20 207d 2c0a 2020 7b0a  ".   ].  },.  {.
-000004d0: 2020 2022 6365 6c6c 5f74 7970 6522 3a20     "cell_type": 
-000004e0: 2263 6f64 6522 2c0a 2020 2022 6578 6563  "code",.   "exec
-000004f0: 7574 696f 6e5f 636f 756e 7422 3a20 6e75  ution_count": nu
-00000500: 6c6c 2c0a 2020 2022 6964 223a 2022 3234  ll,.   "id": "24
-00000510: 6339 3465 3632 222c 0a20 2020 226d 6574  c94e62",.   "met
-00000520: 6164 6174 6122 3a20 7b7d 2c0a 2020 2022  adata": {},.   "
-00000530: 6f75 7470 7574 7322 3a20 5b5d 2c0a 2020  outputs": [],.  
-00000540: 2022 736f 7572 6365 223a 205b 0a20 2020   "source": [.   
-00000550: 2022 2320 4578 7465 6e64 7320 7468 6520   "# Extends the 
-00000560: 4341 4720 5069 7065 6c69 6e65 2061 6e64  CAG Pipeline and
-00000570: 2069 6d70 6c65 6d65 6e74 7320 7468 6520   implements the 
-00000580: 7477 6f20 6d65 7468 6473 3a20 7072 6f63  two methds: proc
-00000590: 6573 735f 696e 7075 7420 616e 6420 696e  ess_input and in
-000005a0: 6974 5f61 6e64 5f72 756e 5c6e 222c 0a20  it_and_run\n",. 
-000005b0: 2020 2022 636c 6173 7320 4d79 4669 7273     "class MyFirs
-000005c0: 7450 6970 656c 696e 6528 5069 7065 6c69  tPipeline(Pipeli
-000005d0: 6e65 293a 5c6e 222c 0a20 2020 2022 2020  ne):\n",.    "  
-000005e0: 2020 6465 6620 5f5f 706f 7374 5f69 6e69    def __post_ini
-000005f0: 745f 5f28 7365 6c66 293a 5c6e 222c 0a20  t__(self):\n",. 
-00000600: 2020 2022 2020 2020 2020 2020 7072 696e     "        prin
-00000610: 7428 5c22 496e 2050 4f53 5420 494e 4954  t(\"In POST INIT
-00000620: 5c22 295c 6e22 2c0a 2020 2020 2220 2020  \")\n",.    "   
-00000630: 2020 2020 2073 656c 662e 6f75 745f 7061       self.out_pa
-00000640: 7468 203d 205c 226d 7966 6972 7374 7069  th = \"myfirstpi
-00000650: 7065 6c69 6e65 5f6f 7574 7075 742e 6373  peline_output.cs
-00000660: 765c 225c 6e22 2c0a 2020 2020 2220 2020  v\"\n",.    "   
-00000670: 2020 2020 2073 656c 662e 6578 6563 5f74       self.exec_t
-00000680: 7261 6e73 666f 726d 6572 5f62 6173 6564  ransformer_based
-00000690: 203d 2046 616c 7365 5c6e 222c 0a20 2020   = False\n",.   
-000006a0: 2022 5c6e 222c 0a20 2020 2022 2020 2020   "\n",.    "    
-000006b0: 2320 436f 6465 2066 6f72 2070 7265 7072  # Code for prepr
-000006c0: 6f63 6573 7369 6e67 2074 6865 2069 6e70  ocessing the inp
-000006d0: 7574 2064 6174 6120 6265 666f 7265 2061  ut data before a
-000006e0: 6e6e 6f74 6174 696e 672e 2049 6e20 7468  nnotating. In th
-000006f0: 6973 2063 6173 6520 6865 7265 2c20 7765  is case here, we
-00000700: 2063 6f6e 7665 7274 2074 6865 206e 6f64   convert the nod
-00000710: 6573 2069 6e74 6f20 6120 6c69 7374 206f  es into a list o
-00000720: 6620 7475 706c 6573 2e5c 6e22 2c0a 2020  f tuples.\n",.  
-00000730: 2020 2220 2020 2023 2045 6163 6820 7475    "    # Each tu
-00000740: 706c 6520 636f 6e74 6169 6e73 2074 6865  ple contains the
-00000750: 2074 6578 7420 6f66 2074 6865 206e 6f64   text of the nod
-00000760: 6520 616e 6420 7468 6520 5f6b 6579 2028  e and the _key (
-00000770: 7468 6520 756e 6971 7565 2069 6420 6f66  the unique id of
-00000780: 2074 6865 206e 6f64 6529 5c6e 222c 0a20   the node)\n",. 
-00000790: 2020 2022 2020 2020 6465 6620 7072 6f63     "    def proc
-000007a0: 6573 735f 696e 7075 7428 7365 6c66 2920  ess_input(self) 
-000007b0: 2d3e 206c 6973 743a 5c6e 222c 0a20 2020  -> list:\n",.   
-000007c0: 2022 2020 2020 2020 2020 7072 6f63 6573   "        proces
-000007d0: 7365 6420 3d20 5b5d 5c6e 222c 0a20 2020  sed = []\n",.   
-000007e0: 2022 2020 2020 2020 2020 666f 7220 7478   "        for tx
-000007f0: 745f 6e6f 6465 2069 6e20 7471 646d 2873  t_node in tqdm(s
-00000800: 656c 662e 696e 7075 7429 3a5c 6e22 2c0a  elf.input):\n",.
-00000810: 2020 2020 2220 2020 2020 2020 2020 2020      "           
-00000820: 2070 726f 6365 7373 6564 2e61 7070 656e   processed.appen
-00000830: 6428 2874 7874 5f6e 6f64 652e 7465 7874  d((txt_node.text
-00000840: 2c20 7b5c 225f 6b65 795c 223a 2074 7874  , {\"_key\": txt
-00000850: 5f6e 6f64 652e 5f6b 6579 7d29 295c 6e22  _node._key}))\n"
-00000860: 2c0a 2020 2020 225c 6e22 2c0a 2020 2020  ,.    "\n",.    
-00000870: 2220 2020 2020 2020 2072 6574 7572 6e20  "        return 
-00000880: 7072 6f63 6573 7365 645c 6e22 2c0a 2020  processed\n",.  
-00000890: 2020 225c 6e22 2c0a 2020 2020 2220 2020    "\n",.    "   
-000008a0: 2064 6566 2069 6e69 745f 616e 645f 7275   def init_and_ru
-000008b0: 6e28 7365 6c66 293a 5c6e 222c 0a20 2020  n(self):\n",.   
-000008c0: 2022 2020 2020 2020 2020 6966 2073 656c   "        if sel
-000008d0: 662e 6578 6563 5f74 7261 6e73 666f 726d  f.exec_transform
-000008e0: 6572 5f62 6173 6564 3a5c 6e22 2c0a 2020  er_based:\n",.  
-000008f0: 2020 2220 2020 2020 2020 2020 2020 2073    "            s
-00000900: 656c 662e 6164 645f 616e 6e6f 7461 7469  elf.add_annotati
-00000910: 6f6e 5f70 6970 6528 5c6e 222c 0a20 2020  on_pipe(\n",.   
-00000920: 2022 2020 2020 2020 2020 2020 2020 2020   "              
-00000930: 2020 6e61 6d65 3d5c 2273 656e 7465 6e63    name=\"sentenc
-00000940: 697a 6572 5c22 2c5c 6e22 2c0a 2020 2020  izer\",\n",.    
-00000950: 2220 2020 2020 2020 2020 2020 2020 2020  "               
-00000960: 2073 6176 655f 6f75 7470 7574 3d46 616c   save_output=Fal
-00000970: 7365 2c5c 6e22 2c0a 2020 2020 2220 2020  se,\n",.    "   
-00000980: 2020 2020 2020 2020 2020 2020 2069 735f               is_
-00000990: 7370 6163 793d 5472 7565 2c5c 6e22 2c0a  spacy=True,\n",.
-000009a0: 2020 2020 2220 2020 2020 2020 2020 2020      "           
-000009b0: 2020 2020 2069 735f 6e61 7469 7665 3d54       is_native=T
-000009c0: 7275 652c 5c6e 222c 0a20 2020 2022 2020  rue,\n",.    "  
-000009d0: 2020 2020 2020 2020 2020 295c 6e22 2c0a            )\n",.
-000009e0: 2020 2020 2220 2020 2020 2020 2020 2020      "           
-000009f0: 2073 656c 662e 6164 645f 616e 6e6f 7461   self.add_annota
-00000a00: 7469 6f6e 5f70 6970 6528 5c6e 222c 0a20  tion_pipe(\n",. 
-00000a10: 2020 2022 2020 2020 2020 2020 2020 2020     "            
-00000a20: 2020 2020 6e61 6d65 3d5c 2245 6d6f 7469      name=\"Emoti
-00000a30: 6f6e 5069 7065 4f72 6368 6573 7472 6174  onPipeOrchestrat
-00000a40: 6f72 5c22 2c20 7361 7665 5f6f 7574 7075  or\", save_outpu
-00000a50: 743d 5472 7565 2c20 6973 5f73 7061 6379  t=True, is_spacy
-00000a60: 3d54 7275 655c 6e22 2c0a 2020 2020 2220  =True\n",.    " 
-00000a70: 2020 2020 2020 2020 2020 2029 5c6e 222c             )\n",
-00000a80: 0a20 2020 2022 2020 2020 2020 2020 2020  .    "          
-00000a90: 2020 2320 7365 6c66 2e61 6464 5f61 6e6e    # self.add_ann
-00000aa0: 6f74 6174 696f 6e5f 7069 7065 285c 6e22  otation_pipe(\n"
-00000ab0: 2c0a 2020 2020 2220 2020 2020 2020 2020  ,.    "         
-00000ac0: 2020 2023 2020 2020 6e61 6d65 3d5c 2248     #    name=\"H
-00000ad0: 6564 6765 5069 7065 4f72 6368 6573 7472  edgePipeOrchestr
-00000ae0: 6174 6f72 5c22 2c20 7361 7665 5f6f 7574  ator\", save_out
-00000af0: 7075 743d 5472 7565 2c20 6973 5f73 7061  put=True, is_spa
-00000b00: 6379 3d54 7275 655c 6e22 2c0a 2020 2020  cy=True\n",.    
-00000b10: 2220 2020 2020 2020 2020 2020 2023 2029  "            # )
-00000b20: 5c6e 222c 0a20 2020 2022 2020 2020 2020  \n",.    "      
-00000b30: 2020 2020 2020 7365 6c66 2e61 6464 5f61        self.add_a
-00000b40: 6e6e 6f74 6174 696f 6e5f 7069 7065 285c  nnotation_pipe(\
-00000b50: 6e22 2c0a 2020 2020 2220 2020 2020 2020  n",.    "       
-00000b60: 2020 2020 2020 2020 206e 616d 653d 5c22           name=\"
-00000b70: 546f 7869 6369 7479 5069 7065 4f72 6368  ToxicityPipeOrch
-00000b80: 6573 7472 6174 6f72 5c22 2c5c 6e22 2c0a  estrator\",\n",.
-00000b90: 2020 2020 2220 2020 2020 2020 2020 2020      "           
-00000ba0: 2020 2020 2073 6176 655f 6f75 7470 7574       save_output
-00000bb0: 3d54 7275 652c 5c6e 222c 0a20 2020 2022  =True,\n",.    "
-00000bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000bd0: 6973 5f73 7061 6379 3d54 7275 652c 5c6e  is_spacy=True,\n
-00000be0: 222c 0a20 2020 2022 2020 2020 2020 2020  ",.    "        
-00000bf0: 2020 2020 295c 6e22 2c0a 2020 2020 2220      )\n",.    " 
-00000c00: 2020 2020 2020 2065 6c73 653a 5c6e 222c         else:\n",
-00000c10: 0a20 2020 2022 2020 2020 2020 2020 2020  .    "          
-00000c20: 2020 7365 6c66 2e61 6464 5f61 6e6e 6f74    self.add_annot
-00000c30: 6174 696f 6e5f 7069 7065 285c 6e22 2c0a  ation_pipe(\n",.
-00000c40: 2020 2020 2220 2020 2020 2020 2020 2020      "           
-00000c50: 2020 2020 206e 616d 653d 5c22 746f 6b32       name=\"tok2
-00000c60: 7665 635c 222c 5c6e 222c 0a20 2020 2022  vec\",\n",.    "
-00000c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000c80: 7361 7665 5f6f 7574 7075 743d 4661 6c73  save_output=Fals
-00000c90: 652c 5c6e 222c 0a20 2020 2022 2020 2020  e,\n",.    "    
-00000ca0: 2020 2020 2020 2020 2020 2020 6973 5f73              is_s
-00000cb0: 7061 6379 3d54 7275 652c 5c6e 222c 0a20  pacy=True,\n",. 
-00000cc0: 2020 2022 2020 2020 2020 2020 2020 2020     "            
-00000cd0: 2020 2020 6973 5f6e 6174 6976 653d 5472      is_native=Tr
-00000ce0: 7565 2c5c 6e22 2c0a 2020 2020 2220 2020  ue,\n",.    "   
-00000cf0: 2020 2020 2020 2020 2029 2020 2320 6d61           )  # ma
-00000d00: 6e64 6174 6f72 7920 666f 7220 4e45 525c  ndatory for NER\
-00000d10: 6e22 2c0a 2020 2020 2220 2020 2020 2020  n",.    "       
-00000d20: 2020 2020 2073 656c 662e 6164 645f 616e       self.add_an
-00000d30: 6e6f 7461 7469 6f6e 5f70 6970 6528 5c6e  notation_pipe(\n
-00000d40: 222c 0a20 2020 2022 2020 2020 2020 2020  ",.    "        
-00000d50: 2020 2020 2020 2020 6e61 6d65 3d5c 224e          name=\"N
-00000d60: 616d 6564 456e 7469 7479 5069 7065 4f72  amedEntityPipeOr
-00000d70: 6368 6573 7472 6174 6f72 5c22 2c5c 6e22  chestrator\",\n"
-00000d80: 2c0a 2020 2020 2220 2020 2020 2020 2020  ,.    "         
-00000d90: 2020 2020 2020 2073 6176 655f 6f75 7470         save_outp
-00000da0: 7574 3d54 7275 652c 5c6e 222c 0a20 2020  ut=True,\n",.   
-00000db0: 2022 2020 2020 2020 2020 2020 2020 2020   "              
-00000dc0: 2020 6973 5f73 7061 6379 3d54 7275 652c    is_spacy=True,
-00000dd0: 5c6e 222c 0a20 2020 2022 2020 2020 2020  \n",.    "      
-00000de0: 2020 2020 2020 295c 6e22 2c0a 2020 2020        )\n",.    
-00000df0: 2220 2020 2020 2020 2020 2020 2073 656c  "            sel
-00000e00: 662e 6164 645f 616e 6e6f 7461 7469 6f6e  f.add_annotation
-00000e10: 5f70 6970 6528 5c6e 222c 0a20 2020 2022  _pipe(\n",.    "
-00000e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000e30: 6e61 6d65 3d5c 226d 7071 615f 7061 7273  name=\"mpqa_pars
-00000e40: 6572 5c22 2c5c 6e22 2c0a 2020 2020 2220  er\",\n",.    " 
-00000e50: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00000e60: 6176 655f 6f75 7470 7574 3d46 616c 7365  ave_output=False
-00000e70: 2c5c 6e22 2c0a 2020 2020 2220 2020 2020  ,\n",.    "     
-00000e80: 2020 2020 2020 2020 2020 2069 735f 7370             is_sp
-00000e90: 6163 793d 5472 7565 2c5c 6e22 2c0a 2020  acy=True,\n",.  
-00000ea0: 2020 2220 2020 2020 2020 2020 2020 2020    "             
-00000eb0: 2020 2069 735f 6e61 7469 7665 3d54 7275     is_native=Tru
-00000ec0: 652c 5c6e 222c 0a20 2020 2022 2020 2020  e,\n",.    "    
-00000ed0: 2020 2020 2020 2020 295c 6e22 2c0a 2020          )\n",.  
-00000ee0: 2020 2220 2020 2020 2020 2020 2020 2073    "            s
-00000ef0: 656c 662e 6164 645f 616e 6e6f 7461 7469  elf.add_annotati
-00000f00: 6f6e 5f70 6970 6528 5c6e 222c 0a20 2020  on_pipe(\n",.   
-00000f10: 2022 2020 2020 2020 2020 2020 2020 2020   "              
-00000f20: 2020 6e61 6d65 3d5c 224d 7071 6150 6970    name=\"MpqaPip
-00000f30: 654f 7263 6865 7374 7261 746f 725c 222c  eOrchestrator\",
-00000f40: 2073 6176 655f 6f75 7470 7574 3d54 7275   save_output=Tru
-00000f50: 652c 2069 735f 7370 6163 793d 5472 7565  e, is_spacy=True
-00000f60: 5c6e 222c 0a20 2020 2022 2020 2020 2020  \n",.    "      
-00000f70: 2020 2020 2020 295c 6e22 2c0a 2020 2020        )\n",.    
-00000f80: 2220 2020 2020 2020 2020 2020 2073 656c  "            sel
-00000f90: 662e 6164 645f 616e 6e6f 7461 7469 6f6e  f.add_annotation
-00000fa0: 5f70 6970 6528 5c6e 222c 0a20 2020 2022  _pipe(\n",.    "
-00000fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000fc0: 6e61 6d65 3d5c 2245 6d70 6174 6850 6970  name=\"EmpathPip
-00000fd0: 654f 7263 6865 7374 7261 746f 725c 222c  eOrchestrator\",
-00000fe0: 2073 6176 655f 6f75 7470 7574 3d54 7275   save_output=Tru
-00000ff0: 652c 2069 735f 7370 6163 793d 5472 7565  e, is_spacy=True
-00001000: 5c6e 222c 0a20 2020 2022 2020 2020 2020  \n",.    "      
-00001010: 2020 2020 2020 295c 6e22 2c0a 2020 2020        )\n",.    
-00001020: 225c 6e22 2c0a 2020 2020 2220 2020 2020  "\n",.    "     
-00001030: 2020 2073 656c 662e 696e 6974 5f70 6970     self.init_pip
-00001040: 655f 7374 6163 6b28 2922 0a20 2020 5d0a  e_stack()".   ].
-00001050: 2020 7d2c 0a20 207b 0a20 2020 2261 7474    },.  {.   "att
-00001060: 6163 686d 656e 7473 223a 207b 7d2c 0a20  achments": {},. 
-00001070: 2020 2263 656c 6c5f 7479 7065 223a 2022    "cell_type": "
-00001080: 6d61 726b 646f 776e 222c 0a20 2020 2269  markdown",.   "i
-00001090: 6422 3a20 2237 3762 3834 3334 3122 2c0a  d": "77b84341",.
-000010a0: 2020 2022 6d65 7461 6461 7461 223a 207b     "metadata": {
-000010b0: 7d2c 0a20 2020 2273 6f75 7263 6522 3a20  },.   "source": 
-000010c0: 5b0a 2020 2020 2223 2320 496e 6974 6961  [.    "## Initia
-000010d0: 6c69 7a65 2079 6f75 7220 6669 7273 7420  lize your first 
-000010e0: 6361 6720 5069 7065 6c69 6e65 220a 2020  cag Pipeline".  
-000010f0: 205d 0a20 207d 2c0a 2020 7b0a 2020 2022   ].  },.  {.   "
-00001100: 6365 6c6c 5f74 7970 6522 3a20 2263 6f64  cell_type": "cod
-00001110: 6522 2c0a 2020 2022 6578 6563 7574 696f  e",.   "executio
-00001120: 6e5f 636f 756e 7422 3a20 6e75 6c6c 2c0a  n_count": null,.
-00001130: 2020 2022 6964 223a 2022 3032 6131 6361     "id": "02a1ca
-00001140: 3465 222c 0a20 2020 226d 6574 6164 6174  4e",.   "metadat
-00001150: 6122 3a20 7b7d 2c0a 2020 2022 6f75 7470  a": {},.   "outp
-00001160: 7574 7322 3a20 5b5d 2c0a 2020 2022 736f  uts": [],.   "so
-00001170: 7572 6365 223a 205b 0a20 2020 2022 6361  urce": [.    "ca
-00001180: 675f 7069 7065 6c69 6e65 203d 204d 7946  g_pipeline = MyF
-00001190: 6972 7374 5069 7065 6c69 6e65 286d 795f  irstPipeline(my_
-000011a0: 636f 6e66 6967 295c 6e22 2c0a 2020 2020  config)\n",.    
-000011b0: 2263 6167 5f70 6970 656c 696e 652e 7370  "cag_pipeline.sp
-000011c0: 6163 795f 6e5f 7072 6f63 6573 736f 7273  acy_n_processors
-000011d0: 203d 2031 2020 2320 496e 2063 6173 6520   = 1  # In case 
-000011e0: 796f 7520 6172 6520 7573 696e 6720 7370  you are using sp
-000011f0: 6163 7920 7069 7065 2c20 7468 6973 2066  acy pipe, this f
-00001200: 6c61 6720 6361 6e20 6265 2073 6574 2074  lag can be set t
-00001210: 6f20 656e 6162 6c65 206d 756c 7469 7072  o enable multipr
-00001220: 6f63 6573 7369 6e67 2c5c 6e22 2c0a 2020  ocessing,\n",.  
-00001230: 2020 2223 204e 4f54 453a 2049 6620 796f    "# NOTE: If yo
-00001240: 7520 6172 6520 7573 696e 6720 7370 6163  u are using spac
-00001250: 7920 7769 7468 2074 7261 6e73 666f 726d  y with transform
-00001260: 6572 2062 6173 6564 2066 6561 7475 7265  er based feature
-00001270: 2c20 7365 7420 7468 6520 666c 6167 2074  , set the flag t
-00001280: 6f20 3120 6f72 2065 6c73 6520 7468 6520  o 1 or else the 
-00001290: 7069 7065 6c69 6e65 2077 696c 6c20 6672  pipeline will fr
-000012a0: 6565 7a65 2028 7468 6973 2069 7320 6120  eeze (this is a 
-000012b0: 7370 6163 7920 6275 6720 616e 6420 6e6f  spacy bug and no
-000012c0: 7420 7265 6c61 7465 6420 746f 2063 6167  t related to cag
-000012d0: 2922 0a20 2020 5d0a 2020 7d2c 0a20 207b  )".   ].  },.  {
-000012e0: 0a20 2020 2261 7474 6163 686d 656e 7473  .   "attachments
-000012f0: 223a 207b 7d2c 0a20 2020 2263 656c 6c5f  ": {},.   "cell_
-00001300: 7479 7065 223a 2022 6d61 726b 646f 776e  type": "markdown
-00001310: 222c 0a20 2020 2269 6422 3a20 2265 3962  ",.   "id": "e9b
-00001320: 6637 6337 6122 2c0a 2020 2022 6d65 7461  f7c7a",.   "meta
-00001330: 6461 7461 223a 207b 7d2c 0a20 2020 2273  data": {},.   "s
-00001340: 6f75 7263 6522 3a20 5b0a 2020 2020 2223  ource": [.    "#
-00001350: 2320 4665 7463 6820 7468 6520 5465 7874  # Fetch the Text
-00001360: 4e6f 6465 2061 6e64 2041 6e6e 6f74 6174  Node and Annotat
-00001370: 6520 2620 5361 7665 220a 2020 205d 0a20  e & Save".   ]. 
-00001380: 207d 2c0a 2020 7b0a 2020 2022 6365 6c6c   },.  {.   "cell
-00001390: 5f74 7970 6522 3a20 2263 6f64 6522 2c0a  _type": "code",.
-000013a0: 2020 2022 6578 6563 7574 696f 6e5f 636f     "execution_co
-000013b0: 756e 7422 3a20 6e75 6c6c 2c0a 2020 2022  unt": null,.   "
-000013c0: 6964 223a 2022 3637 6638 3565 6633 222c  id": "67f85ef3",
-000013d0: 0a20 2020 226d 6574 6164 6174 6122 3a20  .   "metadata": 
-000013e0: 7b7d 2c0a 2020 2022 6f75 7470 7574 7322  {},.   "outputs"
-000013f0: 3a20 5b5d 2c0a 2020 2022 736f 7572 6365  : [],.   "source
-00001400: 223a 205b 0a20 2020 2022 2320 204c 6f6f  ": [.    "#  Loo
-00001410: 7020 6f76 6572 2079 6f75 7220 6461 7461  p over your data
-00001420: 2c20 616e 6e6f 7461 7465 4120 616e 6420  , annotateA and 
-00001430: 7361 7665 5c6e 222c 0a20 2020 2022 6361  save\n",.    "ca
-00001440: 675f 7069 7065 6c69 6e65 2e65 7865 635f  g_pipeline.exec_
-00001450: 7472 616e 7366 6f72 6d65 725f 6261 7365  transformer_base
-00001460: 6420 3d20 4661 6c73 655c 6e22 2c0a 2020  d = False\n",.  
-00001470: 2020 2263 6167 5f70 6970 656c 696e 652e    "cag_pipeline.
-00001480: 696e 6974 5f61 6e64 5f72 756e 2829 5c6e  init_and_run()\n
-00001490: 222c 0a20 2020 2022 5c6e 222c 0a20 2020  ",.    "\n",.   
-000014a0: 2022 636f 6c6c 203d 2063 6167 5f70 6970   "coll = cag_pip
-000014b0: 656c 696e 652e 6461 7461 6261 7365 5f63  eline.database_c
-000014c0: 6f6e 6669 672e 6462 5b5c 2254 6578 744e  onfig.db[\"TextN
-000014d0: 6f64 655c 225d 5c6e 222c 0a20 2020 2022  ode\"]\n",.    "
-000014e0: 646f 6373 203d 2063 6f6c 6c2e 6665 7463  docs = coll.fetc
-000014f0: 6841 6c6c 286c 696d 6974 3d33 3030 295c  hAll(limit=300)\
-00001500: 6e22 2c0a 2020 2020 2266 6574 6368 6564  n",.    "fetched
-00001510: 203d 206c 656e 2864 6f63 7329 5c6e 222c   = len(docs)\n",
-00001520: 0a20 2020 2022 7768 696c 6520 646f 6373  .    "while docs
-00001530: 2069 7320 6e6f 7420 4e6f 6e65 2061 6e64   is not None and
-00001540: 206c 656e 2864 6f63 7329 203e 2030 3a5c   len(docs) > 0:\
-00001550: 6e22 2c0a 2020 2020 2220 2020 2023 2320  n",.    "    ## 
-00001560: 616e 6e6f 7461 7465 5c6e 222c 0a20 2020  annotate\n",.   
-00001570: 2022 5c6e 222c 0a20 2020 2022 2020 2020   "\n",.    "    
-00001580: 2320 5365 7420 7468 6520 494e 5055 5420  # Set the INPUT 
-00001590: 2d20 7468 6973 2077 696c 6c20 6175 746f  - this will auto
-000015a0: 6d61 7469 6361 6c6c 7920 6361 6c6c 2070  matically call p
-000015b0: 7265 7072 6f63 6573 735f 696e 7075 7420  reprocess_input 
-000015c0: 286d 616b 6520 7375 7265 2074 6f20 696d  (make sure to im
-000015d0: 706c 656d 656e 7420 6974 295c 6e22 2c0a  plement it)\n",.
-000015e0: 2020 2020 2220 2020 2063 6167 5f70 6970      "    cag_pip
-000015f0: 656c 696e 652e 7265 7365 745f 696e 7075  eline.reset_inpu
-00001600: 745f 6f75 7470 7574 2829 5c6e 222c 0a20  t_output()\n",. 
-00001610: 2020 2022 2020 2020 6361 675f 7069 7065     "    cag_pipe
-00001620: 6c69 6e65 2e73 6574 5f69 6e70 7574 2864  line.set_input(d
-00001630: 6f63 7329 5c6e 222c 0a20 2020 2022 5c6e  ocs)\n",.    "\n
-00001640: 222c 0a20 2020 2022 2020 2020 6361 675f  ",.    "    cag_
-00001650: 7069 7065 6c69 6e65 2e61 6e6e 6f74 6174  pipeline.annotat
-00001660: 6528 295c 6e22 2c0a 2020 2020 2220 2020  e()\n",.    "   
-00001670: 2063 6167 5f70 6970 656c 696e 652e 7361   cag_pipeline.sa
-00001680: 7665 2829 5c6e 222c 0a20 2020 2022 5c6e  ve()\n",.    "\n
-00001690: 222c 0a20 2020 2022 2020 2020 6361 675f  ",.    "    cag_
-000016a0: 7069 7065 6c69 6e65 2e72 6573 6574 5f69  pipeline.reset_i
-000016b0: 6e70 7574 5f6f 7574 7075 7428 295c 6e22  nput_output()\n"
-000016c0: 2c0a 2020 2020 2220 2020 2070 7269 6e74  ,.    "    print
-000016d0: 2866 5c22 5072 6f63 6573 7365 6420 7b66  (f\"Processed {f
-000016e0: 6574 6368 6564 7d20 646f 6373 5c22 295c  etched} docs\")\
-000016f0: 6e22 2c0a 2020 2020 2220 2020 2064 6f63  n",.    "    doc
-00001700: 7320 3d20 636f 6c6c 2e66 6574 6368 416c  s = coll.fetchAl
-00001710: 6c28 6c69 6d69 743d 3130 302c 2073 6b69  l(limit=100, ski
-00001720: 703d 6665 7463 6865 6429 5c6e 222c 0a20  p=fetched)\n",. 
-00001730: 2020 2022 2020 2020 6665 7463 6865 6420     "    fetched 
-00001740: 3d20 6665 7463 6865 6420 2b20 6c65 6e28  = fetched + len(
-00001750: 646f 6373 2922 0a20 2020 5d0a 2020 7d2c  docs)".   ].  },
-00001760: 0a20 207b 0a20 2020 2261 7474 6163 686d  .  {.   "attachm
-00001770: 656e 7473 223a 207b 7d2c 0a20 2020 2263  ents": {},.   "c
-00001780: 656c 6c5f 7479 7065 223a 2022 6d61 726b  ell_type": "mark
-00001790: 646f 776e 222c 0a20 2020 2269 6422 3a20  down",.   "id": 
-000017a0: 2263 6135 3939 3839 3422 2c0a 2020 2022  "ca599894",.   "
-000017b0: 6d65 7461 6461 7461 223a 207b 7d2c 0a20  metadata": {},. 
-000017c0: 2020 2273 6f75 7263 6522 3a20 5b0a 2020    "source": [.  
-000017d0: 2020 2223 2323 2054 7261 6e73 666f 726d    "### Transform
-000017e0: 6572 2062 6173 6564 2046 6561 7475 7265  er based Feature
-000017f0: 7322 0a20 2020 5d0a 2020 7d2c 0a20 207b  s".   ].  },.  {
-00001800: 0a20 2020 2263 656c 6c5f 7479 7065 223a  .   "cell_type":
-00001810: 2022 636f 6465 222c 0a20 2020 2265 7865   "code",.   "exe
-00001820: 6375 7469 6f6e 5f63 6f75 6e74 223a 206e  cution_count": n
-00001830: 756c 6c2c 0a20 2020 2269 6422 3a20 2262  ull,.   "id": "b
-00001840: 3538 3565 6639 6622 2c0a 2020 2022 6d65  585ef9f",.   "me
-00001850: 7461 6461 7461 223a 207b 7d2c 0a20 2020  tadata": {},.   
-00001860: 226f 7574 7075 7473 223a 205b 5d2c 0a20  "outputs": [],. 
-00001870: 2020 2273 6f75 7263 6522 3a20 5b0a 2020    "source": [.  
-00001880: 2020 2263 6167 5f70 6970 656c 696e 652e    "cag_pipeline.
-00001890: 6578 6563 5f74 7261 6e73 666f 726d 6572  exec_transformer
-000018a0: 5f62 6173 6564 203d 2054 7275 655c 6e22  _based = True\n"
-000018b0: 2c0a 2020 2020 2263 6167 5f70 6970 656c  ,.    "cag_pipel
-000018c0: 696e 652e 6f75 745f 7061 7468 203d 205c  ine.out_path = \
-000018d0: 2274 7261 6e73 666f 726d 6572 5f62 6173  "transformer_bas
-000018e0: 6564 5f66 6561 7475 7265 732e 6373 765c  ed_features.csv\
-000018f0: 225c 6e22 2c0a 2020 2020 2263 6167 5f70  "\n",.    "cag_p
-00001900: 6970 656c 696e 652e 696e 6974 5f61 6e64  ipeline.init_and
-00001910: 5f72 756e 2829 5c6e 222c 0a20 2020 2022  _run()\n",.    "
-00001920: 636f 6c6c 203d 2063 6167 5f70 6970 656c  coll = cag_pipel
-00001930: 696e 652e 6461 7461 6261 7365 5f63 6f6e  ine.database_con
-00001940: 6669 672e 6462 5b5c 2254 6578 744e 6f64  fig.db[\"TextNod
-00001950: 655c 225d 5c6e 222c 0a20 2020 2022 646f  e\"]\n",.    "do
-00001960: 6373 203d 2063 6f6c 6c2e 6665 7463 6841  cs = coll.fetchA
-00001970: 6c6c 286c 696d 6974 3d31 3030 295c 6e22  ll(limit=100)\n"
-00001980: 2c0a 2020 2020 2266 6574 6368 6564 203d  ,.    "fetched =
-00001990: 206c 656e 2864 6f63 7329 5c6e 222c 0a20   len(docs)\n",. 
-000019a0: 2020 2022 7768 696c 6520 646f 6373 2069     "while docs i
-000019b0: 7320 6e6f 7420 4e6f 6e65 2061 6e64 206c  s not None and l
-000019c0: 656e 2864 6f63 7329 203e 2030 3a5c 6e22  en(docs) > 0:\n"
-000019d0: 2c0a 2020 2020 2220 2020 2023 2320 616e  ,.    "    ## an
-000019e0: 6e6f 7461 7465 5c6e 222c 0a20 2020 2022  notate\n",.    "
-000019f0: 5c6e 222c 0a20 2020 2022 2020 2020 2320  \n",.    "    # 
-00001a00: 5365 7420 7468 6520 494e 5055 5420 2d20  Set the INPUT - 
-00001a10: 7468 6973 2077 696c 6c20 6175 746f 6d61  this will automa
-00001a20: 7469 6361 6c6c 7920 6361 6c6c 2070 7265  tically call pre
-00001a30: 7072 6f63 6573 735f 696e 7075 7420 286d  process_input (m
-00001a40: 616b 6520 7375 7265 2074 6f20 696d 706c  ake sure to impl
-00001a50: 656d 656e 7420 6974 295c 6e22 2c0a 2020  ement it)\n",.  
-00001a60: 2020 2220 2020 2063 6167 5f70 6970 656c    "    cag_pipel
-00001a70: 696e 652e 7265 7365 745f 696e 7075 745f  ine.reset_input_
-00001a80: 6f75 7470 7574 2829 5c6e 222c 0a20 2020  output()\n",.   
-00001a90: 2022 2020 2020 6361 675f 7069 7065 6c69   "    cag_pipeli
-00001aa0: 6e65 2e73 6574 5f69 6e70 7574 2864 6f63  ne.set_input(doc
-00001ab0: 7329 5c6e 222c 0a20 2020 2022 5c6e 222c  s)\n",.    "\n",
-00001ac0: 0a20 2020 2022 2020 2020 6361 675f 7069  .    "    cag_pi
-00001ad0: 7065 6c69 6e65 2e61 6e6e 6f74 6174 6528  peline.annotate(
-00001ae0: 295c 6e22 2c0a 2020 2020 2220 2020 2063  )\n",.    "    c
-00001af0: 6167 5f70 6970 656c 696e 652e 7361 7665  ag_pipeline.save
-00001b00: 2829 5c6e 222c 0a20 2020 2022 5c6e 222c  ()\n",.    "\n",
-00001b10: 0a20 2020 2022 2020 2020 7072 696e 7428  .    "    print(
-00001b20: 665c 2250 726f 6365 7373 6564 207b 6665  f\"Processed {fe
-00001b30: 7463 6865 647d 2064 6f63 735c 2229 5c6e  tched} docs\")\n
-00001b40: 222c 0a20 2020 2022 2020 2020 646f 6373  ",.    "    docs
-00001b50: 203d 2063 6f6c 6c2e 6665 7463 6841 6c6c   = coll.fetchAll
-00001b60: 286c 696d 6974 3d31 3030 2c20 736b 6970  (limit=100, skip
-00001b70: 3d66 6574 6368 6564 295c 6e22 2c0a 2020  =fetched)\n",.  
-00001b80: 2020 2220 2020 2066 6574 6368 6564 203d    "    fetched =
-00001b90: 2066 6574 6368 6564 202b 206c 656e 2864   fetched + len(d
-00001ba0: 6f63 7329 220a 2020 205d 0a20 207d 0a20  ocs)".   ].  }. 
-00001bb0: 5d2c 0a20 226d 6574 6164 6174 6122 3a20  ],. "metadata": 
-00001bc0: 7b0a 2020 226b 6572 6e65 6c73 7065 6322  {.  "kernelspec"
-00001bd0: 3a20 7b0a 2020 2022 6469 7370 6c61 795f  : {.   "display_
-00001be0: 6e61 6d65 223a 2022 5079 7468 6f6e 2033  name": "Python 3
-00001bf0: 222c 0a20 2020 226c 616e 6775 6167 6522  ",.   "language"
-00001c00: 3a20 2270 7974 686f 6e22 2c0a 2020 2022  : "python",.   "
-00001c10: 6e61 6d65 223a 2022 7079 7468 6f6e 3322  name": "python3"
-00001c20: 0a20 207d 2c0a 2020 226c 616e 6775 6167  .  },.  "languag
-00001c30: 655f 696e 666f 223a 207b 0a20 2020 2263  e_info": {.   "c
-00001c40: 6f64 656d 6972 726f 725f 6d6f 6465 223a  odemirror_mode":
-00001c50: 207b 0a20 2020 2022 6e61 6d65 223a 2022   {.    "name": "
-00001c60: 6970 7974 686f 6e22 2c0a 2020 2020 2276  ipython",.    "v
-00001c70: 6572 7369 6f6e 223a 2033 0a20 2020 7d2c  ersion": 3.   },
-00001c80: 0a20 2020 2266 696c 655f 6578 7465 6e73  .   "file_extens
-00001c90: 696f 6e22 3a20 222e 7079 222c 0a20 2020  ion": ".py",.   
-00001ca0: 226d 696d 6574 7970 6522 3a20 2274 6578  "mimetype": "tex
-00001cb0: 742f 782d 7079 7468 6f6e 222c 0a20 2020  t/x-python",.   
-00001cc0: 226e 616d 6522 3a20 2270 7974 686f 6e22  "name": "python"
-00001cd0: 2c0a 2020 2022 6e62 636f 6e76 6572 745f  ,.   "nbconvert_
-00001ce0: 6578 706f 7274 6572 223a 2022 7079 7468  exporter": "pyth
-00001cf0: 6f6e 222c 0a20 2020 2270 7967 6d65 6e74  on",.   "pygment
-00001d00: 735f 6c65 7865 7222 3a20 2269 7079 7468  s_lexer": "ipyth
-00001d10: 6f6e 3322 2c0a 2020 2022 7665 7273 696f  on3",.   "versio
-00001d20: 6e22 3a20 2233 2e31 312e 3122 0a20 207d  n": "3.11.1".  }
-00001d30: 2c0a 2020 2276 7363 6f64 6522 3a20 7b0a  ,.  "vscode": {.
-00001d40: 2020 2022 696e 7465 7270 7265 7465 7222     "interpreter"
-00001d50: 3a20 7b0a 2020 2020 2268 6173 6822 3a20  : {.    "hash": 
-00001d60: 2239 3032 3335 3733 3039 3035 3937 6638  "9023573090597f8
-00001d70: 3831 3834 6237 6264 6236 3032 6231 3234  8184b7bdb602b124
-00001d80: 3039 6465 6630 3138 6438 3630 3932 6132  09def018d86092a2
-00001d90: 3066 6261 3439 3933 3866 3133 6434 6632  0fba49938f13d4f2
-00001da0: 6122 0a20 2020 7d0a 2020 7d0a 207d 2c0a  a".   }.  }. },.
-00001db0: 2022 6e62 666f 726d 6174 223a 2034 2c0a   "nbformat": 4,.
-00001dc0: 2022 6e62 666f 726d 6174 5f6d 696e 6f72   "nbformat_minor
-00001dd0: 223a 2035 0a7d 0a                        ": 5.}.
+00000000: 7b0d 0a20 2263 656c 6c73 223a 205b 0d0a  {.. "cells": [..
+00000010: 2020 7b0d 0a20 2020 2263 656c 6c5f 7479    {..   "cell_ty
+00000020: 7065 223a 2022 636f 6465 222c 0d0a 2020  pe": "code",..  
+00000030: 2022 6578 6563 7574 696f 6e5f 636f 756e   "execution_coun
+00000040: 7422 3a20 6e75 6c6c 2c0d 0a20 2020 2269  t": null,..   "i
+00000050: 6422 3a20 2236 6234 6332 3438 3322 2c0d  d": "6b4c2483",.
+00000060: 0a20 2020 226d 6574 6164 6174 6122 3a20  .   "metadata": 
+00000070: 7b7d 2c0d 0a20 2020 226f 7574 7075 7473  {},..   "outputs
+00000080: 223a 205b 5d2c 0d0a 2020 2022 736f 7572  ": [],..   "sour
+00000090: 6365 223a 205b 0d0a 2020 2020 2223 2025  ce": [..    "# %
+000000a0: 7069 7020 696e 7374 616c 6c20 2d65 202e  pip install -e .
+000000b0: 2e2f 220d 0a20 2020 5d0d 0a20 207d 2c0d  ./"..   ]..  },.
+000000c0: 0a20 207b 0d0a 2020 2022 6365 6c6c 5f74  .  {..   "cell_t
+000000d0: 7970 6522 3a20 2263 6f64 6522 2c0d 0a20  ype": "code",.. 
+000000e0: 2020 2265 7865 6375 7469 6f6e 5f63 6f75    "execution_cou
+000000f0: 6e74 223a 206e 756c 6c2c 0d0a 2020 2022  nt": null,..   "
+00000100: 6964 223a 2022 6165 3931 6137 6261 222c  id": "ae91a7ba",
+00000110: 0d0a 2020 2022 6d65 7461 6461 7461 223a  ..   "metadata":
+00000120: 207b 7d2c 0d0a 2020 2022 6f75 7470 7574   {},..   "output
+00000130: 7322 3a20 5b5d 2c0d 0a20 2020 2273 6f75  s": [],..   "sou
+00000140: 7263 6522 3a20 5b0d 0a20 2020 2022 2570  rce": [..    "%p
+00000150: 6970 2073 686f 7720 6361 6722 0d0a 2020  ip show cag"..  
+00000160: 205d 0d0a 2020 7d2c 0d0a 2020 7b0d 0a20   ]..  },..  {.. 
+00000170: 2020 2263 656c 6c5f 7479 7065 223a 2022    "cell_type": "
+00000180: 636f 6465 222c 0d0a 2020 2022 6578 6563  code",..   "exec
+00000190: 7574 696f 6e5f 636f 756e 7422 3a20 6e75  ution_count": nu
+000001a0: 6c6c 2c0d 0a20 2020 2269 6422 3a20 2262  ll,..   "id": "b
+000001b0: 3161 6361 6366 3722 2c0d 0a20 2020 226d  1acacf7",..   "m
+000001c0: 6574 6164 6174 6122 3a20 7b7d 2c0d 0a20  etadata": {},.. 
+000001d0: 2020 226f 7574 7075 7473 223a 205b 5d2c    "outputs": [],
+000001e0: 0d0a 2020 2022 736f 7572 6365 223a 205b  ..   "source": [
+000001f0: 0d0a 2020 2020 2266 726f 6d20 6361 672e  ..    "from cag.
+00000200: 6672 616d 6577 6f72 6b2e 616e 6e6f 7461  framework.annota
+00000210: 746f 722e 7069 7065 6c69 6e65 2e70 6970  tor.pipeline.pip
+00000220: 656c 696e 655f 6261 7365 2069 6d70 6f72  eline_base impor
+00000230: 7420 5069 7065 6c69 6e65 5c6e 222c 0d0a  t Pipeline\n",..
+00000240: 2020 2020 2266 726f 6d20 6361 672e 7574      "from cag.ut
+00000250: 696c 732e 636f 6e66 6967 2069 6d70 6f72  ils.config impor
+00000260: 7420 436f 6e66 6967 5c6e 222c 0d0a 2020  t Config\n",..  
+00000270: 2020 2266 726f 6d20 7471 646d 2069 6d70    "from tqdm imp
+00000280: 6f72 7420 7471 646d 220d 0a20 2020 5d0d  ort tqdm"..   ].
+00000290: 0a20 207d 2c0d 0a20 207b 0d0a 2020 2022  .  },..  {..   "
+000002a0: 6365 6c6c 5f74 7970 6522 3a20 2263 6f64  cell_type": "cod
+000002b0: 6522 2c0d 0a20 2020 2265 7865 6375 7469  e",..   "executi
+000002c0: 6f6e 5f63 6f75 6e74 223a 206e 756c 6c2c  on_count": null,
+000002d0: 0d0a 2020 2022 6964 223a 2022 3835 3730  ..   "id": "8570
+000002e0: 3636 6132 222c 0d0a 2020 2022 6d65 7461  66a2",..   "meta
+000002f0: 6461 7461 223a 207b 7d2c 0d0a 2020 2022  data": {},..   "
+00000300: 6f75 7470 7574 7322 3a20 5b5d 2c0d 0a20  outputs": [],.. 
+00000310: 2020 2273 6f75 7263 6522 3a20 5b0d 0a20    "source": [.. 
+00000320: 2020 2022 2320 6d61 6b65 2073 7572 6520     "# make sure 
+00000330: 6172 616e 676f 6462 2069 7320 7570 2061  arangodb is up a
+00000340: 6e64 2072 756e 6e69 6e67 202d 2045 6e74  nd running - Ent
+00000350: 6572 2079 6f75 7220 6372 6564 656e 7469  er your credenti
+00000360: 616c 7320 6265 6c6f 775c 6e22 2c0d 0a20  als below\n",.. 
+00000370: 2020 2022 6d79 5f63 6f6e 6669 6720 3d20     "my_config = 
+00000380: 436f 6e66 6967 285c 6e22 2c0d 0a20 2020  Config(\n",..   
+00000390: 2022 2020 2020 7572 6c3d 5c22 6874 7470   "    url=\"http
+000003a0: 3a2f 2f31 3237 2e30 2e30 2e31 3a38 3532  ://127.0.0.1:852
+000003b0: 395c 222c 5c6e 222c 0d0a 2020 2020 2220  9\",\n",..    " 
+000003c0: 2020 2075 7365 723d 5c22 726f 6f74 5c22     user=\"root\"
+000003d0: 2c5c 6e22 2c0d 0a20 2020 2022 2020 2020  ,\n",..    "    
+000003e0: 7061 7373 776f 7264 3d5c 2272 6f6f 745c  password=\"root\
+000003f0: 222c 5c6e 222c 0d0a 2020 2020 2220 2020  ",\n",..    "   
+00000400: 2064 6174 6162 6173 653d 5c22 5f73 7973   database=\"_sys
+00000410: 7465 6d5c 222c 5c6e 222c 0d0a 2020 2020  tem\",\n",..    
+00000420: 2220 2020 2067 7261 7068 3d5c 224d 7943  "    graph=\"MyC
+00000430: 6167 4772 6170 685c 222c 5c6e 222c 0d0a  agGraph\",\n",..
+00000440: 2020 2020 2229 220d 0a20 2020 5d0d 0a20      ")"..   ].. 
+00000450: 207d 2c0d 0a20 207b 0d0a 2020 2022 6174   },..  {..   "at
+00000460: 7461 6368 6d65 6e74 7322 3a20 7b7d 2c0d  tachments": {},.
+00000470: 0a20 2020 2263 656c 6c5f 7479 7065 223a  .   "cell_type":
+00000480: 2022 6d61 726b 646f 776e 222c 0d0a 2020   "markdown",..  
+00000490: 2022 6964 223a 2022 6363 3335 6566 6130   "id": "cc35efa0
+000004a0: 222c 0d0a 2020 2022 6d65 7461 6461 7461  ",..   "metadata
+000004b0: 223a 207b 7d2c 0d0a 2020 2022 736f 7572  ": {},..   "sour
+000004c0: 6365 223a 205b 0d0a 2020 2020 2223 2320  ce": [..    "## 
+000004d0: 4372 6561 7465 2079 6f75 7220 6669 7273  Create your firs
+000004e0: 7420 4341 4720 416e 6e6f 7461 7469 6f6e  t CAG Annotation
+000004f0: 2050 6970 656c 696e 6522 0d0a 2020 205d   Pipeline"..   ]
+00000500: 0d0a 2020 7d2c 0d0a 2020 7b0d 0a20 2020  ..  },..  {..   
+00000510: 2263 656c 6c5f 7479 7065 223a 2022 636f  "cell_type": "co
+00000520: 6465 222c 0d0a 2020 2022 6578 6563 7574  de",..   "execut
+00000530: 696f 6e5f 636f 756e 7422 3a20 6e75 6c6c  ion_count": null
+00000540: 2c0d 0a20 2020 2269 6422 3a20 2232 3463  ,..   "id": "24c
+00000550: 3934 6536 3222 2c0d 0a20 2020 226d 6574  94e62",..   "met
+00000560: 6164 6174 6122 3a20 7b7d 2c0d 0a20 2020  adata": {},..   
+00000570: 226f 7574 7075 7473 223a 205b 5d2c 0d0a  "outputs": [],..
+00000580: 2020 2022 736f 7572 6365 223a 205b 0d0a     "source": [..
+00000590: 2020 2020 2223 2045 7874 656e 6473 2074      "# Extends t
+000005a0: 6865 2043 4147 2050 6970 656c 696e 6520  he CAG Pipeline 
+000005b0: 616e 6420 696d 706c 656d 656e 7473 2074  and implements t
+000005c0: 6865 2074 776f 206d 6574 6864 733a 2070  he two methds: p
+000005d0: 726f 6365 7373 5f69 6e70 7574 2061 6e64  rocess_input and
+000005e0: 2069 6e69 745f 616e 645f 7275 6e5c 6e22   init_and_run\n"
+000005f0: 2c0d 0a20 2020 2022 636c 6173 7320 4d79  ,..    "class My
+00000600: 4669 7273 7450 6970 656c 696e 6528 5069  FirstPipeline(Pi
+00000610: 7065 6c69 6e65 293a 5c6e 222c 0d0a 2020  peline):\n",..  
+00000620: 2020 2220 2020 2064 6566 205f 5f70 6f73    "    def __pos
+00000630: 745f 696e 6974 5f5f 2873 656c 6629 3a5c  t_init__(self):\
+00000640: 6e22 2c0d 0a20 2020 2022 2020 2020 2020  n",..    "      
+00000650: 2020 7072 696e 7428 5c22 496e 2050 4f53    print(\"In POS
+00000660: 5420 494e 4954 5c22 295c 6e22 2c0d 0a20  T INIT\")\n",.. 
+00000670: 2020 2022 2020 2020 2020 2020 7365 6c66     "        self
+00000680: 2e6f 7574 5f70 6174 6820 3d20 5c22 6d79  .out_path = \"my
+00000690: 6669 7273 7470 6970 656c 696e 655f 6f75  firstpipeline_ou
+000006a0: 7470 7574 2e63 7376 5c22 5c6e 222c 0d0a  tput.csv\"\n",..
+000006b0: 2020 2020 2220 2020 2020 2020 2073 656c      "        sel
+000006c0: 662e 6578 6563 5f74 7261 6e73 666f 726d  f.exec_transform
+000006d0: 6572 5f62 6173 6564 203d 2046 616c 7365  er_based = False
+000006e0: 5c6e 222c 0d0a 2020 2020 225c 6e22 2c0d  \n",..    "\n",.
+000006f0: 0a20 2020 2022 2020 2020 2320 436f 6465  .    "    # Code
+00000700: 2066 6f72 2070 7265 7072 6f63 6573 7369   for preprocessi
+00000710: 6e67 2074 6865 2069 6e70 7574 2064 6174  ng the input dat
+00000720: 6120 6265 666f 7265 2061 6e6e 6f74 6174  a before annotat
+00000730: 696e 672e 2049 6e20 7468 6973 2063 6173  ing. In this cas
+00000740: 6520 6865 7265 2c20 7765 2063 6f6e 7665  e here, we conve
+00000750: 7274 2074 6865 206e 6f64 6573 2069 6e74  rt the nodes int
+00000760: 6f20 6120 6c69 7374 206f 6620 7475 706c  o a list of tupl
+00000770: 6573 2e5c 6e22 2c0d 0a20 2020 2022 2020  es.\n",..    "  
+00000780: 2020 2320 4561 6368 2074 7570 6c65 2063    # Each tuple c
+00000790: 6f6e 7461 696e 7320 7468 6520 7465 7874  ontains the text
+000007a0: 206f 6620 7468 6520 6e6f 6465 2061 6e64   of the node and
+000007b0: 2074 6865 205f 6b65 7920 2874 6865 2075   the _key (the u
+000007c0: 6e69 7175 6520 6964 206f 6620 7468 6520  nique id of the 
+000007d0: 6e6f 6465 295c 6e22 2c0d 0a20 2020 2022  node)\n",..    "
+000007e0: 2020 2020 6465 6620 7072 6f63 6573 735f      def process_
+000007f0: 696e 7075 7428 7365 6c66 2920 2d3e 206c  input(self) -> l
+00000800: 6973 743a 5c6e 222c 0d0a 2020 2020 2220  ist:\n",..    " 
+00000810: 2020 2020 2020 2070 726f 6365 7373 6564         processed
+00000820: 203d 205b 5d5c 6e22 2c0d 0a20 2020 2022   = []\n",..    "
+00000830: 2020 2020 2020 2020 666f 7220 7478 745f          for txt_
+00000840: 6e6f 6465 2069 6e20 7471 646d 2873 656c  node in tqdm(sel
+00000850: 662e 696e 7075 7429 3a5c 6e22 2c0d 0a20  f.input):\n",.. 
+00000860: 2020 2022 2020 2020 2020 2020 2020 2020     "            
+00000870: 7072 6f63 6573 7365 642e 6170 7065 6e64  processed.append
+00000880: 2828 7478 745f 6e6f 6465 2e74 6578 742c  ((txt_node.text,
+00000890: 207b 5c22 5f6b 6579 5c22 3a20 7478 745f   {\"_key\": txt_
+000008a0: 6e6f 6465 2e5f 6b65 797d 2929 5c6e 222c  node._key}))\n",
+000008b0: 0d0a 2020 2020 225c 6e22 2c0d 0a20 2020  ..    "\n",..   
+000008c0: 2022 2020 2020 2020 2020 7265 7475 726e   "        return
+000008d0: 2070 726f 6365 7373 6564 5c6e 222c 0d0a   processed\n",..
+000008e0: 2020 2020 225c 6e22 2c0d 0a20 2020 2022      "\n",..    "
+000008f0: 2020 2020 6465 6620 696e 6974 5f61 6e64      def init_and
+00000900: 5f72 756e 2873 656c 6629 3a5c 6e22 2c0d  _run(self):\n",.
+00000910: 0a20 2020 2022 2020 2020 2020 2020 6966  .    "        if
+00000920: 2073 656c 662e 6578 6563 5f74 7261 6e73   self.exec_trans
+00000930: 666f 726d 6572 5f62 6173 6564 3a5c 6e22  former_based:\n"
+00000940: 2c0d 0a20 2020 2022 2020 2020 2020 2020  ,..    "        
+00000950: 2020 2020 7365 6c66 2e61 6464 5f61 6e6e      self.add_ann
+00000960: 6f74 6174 696f 6e5f 7069 7065 285c 6e22  otation_pipe(\n"
+00000970: 2c0d 0a20 2020 2022 2020 2020 2020 2020  ,..    "        
+00000980: 2020 2020 2020 2020 6e61 6d65 3d5c 2273          name=\"s
+00000990: 656e 7465 6e63 697a 6572 5c22 2c5c 6e22  entencizer\",\n"
+000009a0: 2c0d 0a20 2020 2022 2020 2020 2020 2020  ,..    "        
+000009b0: 2020 2020 2020 2020 7361 7665 5f6f 7574          save_out
+000009c0: 7075 743d 4661 6c73 652c 5c6e 222c 0d0a  put=False,\n",..
+000009d0: 2020 2020 2220 2020 2020 2020 2020 2020      "           
+000009e0: 2020 2020 2069 735f 7370 6163 793d 5472       is_spacy=Tr
+000009f0: 7565 2c5c 6e22 2c0d 0a20 2020 2022 2020  ue,\n",..    "  
+00000a00: 2020 2020 2020 2020 2020 2020 2020 6973                is
+00000a10: 5f6e 6174 6976 653d 5472 7565 2c5c 6e22  _native=True,\n"
+00000a20: 2c0d 0a20 2020 2022 2020 2020 2020 2020  ,..    "        
+00000a30: 2020 2020 295c 6e22 2c0d 0a20 2020 2022      )\n",..    "
+00000a40: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00000a50: 2e61 6464 5f61 6e6e 6f74 6174 696f 6e5f  .add_annotation_
+00000a60: 7069 7065 285c 6e22 2c0d 0a20 2020 2022  pipe(\n",..    "
+00000a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000a80: 6e61 6d65 3d5c 2245 6d6f 7469 6f6e 5069  name=\"EmotionPi
+00000a90: 7065 4f72 6368 6573 7472 6174 6f72 5c22  peOrchestrator\"
+00000aa0: 2c20 7361 7665 5f6f 7574 7075 743d 5472  , save_output=Tr
+00000ab0: 7565 2c20 6973 5f73 7061 6379 3d54 7275  ue, is_spacy=Tru
+00000ac0: 655c 6e22 2c0d 0a20 2020 2022 2020 2020  e\n",..    "    
+00000ad0: 2020 2020 2020 2020 295c 6e22 2c0d 0a20          )\n",.. 
+00000ae0: 2020 2022 2020 2020 2020 2020 2020 2020     "            
+00000af0: 2320 7365 6c66 2e61 6464 5f61 6e6e 6f74  # self.add_annot
+00000b00: 6174 696f 6e5f 7069 7065 285c 6e22 2c0d  ation_pipe(\n",.
+00000b10: 0a20 2020 2022 2020 2020 2020 2020 2020  .    "          
+00000b20: 2020 2320 2020 206e 616d 653d 5c22 4865    #    name=\"He
+00000b30: 6467 6550 6970 654f 7263 6865 7374 7261  dgePipeOrchestra
+00000b40: 746f 725c 222c 2073 6176 655f 6f75 7470  tor\", save_outp
+00000b50: 7574 3d54 7275 652c 2069 735f 7370 6163  ut=True, is_spac
+00000b60: 793d 5472 7565 5c6e 222c 0d0a 2020 2020  y=True\n",..    
+00000b70: 2220 2020 2020 2020 2020 2020 2023 2029  "            # )
+00000b80: 5c6e 222c 0d0a 2020 2020 2220 2020 2020  \n",..    "     
+00000b90: 2020 2020 2020 2073 656c 662e 6164 645f         self.add_
+00000ba0: 616e 6e6f 7461 7469 6f6e 5f70 6970 6528  annotation_pipe(
+00000bb0: 5c6e 222c 0d0a 2020 2020 2220 2020 2020  \n",..    "     
+00000bc0: 2020 2020 2020 2020 2020 206e 616d 653d             name=
+00000bd0: 5c22 546f 7869 6369 7479 5069 7065 4f72  \"ToxicityPipeOr
+00000be0: 6368 6573 7472 6174 6f72 5c22 2c5c 6e22  chestrator\",\n"
+00000bf0: 2c0d 0a20 2020 2022 2020 2020 2020 2020  ,..    "        
+00000c00: 2020 2020 2020 2020 7361 7665 5f6f 7574          save_out
+00000c10: 7075 743d 5472 7565 2c5c 6e22 2c0d 0a20  put=True,\n",.. 
+00000c20: 2020 2022 2020 2020 2020 2020 2020 2020     "            
+00000c30: 2020 2020 6973 5f73 7061 6379 3d54 7275      is_spacy=Tru
+00000c40: 652c 5c6e 222c 0d0a 2020 2020 2220 2020  e,\n",..    "   
+00000c50: 2020 2020 2020 2020 2029 5c6e 222c 0d0a           )\n",..
+00000c60: 2020 2020 2220 2020 2020 2020 2065 6c73      "        els
+00000c70: 653a 5c6e 222c 0d0a 2020 2020 2220 2020  e:\n",..    "   
+00000c80: 2020 2020 2020 2020 2073 656c 662e 6164           self.ad
+00000c90: 645f 616e 6e6f 7461 7469 6f6e 5f70 6970  d_annotation_pip
+00000ca0: 6528 5c6e 222c 0d0a 2020 2020 2220 2020  e(\n",..    "   
+00000cb0: 2020 2020 2020 2020 2020 2020 206e 616d               nam
+00000cc0: 653d 5c22 746f 6b32 7665 635c 222c 5c6e  e=\"tok2vec\",\n
+00000cd0: 222c 0d0a 2020 2020 2220 2020 2020 2020  ",..    "       
+00000ce0: 2020 2020 2020 2020 2073 6176 655f 6f75           save_ou
+00000cf0: 7470 7574 3d46 616c 7365 2c5c 6e22 2c0d  tput=False,\n",.
+00000d00: 0a20 2020 2022 2020 2020 2020 2020 2020  .    "          
+00000d10: 2020 2020 2020 6973 5f73 7061 6379 3d54        is_spacy=T
+00000d20: 7275 652c 5c6e 222c 0d0a 2020 2020 2220  rue,\n",..    " 
+00000d30: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00000d40: 735f 6e61 7469 7665 3d54 7275 652c 5c6e  s_native=True,\n
+00000d50: 222c 0d0a 2020 2020 2220 2020 2020 2020  ",..    "       
+00000d60: 2020 2020 2029 2020 2320 6d61 6e64 6174       )  # mandat
+00000d70: 6f72 7920 666f 7220 4e45 525c 6e22 2c0d  ory for NER\n",.
+00000d80: 0a20 2020 2022 2020 2020 2020 2020 2020  .    "          
+00000d90: 2020 7365 6c66 2e61 6464 5f61 6e6e 6f74    self.add_annot
+00000da0: 6174 696f 6e5f 7069 7065 285c 6e22 2c0d  ation_pipe(\n",.
+00000db0: 0a20 2020 2022 2020 2020 2020 2020 2020  .    "          
+00000dc0: 2020 2020 2020 6e61 6d65 3d5c 224e 616d        name=\"Nam
+00000dd0: 6564 456e 7469 7479 5069 7065 4f72 6368  edEntityPipeOrch
+00000de0: 6573 7472 6174 6f72 5c22 2c5c 6e22 2c0d  estrator\",\n",.
+00000df0: 0a20 2020 2022 2020 2020 2020 2020 2020  .    "          
+00000e00: 2020 2020 2020 7361 7665 5f6f 7574 7075        save_outpu
+00000e10: 743d 5472 7565 2c5c 6e22 2c0d 0a20 2020  t=True,\n",..   
+00000e20: 2022 2020 2020 2020 2020 2020 2020 2020   "              
+00000e30: 2020 6973 5f73 7061 6379 3d54 7275 652c    is_spacy=True,
+00000e40: 5c6e 222c 0d0a 2020 2020 2220 2020 2020  \n",..    "     
+00000e50: 2020 2020 2020 2029 5c6e 222c 0d0a 2020         )\n",..  
+00000e60: 2020 2220 2020 2020 2020 2020 2020 2073    "            s
+00000e70: 656c 662e 6164 645f 616e 6e6f 7461 7469  elf.add_annotati
+00000e80: 6f6e 5f70 6970 6528 5c6e 222c 0d0a 2020  on_pipe(\n",..  
+00000e90: 2020 2220 2020 2020 2020 2020 2020 2020    "             
+00000ea0: 2020 206e 616d 653d 5c22 6d70 7161 5f70     name=\"mpqa_p
+00000eb0: 6172 7365 725c 222c 5c6e 222c 0d0a 2020  arser\",\n",..  
+00000ec0: 2020 2220 2020 2020 2020 2020 2020 2020    "             
+00000ed0: 2020 2073 6176 655f 6f75 7470 7574 3d46     save_output=F
+00000ee0: 616c 7365 2c5c 6e22 2c0d 0a20 2020 2022  alse,\n",..    "
+00000ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000f00: 6973 5f73 7061 6379 3d54 7275 652c 5c6e  is_spacy=True,\n
+00000f10: 222c 0d0a 2020 2020 2220 2020 2020 2020  ",..    "       
+00000f20: 2020 2020 2020 2020 2069 735f 6e61 7469           is_nati
+00000f30: 7665 3d54 7275 652c 5c6e 222c 0d0a 2020  ve=True,\n",..  
+00000f40: 2020 2220 2020 2020 2020 2020 2020 2029    "            )
+00000f50: 5c6e 222c 0d0a 2020 2020 2220 2020 2020  \n",..    "     
+00000f60: 2020 2020 2020 2073 656c 662e 6164 645f         self.add_
+00000f70: 616e 6e6f 7461 7469 6f6e 5f70 6970 6528  annotation_pipe(
+00000f80: 5c6e 222c 0d0a 2020 2020 2220 2020 2020  \n",..    "     
+00000f90: 2020 2020 2020 2020 2020 206e 616d 653d             name=
+00000fa0: 5c22 4d70 7161 5069 7065 4f72 6368 6573  \"MpqaPipeOrches
+00000fb0: 7472 6174 6f72 5c22 2c20 7361 7665 5f6f  trator\", save_o
+00000fc0: 7574 7075 743d 5472 7565 2c20 6973 5f73  utput=True, is_s
+00000fd0: 7061 6379 3d54 7275 655c 6e22 2c0d 0a20  pacy=True\n",.. 
+00000fe0: 2020 2022 2020 2020 2020 2020 2020 2020     "            
+00000ff0: 295c 6e22 2c0d 0a20 2020 2022 2020 2020  )\n",..    "    
+00001000: 2020 2020 2020 2020 7365 6c66 2e61 6464          self.add
+00001010: 5f61 6e6e 6f74 6174 696f 6e5f 7069 7065  _annotation_pipe
+00001020: 285c 6e22 2c0d 0a20 2020 2022 2020 2020  (\n",..    "    
+00001030: 2020 2020 2020 2020 2020 2020 6e61 6d65              name
+00001040: 3d5c 2245 6d70 6174 6850 6970 654f 7263  =\"EmpathPipeOrc
+00001050: 6865 7374 7261 746f 725c 222c 2073 6176  hestrator\", sav
+00001060: 655f 6f75 7470 7574 3d54 7275 652c 2069  e_output=True, i
+00001070: 735f 7370 6163 793d 5472 7565 5c6e 222c  s_spacy=True\n",
+00001080: 0d0a 2020 2020 2220 2020 2020 2020 2020  ..    "         
+00001090: 2020 2029 5c6e 222c 0d0a 2020 2020 225c     )\n",..    "\
+000010a0: 6e22 2c0d 0a20 2020 2022 2020 2020 2020  n",..    "      
+000010b0: 2020 7365 6c66 2e69 6e69 745f 7069 7065    self.init_pipe
+000010c0: 5f73 7461 636b 2829 220d 0a20 2020 5d0d  _stack()"..   ].
+000010d0: 0a20 207d 2c0d 0a20 207b 0d0a 2020 2022  .  },..  {..   "
+000010e0: 6174 7461 6368 6d65 6e74 7322 3a20 7b7d  attachments": {}
+000010f0: 2c0d 0a20 2020 2263 656c 6c5f 7479 7065  ,..   "cell_type
+00001100: 223a 2022 6d61 726b 646f 776e 222c 0d0a  ": "markdown",..
+00001110: 2020 2022 6964 223a 2022 3737 6238 3433     "id": "77b843
+00001120: 3431 222c 0d0a 2020 2022 6d65 7461 6461  41",..   "metada
+00001130: 7461 223a 207b 7d2c 0d0a 2020 2022 736f  ta": {},..   "so
+00001140: 7572 6365 223a 205b 0d0a 2020 2020 2223  urce": [..    "#
+00001150: 2320 496e 6974 6961 6c69 7a65 2079 6f75  # Initialize you
+00001160: 7220 6669 7273 7420 6361 6720 5069 7065  r first cag Pipe
+00001170: 6c69 6e65 220d 0a20 2020 5d0d 0a20 207d  line"..   ]..  }
+00001180: 2c0d 0a20 207b 0d0a 2020 2022 6365 6c6c  ,..  {..   "cell
+00001190: 5f74 7970 6522 3a20 2263 6f64 6522 2c0d  _type": "code",.
+000011a0: 0a20 2020 2265 7865 6375 7469 6f6e 5f63  .   "execution_c
+000011b0: 6f75 6e74 223a 206e 756c 6c2c 0d0a 2020  ount": null,..  
+000011c0: 2022 6964 223a 2022 3032 6131 6361 3465   "id": "02a1ca4e
+000011d0: 222c 0d0a 2020 2022 6d65 7461 6461 7461  ",..   "metadata
+000011e0: 223a 207b 7d2c 0d0a 2020 2022 6f75 7470  ": {},..   "outp
+000011f0: 7574 7322 3a20 5b5d 2c0d 0a20 2020 2273  uts": [],..   "s
+00001200: 6f75 7263 6522 3a20 5b0d 0a20 2020 2022  ource": [..    "
+00001210: 6361 675f 7069 7065 6c69 6e65 203d 204d  cag_pipeline = M
+00001220: 7946 6972 7374 5069 7065 6c69 6e65 286d  yFirstPipeline(m
+00001230: 795f 636f 6e66 6967 295c 6e22 2c0d 0a20  y_config)\n",.. 
+00001240: 2020 2022 6361 675f 7069 7065 6c69 6e65     "cag_pipeline
+00001250: 2e73 7061 6379 5f6e 5f70 726f 6365 7373  .spacy_n_process
+00001260: 6f72 7320 3d20 3120 2023 2049 6e20 6361  ors = 1  # In ca
+00001270: 7365 2079 6f75 2061 7265 2075 7369 6e67  se you are using
+00001280: 2073 7061 6379 2070 6970 652c 2074 6869   spacy pipe, thi
+00001290: 7320 666c 6167 2063 616e 2062 6520 7365  s flag can be se
+000012a0: 7420 746f 2065 6e61 626c 6520 6d75 6c74  t to enable mult
+000012b0: 6970 726f 6365 7373 696e 672c 5c6e 222c  iprocessing,\n",
+000012c0: 0d0a 2020 2020 2223 204e 4f54 453a 2049  ..    "# NOTE: I
+000012d0: 6620 796f 7520 6172 6520 7573 696e 6720  f you are using 
+000012e0: 7370 6163 7920 7769 7468 2074 7261 6e73  spacy with trans
+000012f0: 666f 726d 6572 2062 6173 6564 2066 6561  former based fea
+00001300: 7475 7265 2c20 7365 7420 7468 6520 666c  ture, set the fl
+00001310: 6167 2074 6f20 3120 6f72 2065 6c73 6520  ag to 1 or else 
+00001320: 7468 6520 7069 7065 6c69 6e65 2077 696c  the pipeline wil
+00001330: 6c20 6672 6565 7a65 2028 7468 6973 2069  l freeze (this i
+00001340: 7320 6120 7370 6163 7920 6275 6720 616e  s a spacy bug an
+00001350: 6420 6e6f 7420 7265 6c61 7465 6420 746f  d not related to
+00001360: 2063 6167 2922 0d0a 2020 205d 0d0a 2020   cag)"..   ]..  
+00001370: 7d2c 0d0a 2020 7b0d 0a20 2020 2261 7474  },..  {..   "att
+00001380: 6163 686d 656e 7473 223a 207b 7d2c 0d0a  achments": {},..
+00001390: 2020 2022 6365 6c6c 5f74 7970 6522 3a20     "cell_type": 
+000013a0: 226d 6172 6b64 6f77 6e22 2c0d 0a20 2020  "markdown",..   
+000013b0: 2269 6422 3a20 2265 3962 6637 6337 6122  "id": "e9bf7c7a"
+000013c0: 2c0d 0a20 2020 226d 6574 6164 6174 6122  ,..   "metadata"
+000013d0: 3a20 7b7d 2c0d 0a20 2020 2273 6f75 7263  : {},..   "sourc
+000013e0: 6522 3a20 5b0d 0a20 2020 2022 2323 2046  e": [..    "## F
+000013f0: 6574 6368 2074 6865 2054 6578 744e 6f64  etch the TextNod
+00001400: 6520 616e 6420 416e 6e6f 7461 7465 2026  e and Annotate &
+00001410: 2053 6176 6522 0d0a 2020 205d 0d0a 2020   Save"..   ]..  
+00001420: 7d2c 0d0a 2020 7b0d 0a20 2020 2263 656c  },..  {..   "cel
+00001430: 6c5f 7479 7065 223a 2022 636f 6465 222c  l_type": "code",
+00001440: 0d0a 2020 2022 6578 6563 7574 696f 6e5f  ..   "execution_
+00001450: 636f 756e 7422 3a20 6e75 6c6c 2c0d 0a20  count": null,.. 
+00001460: 2020 2269 6422 3a20 2236 3766 3835 6566    "id": "67f85ef
+00001470: 3322 2c0d 0a20 2020 226d 6574 6164 6174  3",..   "metadat
+00001480: 6122 3a20 7b7d 2c0d 0a20 2020 226f 7574  a": {},..   "out
+00001490: 7075 7473 223a 205b 5d2c 0d0a 2020 2022  puts": [],..   "
+000014a0: 736f 7572 6365 223a 205b 0d0a 2020 2020  source": [..    
+000014b0: 2223 2020 4c6f 6f70 206f 7665 7220 796f  "#  Loop over yo
+000014c0: 7572 2064 6174 612c 2061 6e6e 6f74 6174  ur data, annotat
+000014d0: 6541 2061 6e64 2073 6176 655c 6e22 2c0d  eA and save\n",.
+000014e0: 0a20 2020 2022 6361 675f 7069 7065 6c69  .    "cag_pipeli
+000014f0: 6e65 2e65 7865 635f 7472 616e 7366 6f72  ne.exec_transfor
+00001500: 6d65 725f 6261 7365 6420 3d20 4661 6c73  mer_based = Fals
+00001510: 655c 6e22 2c0d 0a20 2020 2022 6361 675f  e\n",..    "cag_
+00001520: 7069 7065 6c69 6e65 2e69 6e69 745f 616e  pipeline.init_an
+00001530: 645f 7275 6e28 295c 6e22 2c0d 0a20 2020  d_run()\n",..   
+00001540: 2022 5c6e 222c 0d0a 2020 2020 2263 6f6c   "\n",..    "col
+00001550: 6c20 3d20 6361 675f 7069 7065 6c69 6e65  l = cag_pipeline
+00001560: 2e64 6174 6162 6173 655f 636f 6e66 6967  .database_config
+00001570: 2e64 625b 5c22 5465 7874 4e6f 6465 5c22  .db[\"TextNode\"
+00001580: 5d5c 6e22 2c0d 0a20 2020 2022 646f 6373  ]\n",..    "docs
+00001590: 203d 2063 6f6c 6c2e 6665 7463 6841 6c6c   = coll.fetchAll
+000015a0: 286c 696d 6974 3d33 3030 295c 6e22 2c0d  (limit=300)\n",.
+000015b0: 0a20 2020 2022 6665 7463 6865 6420 3d20  .    "fetched = 
+000015c0: 6c65 6e28 646f 6373 295c 6e22 2c0d 0a20  len(docs)\n",.. 
+000015d0: 2020 2022 7768 696c 6520 646f 6373 2069     "while docs i
+000015e0: 7320 6e6f 7420 4e6f 6e65 2061 6e64 206c  s not None and l
+000015f0: 656e 2864 6f63 7329 203e 2030 3a5c 6e22  en(docs) > 0:\n"
+00001600: 2c0d 0a20 2020 2022 2020 2020 2323 2061  ,..    "    ## a
+00001610: 6e6e 6f74 6174 655c 6e22 2c0d 0a20 2020  nnotate\n",..   
+00001620: 2022 5c6e 222c 0d0a 2020 2020 2220 2020   "\n",..    "   
+00001630: 2023 2053 6574 2074 6865 2049 4e50 5554   # Set the INPUT
+00001640: 202d 2074 6869 7320 7769 6c6c 2061 7574   - this will aut
+00001650: 6f6d 6174 6963 616c 6c79 2063 616c 6c20  omatically call 
+00001660: 7072 6570 726f 6365 7373 5f69 6e70 7574  preprocess_input
+00001670: 2028 6d61 6b65 2073 7572 6520 746f 2069   (make sure to i
+00001680: 6d70 6c65 6d65 6e74 2069 7429 5c6e 222c  mplement it)\n",
+00001690: 0d0a 2020 2020 2220 2020 2063 6167 5f70  ..    "    cag_p
+000016a0: 6970 656c 696e 652e 7265 7365 745f 696e  ipeline.reset_in
+000016b0: 7075 745f 6f75 7470 7574 2829 5c6e 222c  put_output()\n",
+000016c0: 0d0a 2020 2020 2220 2020 2063 6167 5f70  ..    "    cag_p
+000016d0: 6970 656c 696e 652e 7365 745f 696e 7075  ipeline.set_inpu
+000016e0: 7428 646f 6373 295c 6e22 2c0d 0a20 2020  t(docs)\n",..   
+000016f0: 2022 5c6e 222c 0d0a 2020 2020 2220 2020   "\n",..    "   
+00001700: 2063 6167 5f70 6970 656c 696e 652e 616e   cag_pipeline.an
+00001710: 6e6f 7461 7465 2829 5c6e 222c 0d0a 2020  notate()\n",..  
+00001720: 2020 2220 2020 2063 6167 5f70 6970 656c    "    cag_pipel
+00001730: 696e 652e 7361 7665 2829 5c6e 222c 0d0a  ine.save()\n",..
+00001740: 2020 2020 225c 6e22 2c0d 0a20 2020 2022      "\n",..    "
+00001750: 2020 2020 6361 675f 7069 7065 6c69 6e65      cag_pipeline
+00001760: 2e72 6573 6574 5f69 6e70 7574 5f6f 7574  .reset_input_out
+00001770: 7075 7428 295c 6e22 2c0d 0a20 2020 2022  put()\n",..    "
+00001780: 2020 2020 7072 696e 7428 665c 2250 726f      print(f\"Pro
+00001790: 6365 7373 6564 207b 6665 7463 6865 647d  cessed {fetched}
+000017a0: 2064 6f63 735c 2229 5c6e 222c 0d0a 2020   docs\")\n",..  
+000017b0: 2020 2220 2020 2064 6f63 7320 3d20 636f    "    docs = co
+000017c0: 6c6c 2e66 6574 6368 416c 6c28 6c69 6d69  ll.fetchAll(limi
+000017d0: 743d 3130 302c 2073 6b69 703d 6665 7463  t=100, skip=fetc
+000017e0: 6865 6429 5c6e 222c 0d0a 2020 2020 2220  hed)\n",..    " 
+000017f0: 2020 2066 6574 6368 6564 203d 2066 6574     fetched = fet
+00001800: 6368 6564 202b 206c 656e 2864 6f63 7329  ched + len(docs)
+00001810: 220d 0a20 2020 5d0d 0a20 207d 2c0d 0a20  "..   ]..  },.. 
+00001820: 207b 0d0a 2020 2022 6174 7461 6368 6d65   {..   "attachme
+00001830: 6e74 7322 3a20 7b7d 2c0d 0a20 2020 2263  nts": {},..   "c
+00001840: 656c 6c5f 7479 7065 223a 2022 6d61 726b  ell_type": "mark
+00001850: 646f 776e 222c 0d0a 2020 2022 6964 223a  down",..   "id":
+00001860: 2022 6361 3539 3938 3934 222c 0d0a 2020   "ca599894",..  
+00001870: 2022 6d65 7461 6461 7461 223a 207b 7d2c   "metadata": {},
+00001880: 0d0a 2020 2022 736f 7572 6365 223a 205b  ..   "source": [
+00001890: 0d0a 2020 2020 2223 2323 2054 7261 6e73  ..    "### Trans
+000018a0: 666f 726d 6572 2062 6173 6564 2046 6561  former based Fea
+000018b0: 7475 7265 7322 0d0a 2020 205d 0d0a 2020  tures"..   ]..  
+000018c0: 7d2c 0d0a 2020 7b0d 0a20 2020 2263 656c  },..  {..   "cel
+000018d0: 6c5f 7479 7065 223a 2022 636f 6465 222c  l_type": "code",
+000018e0: 0d0a 2020 2022 6578 6563 7574 696f 6e5f  ..   "execution_
+000018f0: 636f 756e 7422 3a20 6e75 6c6c 2c0d 0a20  count": null,.. 
+00001900: 2020 2269 6422 3a20 2262 3538 3565 6639    "id": "b585ef9
+00001910: 6622 2c0d 0a20 2020 226d 6574 6164 6174  f",..   "metadat
+00001920: 6122 3a20 7b7d 2c0d 0a20 2020 226f 7574  a": {},..   "out
+00001930: 7075 7473 223a 205b 5d2c 0d0a 2020 2022  puts": [],..   "
+00001940: 736f 7572 6365 223a 205b 0d0a 2020 2020  source": [..    
+00001950: 2263 6167 5f70 6970 656c 696e 652e 6578  "cag_pipeline.ex
+00001960: 6563 5f74 7261 6e73 666f 726d 6572 5f62  ec_transformer_b
+00001970: 6173 6564 203d 2054 7275 655c 6e22 2c0d  ased = True\n",.
+00001980: 0a20 2020 2022 6361 675f 7069 7065 6c69  .    "cag_pipeli
+00001990: 6e65 2e6f 7574 5f70 6174 6820 3d20 5c22  ne.out_path = \"
+000019a0: 7472 616e 7366 6f72 6d65 725f 6261 7365  transformer_base
+000019b0: 645f 6665 6174 7572 6573 2e63 7376 5c22  d_features.csv\"
+000019c0: 5c6e 222c 0d0a 2020 2020 2263 6167 5f70  \n",..    "cag_p
+000019d0: 6970 656c 696e 652e 696e 6974 5f61 6e64  ipeline.init_and
+000019e0: 5f72 756e 2829 5c6e 222c 0d0a 2020 2020  _run()\n",..    
+000019f0: 2263 6f6c 6c20 3d20 6361 675f 7069 7065  "coll = cag_pipe
+00001a00: 6c69 6e65 2e64 6174 6162 6173 655f 636f  line.database_co
+00001a10: 6e66 6967 2e64 625b 5c22 5465 7874 4e6f  nfig.db[\"TextNo
+00001a20: 6465 5c22 5d5c 6e22 2c0d 0a20 2020 2022  de\"]\n",..    "
+00001a30: 646f 6373 203d 2063 6f6c 6c2e 6665 7463  docs = coll.fetc
+00001a40: 6841 6c6c 286c 696d 6974 3d31 3030 295c  hAll(limit=100)\
+00001a50: 6e22 2c0d 0a20 2020 2022 6665 7463 6865  n",..    "fetche
+00001a60: 6420 3d20 6c65 6e28 646f 6373 295c 6e22  d = len(docs)\n"
+00001a70: 2c0d 0a20 2020 2022 7768 696c 6520 646f  ,..    "while do
+00001a80: 6373 2069 7320 6e6f 7420 4e6f 6e65 2061  cs is not None a
+00001a90: 6e64 206c 656e 2864 6f63 7329 203e 2030  nd len(docs) > 0
+00001aa0: 3a5c 6e22 2c0d 0a20 2020 2022 2020 2020  :\n",..    "    
+00001ab0: 2323 2061 6e6e 6f74 6174 655c 6e22 2c0d  ## annotate\n",.
+00001ac0: 0a20 2020 2022 5c6e 222c 0d0a 2020 2020  .    "\n",..    
+00001ad0: 2220 2020 2023 2053 6574 2074 6865 2049  "    # Set the I
+00001ae0: 4e50 5554 202d 2074 6869 7320 7769 6c6c  NPUT - this will
+00001af0: 2061 7574 6f6d 6174 6963 616c 6c79 2063   automatically c
+00001b00: 616c 6c20 7072 6570 726f 6365 7373 5f69  all preprocess_i
+00001b10: 6e70 7574 2028 6d61 6b65 2073 7572 6520  nput (make sure 
+00001b20: 746f 2069 6d70 6c65 6d65 6e74 2069 7429  to implement it)
+00001b30: 5c6e 222c 0d0a 2020 2020 2220 2020 2063  \n",..    "    c
+00001b40: 6167 5f70 6970 656c 696e 652e 7265 7365  ag_pipeline.rese
+00001b50: 745f 696e 7075 745f 6f75 7470 7574 2829  t_input_output()
+00001b60: 5c6e 222c 0d0a 2020 2020 2220 2020 2063  \n",..    "    c
+00001b70: 6167 5f70 6970 656c 696e 652e 7365 745f  ag_pipeline.set_
+00001b80: 696e 7075 7428 646f 6373 295c 6e22 2c0d  input(docs)\n",.
+00001b90: 0a20 2020 2022 5c6e 222c 0d0a 2020 2020  .    "\n",..    
+00001ba0: 2220 2020 2063 6167 5f70 6970 656c 696e  "    cag_pipelin
+00001bb0: 652e 616e 6e6f 7461 7465 2829 5c6e 222c  e.annotate()\n",
+00001bc0: 0d0a 2020 2020 2220 2020 2063 6167 5f70  ..    "    cag_p
+00001bd0: 6970 656c 696e 652e 7361 7665 2829 5c6e  ipeline.save()\n
+00001be0: 222c 0d0a 2020 2020 225c 6e22 2c0d 0a20  ",..    "\n",.. 
+00001bf0: 2020 2022 2020 2020 7072 696e 7428 665c     "    print(f\
+00001c00: 2250 726f 6365 7373 6564 207b 6665 7463  "Processed {fetc
+00001c10: 6865 647d 2064 6f63 735c 2229 5c6e 222c  hed} docs\")\n",
+00001c20: 0d0a 2020 2020 2220 2020 2064 6f63 7320  ..    "    docs 
+00001c30: 3d20 636f 6c6c 2e66 6574 6368 416c 6c28  = coll.fetchAll(
+00001c40: 6c69 6d69 743d 3130 302c 2073 6b69 703d  limit=100, skip=
+00001c50: 6665 7463 6865 6429 5c6e 222c 0d0a 2020  fetched)\n",..  
+00001c60: 2020 2220 2020 2066 6574 6368 6564 203d    "    fetched =
+00001c70: 2066 6574 6368 6564 202b 206c 656e 2864   fetched + len(d
+00001c80: 6f63 7329 220d 0a20 2020 5d0d 0a20 207d  ocs)"..   ]..  }
+00001c90: 0d0a 205d 2c0d 0a20 226d 6574 6164 6174  .. ],.. "metadat
+00001ca0: 6122 3a20 7b0d 0a20 2022 6b65 726e 656c  a": {..  "kernel
+00001cb0: 7370 6563 223a 207b 0d0a 2020 2022 6469  spec": {..   "di
+00001cc0: 7370 6c61 795f 6e61 6d65 223a 2022 5079  splay_name": "Py
+00001cd0: 7468 6f6e 2033 222c 0d0a 2020 2022 6c61  thon 3",..   "la
+00001ce0: 6e67 7561 6765 223a 2022 7079 7468 6f6e  nguage": "python
+00001cf0: 222c 0d0a 2020 2022 6e61 6d65 223a 2022  ",..   "name": "
+00001d00: 7079 7468 6f6e 3322 0d0a 2020 7d2c 0d0a  python3"..  },..
+00001d10: 2020 226c 616e 6775 6167 655f 696e 666f    "language_info
+00001d20: 223a 207b 0d0a 2020 2022 636f 6465 6d69  ": {..   "codemi
+00001d30: 7272 6f72 5f6d 6f64 6522 3a20 7b0d 0a20  rror_mode": {.. 
+00001d40: 2020 2022 6e61 6d65 223a 2022 6970 7974     "name": "ipyt
+00001d50: 686f 6e22 2c0d 0a20 2020 2022 7665 7273  hon",..    "vers
+00001d60: 696f 6e22 3a20 330d 0a20 2020 7d2c 0d0a  ion": 3..   },..
+00001d70: 2020 2022 6669 6c65 5f65 7874 656e 7369     "file_extensi
+00001d80: 6f6e 223a 2022 2e70 7922 2c0d 0a20 2020  on": ".py",..   
+00001d90: 226d 696d 6574 7970 6522 3a20 2274 6578  "mimetype": "tex
+00001da0: 742f 782d 7079 7468 6f6e 222c 0d0a 2020  t/x-python",..  
+00001db0: 2022 6e61 6d65 223a 2022 7079 7468 6f6e   "name": "python
+00001dc0: 222c 0d0a 2020 2022 6e62 636f 6e76 6572  ",..   "nbconver
+00001dd0: 745f 6578 706f 7274 6572 223a 2022 7079  t_exporter": "py
+00001de0: 7468 6f6e 222c 0d0a 2020 2022 7079 676d  thon",..   "pygm
+00001df0: 656e 7473 5f6c 6578 6572 223a 2022 6970  ents_lexer": "ip
+00001e00: 7974 686f 6e33 222c 0d0a 2020 2022 7665  ython3",..   "ve
+00001e10: 7273 696f 6e22 3a20 2233 2e31 312e 3122  rsion": "3.11.1"
+00001e20: 0d0a 2020 7d2c 0d0a 2020 2276 7363 6f64  ..  },..  "vscod
+00001e30: 6522 3a20 7b0d 0a20 2020 2269 6e74 6572  e": {..   "inter
+00001e40: 7072 6574 6572 223a 207b 0d0a 2020 2020  preter": {..    
+00001e50: 2268 6173 6822 3a20 2239 3032 3335 3733  "hash": "9023573
+00001e60: 3039 3035 3937 6638 3831 3834 6237 6264  090597f88184b7bd
+00001e70: 6236 3032 6231 3234 3039 6465 6630 3138  b602b12409def018
+00001e80: 6438 3630 3932 6132 3066 6261 3439 3933  d86092a20fba4993
+00001e90: 3866 3133 6434 6632 6122 0d0a 2020 207d  8f13d4f2a"..   }
+00001ea0: 0d0a 2020 7d0d 0a20 7d2c 0d0a 2022 6e62  ..  }.. },.. "nb
+00001eb0: 666f 726d 6174 223a 2034 2c0d 0a20 226e  format": 4,.. "n
+00001ec0: 6266 6f72 6d61 745f 6d69 6e6f 7222 3a20  bformat_minor": 
+00001ed0: 350d 0a7d 0d0a                           5..}..
```

### Comparing `cag-1.5.0/examples/annotation_example.py` & `cag-1.5.17/examples/annotation_example.py`

 * *Files identical despite different names*

### Comparing `cag-1.5.0/examples/data/periodic_wiki_batches/Machine_learning/10Oct2021-12Oct2021/alphago_revisions.parquet` & `cag-1.5.17/examples/data/periodic_wiki_batches/Machine_learning/10Oct2021-12Oct2021/alphago_revisions.parquet`

 * *Files identical despite different names*

### Comparing `cag-1.5.0/examples/data/periodic_wiki_batches/Machine_learning/10Oct2021-12Oct2021/conference-on-knowledge-discovery-and-data-mining_revisions.parquet` & `cag-1.5.17/examples/data/periodic_wiki_batches/Machine_learning/10Oct2021-12Oct2021/conference-on-knowledge-discovery-and-data-mining_revisions.parquet`

 * *Files identical despite different names*

### Comparing `cag-1.5.0/examples/data/periodic_wiki_batches/Machine_learning/10Oct2021-12Oct2021/differential-evolution_revisions.parquet` & `cag-1.5.17/examples/data/periodic_wiki_batches/Machine_learning/10Oct2021-12Oct2021/differential-evolution_revisions.parquet`

 * *Files identical despite different names*

### Comparing `cag-1.5.0/examples/data/periodic_wiki_batches/Machine_learning/10Oct2021-12Oct2021/feature-engineering_revisions.parquet` & `cag-1.5.17/examples/data/periodic_wiki_batches/Machine_learning/10Oct2021-12Oct2021/feature-engineering_revisions.parquet`

 * *Files identical despite different names*

### Comparing `cag-1.5.0/examples/data/periodic_wiki_batches/Machine_learning/10Oct2021-12Oct2021/feature-machine-learning_revisions.parquet` & `cag-1.5.17/examples/data/periodic_wiki_batches/Machine_learning/10Oct2021-12Oct2021/feature-machine-learning_revisions.parquet`

 * *Files identical despite different names*

### Comparing `cag-1.5.0/examples/data/periodic_wiki_batches/Machine_learning/10Oct2021-12Oct2021/gpt-language-model_revisions.parquet` & `cag-1.5.17/examples/data/periodic_wiki_batches/Machine_learning/10Oct2021-12Oct2021/gpt-language-model_revisions.parquet`

 * *Files identical despite different names*

### Comparing `cag-1.5.0/examples/data/periodic_wiki_batches/Machine_learning/10Oct2021-12Oct2021/gpt3_revisions.parquet` & `cag-1.5.17/examples/data/periodic_wiki_batches/Machine_learning/10Oct2021-12Oct2021/gpt3_revisions.parquet`

 * *Files identical despite different names*

### Comparing `cag-1.5.0/examples/data/periodic_wiki_batches/Machine_learning/10Oct2021-12Oct2021/gram-matrix_revisions.parquet` & `cag-1.5.17/examples/data/periodic_wiki_batches/Machine_learning/10Oct2021-12Oct2021/gram-matrix_revisions.parquet`

 * *Files identical despite different names*

### Comparing `cag-1.5.0/examples/data/periodic_wiki_batches/Machine_learning/10Oct2021-12Oct2021/julia-programming-language_revisions.parquet` & `cag-1.5.17/examples/data/periodic_wiki_batches/Machine_learning/10Oct2021-12Oct2021/julia-programming-language_revisions.parquet`

 * *Files identical despite different names*

### Comparing `cag-1.5.0/examples/data/periodic_wiki_batches/Machine_learning/10Oct2021-12Oct2021/kaggle_revisions.parquet` & `cag-1.5.17/examples/data/periodic_wiki_batches/Machine_learning/10Oct2021-12Oct2021/kaggle_revisions.parquet`

 * *Files identical despite different names*

### Comparing `cag-1.5.0/examples/data/periodic_wiki_batches/Machine_learning/10Oct2021-12Oct2021/knearest-neighbors-algorithm_revisions.parquet` & `cag-1.5.17/examples/data/periodic_wiki_batches/Machine_learning/10Oct2021-12Oct2021/knearest-neighbors-algorithm_revisions.parquet`

 * *Files identical despite different names*

### Comparing `cag-1.5.0/examples/data/periodic_wiki_batches/Machine_learning/10Oct2021-12Oct2021/list-of-datasets-for-machinelearning-research_revisions.parquet` & `cag-1.5.17/examples/data/periodic_wiki_batches/Machine_learning/10Oct2021-12Oct2021/list-of-datasets-for-machinelearning-research_revisions.parquet`

 * *Files identical despite different names*

### Comparing `cag-1.5.0/examples/data/periodic_wiki_batches/Machine_learning/10Oct2021-12Oct2021/machine-learning-in-video-games_revisions.parquet` & `cag-1.5.17/examples/data/periodic_wiki_batches/Machine_learning/10Oct2021-12Oct2021/machine-learning-in-video-games_revisions.parquet`

 * *Files identical despite different names*

### Comparing `cag-1.5.0/examples/data/periodic_wiki_batches/Machine_learning/10Oct2021-12Oct2021/normal-discriminant-analysis_revisions.parquet` & `cag-1.5.17/examples/data/periodic_wiki_batches/Machine_learning/10Oct2021-12Oct2021/normal-discriminant-analysis_revisions.parquet`

 * *Files identical despite different names*

### Comparing `cag-1.5.0/examples/data/periodic_wiki_batches/Machine_learning/10Oct2021-12Oct2021/onnx_revisions.parquet` & `cag-1.5.17/examples/data/periodic_wiki_batches/Machine_learning/10Oct2021-12Oct2021/onnx_revisions.parquet`

 * *Files identical despite different names*

### Comparing `cag-1.5.0/examples/data/periodic_wiki_batches/Machine_learning/10Oct2021-12Oct2021/perceiver_revisions.parquet` & `cag-1.5.17/examples/data/periodic_wiki_batches/Machine_learning/10Oct2021-12Oct2021/perceiver_revisions.parquet`

 * *Files identical despite different names*

### Comparing `cag-1.5.0/examples/data/periodic_wiki_batches/Machine_learning/10Oct2021-12Oct2021/rademacher-complexity_revisions.parquet` & `cag-1.5.17/examples/data/periodic_wiki_batches/Machine_learning/10Oct2021-12Oct2021/rademacher-complexity_revisions.parquet`

 * *Files identical despite different names*

### Comparing `cag-1.5.0/examples/data/periodic_wiki_batches/Machine_learning/10Oct2021-12Oct2021/support-vector-machine_revisions.parquet` & `cag-1.5.17/examples/data/periodic_wiki_batches/Machine_learning/10Oct2021-12Oct2021/support-vector-machine_revisions.parquet`

 * *Files identical despite different names*

### Comparing `cag-1.5.0/examples/data/periodic_wiki_batches/Machine_learning/10Oct2021-12Oct2021/underfitting_revisions.parquet` & `cag-1.5.17/examples/data/periodic_wiki_batches/Machine_learning/10Oct2021-12Oct2021/underfitting_revisions.parquet`

 * *Files identical despite different names*

### Comparing `cag-1.5.0/examples/data/periodic_wiki_batches/Machine_learning/10Oct2021-12Oct2021/unsupervised-learning_revisions.parquet` & `cag-1.5.17/examples/data/periodic_wiki_batches/Machine_learning/10Oct2021-12Oct2021/unsupervised-learning_revisions.parquet`

 * *Files identical despite different names*

### Comparing `cag-1.5.0/examples/data/periodic_wiki_batches/Machine_learning/10Oct2021-12Oct2021/validation-set_revisions.parquet` & `cag-1.5.17/examples/data/periodic_wiki_batches/Machine_learning/10Oct2021-12Oct2021/validation-set_revisions.parquet`

 * *Files identical despite different names*

### Comparing `cag-1.5.0/examples/data/periodic_wiki_batches/Machine_learning/10Oct2021-12Oct2021/weak-supervision_revisions.parquet` & `cag-1.5.17/examples/data/periodic_wiki_batches/Machine_learning/10Oct2021-12Oct2021/weak-supervision_revisions.parquet`

 * *Files identical despite different names*

### Comparing `cag-1.5.0/examples/data/periodic_wiki_batches/Machine_learning/10Oct2022-12Oct2022/alex-james-professor_revisions.parquet` & `cag-1.5.17/examples/data/periodic_wiki_batches/Machine_learning/10Oct2022-12Oct2022/alex-james-professor_revisions.parquet`

 * *Files identical despite different names*

### Comparing `cag-1.5.0/examples/data/periodic_wiki_batches/Machine_learning/10Oct2022-12Oct2022/data-version-control_revisions.parquet` & `cag-1.5.17/examples/data/periodic_wiki_batches/Machine_learning/10Oct2022-12Oct2022/data-version-control_revisions.parquet`

 * *Files identical despite different names*

### Comparing `cag-1.5.0/examples/data/periodic_wiki_batches/Machine_learning/10Oct2022-12Oct2022/deepnude_revisions.parquet` & `cag-1.5.17/examples/data/periodic_wiki_batches/Machine_learning/10Oct2022-12Oct2022/deepnude_revisions.parquet`

 * *Files identical despite different names*

### Comparing `cag-1.5.0/examples/data/periodic_wiki_batches/Machine_learning/10Oct2022-12Oct2022/facial-recognition-system_revisions.parquet` & `cag-1.5.17/examples/data/periodic_wiki_batches/Machine_learning/10Oct2022-12Oct2022/facial-recognition-system_revisions.parquet`

 * *Files identical despite different names*

### Comparing `cag-1.5.0/examples/data/periodic_wiki_batches/Machine_learning/10Oct2022-12Oct2022/feature-learning_revisions.parquet` & `cag-1.5.17/examples/data/periodic_wiki_batches/Machine_learning/10Oct2022-12Oct2022/feature-learning_revisions.parquet`

 * *Files identical despite different names*

### Comparing `cag-1.5.0/examples/data/periodic_wiki_batches/Machine_learning/10Oct2022-12Oct2022/julia-programming-language_revisions.parquet` & `cag-1.5.17/examples/data/periodic_wiki_batches/Machine_learning/10Oct2022-12Oct2022/julia-programming-language_revisions.parquet`

 * *Files identical despite different names*

### Comparing `cag-1.5.0/examples/data/periodic_wiki_batches/Machine_learning/10Oct2022-12Oct2022/models-of-dna-evolution_revisions.parquet` & `cag-1.5.17/examples/data/periodic_wiki_batches/Machine_learning/10Oct2022-12Oct2022/models-of-dna-evolution_revisions.parquet`

 * *Files identical despite different names*

### Comparing `cag-1.5.0/examples/data/periodic_wiki_batches/Machine_learning/10Oct2022-12Oct2022/multipleinstance-learning_revisions.parquet` & `cag-1.5.17/examples/data/periodic_wiki_batches/Machine_learning/10Oct2022-12Oct2022/multipleinstance-learning_revisions.parquet`

 * *Files identical despite different names*

### Comparing `cag-1.5.0/examples/data/periodic_wiki_batches/Machine_learning/10Oct2022-12Oct2022/nikiai_revisions.parquet` & `cag-1.5.17/examples/data/periodic_wiki_batches/Machine_learning/10Oct2022-12Oct2022/nikiai_revisions.parquet`

 * *Files identical despite different names*

### Comparing `cag-1.5.0/examples/data/periodic_wiki_batches/Machine_learning/10Oct2022-12Oct2022/onnx_revisions.parquet` & `cag-1.5.17/examples/data/periodic_wiki_batches/Machine_learning/10Oct2022-12Oct2022/onnx_revisions.parquet`

 * *Files identical despite different names*

### Comparing `cag-1.5.0/examples/data/periodic_wiki_batches/Machine_learning/10Oct2022-12Oct2022/overfitting_revisions.parquet` & `cag-1.5.17/examples/data/periodic_wiki_batches/Machine_learning/10Oct2022-12Oct2022/overfitting_revisions.parquet`

 * *Files identical despite different names*

### Comparing `cag-1.5.0/examples/data/periodic_wiki_batches/Machine_learning/10Oct2022-12Oct2022/pop-music-automation_revisions.parquet` & `cag-1.5.17/examples/data/periodic_wiki_batches/Machine_learning/10Oct2022-12Oct2022/pop-music-automation_revisions.parquet`

 * *Files identical despite different names*

### Comparing `cag-1.5.0/examples/data/periodic_wiki_batches/Machine_learning/10Oct2022-12Oct2022/prescription-monitoring-program_revisions.parquet` & `cag-1.5.17/examples/data/periodic_wiki_batches/Machine_learning/10Oct2022-12Oct2022/prescription-monitoring-program_revisions.parquet`

 * *Files identical despite different names*

### Comparing `cag-1.5.0/examples/data/periodic_wiki_batches/Machine_learning/10Oct2022-12Oct2022/squared-error-loss_revisions.parquet` & `cag-1.5.17/examples/data/periodic_wiki_batches/Machine_learning/10Oct2022-12Oct2022/squared-error-loss_revisions.parquet`

 * *Files identical despite different names*

### Comparing `cag-1.5.0/examples/data/periodic_wiki_batches/Machine_learning/10Oct2022-12Oct2022/stochastic-gradient-descent_revisions.parquet` & `cag-1.5.17/examples/data/periodic_wiki_batches/Machine_learning/10Oct2022-12Oct2022/stochastic-gradient-descent_revisions.parquet`

 * *Files identical despite different names*

### Comparing `cag-1.5.0/examples/data/periodic_wiki_batches/Machine_learning/10Oct2022-12Oct2022/symbolic-regression_revisions.parquet` & `cag-1.5.17/examples/data/periodic_wiki_batches/Machine_learning/10Oct2022-12Oct2022/symbolic-regression_revisions.parquet`

 * *Files identical despite different names*

### Comparing `cag-1.5.0/examples/data/periodic_wiki_batches/Machine_learning/10Oct2022-12Oct2022/word2vec_revisions.parquet` & `cag-1.5.17/examples/data/periodic_wiki_batches/Machine_learning/10Oct2022-12Oct2022/word2vec_revisions.parquet`

 * *Files identical despite different names*

### Comparing `cag-1.5.0/examples/example.html` & `cag-1.5.17/examples/example.html`

 * *Files identical despite different names*

### Comparing `cag-1.5.0/examples/view_creation_example.py` & `cag-1.5.17/examples/view_creation_example.py`

 * *Files identical despite different names*

### Comparing `cag-1.5.0/pyproject.toml` & `cag-1.5.17/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -3,109 +3,90 @@
 00000020: 7465 6d5d 0d0a 7265 7175 6972 6573 203d  tem]..requires =
 00000030: 205b 2266 6c69 745f 636f 7265 203e 3d33   ["flit_core >=3
 00000040: 2e32 2c3c 3422 5d0d 0a62 7569 6c64 2d62  .2,<4"]..build-b
 00000050: 6163 6b65 6e64 203d 2022 666c 6974 5f63  ackend = "flit_c
 00000060: 6f72 652e 6275 696c 6461 7069 220d 0a0d  ore.buildapi"...
 00000070: 0a5b 7072 6f6a 6563 745d 0d0a 6e61 6d65  .[project]..name
 00000080: 203d 2022 6361 6722 0d0a 7665 7273 696f   = "cag"..versio
-00000090: 6e20 3d20 2231 2e35 2e30 220d 0a64 6573  n = "1.5.0"..des
-000000a0: 6372 6970 7469 6f6e 3d27 5468 6973 2069  cription='This i
-000000b0: 7320 6120 6765 6e65 7261 6c20 6672 616d  s a general fram
-000000c0: 6577 6f72 6b20 746f 2063 7265 6174 6520  ework to create 
-000000d0: 6172 616e 676f 2064 6220 6772 6170 6873  arango db graphs
-000000e0: 2061 6e64 2061 6e6e 6f74 6174 6520 7468   and annotate th
-000000f0: 656d 2e27 0d0a 7265 6164 6d65 203d 2022  em.'..readme = "
-00000100: 5245 4144 4d45 2e6d 6422 0d0a 6175 7468  README.md"..auth
-00000110: 6f72 7320 3d20 5b7b 206e 616d 6520 3d20  ors = [{ name = 
-00000120: 2252 6f78 616e 6e65 2045 6c20 4261 6666  "Roxanne El Baff
-00000130: 222c 2065 6d61 696c 203d 2022 726f 7861  ", email = "roxa
-00000140: 6e6e 652e 656c 6261 6666 4064 6c72 2e64  nne.elbaff@dlr.d
-00000150: 6522 207d 2c0d 0a20 2020 2020 2020 2020  e" },..         
-00000160: 2020 207b 206e 616d 6520 3d20 2254 6f62     { name = "Tob
-00000170: 6961 7320 4865 636b 696e 6722 2c20 656d  ias Hecking", em
-00000180: 6169 6c20 3d20 2274 6f62 6961 732e 6865  ail = "tobias.he
-00000190: 636b 696e 6740 646c 722e 6465 2220 7d5d  cking@dlr.de" }]
+00000090: 6e20 3d20 2231 2e35 2e31 3722 0d0a 6465  n = "1.5.17"..de
+000000a0: 7363 7269 7074 696f 6e20 3d20 2754 6869  scription = 'Thi
+000000b0: 7320 6973 2061 2067 656e 6572 616c 2066  s is a general f
+000000c0: 7261 6d65 776f 726b 2074 6f20 6372 6561  ramework to crea
+000000d0: 7465 2061 7261 6e67 6f20 6462 2067 7261  te arango db gra
+000000e0: 7068 7320 616e 6420 616e 6e6f 7461 7465  phs and annotate
+000000f0: 2074 6865 6d2e 270d 0a72 6561 646d 6520   them.'..readme 
+00000100: 3d20 2252 4541 444d 452e 6d64 220d 0a61  = "README.md"..a
+00000110: 7574 686f 7273 203d 205b 0d0a 2020 7b20  uthors = [..  { 
+00000120: 6e61 6d65 203d 2022 526f 7861 6e6e 6520  name = "Roxanne 
+00000130: 456c 2042 6166 6622 2c20 656d 6169 6c20  El Baff", email 
+00000140: 3d20 2272 6f78 616e 6e65 2e65 6c62 6166  = "roxanne.elbaf
+00000150: 6640 646c 722e 6465 2220 7d2c 0d0a 2020  f@dlr.de" },..  
+00000160: 7b20 6e61 6d65 203d 2022 546f 6269 6173  { name = "Tobias
+00000170: 2048 6563 6b69 6e67 222c 2065 6d61 696c   Hecking", email
+00000180: 203d 2022 746f 6269 6173 2e68 6563 6b69   = "tobias.hecki
+00000190: 6e67 4064 6c72 2e64 6522 207d 2c0d 0a5d  ng@dlr.de" },..]
 000001a0: 0d0a 6c69 6365 6e73 6520 3d20 7b20 6669  ..license = { fi
 000001b0: 6c65 203d 2022 4c49 4345 4e53 4522 207d  le = "LICENSE" }
 000001c0: 0d0a 636c 6173 7369 6669 6572 7320 3d20  ..classifiers = 
-000001d0: 5b0d 0a20 2020 2022 4c69 6365 6e73 6520  [..    "License 
-000001e0: 3a3a 204f 5349 2041 7070 726f 7665 6420  :: OSI Approved 
-000001f0: 3a3a 204d 4954 204c 6963 656e 7365 222c  :: MIT License",
-00000200: 0d0a 2020 2020 2250 726f 6772 616d 6d69  ..    "Programmi
-00000210: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-00000220: 7974 686f 6e22 2c0d 0a20 2020 2022 5072  ython",..    "Pr
-00000230: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
-00000240: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
-00000250: 3322 2c0d 0a20 2020 2027 4465 7665 6c6f  3",..    'Develo
-00000260: 706d 656e 7420 5374 6174 7573 203a 3a20  pment Status :: 
-00000270: 3320 2d20 416c 7068 6127 2c0d 0a20 2020  3 - Alpha',..   
-00000280: 2027 496e 7465 6e64 6564 2041 7564 6965   'Intended Audie
-00000290: 6e63 6520 3a3a 2053 6369 656e 6365 2f52  nce :: Science/R
-000002a0: 6573 6561 7263 6827 2c0d 0a0d 0a5d 0d0a  esearch',....]..
-000002b0: 6b65 7977 6f72 6473 3d5b 2767 7261 7068  keywords=['graph
-000002c0: 272c 2027 6172 6368 6974 6563 7475 7261  ', 'architectura
-000002d0: 6c20 6672 616d 6577 6f72 6b27 2c20 2767  l framework', 'g
-000002e0: 7261 7068 2063 7265 6174 6f72 272c 2027  raph creator', '
-000002f0: 6772 6170 6820 616e 6e6f 7461 746f 7227  graph annotator'
-00000300: 5d0d 0a64 6570 656e 6465 6e63 6965 7320  ]..dependencies 
-00000310: 3d20 5b27 6461 7461 636c 6173 7365 733e  = ['dataclasses>
-00000320: 3d30 2e36 272c 0d0a 2020 2020 2020 2020  =0.6',..        
-00000330: 2020 2020 2020 2020 2020 2020 2773 7061              'spa
-00000340: 6379 3e3d 332e 342e 3127 2c0d 0a20 2020  cy>=3.4.1',..   
-00000350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000360: 2027 7370 6163 795f 6172 6775 696e 675f   'spacy_arguing_
-00000370: 6c65 7869 636f 6e3e 3d30 2e30 2e33 272c  lexicon>=0.0.3',
-00000380: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00000390: 2020 2020 2020 2765 6d70 6174 683e 3d30        'empath>=0
-000003a0: 2e38 3927 2c0d 0a20 2020 2020 2020 2020  .89',..         
-000003b0: 2020 2020 2020 2020 2020 2027 7079 7465             'pyte
-000003c0: 7374 3e3d 372e 312e 3227 2c0d 0a20 2020  st>=7.1.2',..   
-000003d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000003e0: 2027 6e65 7477 6f72 6b78 3e3d 322e 382e   'networkx>=2.8.
-000003f0: 3527 2c0d 0a20 2020 2020 2020 2020 2020  5',..           
-00000400: 2020 2020 2020 2020 2027 6e6c 746b 3e3d           'nltk>=
-00000410: 332e 342e 3527 2c0d 0a20 2020 2020 2020  3.4.5',..       
-00000420: 2020 2020 2020 2020 2020 2020 2027 7079               'py
-00000430: 7669 733e 3d30 2e32 2e31 272c 0d0a 2020  vis>=0.2.1',..  
-00000440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000450: 2020 2774 7164 6d3e 3d34 2e34 332e 3027    'tqdm>=4.43.0'
-00000460: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00000470: 2020 2020 2020 2027 7079 7468 6f6e 2d61         'python-a
-00000480: 7261 6e67 6f3e 3d37 2e34 2e31 272c 0d0a  rango>=7.4.1',..
-00000490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000004a0: 2020 2020 2770 7941 7261 6e67 6f3e 3d32      'pyArango>=2
-000004b0: 2e30 2e31 272c 0d0a 2020 2020 2020 2020  .0.1',..        
-000004c0: 2020 2020 2020 2020 2020 2020 2774 6f6d              'tom
-000004d0: 6c69 3e3d 322e 302e 3127 2c0d 0a20 2020  li>=2.0.1',..   
-000004e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000004f0: 2027 7472 616e 7366 6f72 6d65 7273 3e3d   'transformers>=
-00000500: 342e 3236 2e31 272c 0d0a 2020 2020 2020  4.26.1',..      
-00000510: 2020 2020 2020 2020 2020 2020 2020 2774                't
-00000520: 656e 6163 6974 793e 3d38 2e32 2e32 272c  enacity>=8.2.2',
-00000530: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00000540: 2020 2020 2020 2770 616e 6461 7327 2c0d        'pandas',.
-00000550: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000560: 2020 2020 2027 7079 7468 6f6e 2d73 6c75       'python-slu
-00000570: 6769 6679 7e3d 362e 312e 3227 2c0d 0a20  gify~=6.1.2',.. 
-00000580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000590: 2020 2027 7269 6368 7e3d 3132 2e36 2e30     'rich~=12.6.0
-000005a0: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
-000005b0: 2020 2020 2020 2020 2763 6f6f 6b69 6563          'cookiec
-000005c0: 7574 7465 723e 3d32 2e31 2e31 270d 0a20  utter>=2.1.1'.. 
-000005d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000005e0: 2020 2020 205d 0d0a 7265 7175 6972 6573       ]..requires
-000005f0: 2d70 7974 686f 6e20 3d20 223e 3d33 2e38  -python = ">=3.8
-00000600: 220d 0a0d 0a5b 7072 6f6a 6563 742e 6f70  "....[project.op
-00000610: 7469 6f6e 616c 2d64 6570 656e 6465 6e63  tional-dependenc
-00000620: 6965 735d 0d0a 6465 7620 3d20 5b20 2270  ies]..dev = [ "p
-00000630: 6970 2d74 6f6f 6c73 222c 2022 7079 7465  ip-tools", "pyte
-00000640: 7374 225d 0d0a 0d0a 5b70 726f 6a65 6374  st"]....[project
-00000650: 2e75 726c 735d 0d0a 486f 6d65 7061 6765  .urls]..Homepage
-00000660: 203d 2027 6874 7470 733a 2f2f 6769 7468   = 'https://gith
-00000670: 7562 2e63 6f6d 2f44 4c52 2d53 432f 636f  ub.com/DLR-SC/co
-00000680: 7270 7573 2d61 6e6e 6f74 6174 696f 6e2d  rpus-annotation-
-00000690: 6772 6170 682d 6275 696c 6465 7227 0d0a  graph-builder'..
-000006a0: 0d0a 0d0a 5b70 726f 6a65 6374 2e73 6372  ....[project.scr
-000006b0: 6970 7473 5d0d 0a63 6167 3d22 6361 672e  ipts]..cag="cag.
-000006c0: 636c 693a 6170 7022 0d0a 0d0a 5b74 6f6f  cli:app"....[too
-000006d0: 6c2e 626c 6163 6b5d 0d0a 6c69 6e65 2d6c  l.black]..line-l
-000006e0: 656e 6774 6820 3d20 3739 0d0a            ength = 79..
+000001d0: 5b0d 0a20 2022 4c69 6365 6e73 6520 3a3a  [..  "License ::
+000001e0: 204f 5349 2041 7070 726f 7665 6420 3a3a   OSI Approved ::
+000001f0: 204d 4954 204c 6963 656e 7365 222c 0d0a   MIT License",..
+00000200: 2020 2250 726f 6772 616d 6d69 6e67 204c    "Programming L
+00000210: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
+00000220: 6e22 2c0d 0a20 2022 5072 6f67 7261 6d6d  n",..  "Programm
+00000230: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
+00000240: 5079 7468 6f6e 203a 3a20 3322 2c0d 0a20  Python :: 3",.. 
+00000250: 2027 4465 7665 6c6f 706d 656e 7420 5374   'Development St
+00000260: 6174 7573 203a 3a20 3320 2d20 416c 7068  atus :: 3 - Alph
+00000270: 6127 2c0d 0a20 2027 496e 7465 6e64 6564  a',..  'Intended
+00000280: 2041 7564 6965 6e63 6520 3a3a 2053 6369   Audience :: Sci
+00000290: 656e 6365 2f52 6573 6561 7263 6827 2c0d  ence/Research',.
+000002a0: 0a0d 0a5d 0d0a 6b65 7977 6f72 6473 203d  ...]..keywords =
+000002b0: 205b 0d0a 2020 2767 7261 7068 272c 0d0a   [..  'graph',..
+000002c0: 2020 2761 7263 6869 7465 6374 7572 616c    'architectural
+000002d0: 2066 7261 6d65 776f 726b 272c 0d0a 2020   framework',..  
+000002e0: 2767 7261 7068 2063 7265 6174 6f72 272c  'graph creator',
+000002f0: 0d0a 2020 2767 7261 7068 2061 6e6e 6f74  ..  'graph annot
+00000300: 6174 6f72 272c 0d0a 5d0d 0a64 6570 656e  ator',..]..depen
+00000310: 6465 6e63 6965 7320 3d20 5b0d 0a20 2027  dencies = [..  '
+00000320: 6461 7461 636c 6173 7365 733e 3d30 2e36  dataclasses>=0.6
+00000330: 272c 0d0a 2020 2773 7061 6379 3e3d 332e  ',..  'spacy>=3.
+00000340: 342e 3127 2c0d 0a20 2027 7370 6163 795f  4.1',..  'spacy_
+00000350: 6172 6775 696e 675f 6c65 7869 636f 6e3e  arguing_lexicon>
+00000360: 3d30 2e30 2e33 272c 0d0a 2020 2765 6d70  =0.0.3',..  'emp
+00000370: 6174 683e 3d30 2e38 3927 2c0d 0a20 2027  ath>=0.89',..  '
+00000380: 7079 7465 7374 3e3d 372e 312e 3227 2c0d  pytest>=7.1.2',.
+00000390: 0a20 2027 6e65 7477 6f72 6b78 3e3d 322e  .  'networkx>=2.
+000003a0: 382e 3527 2c0d 0a20 2027 6e6c 746b 3e3d  8.5',..  'nltk>=
+000003b0: 332e 342e 3527 2c0d 0a20 2027 7079 7669  3.4.5',..  'pyvi
+000003c0: 733e 3d30 2e32 2e31 272c 0d0a 2020 2774  s>=0.2.1',..  't
+000003d0: 7164 6d3e 3d34 2e34 332e 3027 2c0d 0a20  qdm>=4.43.0',.. 
+000003e0: 2027 7079 7468 6f6e 2d61 7261 6e67 6f3e   'python-arango>
+000003f0: 3d37 2e34 2e31 272c 0d0a 2020 2770 7941  =7.4.1',..  'pyA
+00000400: 7261 6e67 6f3e 3d32 2e30 2e31 272c 0d0a  rango>=2.0.1',..
+00000410: 2020 2774 6f6d 6c69 3e3d 322e 302e 3127    'tomli>=2.0.1'
+00000420: 2c0d 0a20 2027 7472 616e 7366 6f72 6d65  ,..  'transforme
+00000430: 7273 3e3d 342e 3236 2e31 272c 0d0a 2020  rs>=4.26.1',..  
+00000440: 2774 656e 6163 6974 793e 3d38 2e32 2e32  'tenacity>=8.2.2
+00000450: 272c 0d0a 2020 2770 616e 6461 7327 2c0d  ',..  'pandas',.
+00000460: 0a20 2027 7079 7468 6f6e 2d73 6c75 6769  .  'python-slugi
+00000470: 6679 7e3d 362e 312e 3227 2c0d 0a20 2027  fy~=6.1.2',..  '
+00000480: 7269 6368 7e3d 3132 2e36 2e30 272c 0d0a  rich~=12.6.0',..
+00000490: 2020 2763 6f6f 6b69 6563 7574 7465 723e    'cookiecutter>
+000004a0: 3d32 2e31 2e31 272c 0d0a 5d0d 0a72 6571  =2.1.1',..]..req
+000004b0: 7569 7265 732d 7079 7468 6f6e 203d 2022  uires-python = "
+000004c0: 3e3d 332e 3822 0d0a 0d0a 5b70 726f 6a65  >=3.8"....[proje
+000004d0: 6374 2e6f 7074 696f 6e61 6c2d 6465 7065  ct.optional-depe
+000004e0: 6e64 656e 6369 6573 5d0d 0a64 6576 203d  ndencies]..dev =
+000004f0: 205b 2270 6970 2d74 6f6f 6c73 222c 2022   ["pip-tools", "
+00000500: 7079 7465 7374 225d 0d0a 0d0a 5b70 726f  pytest"]....[pro
+00000510: 6a65 6374 2e75 726c 735d 0d0a 486f 6d65  ject.urls]..Home
+00000520: 7061 6765 203d 2027 6874 7470 733a 2f2f  page = 'https://
+00000530: 6769 7468 7562 2e63 6f6d 2f44 4c52 2d53  github.com/DLR-S
+00000540: 432f 636f 7270 7573 2d61 6e6e 6f74 6174  C/corpus-annotat
+00000550: 696f 6e2d 6772 6170 682d 6275 696c 6465  ion-graph-builde
+00000560: 7227 0d0a 0d0a 0d0a 5b70 726f 6a65 6374  r'......[project
+00000570: 2e73 6372 6970 7473 5d0d 0a63 6167 203d  .scripts]..cag =
+00000580: 2022 6361 672e 636c 693a 6170 7022 0d0a   "cag.cli:app"..
+00000590: 0d0a 5b74 6f6f 6c2e 626c 6163 6b5d 0d0a  ..[tool.black]..
+000005a0: 6c69 6e65 2d6c 656e 6774 6820 3d20 3739  line-length = 79
+000005b0: 0d0a                                     ..
```

### Comparing `cag-1.5.0/tests/__init__.py` & `cag-1.5.17/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cag-1.5.0/tests/test_graph_creator.py` & `cag-1.5.17/tests/test_graph_creator.py`

 * *Files identical despite different names*

### Comparing `cag-1.5.0/tests/test_graph_creator/test_improve_edge_definitions.py` & `cag-1.5.17/tests/test_graph_creator/test_improve_edge_definitions.py`

 * *Files identical despite different names*

### Comparing `cag-1.5.0/tests/test_view.py` & `cag-1.5.17/tests/test_view.py`

 * *Files identical despite different names*

### Comparing `cag-1.5.0/PKG-INFO` & `cag-1.5.17/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cag
-Version: 1.5.0
+Version: 1.5.17
 Summary: This is a general framework to create arango db graphs and annotate them.
 Keywords: graph,architectural framework,graph creator,graph annotator
 Author-email: Roxanne El Baff <roxanne.elbaff@dlr.de>, Tobias Hecking <tobias.hecking@dlr.de>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -61,15 +61,15 @@
 
 > `cag` is a Python Library offering an architectural framework to employ the build-annotate pattern when building Graphs.
 
 ---
 
 
 
-[Paper video](https://drive.google.com/drive/folders/1KE4NT2NQyfj4VYsAdQAE8WoBpGWA33O0?usp=sharing).
+[Official Documentation](https://cagraph.info/).
 
 **Corpus Annotation Graph builder (CAG)**  is an *architectural framework* that employs the *build-and-annotate* pattern for creating a graph. CAG is built on top of [ArangoDB](https://www.arangodb.com) and its Python drivers ([PyArango](https://pyarango.readthedocs.io/en/latest/)). The *build-and-annotate* pattern consists of two phases (see Figure below): (1) data is collected from different sources (e.g., publication databases, online encyclopedias, news feeds, web portals, electronic libraries, repositories, media platforms) and preprocessed to build the core nodes, which we call *Objects of Interest*. The component responsible for this phase is the **Graph-Creator**. (2) Annotations are extracted from the OOIs, and corresponding annotation nodes are created and linked to the core nodes. The component dealing with this phase is the **Graph-Annotator**.
 
 
 ![cag](https://github.com/DLR-SC/corpus-annotation-graph-builder/blob/main/docs/cag.png?raw=true)
 
 
@@ -89,31 +89,42 @@
 
 ### Manual cloning
 Clone the repository, go to the root folder and then run:
 
 ```
 pip install -e .
 ```
+
+## Citation
+Please cite us in case you use CAG
+
+    @inproceedings{el-baff-etal-2023-corpus,
+      title = "Corpus Annotation Graph Builder ({CAG}): An Architectural Framework to Create and Annotate a Multi-source Graph",
+      author = "El Baff, Roxanne  and
+        Hecking, Tobias  and
+        Hamm, Andreas  and
+        Korte, Jasper W.  and
+        Bartsch, Sabine",
+      booktitle = "Proceedings of the 17th Conference of the European Chapter of the Association for Computational Linguistics: System Demonstrations",
+      month = may,
+      year = "2023",
+      address = "Dubrovnik, Croatia",
+      publisher = "Association for Computational Linguistics",
+      url = "https://aclanthology.org/2023.eacl-demo.28",
+      pages = "248--255"
+    }
+
+
 ## Usage
 * After the installation, a project scaffold can be created with the command `cag start-project`
 * Graph Creation [[jupyter notebook](https://github.com/DLR-SC/corpus-annotation-graph-builder/blob/main/examples/1_create_graph.ipynb)]
 * Graph Annotation [[jupyter notebook](https://github.com/DLR-SC/corpus-annotation-graph-builder/blob/main/examples/2_annotate_graph.ipynb)]
 
 
-## Citation
-Please cite us in case you use CAG
 
-      @InProceedings{elbaffdemo:2023,
-        author =  {Roxanne {El Baff} and Tobias Hecking and Andreas Hamm and Jasper W. Korte and Sabine Bartsch},
-        title     = {Corpus {A}nnotation {G}raph Builder ({CAG}):  An Architectural Framework to Create and Annotate a Multi-source Graph},
-        booktitle = {The 17th Conference of the European Chapter of the Association for Computational Linguistics (EACL 2023): : System Demonstrations },
-        month = "may",
-        year = "2023"
-        address = "Dubrovnik, Croatia",
-        publisher = "Association for Computational Linguistics",
-        }
+## Zenodo refs
 
+* v1.5.0 [![DOI](https://zenodo.org/badge/572124344.svg)](https://zenodo.org/badge/latestdoi/572124344)
+* v1.4.0 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7701921.svg)](https://doi.org/10.5281/zenodo.7701921)
 
-## Zenodo refs
-v1.4.0 [![DOI](https://zenodo.org/badge/572124344.svg)](https://zenodo.org/badge/latestdoi/572124344)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cag Version: 1.5.0 Summary: This is a general
+Metadata-Version: 2.1 Name: cag Version: 1.5.17 Summary: This is a general
 framework to create arango db graphs and annotate them. Keywords:
 graph,architectural framework,graph creator,graph annotator Author-email:
 Roxanne El Baff
 elbaff@dlr.de>, Tobias Hecking
 hecking@dlr.de> Requires-Python: >=3.8 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python Classifier: Programming Language :: Python :: 3 Classifier:
@@ -17,43 +17,46 @@
 Requires-Dist: cookiecutter>=2.1.1 Requires-Dist: pip-tools ; extra == "dev"
 Requires-Dist: pytest ; extra == "dev" Project-URL: Homepage, https://
 github.com/DLR-SC/corpus-annotation-graph-builder Provides-Extra: dev
       ****** Welcome to the Corpus Annotation Graph Builder (CAG) ******
 [Badge:_PyPI_version] [Badge:_Made_with_Python] [Badge:_Open_in_VSCode] [Badge:
               Black] [DOI] [License:_MIT] [Twitter:_DLR_Software]
 > `cag` is a Python Library offering an architectural framework to employ the
-build-annotate pattern when building Graphs. --- [Paper video](https://
-drive.google.com/drive/folders/1KE4NT2NQyfj4VYsAdQAE8WoBpGWA33O0?usp=sharing).
-**Corpus Annotation Graph builder (CAG)** is an *architectural framework* that
-employs the *build-and-annotate* pattern for creating a graph. CAG is built on
-top of [ArangoDB](https://www.arangodb.com) and its Python drivers ([PyArango]
-(https://pyarango.readthedocs.io/en/latest/)). The *build-and-annotate* pattern
-consists of two phases (see Figure below): (1) data is collected from different
-sources (e.g., publication databases, online encyclopedias, news feeds, web
-portals, electronic libraries, repositories, media platforms) and preprocessed
-to build the core nodes, which we call *Objects of Interest*. The component
-responsible for this phase is the **Graph-Creator**. (2) Annotations are
-extracted from the OOIs, and corresponding annotation nodes are created and
-linked to the core nodes. The component dealing with this phase is the **Graph-
-Annotator**. ![cag](https://github.com/DLR-SC/corpus-annotation-graph-builder/
-blob/main/docs/cag.png?raw=true) This framework aims to offer researchers a
-flexible but unified and reproducible way of organizing and maintaining their
-interlinked document collections in a Corpus Annotation Graph. ## Installation
-### Direct install via pip The package can also be installed directly via pip.
-``` pip install cag ``` This will allow you to use the module **`cag`** from
-any python script locally. The two main packages are **`cag.framework`** and
+build-annotate pattern when building Graphs. --- [Official Documentation]
+(https://cagraph.info/). **Corpus Annotation Graph builder (CAG)** is an
+*architectural framework* that employs the *build-and-annotate* pattern for
+creating a graph. CAG is built on top of [ArangoDB](https://www.arangodb.com)
+and its Python drivers ([PyArango](https://pyarango.readthedocs.io/en/latest/
+)). The *build-and-annotate* pattern consists of two phases (see Figure below):
+(1) data is collected from different sources (e.g., publication databases,
+online encyclopedias, news feeds, web portals, electronic libraries,
+repositories, media platforms) and preprocessed to build the core nodes, which
+we call *Objects of Interest*. The component responsible for this phase is the
+**Graph-Creator**. (2) Annotations are extracted from the OOIs, and
+corresponding annotation nodes are created and linked to the core nodes. The
+component dealing with this phase is the **Graph-Annotator**. ![cag](https://
+github.com/DLR-SC/corpus-annotation-graph-builder/blob/main/docs/
+cag.png?raw=true) This framework aims to offer researchers a flexible but
+unified and reproducible way of organizing and maintaining their interlinked
+document collections in a Corpus Annotation Graph. ## Installation ### Direct
+install via pip The package can also be installed directly via pip. ``` pip
+install cag ``` This will allow you to use the module **`cag`** from any python
+script locally. The two main packages are **`cag.framework`** and
 **`cag.view_wrapper`**. ### Manual cloning Clone the repository, go to the root
-folder and then run: ``` pip install -e . ``` ## Usage * After the
-installation, a project scaffold can be created with the command `cag start-
-project` * Graph Creation [[jupyter notebook](https://github.com/DLR-SC/corpus-
-annotation-graph-builder/blob/main/examples/1_create_graph.ipynb)] * Graph
-Annotation [[jupyter notebook](https://github.com/DLR-SC/corpus-annotation-
-graph-builder/blob/main/examples/2_annotate_graph.ipynb)] ## Citation Please
-cite us in case you use CAG @InProceedings{elbaffdemo:2023, author = {Roxanne
-{El Baff} and Tobias Hecking and Andreas Hamm and Jasper W. Korte and Sabine
-Bartsch}, title = {Corpus {A}nnotation {G}raph Builder ({CAG}): An
-Architectural Framework to Create and Annotate a Multi-source Graph}, booktitle
-= {The 17th Conference of the European Chapter of the Association for
-Computational Linguistics (EACL 2023): : System Demonstrations }, month =
-"may", year = "2023" address = "Dubrovnik, Croatia", publisher = "Association
-for Computational Linguistics", } ## Zenodo refs v1.4.0 [![DOI](https://
-zenodo.org/badge/572124344.svg)](https://zenodo.org/badge/latestdoi/572124344)
+folder and then run: ``` pip install -e . ``` ## Citation Please cite us in
+case you use CAG @inproceedings{el-baff-etal-2023-corpus, title = "Corpus
+Annotation Graph Builder ({CAG}): An Architectural Framework to Create and
+Annotate a Multi-source Graph", author = "El Baff, Roxanne and Hecking, Tobias
+and Hamm, Andreas and Korte, Jasper W. and Bartsch, Sabine", booktitle =
+"Proceedings of the 17th Conference of the European Chapter of the Association
+for Computational Linguistics: System Demonstrations", month = may, year =
+"2023", address = "Dubrovnik, Croatia", publisher = "Association for
+Computational Linguistics", url = "https://aclanthology.org/2023.eacl-demo.28",
+pages = "248--255" } ## Usage * After the installation, a project scaffold can
+be created with the command `cag start-project` * Graph Creation [[jupyter
+notebook](https://github.com/DLR-SC/corpus-annotation-graph-builder/blob/main/
+examples/1_create_graph.ipynb)] * Graph Annotation [[jupyter notebook](https://
+github.com/DLR-SC/corpus-annotation-graph-builder/blob/main/examples/
+2_annotate_graph.ipynb)] ## Zenodo refs * v1.5.0 [![DOI](https://zenodo.org/
+badge/572124344.svg)](https://zenodo.org/badge/latestdoi/572124344) * v1.4.0 [!
+[DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7701921.svg)](https://
+doi.org/10.5281/zenodo.7701921)
```

