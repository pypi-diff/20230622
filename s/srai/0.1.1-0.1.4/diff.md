# Comparing `tmp/srai-0.1.1.tar.gz` & `tmp/srai-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "srai-0.1.1.tar", last modified: Thu Apr 27 21:17:23 2023, max compression
+gzip compressed data, was "srai-0.1.4.tar", last modified: Thu Jun 22 17:29:50 2023, max compression
```

## Comparing `srai-0.1.1.tar` & `srai-0.1.4.tar`

### file list

```diff
@@ -1,126 +1,126 @@
--rw-r--r--   0        0        0    10760 2023-04-27 21:17:06.196857 srai-0.1.1/LICENSE.md
--rw-r--r--   0        0        0    14916 2023-04-27 21:17:06.196857 srai-0.1.1/README.md
--rw-r--r--   0        0        0     4456 2023-04-27 21:17:23.285179 srai-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      404 2023-04-27 21:17:06.212857 srai-0.1.1/srai/__init__.py
--rw-r--r--   0        0        0      155 2023-04-27 21:17:06.212857 srai-0.1.1/srai/constants.py
--rw-r--r--   0        0        0      755 2023-04-27 21:17:06.212857 srai-0.1.1/srai/embedders/__init__.py
--rw-r--r--   0        0        0     2722 2023-04-27 21:17:06.212857 srai-0.1.1/srai/embedders/_base.py
--rw-r--r--   0        0        0     8327 2023-04-27 21:17:06.212857 srai-0.1.1/srai/embedders/contextual_count_embedder.py
--rw-r--r--   0        0        0     4840 2023-04-27 21:17:06.212857 srai-0.1.1/srai/embedders/count_embedder.py
--rw-r--r--   0        0        0      136 2023-04-27 21:17:06.212857 srai-0.1.1/srai/embedders/gtfs2vec/__init__.py
--rw-r--r--   0        0        0     9413 2023-04-27 21:17:06.212857 srai-0.1.1/srai/embedders/gtfs2vec/embedder.py
--rw-r--r--   0        0        0     2369 2023-04-27 21:17:06.212857 srai-0.1.1/srai/embedders/gtfs2vec/model.py
--rw-r--r--   0        0        0      247 2023-04-27 21:17:06.212857 srai-0.1.1/srai/embedders/hex2vec/__init__.py
--rw-r--r--   0        0        0     8553 2023-04-27 21:17:06.212857 srai-0.1.1/srai/embedders/hex2vec/embedder.py
--rw-r--r--   0        0        0     6932 2023-04-27 21:17:06.212857 srai-0.1.1/srai/embedders/hex2vec/model.py
--rw-r--r--   0        0        0     6319 2023-04-27 21:17:06.212857 srai-0.1.1/srai/embedders/hex2vec/neighbour_dataset.py
--rw-r--r--   0        0        0      153 2023-04-27 21:17:06.212857 srai-0.1.1/srai/embedders/highway2vec/__init__.py
--rw-r--r--   0        0        0     6148 2023-04-27 21:17:06.212857 srai-0.1.1/srai/embedders/highway2vec/embedder.py
--rw-r--r--   0        0        0     2908 2023-04-27 21:17:06.212857 srai-0.1.1/srai/embedders/highway2vec/model.py
--rw-r--r--   0        0        0      580 2023-04-27 21:17:06.212857 srai-0.1.1/srai/exceptions.py
--rw-r--r--   0        0        0      531 2023-04-27 21:17:06.212857 srai-0.1.1/srai/joiners/__init__.py
--rw-r--r--   0        0        0      731 2023-04-27 21:17:06.212857 srai-0.1.1/srai/joiners/_base.py
--rw-r--r--   0        0        0     3836 2023-04-27 21:17:06.212857 srai-0.1.1/srai/joiners/intersection_joiner.py
--rw-r--r--   0        0        0      725 2023-04-27 21:17:06.212857 srai-0.1.1/srai/loaders/__init__.py
--rw-r--r--   0        0        0      591 2023-04-27 21:17:06.212857 srai-0.1.1/srai/loaders/_base.py
--rw-r--r--   0        0        0     2195 2023-04-27 21:17:06.212857 srai-0.1.1/srai/loaders/geoparquet_loader.py
--rw-r--r--   0        0        0     5371 2023-04-27 21:17:06.212857 srai-0.1.1/srai/loaders/gtfs_loader.py
--rw-r--r--   0        0        0      257 2023-04-27 21:17:06.212857 srai-0.1.1/srai/loaders/osm_loaders/__init__.py
--rw-r--r--   0        0        0     6424 2023-04-27 21:17:06.212857 srai-0.1.1/srai/loaders/osm_loaders/_base.py
--rw-r--r--   0        0        0      469 2023-04-27 21:17:06.212857 srai-0.1.1/srai/loaders/osm_loaders/filters/__init__.py
--rw-r--r--   0        0        0     2011 2023-04-27 21:17:06.212857 srai-0.1.1/srai/loaders/osm_loaders/filters/_typing.py
--rw-r--r--   0        0        0     5324 2023-04-27 21:17:06.212857 srai-0.1.1/srai/loaders/osm_loaders/filters/base_osm_groups.py
--rw-r--r--   0        0        0     8849 2023-04-27 21:17:06.212857 srai-0.1.1/srai/loaders/osm_loaders/filters/geofabrik.py
--rw-r--r--   0        0        0    15758 2023-04-27 21:17:06.212857 srai-0.1.1/srai/loaders/osm_loaders/filters/hex2vec.py
--rw-r--r--   0        0        0     2438 2023-04-27 21:17:06.212857 srai-0.1.1/srai/loaders/osm_loaders/filters/popular.py
--rw-r--r--   0        0        0     5536 2023-04-27 21:17:06.212857 srai-0.1.1/srai/loaders/osm_loaders/osm_online_loader.py
--rw-r--r--   0        0        0     5772 2023-04-27 21:17:06.212857 srai-0.1.1/srai/loaders/osm_loaders/osm_pbf_loader.py
--rw-r--r--   0        0        0     2777 2023-04-27 21:17:06.212857 srai-0.1.1/srai/loaders/osm_loaders/osm_tile_data_collector.py
--rw-r--r--   0        0        0     4691 2023-04-27 21:17:06.212857 srai-0.1.1/srai/loaders/osm_loaders/osm_tile_loader.py
--rw-r--r--   0        0        0    10106 2023-04-27 21:17:06.212857 srai-0.1.1/srai/loaders/osm_loaders/pbf_file_downloader.py
--rw-r--r--   0        0        0    10000 2023-04-27 21:17:06.212857 srai-0.1.1/srai/loaders/osm_loaders/pbf_file_handler.py
--rw-r--r--   0        0        0      118 2023-04-27 21:17:06.212857 srai-0.1.1/srai/loaders/osm_way_loader/__init__.py
--rw-r--r--   0        0        0     7587 2023-04-27 21:17:06.212857 srai-0.1.1/srai/loaders/osm_way_loader/constants.py
--rw-r--r--   0        0        0    13854 2023-04-27 21:17:06.212857 srai-0.1.1/srai/loaders/osm_way_loader/osm_way_loader.py
--rw-r--r--   0        0        0      465 2023-04-27 21:17:06.212857 srai-0.1.1/srai/neighbourhoods/__init__.py
--rw-r--r--   0        0        0     3679 2023-04-27 21:17:06.212857 srai-0.1.1/srai/neighbourhoods/_base.py
--rw-r--r--   0        0        0     2887 2023-04-27 21:17:06.212857 srai-0.1.1/srai/neighbourhoods/adjacency_neighbourhood.py
--rw-r--r--   0        0        0     3221 2023-04-27 21:17:06.212857 srai-0.1.1/srai/neighbourhoods/h3_neighbourhood.py
--rw-r--r--   0        0        0      496 2023-04-27 21:17:06.212857 srai-0.1.1/srai/plotting/__init__.py
--rw-r--r--   0        0        0    11189 2023-04-27 21:17:06.212857 srai-0.1.1/srai/plotting/folium_wrapper.py
--rw-r--r--   0        0        0    14174 2023-04-27 21:17:06.212857 srai-0.1.1/srai/plotting/plotly_wrapper.py
--rw-r--r--   0        0        0      894 2023-04-27 21:17:06.212857 srai-0.1.1/srai/regionizers/__init__.py
--rw-r--r--   0        0        0      945 2023-04-27 21:17:06.212857 srai-0.1.1/srai/regionizers/_base.py
--rw-r--r--   0        0        0    11462 2023-04-27 21:17:06.212857 srai-0.1.1/srai/regionizers/_spherical_voronoi.py
--rw-r--r--   0        0        0    15447 2023-04-27 21:17:06.212857 srai-0.1.1/srai/regionizers/administrative_boundary_regionizer.py
--rw-r--r--   0        0        0     6629 2023-04-27 21:17:06.212857 srai-0.1.1/srai/regionizers/h3_regionizer.py
--rw-r--r--   0        0        0     3118 2023-04-27 21:17:06.212857 srai-0.1.1/srai/regionizers/s2_regionizer.py
--rw-r--r--   0        0        0     4130 2023-04-27 21:17:06.212857 srai-0.1.1/srai/regionizers/slippy_map_regionizer.py
--rw-r--r--   0        0        0     5916 2023-04-27 21:17:06.212857 srai-0.1.1/srai/regionizers/voronoi_regionizer.py
--rw-r--r--   0        0        0      654 2023-04-27 21:17:06.212857 srai-0.1.1/srai/utils/__init__.py
--rw-r--r--   0        0        0     2910 2023-04-27 21:17:06.212857 srai-0.1.1/srai/utils/_optional.py
--rw-r--r--   0        0        0      239 2023-04-27 21:17:06.212857 srai-0.1.1/srai/utils/_pytorch_stubs.py
--rw-r--r--   0        0        0      999 2023-04-27 21:17:06.212857 srai-0.1.1/srai/utils/download.py
--rw-r--r--   0        0        0      944 2023-04-27 21:17:06.212857 srai-0.1.1/srai/utils/geocode.py
--rw-r--r--   0        0        0     2521 2023-04-27 21:17:06.212857 srai-0.1.1/srai/utils/geometry.py
--rw-r--r--   0        0        0     1153 2023-04-27 21:17:06.212857 srai-0.1.1/srai/utils/merge.py
--rw-r--r--   0        0        0      717 2023-04-27 21:17:06.212857 srai-0.1.1/srai/utils/typing.py
--rw-r--r--   0        0        0       29 2023-04-27 21:17:06.212857 srai-0.1.1/tests/__init__.py
--rw-r--r--   0        0        0     7806 2023-04-27 21:17:06.212857 srai-0.1.1/tests/embedders/conftest.py
--rw-r--r--   0        0        0      557 2023-04-27 21:17:06.212857 srai-0.1.1/tests/embedders/hex2vec/constants.py
--rw-r--r--   0        0        0     2590 2023-04-27 21:17:06.212857 srai-0.1.1/tests/embedders/hex2vec/generation.py
--rw-r--r--   0        0        0     2716 2023-04-27 21:17:06.212857 srai-0.1.1/tests/embedders/hex2vec/test_embedder.py
--rw-r--r--   0        0        0    97383 2023-04-27 21:17:06.216858 srai-0.1.1/tests/embedders/hex2vec/test_files/poz_8_features.parquet
--rw-r--r--   0        0        0   111218 2023-04-27 21:17:06.216858 srai-0.1.1/tests/embedders/hex2vec/test_files/poz_8_joint.parquet
--rw-r--r--   0        0        0    14226 2023-04-27 21:17:06.216858 srai-0.1.1/tests/embedders/hex2vec/test_files/poz_8_regions.parquet
--rw-r--r--   0        0        0    14498 2023-04-27 21:17:06.216858 srai-0.1.1/tests/embedders/hex2vec/test_files/poz_8_result.parquet
--rw-r--r--   0        0        0    89227 2023-04-27 21:17:06.216858 srai-0.1.1/tests/embedders/hex2vec/test_files/wro_9_features.parquet
--rw-r--r--   0        0        0    86944 2023-04-27 21:17:06.216858 srai-0.1.1/tests/embedders/hex2vec/test_files/wro_9_joint.parquet
--rw-r--r--   0        0        0    16794 2023-04-27 21:17:06.216858 srai-0.1.1/tests/embedders/hex2vec/test_files/wro_9_regions.parquet
--rw-r--r--   0        0        0    15781 2023-04-27 21:17:06.216858 srai-0.1.1/tests/embedders/hex2vec/test_files/wro_9_result.parquet
--rw-r--r--   0        0        0     1061 2023-04-27 21:17:06.216858 srai-0.1.1/tests/embedders/hex2vec/test_model.py
--rw-r--r--   0        0        0     3037 2023-04-27 21:17:06.216858 srai-0.1.1/tests/embedders/hex2vec/test_neighbour_dataset.py
--rw-r--r--   0        0        0    24053 2023-04-27 21:17:06.216858 srai-0.1.1/tests/embedders/test_contextual_count_embedder.py
--rw-r--r--   0        0        0     8273 2023-04-27 21:17:06.216858 srai-0.1.1/tests/embedders/test_count_embedder.py
--rw-r--r--   0        0        0     7091 2023-04-27 21:17:06.216858 srai-0.1.1/tests/embedders/test_gtfs2vec_embedder.py
--rw-r--r--   0        0        0     3630 2023-04-27 21:17:06.216858 srai-0.1.1/tests/embedders/test_highway2vec_embedder.py
--rw-r--r--   0        0        0     1765 2023-04-27 21:17:06.216858 srai-0.1.1/tests/joiners/conftest.py
--rw-r--r--   0        0        0     2529 2023-04-27 21:17:06.216858 srai-0.1.1/tests/joiners/test_intersection_joiner.py
--rw-r--r--   0        0        0     3001 2023-04-27 21:17:06.216858 srai-0.1.1/tests/loaders/conftest.py
--rw-r--r--   0        0        0     4284 2023-04-27 21:17:06.216858 srai-0.1.1/tests/loaders/osm_loaders/conftest.py
--rw-r--r--   0        0        0     4824 2023-04-27 21:17:06.216858 srai-0.1.1/tests/loaders/osm_loaders/filters/popular_filter_example.json
--rw-r--r--   0        0        0     3413 2023-04-27 21:17:06.216858 srai-0.1.1/tests/loaders/osm_loaders/filters/test_merge_filter_types.py
--rw-r--r--   0        0        0     3276 2023-04-27 21:17:06.216858 srai-0.1.1/tests/loaders/osm_loaders/filters/test_popular_tag_downloader.py
--rw-r--r--   0        0        0      342 2023-04-27 21:17:06.216858 srai-0.1.1/tests/loaders/osm_loaders/test_files/529cdcbb7a3cc103658ef31b39bed24984e421127d319c867edf2f86ff3bb098.osm.pbf
--rw-r--r--   0        0        0      100 2023-04-27 21:17:06.216858 srai-0.1.1/tests/loaders/osm_loaders/test_files/7a0163cb721992d6219d486b3d29517d06aa0db19dd7be049f4f1fabf6146073.osm.pbf
--rw-r--r--   0        0        0      770 2023-04-27 21:17:06.216858 srai-0.1.1/tests/loaders/osm_loaders/test_files/aa756ad3a961ba6d9da46c712b0d979d0c7d4768641ceea7409b287e2d18a48f.osm.pbf
--rw-r--r--   0        0        0    73746 2023-04-27 21:17:06.216858 srai-0.1.1/tests/loaders/osm_loaders/test_files/d17f922ed15e9609013a6b895e1e7af2d49158f03586f2c675d17b760af3452e.osm.pbf
--rw-r--r--   0        0        0     1013 2023-04-27 21:17:06.216858 srai-0.1.1/tests/loaders/osm_loaders/test_files/eb2848d259345ce7dfe8af34fd1ab24503bb0b952e04e872c87c55550fa50fbf.osm.pbf
--rw-r--r--   0        0        0   111539 2023-04-27 21:17:06.220857 srai-0.1.1/tests/loaders/osm_loaders/test_files/poland.geojson
--rw-r--r--   0        0        0   252620 2023-04-27 21:17:06.220857 srai-0.1.1/tests/loaders/osm_loaders/test_files/south_africa_without_islands.geojson
--rw-r--r--   0        0        0     2811 2023-04-27 21:17:06.220857 srai-0.1.1/tests/loaders/osm_loaders/test_osm_online_loader.py
--rw-r--r--   0        0        0     8690 2023-04-27 21:17:06.220857 srai-0.1.1/tests/loaders/osm_loaders/test_osm_pbf_loader.py
--rw-r--r--   0        0        0     3156 2023-04-27 21:17:06.220857 srai-0.1.1/tests/loaders/osm_loaders/test_osm_tile_data_collector.py
--rw-r--r--   0        0        0     3165 2023-04-27 21:17:06.220857 srai-0.1.1/tests/loaders/osm_loaders/test_osm_tile_loader.py
--rw-r--r--   0        0        0     3353 2023-04-27 21:17:06.220857 srai-0.1.1/tests/loaders/osm_way_loader/files/1f0fafc11b7ab7aea5124d2a89c634fc.pkl
--rw-r--r--   0        0        0     2804 2023-04-27 21:17:06.220857 srai-0.1.1/tests/loaders/osm_way_loader/files/20c9119c4dcc233c37382696f483239e.pkl
--rw-r--r--   0        0        0     3822 2023-04-27 21:17:06.220857 srai-0.1.1/tests/loaders/osm_way_loader/files/4310fe8d3c435f2a83fac55fc79f9166.pkl
--rw-r--r--   0        0        0     5109 2023-04-27 21:17:06.220857 srai-0.1.1/tests/loaders/osm_way_loader/files/7be5387a594790ea98ef0bd07bfcb58e.pkl
--rw-r--r--   0        0        0     3822 2023-04-27 21:17:06.220857 srai-0.1.1/tests/loaders/osm_way_loader/files/97e1befc51831ce8f8f482077f5042f2.pkl
--rw-r--r--   0        0        0      629 2023-04-27 21:17:06.220857 srai-0.1.1/tests/loaders/osm_way_loader/files/eebaa127015feec3e21491d4c32e4efe.pkl
--rw-r--r--   0        0        0    10789 2023-04-27 21:17:06.220857 srai-0.1.1/tests/loaders/osm_way_loader/test_osm_way_loader.py
--rw-r--r--   0        0        0    27801 2023-04-27 21:17:06.220857 srai-0.1.1/tests/loaders/test_files/example.parquet
--rw-r--r--   0        0        0     2181 2023-04-27 21:17:06.220857 srai-0.1.1/tests/loaders/test_geoparquet_loader.py
--rw-r--r--   0        0        0     3176 2023-04-27 21:17:06.220857 srai-0.1.1/tests/loaders/test_gtfs_loader.py
--rw-r--r--   0        0        0     4743 2023-04-27 21:17:06.220857 srai-0.1.1/tests/miscellaneous/test_optional_dependencies.py
--rw-r--r--   0        0        0     4028 2023-04-27 21:17:06.220857 srai-0.1.1/tests/neighbourhoods/h3/test_no_regions.py
--rw-r--r--   0        0        0     5668 2023-04-27 21:17:06.220857 srai-0.1.1/tests/neighbourhoods/h3/test_with_regions.py
--rw-r--r--   0        0        0     8063 2023-04-27 21:17:06.220857 srai-0.1.1/tests/neighbourhoods/test_adjacency_neighbourhood.py
--rw-r--r--   0        0        0     5586 2023-04-27 21:17:06.220857 srai-0.1.1/tests/neighbourhoods/test_neighbourhood.py
--rw-r--r--   0        0        0     3665 2023-04-27 21:17:06.220857 srai-0.1.1/tests/regionizers/conftest.py
--rw-r--r--   0        0        0     6469 2023-04-27 21:17:06.220857 srai-0.1.1/tests/regionizers/test_administrative_boundary_regionizer.py
--rw-r--r--   0        0        0     2198 2023-04-27 21:17:06.220857 srai-0.1.1/tests/regionizers/test_h3_regionizer.py
--rw-r--r--   0        0        0     1831 2023-04-27 21:17:06.220857 srai-0.1.1/tests/regionizers/test_s2_regionizer.py
--rw-r--r--   0        0        0     2651 2023-04-27 21:17:06.220857 srai-0.1.1/tests/regionizers/test_slippy_map_regionizer.py
--rw-r--r--   0        0        0     4957 2023-04-27 21:17:06.220857 srai-0.1.1/tests/regionizers/test_voronoi_regionizer.py
--rw-r--r--   0        0        0    17007 1970-01-01 00:00:00.000000 srai-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    10760 2023-06-22 17:29:25.324639 srai-0.1.4/LICENSE.md
+-rw-r--r--   0        0        0    16318 2023-06-22 17:29:25.324639 srai-0.1.4/README.md
+-rw-r--r--   0        0        0     4602 2023-06-22 17:29:50.605131 srai-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      404 2023-06-22 17:29:25.336639 srai-0.1.4/srai/__init__.py
+-rw-r--r--   0        0        0      155 2023-06-22 17:29:25.336639 srai-0.1.4/srai/constants.py
+-rw-r--r--   0        0        0      755 2023-06-22 17:29:25.336639 srai-0.1.4/srai/embedders/__init__.py
+-rw-r--r--   0        0        0     2722 2023-06-22 17:29:25.336639 srai-0.1.4/srai/embedders/_base.py
+-rw-r--r--   0        0        0     8327 2023-06-22 17:29:25.336639 srai-0.1.4/srai/embedders/contextual_count_embedder.py
+-rw-r--r--   0        0        0     4840 2023-06-22 17:29:25.336639 srai-0.1.4/srai/embedders/count_embedder.py
+-rw-r--r--   0        0        0      136 2023-06-22 17:29:25.336639 srai-0.1.4/srai/embedders/gtfs2vec/__init__.py
+-rw-r--r--   0        0        0     9413 2023-06-22 17:29:25.336639 srai-0.1.4/srai/embedders/gtfs2vec/embedder.py
+-rw-r--r--   0        0        0     2369 2023-06-22 17:29:25.336639 srai-0.1.4/srai/embedders/gtfs2vec/model.py
+-rw-r--r--   0        0        0      247 2023-06-22 17:29:25.336639 srai-0.1.4/srai/embedders/hex2vec/__init__.py
+-rw-r--r--   0        0        0     8553 2023-06-22 17:29:25.336639 srai-0.1.4/srai/embedders/hex2vec/embedder.py
+-rw-r--r--   0        0        0     6932 2023-06-22 17:29:25.336639 srai-0.1.4/srai/embedders/hex2vec/model.py
+-rw-r--r--   0        0        0     6319 2023-06-22 17:29:25.336639 srai-0.1.4/srai/embedders/hex2vec/neighbour_dataset.py
+-rw-r--r--   0        0        0      153 2023-06-22 17:29:25.336639 srai-0.1.4/srai/embedders/highway2vec/__init__.py
+-rw-r--r--   0        0        0     6148 2023-06-22 17:29:25.336639 srai-0.1.4/srai/embedders/highway2vec/embedder.py
+-rw-r--r--   0        0        0     2908 2023-06-22 17:29:25.336639 srai-0.1.4/srai/embedders/highway2vec/model.py
+-rw-r--r--   0        0        0      580 2023-06-22 17:29:25.336639 srai-0.1.4/srai/exceptions.py
+-rw-r--r--   0        0        0      531 2023-06-22 17:29:25.336639 srai-0.1.4/srai/joiners/__init__.py
+-rw-r--r--   0        0        0      731 2023-06-22 17:29:25.336639 srai-0.1.4/srai/joiners/_base.py
+-rw-r--r--   0        0        0     3836 2023-06-22 17:29:25.336639 srai-0.1.4/srai/joiners/intersection_joiner.py
+-rw-r--r--   0        0        0      725 2023-06-22 17:29:25.336639 srai-0.1.4/srai/loaders/__init__.py
+-rw-r--r--   0        0        0      591 2023-06-22 17:29:25.336639 srai-0.1.4/srai/loaders/_base.py
+-rw-r--r--   0        0        0     2195 2023-06-22 17:29:25.336639 srai-0.1.4/srai/loaders/geoparquet_loader.py
+-rw-r--r--   0        0        0     5371 2023-06-22 17:29:25.336639 srai-0.1.4/srai/loaders/gtfs_loader.py
+-rw-r--r--   0        0        0      257 2023-06-22 17:29:25.336639 srai-0.1.4/srai/loaders/osm_loaders/__init__.py
+-rw-r--r--   0        0        0     6424 2023-06-22 17:29:25.340639 srai-0.1.4/srai/loaders/osm_loaders/_base.py
+-rw-r--r--   0        0        0      469 2023-06-22 17:29:25.340639 srai-0.1.4/srai/loaders/osm_loaders/filters/__init__.py
+-rw-r--r--   0        0        0     2011 2023-06-22 17:29:25.340639 srai-0.1.4/srai/loaders/osm_loaders/filters/_typing.py
+-rw-r--r--   0        0        0     5324 2023-06-22 17:29:25.340639 srai-0.1.4/srai/loaders/osm_loaders/filters/base_osm_groups.py
+-rw-r--r--   0        0        0     8849 2023-06-22 17:29:25.340639 srai-0.1.4/srai/loaders/osm_loaders/filters/geofabrik.py
+-rw-r--r--   0        0        0    15758 2023-06-22 17:29:25.340639 srai-0.1.4/srai/loaders/osm_loaders/filters/hex2vec.py
+-rw-r--r--   0        0        0     2438 2023-06-22 17:29:25.340639 srai-0.1.4/srai/loaders/osm_loaders/filters/popular.py
+-rw-r--r--   0        0        0     5536 2023-06-22 17:29:25.340639 srai-0.1.4/srai/loaders/osm_loaders/osm_online_loader.py
+-rw-r--r--   0        0        0     5772 2023-06-22 17:29:25.340639 srai-0.1.4/srai/loaders/osm_loaders/osm_pbf_loader.py
+-rw-r--r--   0        0        0     2777 2023-06-22 17:29:25.340639 srai-0.1.4/srai/loaders/osm_loaders/osm_tile_data_collector.py
+-rw-r--r--   0        0        0     4703 2023-06-22 17:29:25.340639 srai-0.1.4/srai/loaders/osm_loaders/osm_tile_loader.py
+-rw-r--r--   0        0        0    10106 2023-06-22 17:29:25.340639 srai-0.1.4/srai/loaders/osm_loaders/pbf_file_downloader.py
+-rw-r--r--   0        0        0    11124 2023-06-22 17:29:25.340639 srai-0.1.4/srai/loaders/osm_loaders/pbf_file_handler.py
+-rw-r--r--   0        0        0      118 2023-06-22 17:29:25.340639 srai-0.1.4/srai/loaders/osm_way_loader/__init__.py
+-rw-r--r--   0        0        0     7587 2023-06-22 17:29:25.340639 srai-0.1.4/srai/loaders/osm_way_loader/constants.py
+-rw-r--r--   0        0        0    13854 2023-06-22 17:29:25.340639 srai-0.1.4/srai/loaders/osm_way_loader/osm_way_loader.py
+-rw-r--r--   0        0        0      467 2023-06-22 17:29:25.340639 srai-0.1.4/srai/neighbourhoods/__init__.py
+-rw-r--r--   0        0        0     3679 2023-06-22 17:29:25.340639 srai-0.1.4/srai/neighbourhoods/_base.py
+-rw-r--r--   0        0        0     2887 2023-06-22 17:29:25.340639 srai-0.1.4/srai/neighbourhoods/adjacency_neighbourhood.py
+-rw-r--r--   0        0        0     3221 2023-06-22 17:29:25.340639 srai-0.1.4/srai/neighbourhoods/h3_neighbourhood.py
+-rw-r--r--   0        0        0      496 2023-06-22 17:29:25.340639 srai-0.1.4/srai/plotting/__init__.py
+-rw-r--r--   0        0        0    11189 2023-06-22 17:29:25.340639 srai-0.1.4/srai/plotting/folium_wrapper.py
+-rw-r--r--   0        0        0    14174 2023-06-22 17:29:25.340639 srai-0.1.4/srai/plotting/plotly_wrapper.py
+-rw-r--r--   0        0        0      934 2023-06-22 17:29:25.340639 srai-0.1.4/srai/regionalizers/__init__.py
+-rw-r--r--   0        0        0      957 2023-06-22 17:29:25.340639 srai-0.1.4/srai/regionalizers/_base.py
+-rw-r--r--   0        0        0    11462 2023-06-22 17:29:25.340639 srai-0.1.4/srai/regionalizers/_spherical_voronoi.py
+-rw-r--r--   0        0        0    15475 2023-06-22 17:29:25.340639 srai-0.1.4/srai/regionalizers/administrative_boundary_regionalizer.py
+-rw-r--r--   0        0        0     6651 2023-06-22 17:29:25.340639 srai-0.1.4/srai/regionalizers/h3_regionalizer.py
+-rw-r--r--   0        0        0     3142 2023-06-22 17:29:25.340639 srai-0.1.4/srai/regionalizers/s2_regionalizer.py
+-rw-r--r--   0        0        0     4163 2023-06-22 17:29:25.340639 srai-0.1.4/srai/regionalizers/slippy_map_regionalizer.py
+-rw-r--r--   0        0        0     5940 2023-06-22 17:29:25.340639 srai-0.1.4/srai/regionalizers/voronoi_regionalizer.py
+-rw-r--r--   0        0        0      654 2023-06-22 17:29:25.340639 srai-0.1.4/srai/utils/__init__.py
+-rw-r--r--   0        0        0     2910 2023-06-22 17:29:25.340639 srai-0.1.4/srai/utils/_optional.py
+-rw-r--r--   0        0        0      239 2023-06-22 17:29:25.340639 srai-0.1.4/srai/utils/_pytorch_stubs.py
+-rw-r--r--   0        0        0      999 2023-06-22 17:29:25.340639 srai-0.1.4/srai/utils/download.py
+-rw-r--r--   0        0        0      944 2023-06-22 17:29:25.340639 srai-0.1.4/srai/utils/geocode.py
+-rw-r--r--   0        0        0     2521 2023-06-22 17:29:25.340639 srai-0.1.4/srai/utils/geometry.py
+-rw-r--r--   0        0        0     1153 2023-06-22 17:29:25.340639 srai-0.1.4/srai/utils/merge.py
+-rw-r--r--   0        0        0      717 2023-06-22 17:29:25.340639 srai-0.1.4/srai/utils/typing.py
+-rw-r--r--   0        0        0       29 2023-06-22 17:29:25.340639 srai-0.1.4/tests/__init__.py
+-rw-r--r--   0        0        0     7806 2023-06-22 17:29:25.340639 srai-0.1.4/tests/embedders/conftest.py
+-rw-r--r--   0        0        0      534 2023-06-22 17:29:25.340639 srai-0.1.4/tests/embedders/hex2vec/constants.py
+-rw-r--r--   0        0        0     2600 2023-06-22 17:29:25.340639 srai-0.1.4/tests/embedders/hex2vec/generation.py
+-rw-r--r--   0        0        0     2716 2023-06-22 17:29:25.340639 srai-0.1.4/tests/embedders/hex2vec/test_embedder.py
+-rw-r--r--   0        0        0    97383 2023-06-22 17:29:25.340639 srai-0.1.4/tests/embedders/hex2vec/test_files/poz_8_features.parquet
+-rw-r--r--   0        0        0   111218 2023-06-22 17:29:25.340639 srai-0.1.4/tests/embedders/hex2vec/test_files/poz_8_joint.parquet
+-rw-r--r--   0        0        0    14226 2023-06-22 17:29:25.340639 srai-0.1.4/tests/embedders/hex2vec/test_files/poz_8_regions.parquet
+-rw-r--r--   0        0        0    14498 2023-06-22 17:29:25.340639 srai-0.1.4/tests/embedders/hex2vec/test_files/poz_8_result.parquet
+-rw-r--r--   0        0        0    89227 2023-06-22 17:29:25.344639 srai-0.1.4/tests/embedders/hex2vec/test_files/wro_9_features.parquet
+-rw-r--r--   0        0        0    86944 2023-06-22 17:29:25.344639 srai-0.1.4/tests/embedders/hex2vec/test_files/wro_9_joint.parquet
+-rw-r--r--   0        0        0    16794 2023-06-22 17:29:25.344639 srai-0.1.4/tests/embedders/hex2vec/test_files/wro_9_regions.parquet
+-rw-r--r--   0        0        0    15781 2023-06-22 17:29:25.344639 srai-0.1.4/tests/embedders/hex2vec/test_files/wro_9_result.parquet
+-rw-r--r--   0        0        0     1061 2023-06-22 17:29:25.344639 srai-0.1.4/tests/embedders/hex2vec/test_model.py
+-rw-r--r--   0        0        0     3037 2023-06-22 17:29:25.344639 srai-0.1.4/tests/embedders/hex2vec/test_neighbour_dataset.py
+-rw-r--r--   0        0        0    24053 2023-06-22 17:29:25.344639 srai-0.1.4/tests/embedders/test_contextual_count_embedder.py
+-rw-r--r--   0        0        0     8273 2023-06-22 17:29:25.344639 srai-0.1.4/tests/embedders/test_count_embedder.py
+-rw-r--r--   0        0        0     7091 2023-06-22 17:29:25.344639 srai-0.1.4/tests/embedders/test_gtfs2vec_embedder.py
+-rw-r--r--   0        0        0     3630 2023-06-22 17:29:25.344639 srai-0.1.4/tests/embedders/test_highway2vec_embedder.py
+-rw-r--r--   0        0        0     1765 2023-06-22 17:29:25.344639 srai-0.1.4/tests/joiners/conftest.py
+-rw-r--r--   0        0        0     2529 2023-06-22 17:29:25.344639 srai-0.1.4/tests/joiners/test_intersection_joiner.py
+-rw-r--r--   0        0        0     3001 2023-06-22 17:29:25.344639 srai-0.1.4/tests/loaders/conftest.py
+-rw-r--r--   0        0        0     4284 2023-06-22 17:29:25.344639 srai-0.1.4/tests/loaders/osm_loaders/conftest.py
+-rw-r--r--   0        0        0     4824 2023-06-22 17:29:25.344639 srai-0.1.4/tests/loaders/osm_loaders/filters/popular_filter_example.json
+-rw-r--r--   0        0        0     3413 2023-06-22 17:29:25.344639 srai-0.1.4/tests/loaders/osm_loaders/filters/test_merge_filter_types.py
+-rw-r--r--   0        0        0     3276 2023-06-22 17:29:25.344639 srai-0.1.4/tests/loaders/osm_loaders/filters/test_popular_tag_downloader.py
+-rw-r--r--   0        0        0      342 2023-06-22 17:29:25.344639 srai-0.1.4/tests/loaders/osm_loaders/test_files/529cdcbb7a3cc103658ef31b39bed24984e421127d319c867edf2f86ff3bb098.osm.pbf
+-rw-r--r--   0        0        0      100 2023-06-22 17:29:25.344639 srai-0.1.4/tests/loaders/osm_loaders/test_files/7a0163cb721992d6219d486b3d29517d06aa0db19dd7be049f4f1fabf6146073.osm.pbf
+-rw-r--r--   0        0        0      770 2023-06-22 17:29:25.344639 srai-0.1.4/tests/loaders/osm_loaders/test_files/aa756ad3a961ba6d9da46c712b0d979d0c7d4768641ceea7409b287e2d18a48f.osm.pbf
+-rw-r--r--   0        0        0    73746 2023-06-22 17:29:25.344639 srai-0.1.4/tests/loaders/osm_loaders/test_files/d17f922ed15e9609013a6b895e1e7af2d49158f03586f2c675d17b760af3452e.osm.pbf
+-rw-r--r--   0        0        0     1013 2023-06-22 17:29:25.344639 srai-0.1.4/tests/loaders/osm_loaders/test_files/eb2848d259345ce7dfe8af34fd1ab24503bb0b952e04e872c87c55550fa50fbf.osm.pbf
+-rw-r--r--   0        0        0   111539 2023-06-22 17:29:25.344639 srai-0.1.4/tests/loaders/osm_loaders/test_files/poland.geojson
+-rw-r--r--   0        0        0   252620 2023-06-22 17:29:25.344639 srai-0.1.4/tests/loaders/osm_loaders/test_files/south_africa_without_islands.geojson
+-rw-r--r--   0        0        0     2811 2023-06-22 17:29:25.344639 srai-0.1.4/tests/loaders/osm_loaders/test_osm_online_loader.py
+-rw-r--r--   0        0        0     8690 2023-06-22 17:29:25.344639 srai-0.1.4/tests/loaders/osm_loaders/test_osm_pbf_loader.py
+-rw-r--r--   0        0        0     3156 2023-06-22 17:29:25.344639 srai-0.1.4/tests/loaders/osm_loaders/test_osm_tile_data_collector.py
+-rw-r--r--   0        0        0     3165 2023-06-22 17:29:25.344639 srai-0.1.4/tests/loaders/osm_loaders/test_osm_tile_loader.py
+-rw-r--r--   0        0        0     3353 2023-06-22 17:29:25.348639 srai-0.1.4/tests/loaders/osm_way_loader/files/1f0fafc11b7ab7aea5124d2a89c634fc.pkl
+-rw-r--r--   0        0        0     2804 2023-06-22 17:29:25.348639 srai-0.1.4/tests/loaders/osm_way_loader/files/20c9119c4dcc233c37382696f483239e.pkl
+-rw-r--r--   0        0        0     3822 2023-06-22 17:29:25.348639 srai-0.1.4/tests/loaders/osm_way_loader/files/4310fe8d3c435f2a83fac55fc79f9166.pkl
+-rw-r--r--   0        0        0     5109 2023-06-22 17:29:25.348639 srai-0.1.4/tests/loaders/osm_way_loader/files/7be5387a594790ea98ef0bd07bfcb58e.pkl
+-rw-r--r--   0        0        0     3822 2023-06-22 17:29:25.348639 srai-0.1.4/tests/loaders/osm_way_loader/files/97e1befc51831ce8f8f482077f5042f2.pkl
+-rw-r--r--   0        0        0      629 2023-06-22 17:29:25.348639 srai-0.1.4/tests/loaders/osm_way_loader/files/eebaa127015feec3e21491d4c32e4efe.pkl
+-rw-r--r--   0        0        0    10789 2023-06-22 17:29:25.348639 srai-0.1.4/tests/loaders/osm_way_loader/test_osm_way_loader.py
+-rw-r--r--   0        0        0    27801 2023-06-22 17:29:25.348639 srai-0.1.4/tests/loaders/test_files/example.parquet
+-rw-r--r--   0        0        0     2181 2023-06-22 17:29:25.348639 srai-0.1.4/tests/loaders/test_geoparquet_loader.py
+-rw-r--r--   0        0        0     3176 2023-06-22 17:29:25.348639 srai-0.1.4/tests/loaders/test_gtfs_loader.py
+-rw-r--r--   0        0        0     4755 2023-06-22 17:29:25.348639 srai-0.1.4/tests/miscellaneous/test_optional_dependencies.py
+-rw-r--r--   0        0        0     4028 2023-06-22 17:29:25.348639 srai-0.1.4/tests/neighbourhoods/h3/test_no_regions.py
+-rw-r--r--   0        0        0     5668 2023-06-22 17:29:25.348639 srai-0.1.4/tests/neighbourhoods/h3/test_with_regions.py
+-rw-r--r--   0        0        0     8063 2023-06-22 17:29:25.348639 srai-0.1.4/tests/neighbourhoods/test_adjacency_neighbourhood.py
+-rw-r--r--   0        0        0     5586 2023-06-22 17:29:25.348639 srai-0.1.4/tests/neighbourhoods/test_neighbourhood.py
+-rw-r--r--   0        0        0     3667 2023-06-22 17:29:25.348639 srai-0.1.4/tests/regionalizers/conftest.py
+-rw-r--r--   0        0        0     6505 2023-06-22 17:29:25.348639 srai-0.1.4/tests/regionalizers/test_administrative_boundary_regionalizer.py
+-rw-r--r--   0        0        0     2208 2023-06-22 17:29:25.348639 srai-0.1.4/tests/regionalizers/test_h3_regionalizer.py
+-rw-r--r--   0        0        0     1841 2023-06-22 17:29:25.348639 srai-0.1.4/tests/regionalizers/test_s2_regionalizer.py
+-rw-r--r--   0        0        0     2689 2023-06-22 17:29:25.348639 srai-0.1.4/tests/regionalizers/test_slippy_map_regionalizer.py
+-rw-r--r--   0        0        0     4983 2023-06-22 17:29:25.348639 srai-0.1.4/tests/regionalizers/test_voronoi_regionalizer.py
+-rw-r--r--   0        0        0    18478 1970-01-01 00:00:00.000000 srai-0.1.4/PKG-INFO
```

### Comparing `srai-0.1.1/LICENSE.md` & `srai-0.1.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `srai-0.1.1/README.md` & `srai-0.1.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -26,35 +26,45 @@
     </a>
 </p>
 
 # Spatial Representations for Artificial Intelligence
 
 <p align="center">⚠️🚧 This library is under HEAVY development. Expect breaking changes between <i>minor</i> versions 🚧⚠️</p>
 
-<p align="center">💬 Feel free to open an issue if you find anything confusing or not working 🗨️</p>
+<p align="center">💬 Feel free to open an issue if you find anything confusing or not working 💬</p>
 
-Project **Spatial Representations for Artificial Intelligence** (`srai`) aims to provide simple and efficient solutions to geospatial problems that are accessible to everybody and reusable in various contexts where geospatial data can be used. It is a Python module integrating many geo-related algorithms in a single package with unified API. Please see getting starded for installation and quick srart instructions.
+Project **Spatial Representations for Artificial Intelligence** (`srai`) aims to provide simple and efficient solutions to geospatial problems that are accessible to everybody and reusable in various contexts where geospatial data can be used. It is a Python module integrating many geo-related algorithms in a single package with unified API. Please see getting started for installation and quick start instructions.
+
+<p align="center">
+  <img src="https://drive.google.com/uc?export=view&id=1iyajkX81PLrel-Xmz1lQpYQvePnLoO1U"  style="max-width:600px;width:100%"/>
+</p>
 
 ## Use cases
 
 In the current state, `srai` provides the following functionalities:
 
 * **OSM data download** - downloading OpenStreetMap data for a given area using different sources
 * **OSM data processing** - processing OSM data to extract useful information (e.g. road network, buildings, POIs, etc.)
 * **GTFS processing** - extracting features from GTFS data
-* **Regionization** - splitting a given area into smaller regions using different algorithms (e.g. Uber's H3[1], Voronoi, etc.)
+* **Regionalization** - splitting a given area into smaller regions using different algorithms (e.g. Uber's H3[1], Voronoi, etc.)
 * **Embedding** - embedding regions into a vector space based on different spatial features, and using different algorithms (eg. hex2vec[2], etc.)
 * Utilities for spatial data visualization and processing
 
 For future releases, we plan to add more functionalities, such as:
 
 * **Pre-computed embeddings** - pre-computed embeddings for different regions and different embedding algorithms
 * **Full pipelines** - full pipelines for different embedding approaches, pre-configured from `srai` components
 * **Image data download and processing** - downloading and processing image data (eg. OSM tiles, etc.)
 
+### End-to-end examples
+
+Right now, `srai` provides a toolset for data download and processing sufficient to solve downstream tasks. Please see [this project](https://pwr-inf.github.io/Transfer-learning-approach-to-bicycle-sharing-systems-station-location-planning-using-OpenStreetMap/) by [@RaczeQ](https://github.com/RaczeQ), which predicts Bike Sharing System (BSS) stations' locations for a wide range of cities worldwide.
+
+For `srai` integration into full [kedro](https://kedro.org/) pipeline, see [this project](https://github.com/Calychas/highway2vec_remaster/) by [@Calychas](https://github.com/Calychas).
+
 ## Installation
 
 To install `srai` simply run:
 
 ```bash
 pip install srai
 ```
@@ -63,21 +73,23 @@
 
 ### Optional dependencies
 
 The following optional dependencies can be installed to enable additional functionality:
 
 * `srai[all]` - all optional dependencies
 * `srai[osm]` - dependencies required to download OpenStreetMap data
-* `srai[voronoi]` - dependencies to use Voronoi-based regionization method
+* `srai[voronoi]` - dependencies to use Voronoi-based regionalization method
 * `srai[gtfs]` - dependencies to process GTFS data
 * `srai[plotting]` - dependencies to plot graphs and maps
 * `srai[torch]` - dependencies to use torch-based embedders
 
 ## Usage
 
+If you prefer an interactive notebook, examples of `srai` usage are available in this [Colab Notebook](https://colab.research.google.com/drive/17z2OYZG82FZNRK86Kt-eSgbJn9m7meSH?usp=sharing)
+
 ### Downloading OSM data
 
 To download OSM data for a given area, using a set of tags use one of `OSMLoader` classes:
 
 * `OSMOnlineLoader` - downloads data from OpenStreetMap API using [osmnx](https://github.com/gboeing/osmnx) - this is faster for smaller areas or tags counts
 * `OSMPbfLoader` - loads data from automatically downloaded PBF file from [protomaps](https://protomaps.com/) - this is faster for larger areas or tags counts
 
@@ -146,70 +158,70 @@
 features[["trips_at_8", "geometry"]].explore("trips_at_8", m=folium_map)
 ```
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/srai-lab/srai/main/docs/assets/images/downloading_gtfs_data.jpg" style="max-width:600px;width:100%"/>
 </p>
 
-### Regionization
+### Regionalization
 
-Regionization is a process of dividing a given area into smaller regions. This can be done in a variety of ways:
+Regionalization is a process of dividing a given area into smaller regions. This can be done in a variety of ways:
 
-* `H3Regionizer` - regionization using [Uber's H3 library](https://github.com/uber/h3)
-* `S2Regionizer` - regionization using [Google's S2 library](https://github.com/google/s2geometry)
-* `VoronoiRegionizer` - regionization using Voronoi diagram
-* `AdministativeBoundaryRegionizer` - regionization using administrative boundaries
+* `H3Regionalizer` - regionalization using [Uber's H3 library](https://github.com/uber/h3)
+* `S2Regionalizer` - regionalization using [Google's S2 library](https://github.com/google/s2geometry)
+* `VoronoiRegionalizer` - regionalization using Voronoi diagram
+* `AdministativeBoundaryRegionalizer` - regionalization using administrative boundaries
 
 Example:
 
 ```python
-from srai.regionizers import H3Regionizer
+from srai.regionalizers import H3Regionalizer
 from srai.utils import geocode_to_region_gdf
 
 area = geocode_to_region_gdf("Berlin, Germany")
-regionizer = H3Regionizer(resolution=7)
+regionalizer = H3Regionalizer(resolution=7)
 
-regions = regionizer.transform(area)
+regions = regionalizer.transform(area)
 
 folium_map = plot_regions(area, colormap=["rgba(0,0,0,0.1)"], tiles_style="CartoDB positron")
 plot_regions(regions_gdf=regions, map=folium_map)
 ```
 
 <p align="center">
-  <img src="https://raw.githubusercontent.com/srai-lab/srai/main/docs/assets/images/regionization.jpg" style="max-width:600px;width:100%"/>
+  <img src="https://raw.githubusercontent.com/srai-lab/srai/main/docs/assets/images/regionalization.jpg" style="max-width:600px;width:100%"/>
 </p>
 
 ### Embedding
 
 Embedding is a process of mapping regions into a vector space. This can be done in a variety of ways:
 
 * `Hex2VecEmbedder` - embedding using hex2vec[1] algorithm
 * `GTFS2VecEmbedder` - embedding using GTFS2Vec[2] algorithm
 * `CountEmbedder` - embedding based on features counts
 * `ContextualCountEmbedder` - embedding based on features counts with neighbourhood context (proposed in [3])
 * `Highway2VecEmbedder` - embedding using Highway2Vec[4] algorithm
 
-All of those methods share the same API. All of them require results from `Loader` (load features), `Regionizer` (split area into regions) and `Joiner` (join features to regions) to work. An example using `CountEmbedder`:
+All of those methods share the same API. All of them require results from `Loader` (load features), `Regionalizer` (split area into regions) and `Joiner` (join features to regions) to work. An example using `CountEmbedder`:
 
 ```python
 from srai.embedders import CountEmbedder
 from srai.joiners import IntersectionJoiner
 from srai.loaders import OSMOnlineLoader
 from srai.plotting import plot_regions, plot_numeric_data
-from srai.regionizers import H3Regionizer
+from srai.regionalizers import H3Regionalizer
 from srai.utils import geocode_to_region_gdf
 
 loader = OSMOnlineLoader()
-regionizer = H3Regionizer(resolution=9)
+regionalizer = H3Regionalizer(resolution=9)
 joiner = IntersectionJoiner()
 
 query = {"amenity": "bicycle_parking"}
 area = geocode_to_region_gdf("Malmö, Sweden")
 features = loader.load(area, query)
-regions = regionizer.transform(area)
+regions = regionalizer.transform(area)
 joint = joiner.transform(regions, features)
 
 embedder = CountEmbedder()
 embeddings = embedder.transform(regions, features, joint)
 
 folium_map = plot_regions(area, colormap=["rgba(0,0,0,0.1)"], tiles_style="CartoDB positron")
 plot_numeric_data(regions, embeddings, "amenity_bicycle_parking", map=folium_map)
@@ -223,25 +235,25 @@
 
 ```python
 from srai.embedders import Hex2VecEmbedder
 from srai.joiners import IntersectionJoiner
 from srai.loaders import OSMPbfLoader
 from srai.loaders.osm_loaders.filters import HEX2VEC_FILTER
 from srai.neighbourhoods.h3_neighbourhood import H3Neighbourhood
-from srai.regionizers import H3Regionizer
+from srai.regionalizers import H3Regionalizer
 from srai.utils import geocode_to_region_gdf
 from srai.plotting import plot_regions, plot_numeric_data
 
 loader = OSMPbfLoader()
-regionizer = H3Regionizer(resolution=11)
+regionalizer = H3Regionalizer(resolution=11)
 joiner = IntersectionJoiner()
 
 area = geocode_to_region_gdf("City of London")
 features = loader.load(area, HEX2VEC_FILTER)
-regions = regionizer.transform(area)
+regions = regionalizer.transform(area)
 joint = joiner.transform(regions, features)
 
 embedder = Hex2VecEmbedder()
 neighbourhood = H3Neighbourhood(regions_gdf=regions)
 
 embedder = Hex2VecEmbedder([15, 10, 3])
 
@@ -271,18 +283,22 @@
 ## Publications
 
 Some of the methods implemented in `srai` have been published in scientific journals and conferences.
 
 1. Szymon Woźniak and Piotr Szymański. 2021. Hex2vec: Context-Aware Embedding H3 Hexagons with OpenStreetMap Tags. In Proceedings of the 4th ACM SIGSPATIAL International Workshop on AI for Geographic Knowledge Discovery (GEOAI '21). Association for Computing Machinery, New York, NY, USA, 61–71. [paper](https://doi.org/10.1145/3486635.3491076), [arXiv](https://arxiv.org/abs/2111.00970)
 2. Piotr Gramacki, Szymon Woźniak, and Piotr Szymański. 2021. Gtfs2vec: Learning GTFS Embeddings for comparing Public Transport Offer in Microregions. In Proceedings of the 1st ACM SIGSPATIAL International Workshop on Searching and Mining Large Collections of Geospatial Data (GeoSearch'21). Association for Computing Machinery, New York, NY, USA, 5–12. [paper](https://doi.org/10.1145/3486640.3491392), [arXiv](https://arxiv.org/abs/2111.00960)
 3. Kamil Raczycki and Piotr Szymański. 2021. Transfer learning approach to bicycle-sharing systems' station location planning using OpenStreetMap data. In Proceedings of the 4th ACM SIGSPATIAL International Workshop on Advances in Resilient and Intelligent Cities (ARIC '21). Association for Computing Machinery, New York, NY, USA, 1–12. [paper](https://doi.org/10.1145/3486626.3493434), [arXiv](https://arxiv.org/abs/2111.00990)
-4. Kacper Leśniara and Piotr Szymański. 2022. Highway2vec: representing OpenStreetMap microregions with respect to their road network characteristics. In Proceedings of the 5th ACM SIGSPATIAL International Workshop on AI for Geographic Knowledge Discovery (GeoAI '22). Association for Computing Machinery, New York, NY, USA, 18–29. [paper](https://doi.org/10.1145/3557918.3565865)
+4. Kacper Leśniara and Piotr Szymański. 2022. Highway2vec: representing OpenStreetMap microregions with respect to their road network characteristics. In Proceedings of the 5th ACM SIGSPATIAL International Workshop on AI for Geographic Knowledge Discovery (GeoAI '22). Association for Computing Machinery, New York, NY, USA, 18–29. [paper](https://doi.org/10.1145/3557918.3565865), [arXiv](https://arxiv.org/abs/2304.13865)
+
+## Acknowledgements
+
+We would like to thank Piotr Szymański PhD \([@niedakh](https://twitter.com/niedakh)\) for his invaluable guidance and support in the development of this library. His expertise and mentorship have been instrumental in shaping the library's design and functionality, and we are very grateful for his input.
 
 ## Citation
 
 TBD
 
 ## License
 
-This library is licensed under the [Apache Licence 2.0](https://github.com/srai-lab/srai/blob/main/LICENSE.md).
+This library is licensed under the [Apache License 2.0](https://github.com/srai-lab/srai/blob/main/LICENSE.md).
 
 The free [OpenStreetMap](https://www.openstreetmap.org/) data, which is used for the development of SRAI, is licensed under the [Open Data Commons Open Database License](https://opendatacommons.org/licenses/odbl/) (ODbL) by the [OpenStreetMap Foundation](https://osmfoundation.org/) (OSMF).
```

#### html2text {}

```diff
@@ -3,46 +3,58 @@
   [GitHub] [Checks] [GitHub_Workflow_Status_-_DEV] [GitHub_Workflow_Status_-
  PROD] [pre-commit.ci_status] [CodeFactor_Grade] [Codecov] [Package_version]
                 [Supported_Python_versions] [PyPI_-_Downloads]
 # Spatial Representations for Artificial Intelligence
   â ï¸ð§ This library is under HEAVY development. Expect breaking changes
                        between minor versions ð§â ï¸
  ð¬ Feel free to open an issue if you find anything confusing or not working
-                                    ð¨ï¸
+                                     ð¬
 Project **Spatial Representations for Artificial Intelligence** (`srai`) aims
 to provide simple and efficient solutions to geospatial problems that are
 accessible to everybody and reusable in various contexts where geospatial data
 can be used. It is a Python module integrating many geo-related algorithms in a
-single package with unified API. Please see getting starded for installation
-and quick srart instructions. ## Use cases In the current state, `srai`
-provides the following functionalities: * **OSM data download** - downloading
-OpenStreetMap data for a given area using different sources * **OSM data
-processing** - processing OSM data to extract useful information (e.g. road
-network, buildings, POIs, etc.) * **GTFS processing** - extracting features
-from GTFS data * **Regionization** - splitting a given area into smaller
-regions using different algorithms (e.g. Uber's H3[1], Voronoi, etc.) *
-**Embedding** - embedding regions into a vector space based on different
-spatial features, and using different algorithms (eg. hex2vec[2], etc.) *
-Utilities for spatial data visualization and processing For future releases, we
-plan to add more functionalities, such as: * **Pre-computed embeddings** - pre-
-computed embeddings for different regions and different embedding algorithms *
-**Full pipelines** - full pipelines for different embedding approaches, pre-
-configured from `srai` components * **Image data download and processing** -
-downloading and processing image data (eg. OSM tiles, etc.) ## Installation To
-install `srai` simply run: ```bash pip install srai ``` This will install the
-`srai` package and dependencies required by most of the use cases. There are
-several optional dependencies that can be installed to enable additional
-functionality. These are listed in the [optional dependencies](#optional-
-dependencies) section. ### Optional dependencies The following optional
-dependencies can be installed to enable additional functionality: * `srai[all]`
-- all optional dependencies * `srai[osm]` - dependencies required to download
-OpenStreetMap data * `srai[voronoi]` - dependencies to use Voronoi-based
-regionization method * `srai[gtfs]` - dependencies to process GTFS data * `srai
-[plotting]` - dependencies to plot graphs and maps * `srai[torch]` -
-dependencies to use torch-based embedders ## Usage ### Downloading OSM data To
+single package with unified API. Please see getting started for installation
+and quick start instructions.
+[https://drive.google.com/uc?export=view&id=1iyajkX81PLrel-Xmz1lQpYQvePnLoO1U]
+## Use cases In the current state, `srai` provides the following
+functionalities: * **OSM data download** - downloading OpenStreetMap data for a
+given area using different sources * **OSM data processing** - processing OSM
+data to extract useful information (e.g. road network, buildings, POIs, etc.) *
+**GTFS processing** - extracting features from GTFS data * **Regionalization**
+- splitting a given area into smaller regions using different algorithms (e.g.
+Uber's H3[1], Voronoi, etc.) * **Embedding** - embedding regions into a vector
+space based on different spatial features, and using different algorithms (eg.
+hex2vec[2], etc.) * Utilities for spatial data visualization and processing For
+future releases, we plan to add more functionalities, such as: * **Pre-computed
+embeddings** - pre-computed embeddings for different regions and different
+embedding algorithms * **Full pipelines** - full pipelines for different
+embedding approaches, pre-configured from `srai` components * **Image data
+download and processing** - downloading and processing image data (eg. OSM
+tiles, etc.) ### End-to-end examples Right now, `srai` provides a toolset for
+data download and processing sufficient to solve downstream tasks. Please see
+[this project](https://pwr-inf.github.io/Transfer-learning-approach-to-bicycle-
+sharing-systems-station-location-planning-using-OpenStreetMap/) by [@RaczeQ]
+(https://github.com/RaczeQ), which predicts Bike Sharing System (BSS) stations'
+locations for a wide range of cities worldwide. For `srai` integration into
+full [kedro](https://kedro.org/) pipeline, see [this project](https://
+github.com/Calychas/highway2vec_remaster/) by [@Calychas](https://github.com/
+Calychas). ## Installation To install `srai` simply run: ```bash pip install
+srai ``` This will install the `srai` package and dependencies required by most
+of the use cases. There are several optional dependencies that can be installed
+to enable additional functionality. These are listed in the [optional
+dependencies](#optional-dependencies) section. ### Optional dependencies The
+following optional dependencies can be installed to enable additional
+functionality: * `srai[all]` - all optional dependencies * `srai[osm]` -
+dependencies required to download OpenStreetMap data * `srai[voronoi]` -
+dependencies to use Voronoi-based regionalization method * `srai[gtfs]` -
+dependencies to process GTFS data * `srai[plotting]` - dependencies to plot
+graphs and maps * `srai[torch]` - dependencies to use torch-based embedders ##
+Usage If you prefer an interactive notebook, examples of `srai` usage are
+available in this [Colab Notebook](https://colab.research.google.com/drive/
+17z2OYZG82FZNRK86Kt-eSgbJn9m7meSH?usp=sharing) ### Downloading OSM data To
 download OSM data for a given area, using a set of tags use one of `OSMLoader`
 classes: * `OSMOnlineLoader` - downloads data from OpenStreetMap API using
 [osmnx](https://github.com/gboeing/osmnx) - this is faster for smaller areas or
 tags counts * `OSMPbfLoader` - loads data from automatically downloaded PBF
 file from [protomaps](https://protomaps.com/) - this is faster for larger areas
 or tags counts Example with `OSMOnlineLoader`: ```python from srai.loaders
 import OSMOnlineLoader from srai.utils import geocode_to_region_gdf from
@@ -72,71 +84,72 @@
 Path("vienna_gtfs.zip") download_file("https://transitfeeds.com/p/stadt-wien/
 888/latest/download", gtfs_file.as_posix()) loader = GTFSLoader() features =
 loader.load(gtfs_file) folium_map = plot_regions(area, colormap=["rgba
 (0,0,0,0.1)"], tiles_style="CartoDB positron") features[["trips_at_8",
 "geometry"]].explore("trips_at_8", m=folium_map) ```
    [https://raw.githubusercontent.com/srai-lab/srai/main/docs/assets/images/
                           downloading_gtfs_data.jpg]
-### Regionization Regionization is a process of dividing a given area into
-smaller regions. This can be done in a variety of ways: * `H3Regionizer` -
-regionization using [Uber's H3 library](https://github.com/uber/h3) *
-`S2Regionizer` - regionization using [Google's S2 library](https://github.com/
-google/s2geometry) * `VoronoiRegionizer` - regionization using Voronoi diagram
-* `AdministativeBoundaryRegionizer` - regionization using administrative
-boundaries Example: ```python from srai.regionizers import H3Regionizer from
-srai.utils import geocode_to_region_gdf area = geocode_to_region_gdf("Berlin,
-Germany") regionizer = H3Regionizer(resolution=7) regions =
-regionizer.transform(area) folium_map = plot_regions(area, colormap=["rgba
-(0,0,0,0.1)"], tiles_style="CartoDB positron") plot_regions
-(regions_gdf=regions, map=folium_map) ```
+### Regionalization Regionalization is a process of dividing a given area into
+smaller regions. This can be done in a variety of ways: * `H3Regionalizer` -
+regionalization using [Uber's H3 library](https://github.com/uber/h3) *
+`S2Regionalizer` - regionalization using [Google's S2 library](https://
+github.com/google/s2geometry) * `VoronoiRegionalizer` - regionalization using
+Voronoi diagram * `AdministativeBoundaryRegionalizer` - regionalization using
+administrative boundaries Example: ```python from srai.regionalizers import
+H3Regionalizer from srai.utils import geocode_to_region_gdf area =
+geocode_to_region_gdf("Berlin, Germany") regionalizer = H3Regionalizer
+(resolution=7) regions = regionalizer.transform(area) folium_map = plot_regions
+(area, colormap=["rgba(0,0,0,0.1)"], tiles_style="CartoDB positron")
+plot_regions(regions_gdf=regions, map=folium_map) ```
    [https://raw.githubusercontent.com/srai-lab/srai/main/docs/assets/images/
-                              regionization.jpg]
+                             regionalization.jpg]
 ### Embedding Embedding is a process of mapping regions into a vector space.
 This can be done in a variety of ways: * `Hex2VecEmbedder` - embedding using
 hex2vec[1] algorithm * `GTFS2VecEmbedder` - embedding using GTFS2Vec[2]
 algorithm * `CountEmbedder` - embedding based on features counts *
 `ContextualCountEmbedder` - embedding based on features counts with
 neighbourhood context (proposed in [3]) * `Highway2VecEmbedder` - embedding
 using Highway2Vec[4] algorithm All of those methods share the same API. All of
-them require results from `Loader` (load features), `Regionizer` (split area
+them require results from `Loader` (load features), `Regionalizer` (split area
 into regions) and `Joiner` (join features to regions) to work. An example using
 `CountEmbedder`: ```python from srai.embedders import CountEmbedder from
 srai.joiners import IntersectionJoiner from srai.loaders import OSMOnlineLoader
-from srai.plotting import plot_regions, plot_numeric_data from srai.regionizers
-import H3Regionizer from srai.utils import geocode_to_region_gdf loader =
-OSMOnlineLoader() regionizer = H3Regionizer(resolution=9) joiner =
-IntersectionJoiner() query = {"amenity": "bicycle_parking"} area =
-geocode_to_region_gdf("MalmÃ¶, Sweden") features = loader.load(area, query)
-regions = regionizer.transform(area) joint = joiner.transform(regions,
-features) embedder = CountEmbedder() embeddings = embedder.transform(regions,
-features, joint) folium_map = plot_regions(area, colormap=["rgba(0,0,0,0.1)"],
-tiles_style="CartoDB positron") plot_numeric_data(regions, embeddings,
-"amenity_bicycle_parking", map=folium_map) ```
+from srai.plotting import plot_regions, plot_numeric_data from
+srai.regionalizers import H3Regionalizer from srai.utils import
+geocode_to_region_gdf loader = OSMOnlineLoader() regionalizer = H3Regionalizer
+(resolution=9) joiner = IntersectionJoiner() query = {"amenity":
+"bicycle_parking"} area = geocode_to_region_gdf("MalmÃ¶, Sweden") features =
+loader.load(area, query) regions = regionalizer.transform(area) joint =
+joiner.transform(regions, features) embedder = CountEmbedder() embeddings =
+embedder.transform(regions, features, joint) folium_map = plot_regions(area,
+colormap=["rgba(0,0,0,0.1)"], tiles_style="CartoDB positron") plot_numeric_data
+(regions, embeddings, "amenity_bicycle_parking", map=folium_map) ```
    [https://raw.githubusercontent.com/srai-lab/srai/main/docs/assets/images/
                          embedding_count_embedder.jpg]
 `CountEmbedder` is a simple method, which does not require fitting. Other
 methods, such as `Hex2VecEmbedder` or `GTFS2VecEmbedder` require fitting and
 can be used in a similar way to `scikit-learn` estimators: ```python from
 srai.embedders import Hex2VecEmbedder from srai.joiners import
 IntersectionJoiner from srai.loaders import OSMPbfLoader from
 srai.loaders.osm_loaders.filters import HEX2VEC_FILTER from
 srai.neighbourhoods.h3_neighbourhood import H3Neighbourhood from
-srai.regionizers import H3Regionizer from srai.utils import
+srai.regionalizers import H3Regionalizer from srai.utils import
 geocode_to_region_gdf from srai.plotting import plot_regions, plot_numeric_data
-loader = OSMPbfLoader() regionizer = H3Regionizer(resolution=11) joiner =
+loader = OSMPbfLoader() regionalizer = H3Regionalizer(resolution=11) joiner =
 IntersectionJoiner() area = geocode_to_region_gdf("City of London") features =
-loader.load(area, HEX2VEC_FILTER) regions = regionizer.transform(area) joint =
-joiner.transform(regions, features) embedder = Hex2VecEmbedder() neighbourhood
-= H3Neighbourhood(regions_gdf=regions) embedder = Hex2VecEmbedder([15, 10, 3])
-# Option 1: fit and transform # embedder.fit(regions, features, joint,
-neighbourhood, batch_size=128) # embeddings = embedder.transform(regions,
-features, joint) # Option 2: fit_transform embeddings = embedder.fit_transform
-(regions, features, joint, neighbourhood, batch_size=128) folium_map =
-plot_regions(area, colormap=["rgba(0,0,0,0.1)"], tiles_style="CartoDB
-positron") plot_numeric_data(regions, embeddings, 0, map=folium_map) ```
+loader.load(area, HEX2VEC_FILTER) regions = regionalizer.transform(area) joint
+= joiner.transform(regions, features) embedder = Hex2VecEmbedder()
+neighbourhood = H3Neighbourhood(regions_gdf=regions) embedder = Hex2VecEmbedder
+([15, 10, 3]) # Option 1: fit and transform # embedder.fit(regions, features,
+joint, neighbourhood, batch_size=128) # embeddings = embedder.transform
+(regions, features, joint) # Option 2: fit_transform embeddings =
+embedder.fit_transform(regions, features, joint, neighbourhood, batch_size=128)
+folium_map = plot_regions(area, colormap=["rgba(0,0,0,0.1)"],
+tiles_style="CartoDB positron") plot_numeric_data(regions, embeddings, 0,
+map=folium_map) ```
    [https://raw.githubusercontent.com/srai-lab/srai/main/docs/assets/images/
                         embedding_hex2vec_embedder.jpg]
 ### Plotting, utilities and more We also provide utilities for different
 spatial operations and plotting functions adopted to data formats used in
 `srai` For a full list of available methods, please refer to the
 [documentation](https://srai-lab.github.io/srai). ## Contributing If you are
 willing to contribute to `srai`, feel free to do so! Visit [our contributing
@@ -159,14 +172,19 @@
 Resilient and Intelligent Cities (ARIC '21). Association for Computing
 Machinery, New York, NY, USA, 1â12. [paper](https://doi.org/10.1145/
 3486626.3493434), [arXiv](https://arxiv.org/abs/2111.00990) 4. Kacper LeÅniara
 and Piotr SzymaÅski. 2022. Highway2vec: representing OpenStreetMap
 microregions with respect to their road network characteristics. In Proceedings
 of the 5th ACM SIGSPATIAL International Workshop on AI for Geographic Knowledge
 Discovery (GeoAI '22). Association for Computing Machinery, New York, NY, USA,
-18â29. [paper](https://doi.org/10.1145/3557918.3565865) ## Citation TBD ##
-License This library is licensed under the [Apache Licence 2.0](https://
+18â29. [paper](https://doi.org/10.1145/3557918.3565865), [arXiv](https://
+arxiv.org/abs/2304.13865) ## Acknowledgements We would like to thank Piotr
+SzymaÅski PhD \([@niedakh](https://twitter.com/niedakh)\) for his invaluable
+guidance and support in the development of this library. His expertise and
+mentorship have been instrumental in shaping the library's design and
+functionality, and we are very grateful for his input. ## Citation TBD ##
+License This library is licensed under the [Apache License 2.0](https://
 github.com/srai-lab/srai/blob/main/LICENSE.md). The free [OpenStreetMap](https:
 //www.openstreetmap.org/) data, which is used for the development of SRAI, is
 licensed under the [Open Data Commons Open Database License](https://
 opendatacommons.org/licenses/odbl/) (ODbL) by the [OpenStreetMap Foundation]
 (https://osmfoundation.org/) (OSMF).
```

### Comparing `srai-0.1.1/pyproject.toml` & `srai-0.1.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 [project]
 name = "srai"
-version = "0.1.1"
+version = "0.1.4"
 description = "A set of python modules for geospatial machine learning and data mining"
 authors = [
-    { name = "srai", email = "spatialrepresentationsforai@gmail.com" },
+    { name = "SRAI Lab", email = "spatialrepresentationsforai@gmail.com" },
+    { name = "Piotr Gramacki" },
+    { name = "Kacper Leśniara" },
+    { name = "Kamil Raczycki" },
+    { name = "Szymon Woźniak" },
 ]
 dependencies = [
     "pandas",
     "geopandas",
     "shapely",
     "h3>=4.0.0b1",
     "numpy",
@@ -65,15 +69,15 @@
 gtfs = [
     "gtfs-kit",
 ]
 plotting = [
     "folium",
     "mapclassify",
     "plotly",
-    "kaleido",
+    "kaleido<=0.2.1",
 ]
 torch = [
     "pytorch-lightning",
     "torch",
 ]
 all = [
     "srai[osm,voronoi,gtfs,plotting,torch]",
@@ -191,15 +195,15 @@
 tab-width = 4
 blank = false
 pre-summary-newline = true
 close-quotes-on-newline = true
 wrap-one-line = true
 
 [tool.bumpver]
-current_version = "0.1.1"
+current_version = "0.1.4"
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message = "chore: bump version {old_version} -> {new_version}"
 commit = true
 tag = false
 push = false
 
 [tool.bumpver.file_patterns]
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `srai-0.1.1/srai/embedders/__init__.py` & `srai-0.1.4/srai/embedders/__init__.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.1/srai/embedders/_base.py` & `srai-0.1.4/srai/embedders/_base.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.1/srai/embedders/contextual_count_embedder.py` & `srai-0.1.4/srai/embedders/contextual_count_embedder.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.1/srai/embedders/count_embedder.py` & `srai-0.1.4/srai/embedders/count_embedder.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.1/srai/embedders/gtfs2vec/embedder.py` & `srai-0.1.4/srai/embedders/gtfs2vec/embedder.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-gtfs2vec embedder.
+Gtfs2vec embedder.
 
 This module contains embedder from gtfs2vec paper [1].
 
 References:
     1. https://doi.org/10.1145/3486640.3491392
 """
```

### Comparing `srai-0.1.1/srai/embedders/gtfs2vec/model.py` & `srai-0.1.4/srai/embedders/gtfs2vec/model.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.1/srai/embedders/hex2vec/embedder.py` & `srai-0.1.4/srai/embedders/hex2vec/embedder.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.1/srai/embedders/hex2vec/model.py` & `srai-0.1.4/srai/embedders/hex2vec/model.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.1/srai/embedders/hex2vec/neighbour_dataset.py` & `srai-0.1.4/srai/embedders/hex2vec/neighbour_dataset.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.1/srai/embedders/highway2vec/embedder.py` & `srai-0.1.4/srai/embedders/highway2vec/embedder.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.1/srai/embedders/highway2vec/model.py` & `srai-0.1.4/srai/embedders/highway2vec/model.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.1/srai/exceptions.py` & `srai-0.1.4/srai/exceptions.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.1/srai/joiners/__init__.py` & `srai-0.1.4/srai/joiners/__init__.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.1/srai/joiners/_base.py` & `srai-0.1.4/srai/joiners/_base.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.1/srai/joiners/intersection_joiner.py` & `srai-0.1.4/srai/joiners/intersection_joiner.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.1/srai/loaders/__init__.py` & `srai-0.1.4/srai/loaders/__init__.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.1/srai/loaders/_base.py` & `srai-0.1.4/srai/loaders/_base.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.1/srai/loaders/geoparquet_loader.py` & `srai-0.1.4/srai/loaders/geoparquet_loader.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.1/srai/loaders/gtfs_loader.py` & `srai-0.1.4/srai/loaders/gtfs_loader.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.1/srai/loaders/osm_loaders/_base.py` & `srai-0.1.4/srai/loaders/osm_loaders/_base.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.1/srai/loaders/osm_loaders/filters/_typing.py` & `srai-0.1.4/srai/loaders/osm_loaders/filters/_typing.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.1/srai/loaders/osm_loaders/filters/base_osm_groups.py` & `srai-0.1.4/srai/loaders/osm_loaders/filters/base_osm_groups.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.1/srai/loaders/osm_loaders/filters/geofabrik.py` & `srai-0.1.4/srai/loaders/osm_loaders/filters/geofabrik.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.1/srai/loaders/osm_loaders/filters/hex2vec.py` & `srai-0.1.4/srai/loaders/osm_loaders/filters/hex2vec.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.1/srai/loaders/osm_loaders/filters/popular.py` & `srai-0.1.4/srai/loaders/osm_loaders/filters/popular.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.1/srai/loaders/osm_loaders/osm_online_loader.py` & `srai-0.1.4/srai/loaders/osm_loaders/osm_online_loader.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.1/srai/loaders/osm_loaders/osm_pbf_loader.py` & `srai-0.1.4/srai/loaders/osm_loaders/osm_pbf_loader.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.1/srai/loaders/osm_loaders/osm_tile_data_collector.py` & `srai-0.1.4/srai/loaders/osm_loaders/osm_tile_data_collector.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.1/srai/loaders/osm_loaders/osm_tile_loader.py` & `srai-0.1.4/srai/loaders/osm_loaders/osm_tile_loader.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from typing import Any, Optional, Union
 from urllib.parse import urljoin
 
 import geopandas as gpd
 import pandas as pd
 import requests
 
-from srai.regionizers.slippy_map_regionizer import SlippyMapRegionizer
+from srai.regionalizers.slippy_map_regionalizer import SlippyMapRegionalizer
 from srai.utils._optional import import_optional_dependencies
 
 from .osm_tile_data_collector import (
     DataCollector,
     DataCollectorType,
     InMemoryDataCollector,
     get_collector,
@@ -75,15 +75,15 @@
         self.auth_token = auth_token
         self.save_path = storage_path
         self.data_collector = (
             self._get_collector(data_collector)
             if data_collector is not None
             else InMemoryDataCollector()
         )
-        self.regionizer = SlippyMapRegionizer(zoom=self.zoom)
+        self.regionalizer = SlippyMapRegionalizer(zoom=self.zoom)
 
     def _get_collector(
         self, storage_strategy: Union[str, DataCollectorType, DataCollector]
     ) -> DataCollector:
         if isinstance(storage_strategy, str):
             return get_collector(
                 storage_strategy, save_path=self.save_path, file_extension=self.resource_type
@@ -99,15 +99,15 @@
 
         Args:
             area (gpd.GeoDataFrame): Area for which to download objects.
 
         Returns:
             gpd.GeoDataFrame: Pandas of tiles for each region in area transformed by DataCollector
         """
-        regions = self.regionizer.transform(gdf=area)
+        regions = self.regionalizer.transform(gdf=area)
         regions["tile"] = regions.apply(lambda row: self._get_tile_for_area(row), axis=1)
         return regions
 
     def _get_tile_for_area(self, row: pd.Series) -> Any:
         idx = row.name
         return self.get_tile_by_x_y(row["x"], row["y"], idx=idx)
```

### Comparing `srai-0.1.1/srai/loaders/osm_loaders/pbf_file_downloader.py` & `srai-0.1.4/srai/loaders/osm_loaders/pbf_file_downloader.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.1/srai/loaders/osm_loaders/pbf_file_handler.py` & `srai-0.1.4/srai/loaders/osm_loaders/pbf_file_handler.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 PBF File Handler.
 
 This module contains a handler capable of parsing a PBF file into a GeoDataFrame.
 """
 import warnings
-from typing import TYPE_CHECKING, Any, Callable, Dict, Optional, Sequence, Union
+from typing import TYPE_CHECKING, Any, Callable, Dict, Optional, Sequence, Union, cast
 
 import geopandas as gpd
 import osmium
 import osmium.osm
 import shapely.wkb as wkblib
 from osmium.osm.types import T_obj
 from shapely.geometry import MultiPolygon, Polygon
@@ -71,14 +71,15 @@
         if self.filter_tags:
             self.filter_tags_keys = set(self.filter_tags.keys())
         else:
             self.filter_tags_keys = set()
         self.region_geometry = region_geometry
         self.wkbfab = osmium.geom.WKBFactory()
         self.features_cache: Dict[str, Dict[str, Any]] = {}
+        self.features_count: Optional[int] = None
 
     def get_features_gdf(
         self, file_paths: Sequence[Union[str, "os.PathLike[str]"]], region_id: str = "OSM"
     ) -> gpd.GeoDataFrame:
         """
         Get features GeoDataFrame from a list of PBF files.
 
@@ -92,16 +93,19 @@
                 files to be parsed.
             region_id (str, optional): Region name to be set in progress bar.
                 Defaults to "OSM".
 
         Returns:
             gpd.GeoDataFrame: GeoDataFrame with OSM features.
         """
-        with tqdm(desc="Parsing pbf file") as self.pbar:
-            self._clear_cache()
+        self._clear_cache()
+        if self.features_count is None:
+            self._count_features(file_paths, region_id)
+
+        with tqdm(desc="Parsing pbf file", total=self.features_count) as self.pbar:
             for path_no, path in enumerate(file_paths):
                 self.path_no = path_no + 1
                 description = self._PBAR_FORMAT.format(region_id, str(self.path_no))
                 self.pbar.set_description(description)
                 self.apply_file(path)
             if self.features_cache:
                 features_gdf = (
@@ -109,72 +113,98 @@
                     .set_crs(WGS84_CRS)
                     .set_index(FEATURES_INDEX)
                 )
             else:
                 features_gdf = gpd.GeoDataFrame(
                     index=gpd.pd.Index(name=FEATURES_INDEX, data=[]), crs=WGS84_CRS, geometry=[]
                 )
-            self._clear_cache()
+
+        self._clear_cache()
         return features_gdf
 
     def node(self, node: osmium.osm.Node) -> None:
         """
         Implementation of the required `node` function.
 
         See [1] for more information.
 
         Args:
             node (osmium.osm.Node): Node to be parsed.
 
         References:
             1. https://docs.osmcode.org/pyosmium/latest/ref_osm.html#osmium.osm.Node
         """
-        self._parse_osm_object(
-            osm_object=node, osm_type="node", parse_to_wkb_function=self.wkbfab.create_point
-        )
+        if self.counting_features:
+            self._count_feature()
+        else:
+            self._parse_osm_object(
+                osm_object=node, osm_type="node", parse_to_wkb_function=self.wkbfab.create_point
+            )
 
     def way(self, way: osmium.osm.Way) -> None:
         """
         Implementation of the required `way` function.
 
         See [1] for more information.
 
         Args:
             way (osmium.osm.Way): Way to be parsed.
 
         References:
             1. https://docs.osmcode.org/pyosmium/latest/ref_osm.html#osmium.osm.Way
         """
-        self._parse_osm_object(
-            osm_object=way, osm_type="way", parse_to_wkb_function=self.wkbfab.create_linestring
-        )
+        if self.counting_features:
+            self._count_feature()
+        else:
+            self._parse_osm_object(
+                osm_object=way, osm_type="way", parse_to_wkb_function=self.wkbfab.create_linestring
+            )
 
     def area(self, area: osmium.osm.Area) -> None:
         """
         Implementation of the required `area` function.
 
         See [1] for more information.
 
         Args:
             area (osmium.osm.Area): Area to be parsed.
 
         References:
             1. https://docs.osmcode.org/pyosmium/latest/ref_osm.html#osmium.osm.Area
         """
-        self._parse_osm_object(
-            osm_object=area,
-            osm_type="way" if area.from_way() else "relation",
-            parse_to_wkb_function=self.wkbfab.create_multipolygon,
-            osm_id=area.orig_id(),
-        )
+        if self.counting_features:
+            self._count_feature()
+        else:
+            self._parse_osm_object(
+                osm_object=area,
+                osm_type="way" if area.from_way() else "relation",
+                parse_to_wkb_function=self.wkbfab.create_multipolygon,
+                osm_id=area.orig_id(),
+            )
 
     def _clear_cache(self) -> None:
         """Clear memory from accumulated features."""
         self.features_cache.clear()
 
+    def _count_features(
+        self, file_paths: Sequence[Union[str, "os.PathLike[str]"]], region_id: str = "OSM"
+    ) -> None:
+        with tqdm(desc=f"[{region_id}] Counting pbf features") as self.pbar:
+            self.counting_features = True
+            self.features_count = 0
+            for path in file_paths:
+                self.apply_file(path)
+            self.pbar.update(n=self.features_count % 100_000)
+            self.counting_features = False
+
+    def _count_feature(self) -> None:
+        self.features_count = cast(int, self.features_count) + 1
+        if self.features_count % 100_000 == 0:
+            self.pbar.update(n=100_000)
+
     def _parse_osm_object(
         self,
         osm_object: osmium.osm.OSMObject[T_obj],
         osm_type: str,
         parse_to_wkb_function: Callable[..., str],
         osm_id: Optional[int] = None,
     ) -> None:
@@ -228,15 +258,15 @@
         self, osm_object: osmium.osm.OSMObject[T_obj], parse_to_wkb_function: Callable[..., str]
     ) -> BaseGeometry:
         """Get geometry from currently parsed OSM object."""
         geometry = None
         try:
             wkb = parse_to_wkb_function(osm_object)
             geometry = wkblib.loads(wkb, hex=True)
-        except RuntimeError as ex:
+        except Exception as ex:
             message = str(ex)
             warnings.warn(message, RuntimeWarning, stacklevel=2)
 
         return geometry
 
     def _add_feature_to_cache(
         self, full_osm_id: str, matching_tags: Dict[str, str], geometry: Optional[BaseGeometry]
```

### Comparing `srai-0.1.1/srai/loaders/osm_way_loader/constants.py` & `srai-0.1.4/srai/loaders/osm_way_loader/constants.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.1/srai/loaders/osm_way_loader/osm_way_loader.py` & `srai-0.1.4/srai/loaders/osm_way_loader/osm_way_loader.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.1/srai/neighbourhoods/_base.py` & `srai-0.1.4/srai/neighbourhoods/_base.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.1/srai/neighbourhoods/adjacency_neighbourhood.py` & `srai-0.1.4/srai/neighbourhoods/adjacency_neighbourhood.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.1/srai/neighbourhoods/h3_neighbourhood.py` & `srai-0.1.4/srai/neighbourhoods/h3_neighbourhood.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.1/srai/plotting/folium_wrapper.py` & `srai-0.1.4/srai/plotting/folium_wrapper.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.1/srai/plotting/plotly_wrapper.py` & `srai-0.1.4/srai/plotting/plotly_wrapper.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.1/srai/regionizers/__init__.py` & `srai-0.1.4/srai/regionalizers/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """
-This module contains regionizers, which are used to divide space before analysis.
+This module contains regionalizers, which are used to divide space before analysis.
 
 Embedding methods available in `srai` operate on a regions, which can be defined in many ways. In
-this module, we aggregate different regionization methods under a common `Regionizer` interface. We
-include both pre-defined spatial indexes (e.g. H3 or S2), data-based ones (e.g. Voronoi) and OSM-
+this module, we aggregate different regionalization methods under a common `Regionalizer` interface.
+We include both pre-defined spatial indexes (e.g. H3 or S2), data-based ones (e.g. Voronoi) and OSM-
 based ones (e.g. administrative boundaries).
 """
 
-from ._base import Regionizer
-from .administrative_boundary_regionizer import AdministrativeBoundaryRegionizer
-from .h3_regionizer import H3Regionizer
-from .s2_regionizer import S2Regionizer
-from .slippy_map_regionizer import SlippyMapRegionizer
-from .voronoi_regionizer import VoronoiRegionizer
+from ._base import Regionalizer
+from .administrative_boundary_regionalizer import AdministrativeBoundaryRegionalizer
+from .h3_regionalizer import H3Regionalizer
+from .s2_regionalizer import S2Regionalizer
+from .slippy_map_regionalizer import SlippyMapRegionalizer
+from .voronoi_regionalizer import VoronoiRegionalizer
 
 __all__ = [
-    "Regionizer",
-    "AdministrativeBoundaryRegionizer",
-    "H3Regionizer",
-    "S2Regionizer",
-    "VoronoiRegionizer",
-    "SlippyMapRegionizer",
+    "Regionalizer",
+    "AdministrativeBoundaryRegionalizer",
+    "H3Regionalizer",
+    "S2Regionalizer",
+    "VoronoiRegionalizer",
+    "SlippyMapRegionalizer",
 ]
```

### Comparing `srai-0.1.1/srai/regionizers/_base.py` & `srai-0.1.4/srai/regionalizers/_base.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-"""Base class for regionizers."""
+"""Base class for regionalizers."""
 
 import abc
 
 import geopandas as gpd
 
 
-class Regionizer(abc.ABC):
-    """Abstract class for regionizers."""
+class Regionalizer(abc.ABC):
+    """Abstract class for regionalizers."""
 
     @abc.abstractmethod
     def transform(self, gdf: gpd.GeoDataFrame) -> gpd.GeoDataFrame:  # pragma: no cover
         """
-        Regionize a given GeoDataFrame.
+        Regionalize a given GeoDataFrame.
 
         This one should treat the input as a single region.
 
         Args:
-            gdf (gpd.GeoDataFrame): GeoDataFrame to be regionized.
+            gdf (gpd.GeoDataFrame): GeoDataFrame to be regionalized.
 
         Returns:
-            GeoDataFrame with the regionized data.
+            GeoDataFrame with the regionalized data.
         """
         raise NotImplementedError
 
     def _explode_multipolygons(self, gdf: gpd.GeoDataFrame) -> gpd.GeoDataFrame:
         """
         Explode multipolygons into multiple polygons.
```

### Comparing `srai-0.1.1/srai/regionizers/_spherical_voronoi.py` & `srai-0.1.4/srai/regionalizers/_spherical_voronoi.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.1/srai/regionizers/administrative_boundary_regionizer.py` & `srai-0.1.4/srai/regionalizers/administrative_boundary_regionalizer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 """
-Administrative Boundary Regionizer.
+Administrative Boundary Regionalizer.
 
-This module contains administrative boundary regionizer implementation.
+This module contains administrative boundary regionalizer implementation.
 """
 import time
 from typing import Any, Dict, List, Optional, Union
 
 import geopandas as gpd
 import topojson as tp
 from shapely.geometry import MultiPolygon, Point, Polygon
 from shapely.geometry.base import BaseGeometry
 from shapely.ops import unary_union
 from shapely.validation import make_valid
 from tqdm import tqdm
 
 from srai.constants import GEOMETRY_COLUMN, REGIONS_INDEX, WGS84_CRS
-from srai.regionizers import Regionizer
+from srai.regionalizers import Regionalizer
 from srai.utils import flatten_geometry_series
 from srai.utils._optional import import_optional_dependencies
 
 
-class AdministrativeBoundaryRegionizer(Regionizer):
+class AdministrativeBoundaryRegionalizer(Regionalizer):
     """
-    AdministrativeBoundaryRegionizer.
+    AdministrativeBoundaryRegionalizer.
 
-    Administrative boundary regionizer allows the given geometries to be divided
+    Administrative boundary regionalizer allows the given geometries to be divided
     into boundaries from OpenStreetMap on a given `admin_level` [1].
 
     Downloads those boundaries online using `overpass` and `osmnx` libraries.
 
     Note: offline .pbf loading will be implemented in the future.
     Note: option to download historic data will be implemented in the future.
 
@@ -44,15 +44,15 @@
         clip_regions: bool = True,
         return_empty_region: bool = False,
         prioritize_english_name: bool = True,
         toposimplify: Union[bool, float] = True,
         remove_artefact_regions: bool = True,
     ) -> None:
         """
-        Init AdministrativeBoundaryRegionizer.
+        Init AdministrativeBoundaryRegionalizer.
 
         Args:
             admin_level (int): OpenStreetMap admin_level value. See [1] for detailed description of
                 available values.
             clip_regions (bool, optional): Whether to clip regions using a provided mask.
                 Turning it off can an be useful when trying to load regions using list a of points.
                 Defaults to True.
@@ -101,15 +101,15 @@
         else:
             self.toposimplify = False
 
         self.overpass_api = API(timeout=60)
 
     def transform(self, gdf: gpd.GeoDataFrame) -> gpd.GeoDataFrame:
         """
-        Regionize a given GeoDataFrame.
+        Regionalize a given GeoDataFrame.
 
         Will query Overpass [1] server using `overpass` [2] library for closed administrative
         boundaries on a given admin_level and then download geometries for each relation using
         `osmnx` [3] library.
 
         If `prioritize_english_name` is set to `True`, method will try to extract the `name:en` tag
         first before resorting to the `name` tag. If boundary doesn't have a `name` tag, an `id`
@@ -119,19 +119,19 @@
         size of geometries while keeping neighbouring regions together without introducing gaps.
         `Topojson` library [4] is used for this operation.
 
         Additionally, an empty region with name `EMPTY` can be introduced if returned regions do
         not fully cover a clipping mask.
 
         Args:
-            gdf (gpd.GeoDataFrame): GeoDataFrame to be regionized.
+            gdf (gpd.GeoDataFrame): GeoDataFrame to be regionalized.
                 Will use this list of geometries to crop resulting regions.
 
         Returns:
-            gpd.GeoDataFrame: GeoDataFrame with the regionized data cropped using input
+            gpd.GeoDataFrame: GeoDataFrame with the regionalized data cropped using input
                 GeoDataFrame.
 
         Raises:
             RuntimeError: If simplification can't preserve a topology.
 
         References:
             1. https://wiki.openstreetmap.org/wiki/Overpass_API
@@ -182,15 +182,15 @@
         if self.clip_regions:
             regions_gdf = regions_gdf.clip(mask=gdf_wgs84, keep_geom_type=False)
 
         if self.return_empty_region:
             empty_region = self._generate_empty_region(mask=gdf_wgs84, regions_gdf=regions_gdf)
             if not empty_region.is_empty:
                 regions_gdf.loc[
-                    AdministrativeBoundaryRegionizer.EMPTY_REGION_NAME, GEOMETRY_COLUMN
+                    AdministrativeBoundaryRegionalizer.EMPTY_REGION_NAME, GEOMETRY_COLUMN
                 ] = empty_region
 
         return regions_gdf
 
     def _generate_regions_from_all_geometries(
         self, gdf_wgs84: gpd.GeoDataFrame
     ) -> List[Dict[str, Any]]:
@@ -330,15 +330,15 @@
 
     def _get_empty_geodataframe(self, gdf: gpd.GeoDataFrame) -> gpd.GeoDataFrame:
         """Get empty GeoDataFrame when zero boundaries have been found."""
         if self.return_empty_region:
             regions_gdf = gpd.GeoDataFrame(
                 data={
                     GEOMETRY_COLUMN: [gdf.geometry.unary_union],
-                    REGIONS_INDEX: [AdministrativeBoundaryRegionizer.EMPTY_REGION_NAME],
+                    REGIONS_INDEX: [AdministrativeBoundaryRegionalizer.EMPTY_REGION_NAME],
                 },
                 crs=WGS84_CRS,
             ).set_index(REGIONS_INDEX)
         else:
             regions_gdf = gpd.GeoDataFrame(
                 data={
                     GEOMETRY_COLUMN: [],
```

### Comparing `srai-0.1.1/srai/regionizers/h3_regionizer.py` & `srai-0.1.4/srai/regionalizers/h3_regionalizer.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
-H3 regionizer.
+H3 regionalizer.
 
-This module exposes Uber's H3 Hexagonal Hierarchical Geospatial Indexing System [1] as a regionizer.
+This module exposes Uber's H3 Hexagonal Hierarchical Geospatial Indexing System [1] as
+a regionalizer.
 
 Note:
     The default API [2] was chosen (basic_str) to ease the implementation.
     It may be beneficial to try the NumPy API for computationally-heavy work.
 
 References:
     1. https://uber.github.io/h3-py/
@@ -16,29 +17,29 @@
 
 import geopandas as gpd
 import h3
 from functional import seq
 from shapely import geometry
 
 from srai.constants import GEOMETRY_COLUMN, REGIONS_INDEX, WGS84_CRS
-from srai.regionizers import Regionizer
+from srai.regionalizers import Regionalizer
 from srai.utils import buffer_geometry
 
 
-class H3Regionizer(Regionizer):
+class H3Regionalizer(Regionalizer):
     """
-    H3 Regionizer.
+    H3 Regionalizer.
 
-    H3 Regionizer allows the given geometries to be divided
+    H3 Regionalizer allows the given geometries to be divided
     into H3 cells - hexagons with pentagons as a very rare exception
     """
 
     def __init__(self, resolution: int, buffer: bool = True) -> None:
         """
-        Init H3Regionizer.
+        Init H3Regionalizer.
 
         Args:
             resolution (int): Resolution of the cells. See [1] for a full comparison.
             buffer (bool, optional): Whether to fully cover the geometries with
                 H3 Cells (visible on the borders). Defaults to True.
 
         Raises:
@@ -51,21 +52,21 @@
             raise ValueError(f"Resolution {resolution} is not between 0 and 15.")
 
         self.resolution = resolution
         self.buffer = buffer
 
     def transform(self, gdf: gpd.GeoDataFrame) -> gpd.GeoDataFrame:
         """
-        Regionize a given GeoDataFrame.
+        Regionalize a given GeoDataFrame.
 
         Transforms given geometries into H3 cells of given resolution
         and optionally applies buffering.
 
         Args:
-            gdf (gpd.GeoDataFrame): (Multi)Polygons to be regionized.
+            gdf (gpd.GeoDataFrame): (Multi)Polygons to be regionalized.
 
         Returns:
             gpd.GeoDataFrame: H3 cells.
 
         Raises:
             ValueError: If provided GeoDataFrame has no crs defined.
         """
```

### Comparing `srai-0.1.1/srai/regionizers/s2_regionizer.py` & `srai-0.1.4/srai/regionalizers/s2_regionalizer.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
-S2 regionizer.
+S2 Regionalizer.
 
-This module exposes Google's S2 Geospatial Indexing System [1] as a regionizer.
+This module exposes Google's S2 Geospatial Indexing System [1] as a regionalizer.
 It uses the Python API [2].
 
 References:
     1. https://s2geometry.io/
     2. https://github.com/JoaoCarabetta/s2-py
 """
 
@@ -15,27 +15,27 @@
 import geopandas as gpd
 from functional import seq
 from functional.pipeline import Sequence
 from s2 import s2
 from shapely.geometry import Polygon
 
 from srai.constants import GEOMETRY_COLUMN, REGIONS_INDEX, WGS84_CRS
-from srai.regionizers import Regionizer
+from srai.regionalizers import Regionalizer
 
 
-class S2Regionizer(Regionizer):
+class S2Regionalizer(Regionalizer):
     """
-    S2 Regionizer.
+    S2 Regionalizer.
 
-    S2 Regionizer gives an opportunity to divide the given geometries into square S2 cells.
+    S2 Regionalizer gives an opportunity to divide the given geometries into square S2 cells.
     """
 
     def __init__(self, resolution: int, buffer: bool = True) -> None:
         """
-        Init S2 Regionizer.
+        Init S2 Regionalizer.
 
         Args:
             resolution (int): Resolution of the cells (S2 supports 0-30). See [1] for
                 a full comparison.
             buffer (bool, optional): If True then fully cover geometries with S2 cells.
                 Otherwise only use those cells that fully fit into them. Defaults to True.
 
@@ -49,21 +49,21 @@
             raise ValueError(f"Resolution {resolution} is not between 0 and 30.")
 
         self.resolution = resolution
         self.buffer = buffer
 
     def transform(self, gdf: gpd.GeoDataFrame) -> gpd.GeoDataFrame:
         """
-        Regionize a given GeoDataFrame.
+        Regionalize a given GeoDataFrame.
 
         Args:
-            gdf (gpd.GeoDataFrame): GeoDataFrame to be regionized.
+            gdf (gpd.GeoDataFrame): GeoDataFrame to be regionalized.
 
         Returns:
-            gpd.GeoDataFrame: GeoDataFrame with regionized geometries.
+            gpd.GeoDataFrame: GeoDataFrame with regionalized geometries.
         """
         gdf_wgs84 = gdf.to_crs(crs=WGS84_CRS)
 
         s2_gdf = self._fill_with_s2_cells(self._explode_multipolygons(gdf_wgs84))
 
         # s2 library fills also holes in Polygons, so here we remove redundant cells
         res: gpd.GeoDataFrame = gpd.sjoin(
```

### Comparing `srai-0.1.1/srai/regionizers/slippy_map_regionizer.py` & `srai-0.1.4/srai/regionalizers/slippy_map_regionalizer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,54 +1,54 @@
 """
-Slippy map regionizer.
+Slippy map regionalizer.
 
-This module implements Slippy map tilenames [1] as regionizer.
+This module implements Slippy map tilenames [1] as a regionalizer.
 
 References:
     1. https://wiki.openstreetmap.org/wiki/Slippy_map_tilenames
 """
 from itertools import product
 from typing import Any, Dict, List, Tuple
 
 import geopandas as gpd
 import numpy as np
 import shapely.geometry as shpg
 from functional import seq
 
 from srai.constants import GEOMETRY_COLUMN, REGIONS_INDEX, WGS84_CRS
-from srai.regionizers import Regionizer
+from srai.regionalizers import Regionalizer
 
 
-class SlippyMapRegionizer(Regionizer):
-    """Regionizer class."""
+class SlippyMapRegionalizer(Regionalizer):
+    """SlippyMapRegionalizer class."""
 
     def __init__(self, zoom: int) -> None:
         """
-        Initialize SlippyMapRegionizer.
+        Initialize SlippyMapRegionalizer.
 
         Args:
             zoom (int): zoom level
 
         Raises:
             ValueError: if zoom is not in [0, 19]
         """
         if not 0 <= zoom <= 19:
             raise ValueError
         self.zoom = zoom
         super().__init__()
 
     def transform(self, gdf: gpd.GeoDataFrame) -> gpd.GeoDataFrame:
         """
-        Regionize a given GeoDataFrame.
+        Regionalize a given GeoDataFrame.
 
         Args:
-            gdf (gpd.GeoDataFrame): GeoDataFrame to be regionized.
+            gdf (gpd.GeoDataFrame): GeoDataFrame to be regionalized.
 
         Returns:
-            gpd.GeoDataFrame: GeoDataFrame with regionized geometries.
+            gpd.GeoDataFrame: GeoDataFrame with regionalized geometries.
 
         Raises:
             ValueError: If provided GeoDataFrame has no crs defined.
         """
         gdf_wgs84 = gdf.to_crs(crs=WGS84_CRS)
         gdf_exploded = self._explode_multipolygons(gdf_wgs84)
```

### Comparing `srai-0.1.1/srai/regionizers/voronoi_regionizer.py` & `srai-0.1.4/srai/regionalizers/voronoi_regionalizer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
-Voronoi Regionizer.
+Voronoi Regionalizer.
 
-This module contains voronoi regionizer implementation.
+This module contains voronoi regionalizer implementation.
 """
 
 from typing import Hashable, List, Optional
 
 import geopandas as gpd
 from shapely.geometry import Point, box
 
 from srai.constants import GEOMETRY_COLUMN, REGIONS_INDEX, WGS84_CRS
-from srai.regionizers import Regionizer
+from srai.regionalizers import Regionalizer
 from srai.utils._optional import import_optional_dependencies
 
 
-class VoronoiRegionizer(Regionizer):
+class VoronoiRegionalizer(Regionalizer):
     """
-    VoronoiRegionizer.
+    VoronoiRegionalizer.
 
-    Voronoi [1] regionizer allows the given geometries to be divided
+    Voronoi [1] regionalizer allows the given geometries to be divided
     into Thiessen polygons using geometries that are the seeds. To
     minimize distortions tessellation will be performed on a sphere
     using SphericalVoronoi [2] function from scipy library.
 
     References:
         1. https://en.wikipedia.org/wiki/Voronoi_diagram
         2. https://docs.scipy.org/doc/scipy-1.9.2/reference/generated/scipy.spatial.SphericalVoronoi.html
@@ -32,15 +32,15 @@
         self,
         seeds: gpd.GeoDataFrame,
         max_meters_between_points: int = 10_000,
         num_of_multiprocessing_workers: int = -1,
         multiprocessing_activation_threshold: Optional[int] = None,
     ) -> None:
         """
-        Init VoronoiRegionizer.
+        Init VoronoiRegionalizer.
 
         All (multi)polygons from seeds GeoDataFrame will be transformed to their centroids,
         because scipy function requires only points as an input.
 
         Args:
             seeds (gpd.GeoDataFrame): GeoDataFrame with seeds for
                 creating a tessellation. Minimum 4 seeds are required.
@@ -80,27 +80,27 @@
 
         duplicated_seeds_ids = self._get_duplicated_seeds_ids()
         if duplicated_seeds_ids:
             raise ValueError(f"Duplicate seeds present: {duplicated_seeds_ids}.")
 
     def transform(self, gdf: Optional[gpd.GeoDataFrame] = None) -> gpd.GeoDataFrame:
         """
-        Regionize a given GeoDataFrame.
+        Regionalize a given GeoDataFrame.
 
         Returns a list of disjointed regions consisting of Thiessen cells generated
         using a Voronoi diagram on the sphere.
 
         Args:
-            gdf (Optional[gpd.GeoDataFrame], optional): GeoDataFrame to be regionized.
+            gdf (Optional[gpd.GeoDataFrame], optional): GeoDataFrame to be regionalized.
                 Will use this list of geometries to crop resulting regions. If None, a boundary box
                 with bounds (-180, -90, 180, 90) is used to return regions covering whole Earth.
                 Defaults to None.
 
         Returns:
-            gpd.GeoDataFrame: GeoDataFrame with the regionized data cropped using input
+            gpd.GeoDataFrame: GeoDataFrame with the regionalized data cropped using input
                 GeoDataFrame.
 
         Raises:
             ValueError: If provided geodataframe has no crs defined.
             ValueError: If seeds are laying on a single arc.
         """
         from ._spherical_voronoi import generate_voronoi_regions
```

### Comparing `srai-0.1.1/srai/utils/__init__.py` & `srai-0.1.4/srai/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.1/srai/utils/_optional.py` & `srai-0.1.4/srai/utils/_optional.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.1/srai/utils/download.py` & `srai-0.1.4/srai/utils/download.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.1/srai/utils/geocode.py` & `srai-0.1.4/srai/utils/geocode.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.1/srai/utils/geometry.py` & `srai-0.1.4/srai/utils/geometry.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.1/srai/utils/merge.py` & `srai-0.1.4/srai/utils/merge.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.1/srai/utils/typing.py` & `srai-0.1.4/srai/utils/typing.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.1/tests/embedders/conftest.py` & `srai-0.1.4/tests/embedders/conftest.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.1/tests/embedders/hex2vec/generation.py` & `srai-0.1.4/tests/embedders/hex2vec/generation.py`

 * *Files 21% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 from srai.constants import WGS84_CRS
 from srai.embedders.hex2vec.embedder import Hex2VecEmbedder
 from srai.joiners import IntersectionJoiner
 from srai.loaders.osm_loaders import OSMPbfLoader
 from srai.loaders.osm_loaders.filters import osm_tags_type
 from srai.neighbourhoods import H3Neighbourhood
-from srai.regionizers import H3Regionizer
+from srai.regionalizers import H3Regionalizer
 from srai.utils import geocode_to_region_gdf
 from tests.embedders.hex2vec.constants import ENCODER_SIZES, TRAINER_KWARGS
 
 
 def generate_test_case(
     test_case_name: str,
     geocoding_name: str,
@@ -28,17 +28,17 @@
     """Generate test case for Hex2VecEmbedder."""
     if tags is None:
         tags = {"leisure": "park", "amenity": "restaurant"}
     neighbourhood = H3Neighbourhood()
     regions_indexes = neighbourhood.get_neighbours_up_to_distance(root_region_index, radius)
     regions_indexes.add(root_region_index)
     regions_indexes = list(regions_indexes)  # type: ignore
-    regionizer = H3Regionizer(h3_res)
+    regionalizer = H3Regionalizer(h3_res)
 
-    geoms = [regionizer._h3_index_to_shapely_polygon(r) for r in regions_indexes]
+    geoms = [regionalizer._h3_index_to_shapely_polygon(r) for r in regions_indexes]
     regions_gdf = gpd.GeoDataFrame(index=regions_indexes, geometry=geoms, crs=WGS84_CRS)
     regions_gdf.index.name = "region_id"
 
     area_gdf = geocode_to_region_gdf(geocoding_name)
     loader = OSMPbfLoader()
     features_all = loader.load(area_gdf, tags=tags)
```

### Comparing `srai-0.1.1/tests/embedders/hex2vec/test_embedder.py` & `srai-0.1.4/tests/embedders/hex2vec/test_embedder.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.1/tests/embedders/hex2vec/test_files/poz_8_features.parquet` & `srai-0.1.4/tests/embedders/hex2vec/test_files/poz_8_features.parquet`

 * *Files identical despite different names*

### Comparing `srai-0.1.1/tests/embedders/hex2vec/test_files/poz_8_joint.parquet` & `srai-0.1.4/tests/embedders/hex2vec/test_files/poz_8_joint.parquet`

 * *Files identical despite different names*

### Comparing `srai-0.1.1/tests/embedders/hex2vec/test_files/poz_8_regions.parquet` & `srai-0.1.4/tests/embedders/hex2vec/test_files/poz_8_regions.parquet`

 * *Files identical despite different names*

### Comparing `srai-0.1.1/tests/embedders/hex2vec/test_files/poz_8_result.parquet` & `srai-0.1.4/tests/embedders/hex2vec/test_files/poz_8_result.parquet`

 * *Files identical despite different names*

### Comparing `srai-0.1.1/tests/embedders/hex2vec/test_files/wro_9_features.parquet` & `srai-0.1.4/tests/embedders/hex2vec/test_files/wro_9_features.parquet`

 * *Files identical despite different names*

### Comparing `srai-0.1.1/tests/embedders/hex2vec/test_files/wro_9_joint.parquet` & `srai-0.1.4/tests/embedders/hex2vec/test_files/wro_9_joint.parquet`

 * *Files identical despite different names*

### Comparing `srai-0.1.1/tests/embedders/hex2vec/test_files/wro_9_regions.parquet` & `srai-0.1.4/tests/embedders/hex2vec/test_files/wro_9_regions.parquet`

 * *Files identical despite different names*

### Comparing `srai-0.1.1/tests/embedders/hex2vec/test_files/wro_9_result.parquet` & `srai-0.1.4/tests/embedders/hex2vec/test_files/wro_9_result.parquet`

 * *Files identical despite different names*

### Comparing `srai-0.1.1/tests/embedders/hex2vec/test_model.py` & `srai-0.1.4/tests/embedders/hex2vec/test_model.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.1/tests/embedders/hex2vec/test_neighbour_dataset.py` & `srai-0.1.4/tests/embedders/hex2vec/test_neighbour_dataset.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.1/tests/embedders/test_contextual_count_embedder.py` & `srai-0.1.4/tests/embedders/test_contextual_count_embedder.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.1/tests/embedders/test_count_embedder.py` & `srai-0.1.4/tests/embedders/test_count_embedder.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.1/tests/embedders/test_gtfs2vec_embedder.py` & `srai-0.1.4/tests/embedders/test_gtfs2vec_embedder.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.1/tests/embedders/test_highway2vec_embedder.py` & `srai-0.1.4/tests/embedders/test_highway2vec_embedder.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.1/tests/joiners/conftest.py` & `srai-0.1.4/tests/joiners/conftest.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.1/tests/joiners/test_intersection_joiner.py` & `srai-0.1.4/tests/joiners/test_intersection_joiner.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.1/tests/loaders/conftest.py` & `srai-0.1.4/tests/loaders/conftest.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.1/tests/loaders/osm_loaders/conftest.py` & `srai-0.1.4/tests/loaders/osm_loaders/conftest.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.1/tests/loaders/osm_loaders/filters/popular_filter_example.json` & `srai-0.1.4/tests/loaders/osm_loaders/filters/popular_filter_example.json`

 * *Files identical despite different names*

### Comparing `srai-0.1.1/tests/loaders/osm_loaders/filters/test_merge_filter_types.py` & `srai-0.1.4/tests/loaders/osm_loaders/filters/test_merge_filter_types.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.1/tests/loaders/osm_loaders/filters/test_popular_tag_downloader.py` & `srai-0.1.4/tests/loaders/osm_loaders/filters/test_popular_tag_downloader.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.1/tests/loaders/osm_loaders/test_files/aa756ad3a961ba6d9da46c712b0d979d0c7d4768641ceea7409b287e2d18a48f.osm.pbf` & `srai-0.1.4/tests/loaders/osm_loaders/test_files/aa756ad3a961ba6d9da46c712b0d979d0c7d4768641ceea7409b287e2d18a48f.osm.pbf`

 * *Files identical despite different names*

### Comparing `srai-0.1.1/tests/loaders/osm_loaders/test_files/d17f922ed15e9609013a6b895e1e7af2d49158f03586f2c675d17b760af3452e.osm.pbf` & `srai-0.1.4/tests/loaders/osm_loaders/test_files/d17f922ed15e9609013a6b895e1e7af2d49158f03586f2c675d17b760af3452e.osm.pbf`

 * *Files identical despite different names*

### Comparing `srai-0.1.1/tests/loaders/osm_loaders/test_files/eb2848d259345ce7dfe8af34fd1ab24503bb0b952e04e872c87c55550fa50fbf.osm.pbf` & `srai-0.1.4/tests/loaders/osm_loaders/test_files/eb2848d259345ce7dfe8af34fd1ab24503bb0b952e04e872c87c55550fa50fbf.osm.pbf`

 * *Files identical despite different names*

### Comparing `srai-0.1.1/tests/loaders/osm_loaders/test_files/poland.geojson` & `srai-0.1.4/tests/loaders/osm_loaders/test_files/poland.geojson`

 * *Files identical despite different names*

### Comparing `srai-0.1.1/tests/loaders/osm_loaders/test_files/south_africa_without_islands.geojson` & `srai-0.1.4/tests/loaders/osm_loaders/test_files/south_africa_without_islands.geojson`

 * *Files identical despite different names*

### Comparing `srai-0.1.1/tests/loaders/osm_loaders/test_osm_online_loader.py` & `srai-0.1.4/tests/loaders/osm_loaders/test_osm_online_loader.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.1/tests/loaders/osm_loaders/test_osm_pbf_loader.py` & `srai-0.1.4/tests/loaders/osm_loaders/test_osm_pbf_loader.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.1/tests/loaders/osm_loaders/test_osm_tile_data_collector.py` & `srai-0.1.4/tests/loaders/osm_loaders/test_osm_tile_data_collector.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.1/tests/loaders/osm_loaders/test_osm_tile_loader.py` & `srai-0.1.4/tests/loaders/osm_loaders/test_osm_tile_loader.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.1/tests/loaders/osm_way_loader/files/1f0fafc11b7ab7aea5124d2a89c634fc.pkl` & `srai-0.1.4/tests/loaders/osm_way_loader/files/1f0fafc11b7ab7aea5124d2a89c634fc.pkl`

 * *Files identical despite different names*

### Comparing `srai-0.1.1/tests/loaders/osm_way_loader/files/20c9119c4dcc233c37382696f483239e.pkl` & `srai-0.1.4/tests/loaders/osm_way_loader/files/20c9119c4dcc233c37382696f483239e.pkl`

 * *Files identical despite different names*

### Comparing `srai-0.1.1/tests/loaders/osm_way_loader/files/4310fe8d3c435f2a83fac55fc79f9166.pkl` & `srai-0.1.4/tests/loaders/osm_way_loader/files/4310fe8d3c435f2a83fac55fc79f9166.pkl`

 * *Files identical despite different names*

### Comparing `srai-0.1.1/tests/loaders/osm_way_loader/files/7be5387a594790ea98ef0bd07bfcb58e.pkl` & `srai-0.1.4/tests/loaders/osm_way_loader/files/7be5387a594790ea98ef0bd07bfcb58e.pkl`

 * *Files identical despite different names*

### Comparing `srai-0.1.1/tests/loaders/osm_way_loader/files/97e1befc51831ce8f8f482077f5042f2.pkl` & `srai-0.1.4/tests/loaders/osm_way_loader/files/97e1befc51831ce8f8f482077f5042f2.pkl`

 * *Files identical despite different names*

### Comparing `srai-0.1.1/tests/loaders/osm_way_loader/files/eebaa127015feec3e21491d4c32e4efe.pkl` & `srai-0.1.4/tests/loaders/osm_way_loader/files/eebaa127015feec3e21491d4c32e4efe.pkl`

 * *Files identical despite different names*

### Comparing `srai-0.1.1/tests/loaders/osm_way_loader/test_osm_way_loader.py` & `srai-0.1.4/tests/loaders/osm_way_loader/test_osm_way_loader.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.1/tests/loaders/test_files/example.parquet` & `srai-0.1.4/tests/loaders/test_files/example.parquet`

 * *Files identical despite different names*

### Comparing `srai-0.1.1/tests/loaders/test_geoparquet_loader.py` & `srai-0.1.4/tests/loaders/test_geoparquet_loader.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.1/tests/loaders/test_gtfs_loader.py` & `srai-0.1.4/tests/loaders/test_gtfs_loader.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.1/tests/miscellaneous/test_optional_dependencies.py` & `srai-0.1.4/tests/miscellaneous/test_optional_dependencies.py`

 * *Files 7% similar despite different names*

```diff
@@ -64,29 +64,29 @@
     sys.meta_path.remove(d)
 
 
 def _test_voronoi() -> None:
     import geopandas as gpd
     from shapely.geometry import Point
 
-    from srai.regionizers import VoronoiRegionizer
+    from srai.regionalizers import VoronoiRegionalizer
 
     seeds_gdf = gpd.GeoDataFrame(
         {
             GEOMETRY_COLUMN: [
                 Point(17.014997869227177, 51.09919872601259),
                 Point(16.935542631959215, 51.09380600286582),
                 Point(16.900425, 51.1162552343),
                 Point(16.932700, 51.166251),
             ]
         },
         index=[1, 2, 3, 4],
         crs=WGS84_CRS,
     )
-    VoronoiRegionizer(seeds=seeds_gdf)
+    VoronoiRegionalizer(seeds=seeds_gdf)
 
 
 def _test_plotting() -> None:
     from srai.plotting import folium_wrapper, plotly_wrapper
 
     folium_wrapper.plot_regions(_get_regions_gdf())
     plotly_wrapper.plot_regions(_get_regions_gdf(), return_plot=True)
@@ -98,17 +98,17 @@
     Highway2VecEmbedder()
     GTFS2VecEmbedder()
     Hex2VecEmbedder()
 
 
 def _test_osm() -> None:
     from srai.loaders import OSMOnlineLoader, OSMPbfLoader, OSMTileLoader, OSMWayLoader
-    from srai.regionizers import AdministrativeBoundaryRegionizer
+    from srai.regionalizers import AdministrativeBoundaryRegionalizer
 
-    AdministrativeBoundaryRegionizer(2)
+    AdministrativeBoundaryRegionalizer(2)
     OSMPbfLoader()
     OSMOnlineLoader()
     OSMWayLoader("drive")
     OSMTileLoader("https://tile.openstreetmap.de", 9)
 
 
 def _test_gtfs() -> None:
```

### Comparing `srai-0.1.1/tests/neighbourhoods/h3/test_no_regions.py` & `srai-0.1.4/tests/neighbourhoods/h3/test_no_regions.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.1/tests/neighbourhoods/h3/test_with_regions.py` & `srai-0.1.4/tests/neighbourhoods/h3/test_with_regions.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.1/tests/neighbourhoods/test_adjacency_neighbourhood.py` & `srai-0.1.4/tests/neighbourhoods/test_adjacency_neighbourhood.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.1/tests/neighbourhoods/test_neighbourhood.py` & `srai-0.1.4/tests/neighbourhoods/test_neighbourhood.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.1/tests/regionizers/conftest.py` & `srai-0.1.4/tests/regionalizers/conftest.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Conftest for Regionizers."""
+"""Conftest for Regionalizers."""
 
 import geopandas as gpd
 import pytest
 from shapely import geometry
 
 from srai.constants import GEOMETRY_COLUMN, WGS84_CRS
```

### Comparing `srai-0.1.1/tests/regionizers/test_administrative_boundary_regionizer.py` & `srai-0.1.4/tests/regionalizers/test_administrative_boundary_regionalizer.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-"""Voronoi regionizer tests."""
+"""Voronoi regionalizer tests."""
 from contextlib import nullcontext as does_not_raise
 from typing import Any, Union
 
 import geopandas as gpd
 import pytest
 from overpass import API
 from pytest_mock import MockerFixture
 from shapely.geometry import Point, box
 
 from srai.constants import GEOMETRY_COLUMN, WGS84_CRS
-from srai.regionizers import AdministrativeBoundaryRegionizer
+from srai.regionalizers import AdministrativeBoundaryRegionalizer
 from srai.utils import merge_disjointed_gdf_geometries
 
 bbox = box(minx=-180, maxx=180, miny=-90, maxy=90)
 bbox_gdf = gpd.GeoDataFrame({GEOMETRY_COLUMN: [bbox]}, crs=WGS84_CRS)
 
 
 @pytest.mark.parametrize(  # type: ignore
@@ -37,28 +37,28 @@
 )
 def test_admin_level(
     admin_level: int,
     expectation: Any,
 ) -> None:
     """Test checks if illegal admin_level is disallowed."""
     with expectation:
-        AdministrativeBoundaryRegionizer(admin_level=admin_level)
+        AdministrativeBoundaryRegionalizer(admin_level=admin_level)
 
 
 def test_empty_gdf_attribute_error(gdf_empty) -> None:  # type: ignore
     """Test checks if empty GeoDataFrames are disallowed."""
     with pytest.raises(AttributeError):
-        abr = AdministrativeBoundaryRegionizer(admin_level=4)
+        abr = AdministrativeBoundaryRegionalizer(admin_level=4)
         abr.transform(gdf_empty)
 
 
 def test_no_crs_gdf_value_error(gdf_no_crs) -> None:  # type: ignore
     """Test checks if GeoDataFrames without crs are disallowed."""
     with pytest.raises(ValueError):
-        abr = AdministrativeBoundaryRegionizer(admin_level=4)
+        abr = AdministrativeBoundaryRegionalizer(admin_level=4)
         abr.transform(gdf=gdf_no_crs)
 
 
 @pytest.fixture  # type: ignore
 def mock_overpass_api(mocker: MockerFixture) -> None:
     """Mock overpass API."""
     mocker.patch.object(API, "get", return_value={"elements": [{"type": "relation", "id": 2137}]})
@@ -81,15 +81,15 @@
     ],
 )
 def test_empty_region_full_bounding_box(toposimplify: Union[bool, float], request: Any) -> None:
     """Test checks if empty region fills required bounding box."""
     request.getfixturevalue("mock_overpass_api")
     request_bbox = box(minx=0, miny=0, maxx=2, maxy=2)
     request_bbox_gdf = gpd.GeoDataFrame({GEOMETRY_COLUMN: [request_bbox]}, crs=WGS84_CRS)
-    abr = AdministrativeBoundaryRegionizer(
+    abr = AdministrativeBoundaryRegionalizer(
         admin_level=4, return_empty_region=True, toposimplify=toposimplify
     )
     result_gdf = abr.transform(gdf=request_bbox_gdf)
     assert merge_disjointed_gdf_geometries(result_gdf).difference(request_bbox).is_empty
     assert "EMPTY" in result_gdf.index
 
 
@@ -105,15 +105,15 @@
     ],
 )
 def test_no_empty_region_full_bounding_box(toposimplify: Union[bool, float], request: Any) -> None:
     """Test checks if no empty region is generated when not needed."""
     request.getfixturevalue("mock_overpass_api")
     request_bbox = box(minx=0, miny=0, maxx=1, maxy=1)
     request_bbox_gdf = gpd.GeoDataFrame({GEOMETRY_COLUMN: [request_bbox]}, crs=WGS84_CRS)
-    abr = AdministrativeBoundaryRegionizer(
+    abr = AdministrativeBoundaryRegionalizer(
         admin_level=2, return_empty_region=True, toposimplify=toposimplify
     )
     result_gdf = abr.transform(gdf=request_bbox_gdf)
     assert merge_disjointed_gdf_geometries(result_gdf).difference(request_bbox).is_empty
     assert "EMPTY" not in result_gdf.index
 
 
@@ -129,15 +129,15 @@
     ],
 )
 def test_points_in_result(toposimplify: Union[bool, float], request: Any) -> None:
     """Test checks case when points are in a requested region."""
     request.getfixturevalue("mock_overpass_api")
     request_gdf = gpd.GeoDataFrame({GEOMETRY_COLUMN: [Point(0.5, 0.5)]}, crs=WGS84_CRS)
 
-    abr = AdministrativeBoundaryRegionizer(
+    abr = AdministrativeBoundaryRegionalizer(
         admin_level=2, return_empty_region=False, clip_regions=False, toposimplify=toposimplify
     )
 
     result_gdf = abr.transform(gdf=request_gdf)
     assert request_gdf.geometry[0].covered_by(result_gdf.geometry[0])
 
 
@@ -155,15 +155,15 @@
 def test_toposimplify_on_real_data(toposimplify: Union[float, bool]) -> None:
     """Test if toposimplify usage covers an entire region."""
     madagascar_bbox = box(
         minx=43.2541870461, miny=-25.6014344215, maxx=50.4765368996, maxy=-12.0405567359
     )
     madagascar_bbox_gdf = gpd.GeoDataFrame({GEOMETRY_COLUMN: [madagascar_bbox]}, crs=WGS84_CRS)
 
-    abr = AdministrativeBoundaryRegionizer(
+    abr = AdministrativeBoundaryRegionalizer(
         admin_level=4, return_empty_region=True, toposimplify=toposimplify
     )
     madagascar_result_gdf = abr.transform(gdf=madagascar_bbox_gdf)
     assert (
         merge_disjointed_gdf_geometries(madagascar_result_gdf).difference(madagascar_bbox).is_empty
     )
 
@@ -178,15 +178,17 @@
 def test_regions_not_found_on_real_data(return_empty_region: bool) -> None:
     """Test if warns when can't find any regions."""
     null_island_region = box(minx=0, miny=0, maxx=0.1, maxy=0.1)
     null_island_region_gdf = gpd.GeoDataFrame(
         {GEOMETRY_COLUMN: [null_island_region]}, crs=WGS84_CRS
     )
 
-    abr = AdministrativeBoundaryRegionizer(admin_level=10, return_empty_region=return_empty_region)
+    abr = AdministrativeBoundaryRegionalizer(
+        admin_level=10, return_empty_region=return_empty_region
+    )
 
     with pytest.warns(RuntimeWarning):
         madagascar_result_gdf = abr.transform(gdf=null_island_region_gdf)
 
     if return_empty_region:
         assert (
             merge_disjointed_gdf_geometries(madagascar_result_gdf)
```

### Comparing `srai-0.1.1/tests/regionizers/test_h3_regionizer.py` & `srai-0.1.4/tests/regionalizers/test_h3_regionalizer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-"""Tests for H3Regionizer."""
+"""Tests for H3Regionalizer."""
 from contextlib import nullcontext as does_not_raise
 from typing import TYPE_CHECKING, Any, List
 from unittest import TestCase
 
 import pytest
 
 from srai.constants import GEOMETRY_COLUMN
-from srai.regionizers import H3Regionizer
+from srai.regionalizers import H3Regionalizer
 
 if TYPE_CHECKING:
     import geopandas as gpd
 
 
 ut = TestCase()
 H3_RESOLUTION = 3
@@ -54,15 +54,15 @@
     gdf_fixture: str,
     expected_h3_indexes_fixture: str,
     resolution: int,
     buffer: bool,
     expectation: Any,
     request: Any,
 ) -> None:
-    """Test transform of H3Regionizer."""
+    """Test transform of H3Regionalizer."""
     gdf: gpd.GeoDataFrame = request.getfixturevalue(gdf_fixture)
     h3_indexes: List[str] = request.getfixturevalue(expected_h3_indexes_fixture)
     with expectation:
-        gdf_h3 = H3Regionizer(resolution, buffer=buffer).transform(gdf)
+        gdf_h3 = H3Regionalizer(resolution, buffer=buffer).transform(gdf)
 
         ut.assertCountEqual(first=gdf_h3.index.to_list(), second=h3_indexes)
         assert GEOMETRY_COLUMN in gdf_h3
```

### Comparing `srai-0.1.1/tests/regionizers/test_s2_regionizer.py` & `srai-0.1.4/tests/regionalizers/test_s2_regionalizer.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-"""Tests for H3Regionizer."""
+"""Tests for H3Regionalizer."""
 from contextlib import nullcontext as does_not_raise
 from typing import TYPE_CHECKING, Any, List
 from unittest import TestCase
 
 import pytest
 
 from srai.constants import GEOMETRY_COLUMN
-from srai.regionizers import S2Regionizer
+from srai.regionalizers import S2Regionalizer
 
 if TYPE_CHECKING:
     import geopandas as gpd
 
 ut = TestCase()
 S2_RESOLUTION = 7
 
@@ -47,15 +47,15 @@
 def test_transform(
     gdf_fixture: str,
     expected_s2_indexes_fixture: str,
     resolution: int,
     expectation: Any,
     request: Any,
 ) -> None:
-    """Test transform of H3Regionizer."""
+    """Test transform of H3Regionalizer."""
     gdf: gpd.GeoDataFrame = request.getfixturevalue(gdf_fixture)
     s2_indexes: List[str] = request.getfixturevalue(expected_s2_indexes_fixture)
     with expectation:
-        gdf_s2 = S2Regionizer(resolution).transform(gdf)
+        gdf_s2 = S2Regionalizer(resolution).transform(gdf)
 
         ut.assertCountEqual(first=gdf_s2.index.to_list(), second=s2_indexes)
         assert GEOMETRY_COLUMN in gdf_s2
```

### Comparing `srai-0.1.1/tests/regionizers/test_slippy_map_regionizer.py` & `srai-0.1.4/tests/regionalizers/test_slippy_map_regionalizer.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-"""Tests for SlippyMapRegionizer class."""
+"""Tests for SlippyMapRegionalizer class."""
 from contextlib import nullcontext as does_not_raise
 from typing import Any
 
 import geopandas as gpd
 import pytest
 from shapely.geometry import Polygon
 
 from srai.constants import WGS84_CRS
-from srai.regionizers import SlippyMapRegionizer
+from srai.regionalizers import SlippyMapRegionalizer
 
 ZOOM = 11
 
 
 @pytest.fixture  # type: ignore
 def gdf() -> gpd.GeoDataFrame:
     """GeoDataFrame approximating Warsaw bounds."""
@@ -25,22 +25,22 @@
         ],
     )
     gdf = gpd.GeoDataFrame({"geometry": [polygon]}, crs=WGS84_CRS)
     return gdf
 
 
 @pytest.fixture  # type: ignore
-def regionizer() -> SlippyMapRegionizer:
-    """Regionizer fixture."""
-    return SlippyMapRegionizer(zoom=ZOOM)
+def regionalizer() -> SlippyMapRegionalizer:
+    """Regionalizer fixture."""
+    return SlippyMapRegionalizer(zoom=ZOOM)
 
 
-def test_transform(regionizer: SlippyMapRegionizer, gdf: gpd.GeoDataFrame) -> None:
+def test_transform(regionalizer: SlippyMapRegionalizer, gdf: gpd.GeoDataFrame) -> None:
     """Test returned regions."""
-    regions = regionizer.transform(gdf)
+    regions = regionalizer.transform(gdf)
 
     assert regions.shape[0] == 6, f"Invalid length {regions.shape[0]}"
     for x, y in zip([1120, 1119, 1120, 1121, 1120, 1121], [683, 684, 684, 684, 685, 685]):
         expected_id = f"{x}_{y}_{ZOOM}"
         assert expected_id in regions.index, f"{expected_id} not in index but expected"
         assert regions.loc[expected_id]["x"] == x
         assert regions.loc[expected_id]["y"] == y
@@ -55,38 +55,38 @@
         (19, does_not_raise()),
         (20, pytest.raises(ValueError)),
     ],
 )
 def test_zoom_check(z: int, expectation: Any) -> None:
     """Test value checks."""
     with expectation:
-        SlippyMapRegionizer(zoom=z)
+        SlippyMapRegionalizer(zoom=z)
 
 
-def test_coordinates_cast(regionizer: SlippyMapRegionizer) -> None:
+def test_coordinates_cast(regionalizer: SlippyMapRegionalizer) -> None:
     """Test if coordinates_to_x_y gives proper x and y value."""
     # given
     latitude, longitude = 51, 16.8
-    regionizer.zoom = 10
+    regionalizer.zoom = 10
 
     # when
-    x, y = regionizer._coordinates_to_x_y(latitude=latitude, longitude=longitude)
+    x, y = regionalizer._coordinates_to_x_y(latitude=latitude, longitude=longitude)
 
     # then
     assert x == 559
     assert y == 342
 
 
 def test_x_y_to_coordinates_should_be_inverse_to_coordinates_to_x_y(
-    regionizer: SlippyMapRegionizer,
+    regionalizer: SlippyMapRegionalizer,
 ) -> None:
     """Test if `x_y_to_coordinates` is reversible with `coordinates_to_x_y`."""
     # given
     x, y = 50, 100
 
     # when
-    latitude, longitude = regionizer._x_y_to_coordinates(x, y)
-    x_reverse, y_reverse = regionizer._coordinates_to_x_y(latitude, longitude)
+    latitude, longitude = regionalizer._x_y_to_coordinates(x, y)
+    x_reverse, y_reverse = regionalizer._coordinates_to_x_y(latitude, longitude)
 
     # then
     assert x_reverse == x
     assert y_reverse == y
```

### Comparing `srai-0.1.1/tests/regionizers/test_voronoi_regionizer.py` & `srai-0.1.4/tests/regionalizers/test_voronoi_regionalizer.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,69 +1,69 @@
-"""Voronoi regionizer tests."""
+"""Voronoi regionalizer tests."""
 from typing import Any
 
 import geopandas as gpd
 import numpy as np
 import pytest
 from shapely.geometry import Point, Polygon
 
 from srai.constants import GEOMETRY_COLUMN, WGS84_CRS
-from srai.regionizers import VoronoiRegionizer
-from srai.regionizers._spherical_voronoi import generate_voronoi_regions
+from srai.regionalizers import VoronoiRegionalizer
+from srai.regionalizers._spherical_voronoi import generate_voronoi_regions
 from srai.utils import merge_disjointed_gdf_geometries
 
 
 def test_empty_gdf_attribute_error(gdf_empty: gpd.GeoDataFrame) -> None:
     """Test checks if empty GeoDataFrames are disallowed."""
     with pytest.raises(AttributeError):
-        VoronoiRegionizer(seeds=gdf_empty)
+        VoronoiRegionalizer(seeds=gdf_empty)
 
 
 def test_no_crs_gdf_value_error(
     gdf_earth_poles: gpd.GeoDataFrame, gdf_no_crs: gpd.GeoDataFrame
 ) -> None:
     """Test checks if GeoDataFrames without crs are disallowed."""
     with pytest.raises(ValueError):
-        vr = VoronoiRegionizer(seeds=gdf_earth_poles)
+        vr = VoronoiRegionalizer(seeds=gdf_earth_poles)
         vr.transform(gdf=gdf_no_crs)
 
 
 def test_duplicate_seeds_value_error() -> None:
     """Test checks if duplicate points are disallowed."""
     with pytest.raises(ValueError):
         seeds_gdf = gpd.GeoDataFrame(
             {GEOMETRY_COLUMN: [Point(0, 0), Point(0, 0), Point(-1, -1), Point(2, 2)]},
             index=[1, 2, 3, 4],
             crs=WGS84_CRS,
         )
-        VoronoiRegionizer(seeds=seeds_gdf)
+        VoronoiRegionalizer(seeds=seeds_gdf)
 
 
 def test_single_seed_region() -> None:
     """Test checks if single seed is disallowed."""
     with pytest.raises(ValueError):
         seeds_gdf = gpd.GeoDataFrame(
             {GEOMETRY_COLUMN: [Point(0, 0)]},
             index=[1],
             crs=WGS84_CRS,
         )
-        VoronoiRegionizer(seeds=seeds_gdf)
+        VoronoiRegionalizer(seeds=seeds_gdf)
 
 
 def test_single_seed_algorithm_error() -> None:
     """Test checks if single seed is disallowed."""
     with pytest.raises(ValueError):
         generate_voronoi_regions(seeds=[Point(0, 0)], max_meters_between_points=10_000)
 
 
 def test_multiple_seeds_regions(
     gdf_earth_poles: gpd.GeoDataFrame, gdf_earth_bbox: gpd.GeoDataFrame, earth_bbox: Polygon
 ) -> None:
     """Test checks if regions are generated correctly."""
-    vr = VoronoiRegionizer(seeds=gdf_earth_poles)
+    vr = VoronoiRegionalizer(seeds=gdf_earth_poles)
     result_gdf = vr.transform(gdf=gdf_earth_bbox)
     assert len(result_gdf.index) == 6
     assert merge_disjointed_gdf_geometries(result_gdf).difference(earth_bbox).is_empty
 
 
 def test_big_number_of_seeds_regions(gdf_earth_bbox: gpd.GeoDataFrame, earth_bbox: Polygon) -> None:
     """Test checks if regions are generated correctly and multiprocessing working."""
@@ -78,15 +78,15 @@
 
     random_points_gdf = gpd.GeoDataFrame(
         {GEOMETRY_COLUMN: pts},
         index=list(range(len(pts))),
         crs=WGS84_CRS,
     )
 
-    vr = VoronoiRegionizer(seeds=random_points_gdf)
+    vr = VoronoiRegionalizer(seeds=random_points_gdf)
     result_gdf = vr.transform(gdf=gdf_earth_bbox)
     assert len(result_gdf.index) == number_of_points
     assert merge_disjointed_gdf_geometries(result_gdf).difference(earth_bbox).is_empty
 
 
 def test_four_close_seed_region(gdf_earth_bbox: gpd.GeoDataFrame, earth_bbox: Polygon) -> None:
     """Test checks if four close seeds are properly evaluated."""
@@ -98,23 +98,23 @@
                 Point(16.900425, 51.1162552343),
                 Point(16.932700, 51.166251),
             ]
         },
         index=[1, 2, 3, 4],
         crs=WGS84_CRS,
     )
-    vr = VoronoiRegionizer(seeds=seeds_gdf)
+    vr = VoronoiRegionalizer(seeds=seeds_gdf)
     result_gdf = vr.transform(gdf=gdf_earth_bbox)
     assert len(result_gdf.index) == 4
     assert merge_disjointed_gdf_geometries(result_gdf).difference(earth_bbox).is_empty
 
 
 def test_default_parameter(gdf_earth_poles: gpd.GeoDataFrame, earth_bbox: Polygon) -> None:
     """Test checks if regions are generated correctly with a default mask."""
-    vr = VoronoiRegionizer(seeds=gdf_earth_poles)
+    vr = VoronoiRegionalizer(seeds=gdf_earth_poles)
     result_gdf = vr.transform(gdf=None)
     assert len(result_gdf.index) == 6
     assert merge_disjointed_gdf_geometries(result_gdf).difference(earth_bbox).is_empty
 
 
 @pytest.mark.parametrize(  # type: ignore
     "gdf_fixture",
@@ -127,10 +127,10 @@
 def test_clipping_parameter(
     gdf_fixture: str,
     request: Any,
 ) -> None:
     """Test checks if regions are clipped correctly with a provided mask."""
     gdf: gpd.GeoDataFrame = request.getfixturevalue(gdf_fixture)
     gdf_earth_poles: gpd.GeoDataFrame = request.getfixturevalue("gdf_earth_poles")
-    vr = VoronoiRegionizer(seeds=gdf_earth_poles)
+    vr = VoronoiRegionalizer(seeds=gdf_earth_poles)
     result_gdf = vr.transform(gdf=gdf)
     assert merge_disjointed_gdf_geometries(result_gdf).difference(gdf.iloc[0].geometry).is_empty
```

### Comparing `srai-0.1.1/PKG-INFO` & `srai-0.1.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Metadata-Version: 2.1
 Name: srai
-Version: 0.1.1
+Version: 0.1.4
 Summary: A set of python modules for geospatial machine learning and data mining
-Author-Email: srai <spatialrepresentationsforai@gmail.com>
+Author: Piotr Gramacki, Kacper Leśniara, Kamil Raczycki, Szymon Woźniak
+Author-Email: SRAI Lab <spatialrepresentationsforai@gmail.com>
 License: Apache-2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: GIS
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
@@ -45,15 +46,15 @@
 Requires-Dist: pymap3d; extra == "voronoi"
 Requires-Dist: haversine; extra == "voronoi"
 Requires-Dist: spherical-geometry; extra == "voronoi"
 Requires-Dist: gtfs-kit; extra == "gtfs"
 Requires-Dist: folium; extra == "plotting"
 Requires-Dist: mapclassify; extra == "plotting"
 Requires-Dist: plotly; extra == "plotting"
-Requires-Dist: kaleido; extra == "plotting"
+Requires-Dist: kaleido<=0.2.1; extra == "plotting"
 Requires-Dist: pytorch-lightning; extra == "torch"
 Requires-Dist: torch; extra == "torch"
 Requires-Dist: srai[gtfs,osm,plotting,torch,voronoi]; extra == "all"
 Provides-Extra: osm
 Provides-Extra: voronoi
 Provides-Extra: gtfs
 Provides-Extra: plotting
@@ -89,35 +90,45 @@
     </a>
 </p>
 
 # Spatial Representations for Artificial Intelligence
 
 <p align="center">⚠️🚧 This library is under HEAVY development. Expect breaking changes between <i>minor</i> versions 🚧⚠️</p>
 
-<p align="center">💬 Feel free to open an issue if you find anything confusing or not working 🗨️</p>
+<p align="center">💬 Feel free to open an issue if you find anything confusing or not working 💬</p>
 
-Project **Spatial Representations for Artificial Intelligence** (`srai`) aims to provide simple and efficient solutions to geospatial problems that are accessible to everybody and reusable in various contexts where geospatial data can be used. It is a Python module integrating many geo-related algorithms in a single package with unified API. Please see getting starded for installation and quick srart instructions.
+Project **Spatial Representations for Artificial Intelligence** (`srai`) aims to provide simple and efficient solutions to geospatial problems that are accessible to everybody and reusable in various contexts where geospatial data can be used. It is a Python module integrating many geo-related algorithms in a single package with unified API. Please see getting started for installation and quick start instructions.
+
+<p align="center">
+  <img src="https://drive.google.com/uc?export=view&id=1iyajkX81PLrel-Xmz1lQpYQvePnLoO1U"  style="max-width:600px;width:100%"/>
+</p>
 
 ## Use cases
 
 In the current state, `srai` provides the following functionalities:
 
 * **OSM data download** - downloading OpenStreetMap data for a given area using different sources
 * **OSM data processing** - processing OSM data to extract useful information (e.g. road network, buildings, POIs, etc.)
 * **GTFS processing** - extracting features from GTFS data
-* **Regionization** - splitting a given area into smaller regions using different algorithms (e.g. Uber's H3[1], Voronoi, etc.)
+* **Regionalization** - splitting a given area into smaller regions using different algorithms (e.g. Uber's H3[1], Voronoi, etc.)
 * **Embedding** - embedding regions into a vector space based on different spatial features, and using different algorithms (eg. hex2vec[2], etc.)
 * Utilities for spatial data visualization and processing
 
 For future releases, we plan to add more functionalities, such as:
 
 * **Pre-computed embeddings** - pre-computed embeddings for different regions and different embedding algorithms
 * **Full pipelines** - full pipelines for different embedding approaches, pre-configured from `srai` components
 * **Image data download and processing** - downloading and processing image data (eg. OSM tiles, etc.)
 
+### End-to-end examples
+
+Right now, `srai` provides a toolset for data download and processing sufficient to solve downstream tasks. Please see [this project](https://pwr-inf.github.io/Transfer-learning-approach-to-bicycle-sharing-systems-station-location-planning-using-OpenStreetMap/) by [@RaczeQ](https://github.com/RaczeQ), which predicts Bike Sharing System (BSS) stations' locations for a wide range of cities worldwide.
+
+For `srai` integration into full [kedro](https://kedro.org/) pipeline, see [this project](https://github.com/Calychas/highway2vec_remaster/) by [@Calychas](https://github.com/Calychas).
+
 ## Installation
 
 To install `srai` simply run:
 
 ```bash
 pip install srai
 ```
@@ -126,21 +137,23 @@
 
 ### Optional dependencies
 
 The following optional dependencies can be installed to enable additional functionality:
 
 * `srai[all]` - all optional dependencies
 * `srai[osm]` - dependencies required to download OpenStreetMap data
-* `srai[voronoi]` - dependencies to use Voronoi-based regionization method
+* `srai[voronoi]` - dependencies to use Voronoi-based regionalization method
 * `srai[gtfs]` - dependencies to process GTFS data
 * `srai[plotting]` - dependencies to plot graphs and maps
 * `srai[torch]` - dependencies to use torch-based embedders
 
 ## Usage
 
+If you prefer an interactive notebook, examples of `srai` usage are available in this [Colab Notebook](https://colab.research.google.com/drive/17z2OYZG82FZNRK86Kt-eSgbJn9m7meSH?usp=sharing)
+
 ### Downloading OSM data
 
 To download OSM data for a given area, using a set of tags use one of `OSMLoader` classes:
 
 * `OSMOnlineLoader` - downloads data from OpenStreetMap API using [osmnx](https://github.com/gboeing/osmnx) - this is faster for smaller areas or tags counts
 * `OSMPbfLoader` - loads data from automatically downloaded PBF file from [protomaps](https://protomaps.com/) - this is faster for larger areas or tags counts
 
@@ -209,70 +222,70 @@
 features[["trips_at_8", "geometry"]].explore("trips_at_8", m=folium_map)
 ```
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/srai-lab/srai/main/docs/assets/images/downloading_gtfs_data.jpg" style="max-width:600px;width:100%"/>
 </p>
 
-### Regionization
+### Regionalization
 
-Regionization is a process of dividing a given area into smaller regions. This can be done in a variety of ways:
+Regionalization is a process of dividing a given area into smaller regions. This can be done in a variety of ways:
 
-* `H3Regionizer` - regionization using [Uber's H3 library](https://github.com/uber/h3)
-* `S2Regionizer` - regionization using [Google's S2 library](https://github.com/google/s2geometry)
-* `VoronoiRegionizer` - regionization using Voronoi diagram
-* `AdministativeBoundaryRegionizer` - regionization using administrative boundaries
+* `H3Regionalizer` - regionalization using [Uber's H3 library](https://github.com/uber/h3)
+* `S2Regionalizer` - regionalization using [Google's S2 library](https://github.com/google/s2geometry)
+* `VoronoiRegionalizer` - regionalization using Voronoi diagram
+* `AdministativeBoundaryRegionalizer` - regionalization using administrative boundaries
 
 Example:
 
 ```python
-from srai.regionizers import H3Regionizer
+from srai.regionalizers import H3Regionalizer
 from srai.utils import geocode_to_region_gdf
 
 area = geocode_to_region_gdf("Berlin, Germany")
-regionizer = H3Regionizer(resolution=7)
+regionalizer = H3Regionalizer(resolution=7)
 
-regions = regionizer.transform(area)
+regions = regionalizer.transform(area)
 
 folium_map = plot_regions(area, colormap=["rgba(0,0,0,0.1)"], tiles_style="CartoDB positron")
 plot_regions(regions_gdf=regions, map=folium_map)
 ```
 
 <p align="center">
-  <img src="https://raw.githubusercontent.com/srai-lab/srai/main/docs/assets/images/regionization.jpg" style="max-width:600px;width:100%"/>
+  <img src="https://raw.githubusercontent.com/srai-lab/srai/main/docs/assets/images/regionalization.jpg" style="max-width:600px;width:100%"/>
 </p>
 
 ### Embedding
 
 Embedding is a process of mapping regions into a vector space. This can be done in a variety of ways:
 
 * `Hex2VecEmbedder` - embedding using hex2vec[1] algorithm
 * `GTFS2VecEmbedder` - embedding using GTFS2Vec[2] algorithm
 * `CountEmbedder` - embedding based on features counts
 * `ContextualCountEmbedder` - embedding based on features counts with neighbourhood context (proposed in [3])
 * `Highway2VecEmbedder` - embedding using Highway2Vec[4] algorithm
 
-All of those methods share the same API. All of them require results from `Loader` (load features), `Regionizer` (split area into regions) and `Joiner` (join features to regions) to work. An example using `CountEmbedder`:
+All of those methods share the same API. All of them require results from `Loader` (load features), `Regionalizer` (split area into regions) and `Joiner` (join features to regions) to work. An example using `CountEmbedder`:
 
 ```python
 from srai.embedders import CountEmbedder
 from srai.joiners import IntersectionJoiner
 from srai.loaders import OSMOnlineLoader
 from srai.plotting import plot_regions, plot_numeric_data
-from srai.regionizers import H3Regionizer
+from srai.regionalizers import H3Regionalizer
 from srai.utils import geocode_to_region_gdf
 
 loader = OSMOnlineLoader()
-regionizer = H3Regionizer(resolution=9)
+regionalizer = H3Regionalizer(resolution=9)
 joiner = IntersectionJoiner()
 
 query = {"amenity": "bicycle_parking"}
 area = geocode_to_region_gdf("Malmö, Sweden")
 features = loader.load(area, query)
-regions = regionizer.transform(area)
+regions = regionalizer.transform(area)
 joint = joiner.transform(regions, features)
 
 embedder = CountEmbedder()
 embeddings = embedder.transform(regions, features, joint)
 
 folium_map = plot_regions(area, colormap=["rgba(0,0,0,0.1)"], tiles_style="CartoDB positron")
 plot_numeric_data(regions, embeddings, "amenity_bicycle_parking", map=folium_map)
@@ -286,25 +299,25 @@
 
 ```python
 from srai.embedders import Hex2VecEmbedder
 from srai.joiners import IntersectionJoiner
 from srai.loaders import OSMPbfLoader
 from srai.loaders.osm_loaders.filters import HEX2VEC_FILTER
 from srai.neighbourhoods.h3_neighbourhood import H3Neighbourhood
-from srai.regionizers import H3Regionizer
+from srai.regionalizers import H3Regionalizer
 from srai.utils import geocode_to_region_gdf
 from srai.plotting import plot_regions, plot_numeric_data
 
 loader = OSMPbfLoader()
-regionizer = H3Regionizer(resolution=11)
+regionalizer = H3Regionalizer(resolution=11)
 joiner = IntersectionJoiner()
 
 area = geocode_to_region_gdf("City of London")
 features = loader.load(area, HEX2VEC_FILTER)
-regions = regionizer.transform(area)
+regions = regionalizer.transform(area)
 joint = joiner.transform(regions, features)
 
 embedder = Hex2VecEmbedder()
 neighbourhood = H3Neighbourhood(regions_gdf=regions)
 
 embedder = Hex2VecEmbedder([15, 10, 3])
 
@@ -334,18 +347,22 @@
 ## Publications
 
 Some of the methods implemented in `srai` have been published in scientific journals and conferences.
 
 1. Szymon Woźniak and Piotr Szymański. 2021. Hex2vec: Context-Aware Embedding H3 Hexagons with OpenStreetMap Tags. In Proceedings of the 4th ACM SIGSPATIAL International Workshop on AI for Geographic Knowledge Discovery (GEOAI '21). Association for Computing Machinery, New York, NY, USA, 61–71. [paper](https://doi.org/10.1145/3486635.3491076), [arXiv](https://arxiv.org/abs/2111.00970)
 2. Piotr Gramacki, Szymon Woźniak, and Piotr Szymański. 2021. Gtfs2vec: Learning GTFS Embeddings for comparing Public Transport Offer in Microregions. In Proceedings of the 1st ACM SIGSPATIAL International Workshop on Searching and Mining Large Collections of Geospatial Data (GeoSearch'21). Association for Computing Machinery, New York, NY, USA, 5–12. [paper](https://doi.org/10.1145/3486640.3491392), [arXiv](https://arxiv.org/abs/2111.00960)
 3. Kamil Raczycki and Piotr Szymański. 2021. Transfer learning approach to bicycle-sharing systems' station location planning using OpenStreetMap data. In Proceedings of the 4th ACM SIGSPATIAL International Workshop on Advances in Resilient and Intelligent Cities (ARIC '21). Association for Computing Machinery, New York, NY, USA, 1–12. [paper](https://doi.org/10.1145/3486626.3493434), [arXiv](https://arxiv.org/abs/2111.00990)
-4. Kacper Leśniara and Piotr Szymański. 2022. Highway2vec: representing OpenStreetMap microregions with respect to their road network characteristics. In Proceedings of the 5th ACM SIGSPATIAL International Workshop on AI for Geographic Knowledge Discovery (GeoAI '22). Association for Computing Machinery, New York, NY, USA, 18–29. [paper](https://doi.org/10.1145/3557918.3565865)
+4. Kacper Leśniara and Piotr Szymański. 2022. Highway2vec: representing OpenStreetMap microregions with respect to their road network characteristics. In Proceedings of the 5th ACM SIGSPATIAL International Workshop on AI for Geographic Knowledge Discovery (GeoAI '22). Association for Computing Machinery, New York, NY, USA, 18–29. [paper](https://doi.org/10.1145/3557918.3565865), [arXiv](https://arxiv.org/abs/2304.13865)
+
+## Acknowledgements
+
+We would like to thank Piotr Szymański PhD \([@niedakh](https://twitter.com/niedakh)\) for his invaluable guidance and support in the development of this library. His expertise and mentorship have been instrumental in shaping the library's design and functionality, and we are very grateful for his input.
 
 ## Citation
 
 TBD
 
 ## License
 
-This library is licensed under the [Apache Licence 2.0](https://github.com/srai-lab/srai/blob/main/LICENSE.md).
+This library is licensed under the [Apache License 2.0](https://github.com/srai-lab/srai/blob/main/LICENSE.md).
 
 The free [OpenStreetMap](https://www.openstreetmap.org/) data, which is used for the development of SRAI, is licensed under the [Open Data Commons Open Database License](https://opendatacommons.org/licenses/odbl/) (ODbL) by the [OpenStreetMap Foundation](https://osmfoundation.org/) (OSMF).
```

#### html2text {}

```diff
@@ -1,9 +1,10 @@
-Metadata-Version: 2.1 Name: srai Version: 0.1.1 Summary: A set of python
-modules for geospatial machine learning and data mining Author-Email: srai
+Metadata-Version: 2.1 Name: srai Version: 0.1.4 Summary: A set of python
+modules for geospatial machine learning and data mining Author: Piotr Gramacki,
+Kacper LeÅniara, Kamil Raczycki, Szymon WoÅºniak Author-Email: SRAI Lab
 gmail.com> License: Apache-2.0 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Topic :: Scientific/Engineering :: Artificial Intelligence Classifier: Topic ::
 Scientific/Engineering :: GIS Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
@@ -20,60 +21,72 @@
 Requires-Dist: s2 Requires-Dist: typeguard Requires-Dist: requests Requires-
 Dist: osmium; extra == "osm" Requires-Dist: osmnx; extra == "osm" Requires-
 Dist: overpass; extra == "osm" Requires-Dist: pillow; extra == "osm" Requires-
 Dist: pymap3d; extra == "voronoi" Requires-Dist: haversine; extra == "voronoi"
 Requires-Dist: spherical-geometry; extra == "voronoi" Requires-Dist: gtfs-kit;
 extra == "gtfs" Requires-Dist: folium; extra == "plotting" Requires-Dist:
 mapclassify; extra == "plotting" Requires-Dist: plotly; extra == "plotting"
-Requires-Dist: kaleido; extra == "plotting" Requires-Dist: pytorch-lightning;
-extra == "torch" Requires-Dist: torch; extra == "torch" Requires-Dist: srai
-[gtfs,osm,plotting,torch,voronoi]; extra == "all" Provides-Extra: osm Provides-
-Extra: voronoi Provides-Extra: gtfs Provides-Extra: plotting Provides-Extra:
-torch Provides-Extra: all Description-Content-Type: text/markdown
+Requires-Dist: kaleido<=0.2.1; extra == "plotting" Requires-Dist: pytorch-
+lightning; extra == "torch" Requires-Dist: torch; extra == "torch" Requires-
+Dist: srai[gtfs,osm,plotting,torch,voronoi]; extra == "all" Provides-Extra: osm
+Provides-Extra: voronoi Provides-Extra: gtfs Provides-Extra: plotting Provides-
+Extra: torch Provides-Extra: all Description-Content-Type: text/markdown
  [https://raw.githubusercontent.com/srai-lab/srai/main/docs/assets/logos/srai-
                              logo-transparent.png]
   [GitHub] [Checks] [GitHub_Workflow_Status_-_DEV] [GitHub_Workflow_Status_-
  PROD] [pre-commit.ci_status] [CodeFactor_Grade] [Codecov] [Package_version]
                 [Supported_Python_versions] [PyPI_-_Downloads]
 # Spatial Representations for Artificial Intelligence
   â ï¸ð§ This library is under HEAVY development. Expect breaking changes
                        between minor versions ð§â ï¸
  ð¬ Feel free to open an issue if you find anything confusing or not working
-                                    ð¨ï¸
+                                     ð¬
 Project **Spatial Representations for Artificial Intelligence** (`srai`) aims
 to provide simple and efficient solutions to geospatial problems that are
 accessible to everybody and reusable in various contexts where geospatial data
 can be used. It is a Python module integrating many geo-related algorithms in a
-single package with unified API. Please see getting starded for installation
-and quick srart instructions. ## Use cases In the current state, `srai`
-provides the following functionalities: * **OSM data download** - downloading
-OpenStreetMap data for a given area using different sources * **OSM data
-processing** - processing OSM data to extract useful information (e.g. road
-network, buildings, POIs, etc.) * **GTFS processing** - extracting features
-from GTFS data * **Regionization** - splitting a given area into smaller
-regions using different algorithms (e.g. Uber's H3[1], Voronoi, etc.) *
-**Embedding** - embedding regions into a vector space based on different
-spatial features, and using different algorithms (eg. hex2vec[2], etc.) *
-Utilities for spatial data visualization and processing For future releases, we
-plan to add more functionalities, such as: * **Pre-computed embeddings** - pre-
-computed embeddings for different regions and different embedding algorithms *
-**Full pipelines** - full pipelines for different embedding approaches, pre-
-configured from `srai` components * **Image data download and processing** -
-downloading and processing image data (eg. OSM tiles, etc.) ## Installation To
-install `srai` simply run: ```bash pip install srai ``` This will install the
-`srai` package and dependencies required by most of the use cases. There are
-several optional dependencies that can be installed to enable additional
-functionality. These are listed in the [optional dependencies](#optional-
-dependencies) section. ### Optional dependencies The following optional
-dependencies can be installed to enable additional functionality: * `srai[all]`
-- all optional dependencies * `srai[osm]` - dependencies required to download
-OpenStreetMap data * `srai[voronoi]` - dependencies to use Voronoi-based
-regionization method * `srai[gtfs]` - dependencies to process GTFS data * `srai
-[plotting]` - dependencies to plot graphs and maps * `srai[torch]` -
-dependencies to use torch-based embedders ## Usage ### Downloading OSM data To
+single package with unified API. Please see getting started for installation
+and quick start instructions.
+[https://drive.google.com/uc?export=view&id=1iyajkX81PLrel-Xmz1lQpYQvePnLoO1U]
+## Use cases In the current state, `srai` provides the following
+functionalities: * **OSM data download** - downloading OpenStreetMap data for a
+given area using different sources * **OSM data processing** - processing OSM
+data to extract useful information (e.g. road network, buildings, POIs, etc.) *
+**GTFS processing** - extracting features from GTFS data * **Regionalization**
+- splitting a given area into smaller regions using different algorithms (e.g.
+Uber's H3[1], Voronoi, etc.) * **Embedding** - embedding regions into a vector
+space based on different spatial features, and using different algorithms (eg.
+hex2vec[2], etc.) * Utilities for spatial data visualization and processing For
+future releases, we plan to add more functionalities, such as: * **Pre-computed
+embeddings** - pre-computed embeddings for different regions and different
+embedding algorithms * **Full pipelines** - full pipelines for different
+embedding approaches, pre-configured from `srai` components * **Image data
+download and processing** - downloading and processing image data (eg. OSM
+tiles, etc.) ### End-to-end examples Right now, `srai` provides a toolset for
+data download and processing sufficient to solve downstream tasks. Please see
+[this project](https://pwr-inf.github.io/Transfer-learning-approach-to-bicycle-
+sharing-systems-station-location-planning-using-OpenStreetMap/) by [@RaczeQ]
+(https://github.com/RaczeQ), which predicts Bike Sharing System (BSS) stations'
+locations for a wide range of cities worldwide. For `srai` integration into
+full [kedro](https://kedro.org/) pipeline, see [this project](https://
+github.com/Calychas/highway2vec_remaster/) by [@Calychas](https://github.com/
+Calychas). ## Installation To install `srai` simply run: ```bash pip install
+srai ``` This will install the `srai` package and dependencies required by most
+of the use cases. There are several optional dependencies that can be installed
+to enable additional functionality. These are listed in the [optional
+dependencies](#optional-dependencies) section. ### Optional dependencies The
+following optional dependencies can be installed to enable additional
+functionality: * `srai[all]` - all optional dependencies * `srai[osm]` -
+dependencies required to download OpenStreetMap data * `srai[voronoi]` -
+dependencies to use Voronoi-based regionalization method * `srai[gtfs]` -
+dependencies to process GTFS data * `srai[plotting]` - dependencies to plot
+graphs and maps * `srai[torch]` - dependencies to use torch-based embedders ##
+Usage If you prefer an interactive notebook, examples of `srai` usage are
+available in this [Colab Notebook](https://colab.research.google.com/drive/
+17z2OYZG82FZNRK86Kt-eSgbJn9m7meSH?usp=sharing) ### Downloading OSM data To
 download OSM data for a given area, using a set of tags use one of `OSMLoader`
 classes: * `OSMOnlineLoader` - downloads data from OpenStreetMap API using
 [osmnx](https://github.com/gboeing/osmnx) - this is faster for smaller areas or
 tags counts * `OSMPbfLoader` - loads data from automatically downloaded PBF
 file from [protomaps](https://protomaps.com/) - this is faster for larger areas
 or tags counts Example with `OSMOnlineLoader`: ```python from srai.loaders
 import OSMOnlineLoader from srai.utils import geocode_to_region_gdf from
@@ -103,71 +116,72 @@
 Path("vienna_gtfs.zip") download_file("https://transitfeeds.com/p/stadt-wien/
 888/latest/download", gtfs_file.as_posix()) loader = GTFSLoader() features =
 loader.load(gtfs_file) folium_map = plot_regions(area, colormap=["rgba
 (0,0,0,0.1)"], tiles_style="CartoDB positron") features[["trips_at_8",
 "geometry"]].explore("trips_at_8", m=folium_map) ```
    [https://raw.githubusercontent.com/srai-lab/srai/main/docs/assets/images/
                           downloading_gtfs_data.jpg]
-### Regionization Regionization is a process of dividing a given area into
-smaller regions. This can be done in a variety of ways: * `H3Regionizer` -
-regionization using [Uber's H3 library](https://github.com/uber/h3) *
-`S2Regionizer` - regionization using [Google's S2 library](https://github.com/
-google/s2geometry) * `VoronoiRegionizer` - regionization using Voronoi diagram
-* `AdministativeBoundaryRegionizer` - regionization using administrative
-boundaries Example: ```python from srai.regionizers import H3Regionizer from
-srai.utils import geocode_to_region_gdf area = geocode_to_region_gdf("Berlin,
-Germany") regionizer = H3Regionizer(resolution=7) regions =
-regionizer.transform(area) folium_map = plot_regions(area, colormap=["rgba
-(0,0,0,0.1)"], tiles_style="CartoDB positron") plot_regions
-(regions_gdf=regions, map=folium_map) ```
+### Regionalization Regionalization is a process of dividing a given area into
+smaller regions. This can be done in a variety of ways: * `H3Regionalizer` -
+regionalization using [Uber's H3 library](https://github.com/uber/h3) *
+`S2Regionalizer` - regionalization using [Google's S2 library](https://
+github.com/google/s2geometry) * `VoronoiRegionalizer` - regionalization using
+Voronoi diagram * `AdministativeBoundaryRegionalizer` - regionalization using
+administrative boundaries Example: ```python from srai.regionalizers import
+H3Regionalizer from srai.utils import geocode_to_region_gdf area =
+geocode_to_region_gdf("Berlin, Germany") regionalizer = H3Regionalizer
+(resolution=7) regions = regionalizer.transform(area) folium_map = plot_regions
+(area, colormap=["rgba(0,0,0,0.1)"], tiles_style="CartoDB positron")
+plot_regions(regions_gdf=regions, map=folium_map) ```
    [https://raw.githubusercontent.com/srai-lab/srai/main/docs/assets/images/
-                              regionization.jpg]
+                             regionalization.jpg]
 ### Embedding Embedding is a process of mapping regions into a vector space.
 This can be done in a variety of ways: * `Hex2VecEmbedder` - embedding using
 hex2vec[1] algorithm * `GTFS2VecEmbedder` - embedding using GTFS2Vec[2]
 algorithm * `CountEmbedder` - embedding based on features counts *
 `ContextualCountEmbedder` - embedding based on features counts with
 neighbourhood context (proposed in [3]) * `Highway2VecEmbedder` - embedding
 using Highway2Vec[4] algorithm All of those methods share the same API. All of
-them require results from `Loader` (load features), `Regionizer` (split area
+them require results from `Loader` (load features), `Regionalizer` (split area
 into regions) and `Joiner` (join features to regions) to work. An example using
 `CountEmbedder`: ```python from srai.embedders import CountEmbedder from
 srai.joiners import IntersectionJoiner from srai.loaders import OSMOnlineLoader
-from srai.plotting import plot_regions, plot_numeric_data from srai.regionizers
-import H3Regionizer from srai.utils import geocode_to_region_gdf loader =
-OSMOnlineLoader() regionizer = H3Regionizer(resolution=9) joiner =
-IntersectionJoiner() query = {"amenity": "bicycle_parking"} area =
-geocode_to_region_gdf("MalmÃ¶, Sweden") features = loader.load(area, query)
-regions = regionizer.transform(area) joint = joiner.transform(regions,
-features) embedder = CountEmbedder() embeddings = embedder.transform(regions,
-features, joint) folium_map = plot_regions(area, colormap=["rgba(0,0,0,0.1)"],
-tiles_style="CartoDB positron") plot_numeric_data(regions, embeddings,
-"amenity_bicycle_parking", map=folium_map) ```
+from srai.plotting import plot_regions, plot_numeric_data from
+srai.regionalizers import H3Regionalizer from srai.utils import
+geocode_to_region_gdf loader = OSMOnlineLoader() regionalizer = H3Regionalizer
+(resolution=9) joiner = IntersectionJoiner() query = {"amenity":
+"bicycle_parking"} area = geocode_to_region_gdf("MalmÃ¶, Sweden") features =
+loader.load(area, query) regions = regionalizer.transform(area) joint =
+joiner.transform(regions, features) embedder = CountEmbedder() embeddings =
+embedder.transform(regions, features, joint) folium_map = plot_regions(area,
+colormap=["rgba(0,0,0,0.1)"], tiles_style="CartoDB positron") plot_numeric_data
+(regions, embeddings, "amenity_bicycle_parking", map=folium_map) ```
    [https://raw.githubusercontent.com/srai-lab/srai/main/docs/assets/images/
                          embedding_count_embedder.jpg]
 `CountEmbedder` is a simple method, which does not require fitting. Other
 methods, such as `Hex2VecEmbedder` or `GTFS2VecEmbedder` require fitting and
 can be used in a similar way to `scikit-learn` estimators: ```python from
 srai.embedders import Hex2VecEmbedder from srai.joiners import
 IntersectionJoiner from srai.loaders import OSMPbfLoader from
 srai.loaders.osm_loaders.filters import HEX2VEC_FILTER from
 srai.neighbourhoods.h3_neighbourhood import H3Neighbourhood from
-srai.regionizers import H3Regionizer from srai.utils import
+srai.regionalizers import H3Regionalizer from srai.utils import
 geocode_to_region_gdf from srai.plotting import plot_regions, plot_numeric_data
-loader = OSMPbfLoader() regionizer = H3Regionizer(resolution=11) joiner =
+loader = OSMPbfLoader() regionalizer = H3Regionalizer(resolution=11) joiner =
 IntersectionJoiner() area = geocode_to_region_gdf("City of London") features =
-loader.load(area, HEX2VEC_FILTER) regions = regionizer.transform(area) joint =
-joiner.transform(regions, features) embedder = Hex2VecEmbedder() neighbourhood
-= H3Neighbourhood(regions_gdf=regions) embedder = Hex2VecEmbedder([15, 10, 3])
-# Option 1: fit and transform # embedder.fit(regions, features, joint,
-neighbourhood, batch_size=128) # embeddings = embedder.transform(regions,
-features, joint) # Option 2: fit_transform embeddings = embedder.fit_transform
-(regions, features, joint, neighbourhood, batch_size=128) folium_map =
-plot_regions(area, colormap=["rgba(0,0,0,0.1)"], tiles_style="CartoDB
-positron") plot_numeric_data(regions, embeddings, 0, map=folium_map) ```
+loader.load(area, HEX2VEC_FILTER) regions = regionalizer.transform(area) joint
+= joiner.transform(regions, features) embedder = Hex2VecEmbedder()
+neighbourhood = H3Neighbourhood(regions_gdf=regions) embedder = Hex2VecEmbedder
+([15, 10, 3]) # Option 1: fit and transform # embedder.fit(regions, features,
+joint, neighbourhood, batch_size=128) # embeddings = embedder.transform
+(regions, features, joint) # Option 2: fit_transform embeddings =
+embedder.fit_transform(regions, features, joint, neighbourhood, batch_size=128)
+folium_map = plot_regions(area, colormap=["rgba(0,0,0,0.1)"],
+tiles_style="CartoDB positron") plot_numeric_data(regions, embeddings, 0,
+map=folium_map) ```
    [https://raw.githubusercontent.com/srai-lab/srai/main/docs/assets/images/
                         embedding_hex2vec_embedder.jpg]
 ### Plotting, utilities and more We also provide utilities for different
 spatial operations and plotting functions adopted to data formats used in
 `srai` For a full list of available methods, please refer to the
 [documentation](https://srai-lab.github.io/srai). ## Contributing If you are
 willing to contribute to `srai`, feel free to do so! Visit [our contributing
@@ -190,14 +204,19 @@
 Resilient and Intelligent Cities (ARIC '21). Association for Computing
 Machinery, New York, NY, USA, 1â12. [paper](https://doi.org/10.1145/
 3486626.3493434), [arXiv](https://arxiv.org/abs/2111.00990) 4. Kacper LeÅniara
 and Piotr SzymaÅski. 2022. Highway2vec: representing OpenStreetMap
 microregions with respect to their road network characteristics. In Proceedings
 of the 5th ACM SIGSPATIAL International Workshop on AI for Geographic Knowledge
 Discovery (GeoAI '22). Association for Computing Machinery, New York, NY, USA,
-18â29. [paper](https://doi.org/10.1145/3557918.3565865) ## Citation TBD ##
-License This library is licensed under the [Apache Licence 2.0](https://
+18â29. [paper](https://doi.org/10.1145/3557918.3565865), [arXiv](https://
+arxiv.org/abs/2304.13865) ## Acknowledgements We would like to thank Piotr
+SzymaÅski PhD \([@niedakh](https://twitter.com/niedakh)\) for his invaluable
+guidance and support in the development of this library. His expertise and
+mentorship have been instrumental in shaping the library's design and
+functionality, and we are very grateful for his input. ## Citation TBD ##
+License This library is licensed under the [Apache License 2.0](https://
 github.com/srai-lab/srai/blob/main/LICENSE.md). The free [OpenStreetMap](https:
 //www.openstreetmap.org/) data, which is used for the development of SRAI, is
 licensed under the [Open Data Commons Open Database License](https://
 opendatacommons.org/licenses/odbl/) (ODbL) by the [OpenStreetMap Foundation]
 (https://osmfoundation.org/) (OSMF).
```

