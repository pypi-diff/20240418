# Comparing `tmp/ahelper-1.2.tar.gz` & `tmp/ahelper-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ahelper-1.2.tar", last modified: Tue Feb 15 16:13:21 2022, max compression
+gzip compressed data, was "ahelper-1.3.tar", last modified: Thu Apr 18 15:32:51 2024, max compression
```

## Comparing `ahelper-1.2.tar` & `ahelper-1.3.tar`

### file list

```diff
@@ -1,644 +1,18 @@
-drwxrwxr-x   0 jtli      (1007) jtli      (1007)        0 2022-02-15 16:13:21.000000 ahelper-1.2/
-drwxrwxr-x   0 jtli      (1007) jtli      (1007)        0 2022-02-15 16:13:21.000000 ahelper-1.2/Graph_Transformer_Networks/
--rw-------   0 jtli      (1007) jtli      (1007)     1968 2022-02-15 14:45:41.000000 ahelper-1.2/Graph_Transformer_Networks/_Graph_Transformer_Networks-master_README.md.txt
--rw-------   0 jtli      (1007) jtli      (1007)     4239 2022-02-15 14:45:41.000000 ahelper-1.2/Graph_Transformer_Networks/_Graph_Transformer_Networks-master_gcn.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)      972 2022-02-15 14:45:41.000000 ahelper-1.2/Graph_Transformer_Networks/_Graph_Transformer_Networks-master_inits.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     6096 2022-02-15 14:45:41.000000 ahelper-1.2/Graph_Transformer_Networks/_Graph_Transformer_Networks-master_main.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     6744 2022-02-15 14:45:41.000000 ahelper-1.2/Graph_Transformer_Networks/_Graph_Transformer_Networks-master_main_sparse.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     5646 2022-02-15 14:45:41.000000 ahelper-1.2/Graph_Transformer_Networks/_Graph_Transformer_Networks-master_messagepassing.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     4869 2022-02-15 14:45:41.000000 ahelper-1.2/Graph_Transformer_Networks/_Graph_Transformer_Networks-master_model.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     6119 2022-02-15 14:45:41.000000 ahelper-1.2/Graph_Transformer_Networks/_Graph_Transformer_Networks-master_model_sparse.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     3609 2022-02-15 14:45:41.000000 ahelper-1.2/Graph_Transformer_Networks/_Graph_Transformer_Networks-master_utils.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)      188 2022-02-15 16:12:02.000000 ahelper-1.2/MANIFEST.in
--rw-rw-r--   0 jtli      (1007) jtli      (1007)      905 2022-02-15 16:13:21.000000 ahelper-1.2/PKG-INFO
-drwxrwxr-x   0 jtli      (1007) jtli      (1007)        0 2022-02-15 16:13:21.000000 ahelper-1.2/ahelper/
--rw-------   0 jtli      (1007) jtli      (1007)      734 2022-02-15 16:03:41.000000 ahelper-1.2/ahelper/__init__.py
--rw-------   0 jtli      (1007) jtli      (1007)     9944 2022-02-15 09:10:12.000000 ahelper-1.2/ahelper/deepwalk.py
--rw-------   0 jtli      (1007) jtli      (1007)     4074 2022-02-15 09:10:04.000000 ahelper-1.2/ahelper/feature.py
--rw-------   0 jtli      (1007) jtli      (1007)    15521 2022-02-15 13:02:10.000000 ahelper-1.2/ahelper/layers.py
--rw-------   0 jtli      (1007) jtli      (1007)      839 2022-02-15 12:44:45.000000 ahelper-1.2/ahelper/links.py
--rw-------   0 jtli      (1007) jtli      (1007)    12614 2022-02-15 08:58:12.000000 ahelper-1.2/ahelper/snn.py
--rw-------   0 jtli      (1007) jtli      (1007)    14793 2022-02-15 12:51:08.000000 ahelper-1.2/ahelper/utils.py
-drwxrwxr-x   0 jtli      (1007) jtli      (1007)        0 2022-02-15 16:13:21.000000 ahelper-1.2/ahelper.egg-info/
--rw-rw-r--   0 jtli      (1007) jtli      (1007)      905 2022-02-15 16:13:21.000000 ahelper-1.2/ahelper.egg-info/PKG-INFO
--rw-rw-r--   0 jtli      (1007) jtli      (1007)    34017 2022-02-15 16:13:21.000000 ahelper-1.2/ahelper.egg-info/SOURCES.txt
--rw-rw-r--   0 jtli      (1007) jtli      (1007)        1 2022-02-15 16:13:21.000000 ahelper-1.2/ahelper.egg-info/dependency_links.txt
--rw-rw-r--   0 jtli      (1007) jtli      (1007)        8 2022-02-15 16:13:21.000000 ahelper-1.2/ahelper.egg-info/top_level.txt
-drwxrwxr-x   0 jtli      (1007) jtli      (1007)        0 2022-02-15 16:13:21.000000 ahelper-1.2/cogdl/
--rw-------   0 jtli      (1007) jtli      (1007)      714 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_.github_ISSUE_TEMPLATE_bug-report.md.txt
--rw-------   0 jtli      (1007) jtli      (1007)      269 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_.github_ISSUE_TEMPLATE_documentation.md.txt
--rw-------   0 jtli      (1007) jtli      (1007)      625 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_.github_ISSUE_TEMPLATE_feature-request.md.txt
--rw-------   0 jtli      (1007) jtli      (1007)      746 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_.github_ISSUE_TEMPLATE_installation.md.txt
--rw-------   0 jtli      (1007) jtli      (1007)      219 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_.github_ISSUE_TEMPLATE_question-help.md.txt
--rw-------   0 jtli      (1007) jtli      (1007)      594 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_.github_PULL_REQUEST_TEMPLATE.md.txt
--rw-------   0 jtli      (1007) jtli      (1007)    12514 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_README.md.txt
--rw-------   0 jtli      (1007) jtli      (1007)    11397 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_README_CN.md.txt
--rw-------   0 jtli      (1007) jtli      (1007)      117 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl___init__.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)    11806 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_configs.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)      293 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_data___init__.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     4868 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_data_batch.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)    32309 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_data_data.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     2023 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_data_dataloader.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     8532 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_data_dataset.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     6804 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_data_sampler.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)    13813 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_datasets_README.md.txt
--rw-------   0 jtli      (1007) jtli      (1007)     7984 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_datasets___init__.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     4375 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_datasets_customized_data.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     3196 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_datasets_gatne.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     5954 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_datasets_gcc_data.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)    13444 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_datasets_geom_data.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     5582 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_datasets_gtn_data.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     5934 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_datasets_han_data.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     5911 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_datasets_kg_data.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     5925 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_datasets_matlab_matrix.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     2380 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_datasets_oagbert_data.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     8173 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_datasets_ogb.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     6797 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_datasets_planetoid_data.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     5556 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_datasets_rd2cd_data.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     6004 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_datasets_rec_data.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     7192 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_datasets_saint_data.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)    12396 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_datasets_tu_data.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)    12655 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_experiments.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     1121 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_layers___init__.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     1875 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_layers_actgcn_layer.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)      980 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_layers_actgcnii_layer.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)      774 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_layers_actlinear_layer.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     2269 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_layers_actmlp_layer.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     1921 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_layers_actsage_layer.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)      579 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_layers_base_layer.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     6416 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_layers_deepergcn_layer.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     3692 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_layers_disengcn_layer.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     2876 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_layers_gat_layer.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     1872 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_layers_gcn_layer.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)      927 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_layers_gcnii_layer.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     1223 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_layers_gin_layer.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     1299 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_layers_gine_layer.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     1042 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_layers_han_layer.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     1091 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_layers_mixhop_layer.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     2249 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_layers_mlp_layer.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     1896 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_layers_pprgo_layer.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)    19719 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_layers_reversible_layer.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     6099 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_layers_rgcn_layer.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     2376 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_layers_sage_layer.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     4692 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_layers_saint_layer.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)      773 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_layers_se_layer.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     2303 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_layers_set2set.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)      537 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_layers_sgc_layer.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)      413 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_loggers___init__.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)      243 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_loggers_base_logger.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)      663 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_loggers_tensorboard_logger.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)      739 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_loggers_wandb_logger.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     3852 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_models_README.md.txt
--rw-------   0 jtli      (1007) jtli      (1007)     4550 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_models___init__.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)      978 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_models_base_model.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)       37 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_models_emb___init__.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     4381 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_models_emb_deepwalk.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     4630 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_models_emb_dgk.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     6010 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_models_emb_dngr.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)    16187 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_models_emb_gatne.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     4346 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_models_emb_graph2vec.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     3158 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_models_emb_grarep.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     9002 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_models_emb_hin2vec.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     2590 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_models_emb_hope.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     7305 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_models_emb_line.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     5183 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_models_emb_metapath2vec.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     5122 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_models_emb_netmf.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     7113 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_models_emb_netsmf.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     7361 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_models_emb_node2vec.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     4329 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_models_emb_prone.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     7463 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_models_emb_pronepp.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     6670 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_models_emb_pte.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     5721 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_models_emb_sdne.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     1679 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_models_emb_spectral.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)      744 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_models_nn___init__.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     2909 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_models_nn_actgcn.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     2770 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_models_nn_agc.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     9049 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_models_nn_autognn.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)    11764 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_models_nn_compgcn.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     6717 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_models_nn_correct_smooth.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     3310 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_models_nn_daegc.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     4815 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_models_nn_deepergcn.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     2397 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_models_nn_dgi.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)    15721 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_models_nn_diffpool.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     2394 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_models_nn_disengcn.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     1860 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_models_nn_drgat.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     2331 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_models_nn_drgcn.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)    23793 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_models_nn_dropedge_gcn.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     2780 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_models_nn_gae.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     3522 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_models_nn_gat.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)    11067 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_models_nn_gcc_model.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     2702 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_models_nn_gcn.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     4073 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_models_nn_gcnii.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     3579 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_models_nn_gcnmix.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     6587 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_models_nn_gdc_gcn.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     3928 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_models_nn_gin.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     5582 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_models_nn_grace.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     4050 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_models_nn_grand.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     7290 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_models_nn_graph_unet.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     6368 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_models_nn_graphsage.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     6349 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_models_nn_graphsaint.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     7270 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_models_nn_gtn.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     1778 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_models_nn_han.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     6111 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_models_nn_infograph.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)    10090 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_models_nn_lightgcn.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     1966 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_models_nn_m3s.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     1811 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_models_nn_mixhop.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     1641 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_models_nn_mlp.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     4923 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_models_nn_moe_gcn.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     7223 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_models_nn_mvgrl.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     9894 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_models_nn_patchy_san.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     3497 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_models_nn_ppnp.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     2800 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_models_nn_pprgo.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     9834 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_models_nn_revgcn.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     5407 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_models_nn_rgcn.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     9972 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_models_nn_sagn.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)      737 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_models_nn_sgc.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     4908 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_models_nn_sign.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     5063 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_models_nn_sortpool.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     8729 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_models_nn_srgcn.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     2808 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_models_nn_unsup_graphsage.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)    14704 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_oag_README.md.txt
--rw-------   0 jtli      (1007) jtli      (1007)       89 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_oag___init__.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)    23840 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_oag_bert_model.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     5603 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_oag_dual_position_bert_model.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     3816 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_oag_oagbert.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)    37401 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_oag_oagbert_metainfo.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)      688 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_oag_utils.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)      266 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_operators___init__.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     1028 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_operators_edge_softmax.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     1488 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_operators_fused_gat.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     2335 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_operators_linear.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     2127 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_operators_mhspmm.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     4212 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_operators_ops.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)      539 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_operators_sample.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)      969 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_operators_scatter_max.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     5088 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_operators_spmm.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     6613 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_options.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)    10483 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_pipelines.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)       63 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_trainer___init__.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)      141 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_trainer_controller___init__.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     2235 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_trainer_controller_data_controller.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     2559 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_trainer_controller_training_controller.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     2092 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_trainer_embed_trainer.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)    18529 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_trainer_trainer.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     2181 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_trainer_trainer_utils.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)      180 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_utils___init__.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     5233 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_utils_evaluator.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     9038 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_utils_graph_utils.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     1039 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_utils_index.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     7759 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_utils_link_prediction_utils.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     2650 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_utils_optimizer.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     3812 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_utils_ppr_utils.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     7166 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_utils_prone_utils.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     1407 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_utils_rwalk___init__.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     2874 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_utils_sampling.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     8378 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_utils_spmm_utils.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     8343 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_utils_srgcn_utils.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     2895 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_utils_transform.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     8145 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_utils_utils.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)      232 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_wrappers___init__.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     2679 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_wrappers_data_wrapper___init__.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     8762 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_wrappers_data_wrapper_base_data_wrapper.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)      292 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_wrappers_data_wrapper_graph_classification___init__.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     2103 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_wrappers_data_wrapper_graph_classification_graph_classification_dw.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     1105 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_wrappers_data_wrapper_graph_classification_graph_embedding_dw.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)      259 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_wrappers_data_wrapper_graph_classification_infograph_dw.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     1480 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_wrappers_data_wrapper_graph_classification_patchy_san_dw.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)      264 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_wrappers_data_wrapper_heterogeneous___init__.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)      419 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_wrappers_data_wrapper_heterogeneous_heterogeneous_embedding_dw.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)      462 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_wrappers_data_wrapper_heterogeneous_heterogeneous_gnn_dw.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)      428 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_wrappers_data_wrapper_heterogeneous_multiplex_embedding_dw.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)      276 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_wrappers_data_wrapper_link_prediction___init__.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     3067 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_wrappers_data_wrapper_link_prediction_embedding_link_prediction_dw.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)      510 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_wrappers_data_wrapper_link_prediction_gnn_kg_link_prediction_dw.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     3246 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_wrappers_data_wrapper_link_prediction_gnn_link_prediction_dw.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)      391 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_wrappers_data_wrapper_node_classification___init__.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     1447 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_wrappers_data_wrapper_node_classification_cluster_dw.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     2540 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_wrappers_data_wrapper_node_classification_graphsage_dw.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     3709 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_wrappers_data_wrapper_node_classification_m3s_dw.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)      764 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_wrappers_data_wrapper_node_classification_network_embedding_dw.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)      597 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_wrappers_data_wrapper_node_classification_node_classification_dw.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     4692 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_wrappers_data_wrapper_node_classification_pprgo_dw.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     3270 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_wrappers_data_wrapper_node_classification_sagn_dw.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)       95 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_wrappers_data_wrapper_pretraining___init__.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     9184 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_wrappers_data_wrapper_pretraining_gcc_dw.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     4688 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_wrappers_default_match.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     3545 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_wrappers_model_wrapper___init__.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     6298 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_wrappers_model_wrapper_base_model_wrapper.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)      172 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_wrappers_model_wrapper_clustering___init__.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     1245 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_wrappers_model_wrapper_clustering_agc_mw.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     4026 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_wrappers_model_wrapper_clustering_daegc_mw.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     1970 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_wrappers_model_wrapper_clustering_gae_mw.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)      246 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_wrappers_model_wrapper_graph_classification___init__.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     1231 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_wrappers_model_wrapper_graph_classification_graph_classification_mw.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)      818 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_wrappers_model_wrapper_graph_classification_graph_embedding_mw.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     4241 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_wrappers_model_wrapper_graph_classification_infograph_mw.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)      268 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_wrappers_model_wrapper_heterogeneous___init__.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     1498 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_wrappers_model_wrapper_heterogeneous_heterogeneous_embedding_mw.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     1696 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_wrappers_model_wrapper_heterogeneous_heterogeneous_gnn_mw.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     3199 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_wrappers_model_wrapper_heterogeneous_multiplex_embedding_mw.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)      280 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_wrappers_model_wrapper_link_prediction___init__.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     1872 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_wrappers_model_wrapper_link_prediction_embedding_link_prediction_mw.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     2663 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_wrappers_model_wrapper_link_prediction_gnn_kg_link_prediction_mw.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     3062 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_wrappers_model_wrapper_link_prediction_gnn_link_prediction_mw.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)      778 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_wrappers_model_wrapper_node_classification___init__.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     1388 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_wrappers_model_wrapper_node_classification_correct_smooth_mw.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     3329 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_wrappers_model_wrapper_node_classification_dgi_mw.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     6055 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_wrappers_model_wrapper_node_classification_gcnmix_mw.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     3958 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_wrappers_model_wrapper_node_classification_grace_mw.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     2233 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_wrappers_model_wrapper_node_classification_grand_mw.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     1440 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_wrappers_model_wrapper_node_classification_graphsage_mw.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     2871 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_wrappers_model_wrapper_node_classification_m3s_mw.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     1191 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_wrappers_model_wrapper_node_classification_mvgrl_mw.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     2493 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_wrappers_model_wrapper_node_classification_network_embedding_mw.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     1771 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_wrappers_model_wrapper_node_classification_node_classification_mw.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     1730 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_wrappers_model_wrapper_node_classification_pprgo_mw.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     2011 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_wrappers_model_wrapper_node_classification_sagn_mw.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)    18397 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_wrappers_model_wrapper_node_classification_self_auxiliary_mw.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     2366 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_wrappers_model_wrapper_node_classification_unsup_graphsage_mw.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)       97 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_wrappers_model_wrapper_pretraining___init__.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     4243 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_wrappers_model_wrapper_pretraining_gcc_mw.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)       41 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_wrappers_tools___init__.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     2808 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_wrappers_tools_memory_moco.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     9397 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_cogdl_wrappers_tools_wrapper_utils.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     6907 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_docs_source_conf.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)      936 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_examples_VRGCN_README.md.txt
--rw-------   0 jtli      (1007) jtli      (1007)     5262 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_examples_VRGCN_VRGCN.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     2973 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_examples_VRGCN_dataloder.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     3884 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_examples_VRGCN_main.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     1537 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_examples_custom_dataset.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)      967 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_examples_custom_gcn.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     2049 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_examples_cv_search.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)      906 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_examples_generate_emb.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     4433 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_examples_oagbert_calculate_paper_similarity.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     1525 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_examples_oagbert_generate_title.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)      368 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_examples_oagbert_oagbert.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)      953 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_examples_oagbert_oagbert_encode_paper.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     3315 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_examples_oagbert_oagbert_metainfo.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     3854 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_examples_oagbert_oagbert_metainfo_zh.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     3665 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_examples_oagbert_oagbert_metainfo_zh_similarity.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     1026 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_examples_ogb_arxiv_README.md.txt
--rw-------   0 jtli      (1007) jtli      (1007)     5886 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_examples_ogb_arxiv_gnn.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)      864 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_examples_ogb_products_README.md.txt
--rw-------   0 jtli      (1007) jtli      (1007)     2840 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_examples_ogb_products_gnn.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)      450 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_examples_pipeline.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)      522 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_examples_pyg_README.md.txt
--rw-------   0 jtli      (1007) jtli      (1007)     1473 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_examples_pyg_chebnet.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     2194 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_examples_pyg_dgcnn.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     1328 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_examples_pyg_gat.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     1482 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_examples_pyg_gcn.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     1434 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_examples_pyg_unet.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)      772 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_examples_quick_start.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)      422 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_examples_recommendation.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)      447 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_examples_simple_hgn_README.md.txt
--rw-------   0 jtli      (1007) jtli      (1007)     4310 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_examples_simple_hgn_conv.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     4873 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_examples_simple_hgn_run.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)    47196 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_gnn_papers.md.txt
--rw-------   0 jtli      (1007) jtli      (1007)    14831 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_results.md.txt
--rw-------   0 jtli      (1007) jtli      (1007)     2914 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_scripts_display_data.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)      479 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_scripts_download.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)      423 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_scripts_installation_gcc.sh.txt
--rw-------   0 jtli      (1007) jtli      (1007)      240 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_scripts_installation_metis.sh.txt
--rw-------   0 jtli      (1007) jtli      (1007)      295 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_scripts_train.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     4318 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_setup.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     2155 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_tests_datasets_test_customized_data.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     1905 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_tests_datasets_test_data.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)      461 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_tests_datasets_test_gcc_data.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     1799 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_tests_datasets_test_geom_data.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     1107 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_tests_datasets_test_kg_data.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)      401 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_tests_datasets_test_matlab_data.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)      425 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_tests_datasets_test_oagbert_data.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)      692 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_tests_datasets_test_ogb.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)      396 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_tests_datasets_test_planetoid.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)      432 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_tests_datasets_test_rd2cd_data.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)      359 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_tests_datasets_test_rec_data.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     1679 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_tests_datasets_test_saint_data.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     3463 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_tests_models_emb_test_deepwalk.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     2410 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_tests_models_ssl_test_contrastive_models.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     2939 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_tests_models_ssl_test_generative_models.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     3036 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_tests_tasks_test_attributed_graph_clustering.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     1344 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_tests_tasks_test_encode_paper.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     3501 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_tests_tasks_test_graph_classification.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     3825 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_tests_tasks_test_heterogeneous_node_classification.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     3135 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_tests_tasks_test_link_prediction.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     2224 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_tests_tasks_test_multiplex_link_prediction.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)    13504 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_tests_tasks_test_node_classification.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     3078 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_tests_tasks_test_unsupervised_graph_classification.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     4823 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_tests_tasks_test_unsupervised_node_classification.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     2550 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_tests_test_args.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     2218 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_tests_test_experiments.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)      743 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_tests_test_layers.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     2434 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_tests_test_oag.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     3127 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_tests_test_ops.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     1277 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_tests_test_options.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     1738 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_tests_test_pipelines.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     1267 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_tests_test_utils.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)      586 2022-02-15 16:04:02.000000 ahelper-1.2/cogdl/_cogdl1_third_party_README.md.txt
-drwxrwxr-x   0 jtli      (1007) jtli      (1007)        0 2022-02-15 16:13:21.000000 ahelper-1.2/ogb/
--rw-------   0 jtli      (1007) jtli      (1007)      985 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_README.md.txt
--rw-------   0 jtli      (1007) jtli      (1007)     2236 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_graphproppred_code2_README.md.txt
--rw-------   0 jtli      (1007) jtli      (1007)     8997 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_graphproppred_code2_conv.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     3197 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_graphproppred_code2_gnn.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)    11327 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_graphproppred_code2_main_pyg.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     5590 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_graphproppred_code2_py2graph.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     7042 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_graphproppred_code2_utils.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     2702 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_graphproppred_mol_README.md.txt
--rw-------   0 jtli      (1007) jtli      (1007)     8788 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_graphproppred_mol_conv.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     2666 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_graphproppred_mol_gnn.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     6945 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_graphproppred_mol_main_pyg.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     1386 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_graphproppred_ppa_README.md.txt
--rw-------   0 jtli      (1007) jtli      (1007)     8799 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_graphproppred_ppa_conv.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     2666 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_graphproppred_ppa_gnn.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     6158 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_graphproppred_ppa_main_pyg.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)      331 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_linkproppred_biokg_README.md.txt
--rw-------   0 jtli      (1007) jtli      (1007)     5247 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_linkproppred_biokg_dataloader.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)      996 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_linkproppred_biokg_examples.sh.txt
--rw-------   0 jtli      (1007) jtli      (1007)    12752 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_linkproppred_biokg_model.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)    15442 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_linkproppred_biokg_run.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     2160 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_linkproppred_citation2_README.md.txt
--rw-------   0 jtli      (1007) jtli      (1007)     8827 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_linkproppred_citation2_cluster_gcn.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     9364 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_linkproppred_citation2_gnn.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     9189 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_linkproppred_citation2_graph_saint.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     1860 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_linkproppred_citation2_logger.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     6406 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_linkproppred_citation2_mf.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     6595 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_linkproppred_citation2_mlp.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     2249 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_linkproppred_citation2_node2vec.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)    11123 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_linkproppred_citation2_sampler.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     1244 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_linkproppred_collab_README.md.txt
--rw-------   0 jtli      (1007) jtli      (1007)    10596 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_linkproppred_collab_gnn.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     1728 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_linkproppred_collab_logger.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     7392 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_linkproppred_collab_mf.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     7439 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_linkproppred_collab_mlp.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     2123 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_linkproppred_collab_node2vec.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)      923 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_linkproppred_ddi_README.md.txt
--rw-------   0 jtli      (1007) jtli      (1007)    10609 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_linkproppred_ddi_gnn.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     1725 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_linkproppred_ddi_logger.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     7734 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_linkproppred_ddi_mf.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     7622 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_linkproppred_ddi_mlp.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     2116 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_linkproppred_ddi_node2vec.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)      923 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_linkproppred_ppa_README.md.txt
--rw-------   0 jtli      (1007) jtli      (1007)    10470 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_linkproppred_ppa_gnn.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     1725 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_linkproppred_ppa_logger.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     7616 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_linkproppred_ppa_mf.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     7297 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_linkproppred_ppa_mlp.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     2114 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_linkproppred_ppa_node2vec.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)      749 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_linkproppred_wikikg2_README.md.txt
--rw-------   0 jtli      (1007) jtli      (1007)     5457 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_linkproppred_wikikg2_dataloader.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     1741 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_linkproppred_wikikg2_examples.sh.txt
--rw-------   0 jtli      (1007) jtli      (1007)    12683 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_linkproppred_wikikg2_model.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)    14353 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_linkproppred_wikikg2_run.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     4802 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_lsc_mag240m_README.md.txt
--rw-------   0 jtli      (1007) jtli      (1007)     3404 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_lsc_mag240m_correct_and_smooth.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)    10890 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_lsc_mag240m_gnn.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     2954 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_lsc_mag240m_label_prop.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     5370 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_lsc_mag240m_mlp.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     5646 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_lsc_mag240m_preprocess_correct_and_smooth.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     3569 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_lsc_mag240m_preprocess_sgc.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)    18115 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_lsc_mag240m_rgnn.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)       89 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_lsc_mag240m_root.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     5155 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_lsc_mag240m_sgc.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     7028 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_lsc_mag240m_sign.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     4136 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_lsc_pcqm4m-v2_README.md.txt
--rw-------   0 jtli      (1007) jtli      (1007)     8825 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_lsc_pcqm4m-v2_conv.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     2854 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_lsc_pcqm4m-v2_gnn.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     8104 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_lsc_pcqm4m-v2_main_gnn.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)    10025 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_lsc_pcqm4m-v2_main_mlpfp.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     5695 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_lsc_pcqm4m-v2_test_inference_gnn.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     3526 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_lsc_pcqm4m_README.md.txt
--rw-------   0 jtli      (1007) jtli      (1007)     8822 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_lsc_pcqm4m_conv.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     2862 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_lsc_pcqm4m_gnn.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     7621 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_lsc_pcqm4m_main_gnn.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     9451 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_lsc_pcqm4m_main_mlpfp.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     5574 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_lsc_pcqm4m_test_inference_gnn.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     3066 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_lsc_wikikg90m_README.md.txt
--rw-------   0 jtli      (1007) jtli      (1007)      378 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_lsc_wikikg90m_dgl-ke-ogb-lsc_CODE_OF_CONDUCT.md.txt
--rw-------   0 jtli      (1007) jtli      (1007)     3370 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_lsc_wikikg90m_dgl-ke-ogb-lsc_CONTRIBUTING.md.txt
--rw-------   0 jtli      (1007) jtli      (1007)      179 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_lsc_wikikg90m_dgl-ke-ogb-lsc_CONTRIBUTORS.md.txt
--rw-------   0 jtli      (1007) jtli      (1007)     1127 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_lsc_wikikg90m_dgl-ke-ogb-lsc_README.md.txt
--rw-------   0 jtli      (1007) jtli      (1007)       66 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_lsc_wikikg90m_dgl-ke-ogb-lsc_conda_README.md.txt
--rw-------   0 jtli      (1007) jtli      (1007)       67 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_lsc_wikikg90m_dgl-ke-ogb-lsc_docker_README.md.txt
--rw-------   0 jtli      (1007) jtli      (1007)     5614 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_lsc_wikikg90m_dgl-ke-ogb-lsc_docs_source_conf.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     8450 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_lsc_wikikg90m_dgl-ke-ogb-lsc_examples_README.md.txt
--rw-------   0 jtli      (1007) jtli      (1007)      904 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_lsc_wikikg90m_dgl-ke-ogb-lsc_examples_wn18_weighted_README.md.txt
--rw-------   0 jtli      (1007) jtli      (1007)      878 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_lsc_wikikg90m_dgl-ke-ogb-lsc_python_dglke___init__.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)    31959 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_lsc_wikikg90m_dgl-ke-ogb-lsc_python_dglke_dataloader_KGDataset.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)      799 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_lsc_wikikg90m_dgl-ke-ogb-lsc_python_dglke_dataloader___init__.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)    29714 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_lsc_wikikg90m_dgl-ke-ogb-lsc_python_dglke_dataloader_sampler.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     6865 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_lsc_wikikg90m_dgl-ke-ogb-lsc_python_dglke_dist_train.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)    12910 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_lsc_wikikg90m_dgl-ke-ogb-lsc_python_dglke_eval.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     7567 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_lsc_wikikg90m_dgl-ke-ogb-lsc_python_dglke_infer_emb_sim.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)    14985 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_lsc_wikikg90m_dgl-ke-ogb-lsc_python_dglke_infer_score.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     7765 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_lsc_wikikg90m_dgl-ke-ogb-lsc_python_dglke_kvclient.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     6880 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_lsc_wikikg90m_dgl-ke-ogb-lsc_python_dglke_kvserver.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)      939 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_lsc_wikikg90m_dgl-ke-ogb-lsc_python_dglke_models___init__.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     5159 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_lsc_wikikg90m_dgl-ke-ogb-lsc_python_dglke_models_base_loss.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)    31108 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_lsc_wikikg90m_dgl-ke-ogb-lsc_python_dglke_models_general_models.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)    13584 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_lsc_wikikg90m_dgl-ke-ogb-lsc_python_dglke_models_infer.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)    40645 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_lsc_wikikg90m_dgl-ke-ogb-lsc_python_dglke_models_ke_model.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)      751 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_lsc_wikikg90m_dgl-ke-ogb-lsc_python_dglke_models_mxnet___init__.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     1302 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_lsc_wikikg90m_dgl-ke-ogb-lsc_python_dglke_models_mxnet_loss.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)    24986 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_lsc_wikikg90m_dgl-ke-ogb-lsc_python_dglke_models_mxnet_score_fun.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     7802 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_lsc_wikikg90m_dgl-ke-ogb-lsc_python_dglke_models_mxnet_tensor_models.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)      753 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_lsc_wikikg90m_dgl-ke-ogb-lsc_python_dglke_models_pytorch___init__.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     8400 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_lsc_wikikg90m_dgl-ke-ogb-lsc_python_dglke_models_pytorch_ke_tensor.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     3562 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_lsc_wikikg90m_dgl-ke-ogb-lsc_python_dglke_models_pytorch_loss.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)    25185 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_lsc_wikikg90m_dgl-ke-ogb-lsc_python_dglke_models_pytorch_score_fun.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)    13376 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_lsc_wikikg90m_dgl-ke-ogb-lsc_python_dglke_models_pytorch_tensor_models.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     6230 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_lsc_wikikg90m_dgl-ke-ogb-lsc_python_dglke_partition.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)    19734 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_lsc_wikikg90m_dgl-ke-ogb-lsc_python_dglke_train.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     4630 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_lsc_wikikg90m_dgl-ke-ogb-lsc_python_dglke_train_mxnet.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     9236 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_lsc_wikikg90m_dgl-ke-ogb-lsc_python_dglke_train_pytorch.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)    13800 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_lsc_wikikg90m_dgl-ke-ogb-lsc_python_dglke_utils.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)      821 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_lsc_wikikg90m_dgl-ke-ogb-lsc_python_setup.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     2157 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_lsc_wikikg90m_run.sh.txt
--rw-------   0 jtli      (1007) jtli      (1007)     2313 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_lsc_wikikg90m_save_test_submission.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     1215 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_nodeproppred_arxiv_README.md.txt
--rw-------   0 jtli      (1007) jtli      (1007)     5909 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_nodeproppred_arxiv_gnn.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     1727 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_nodeproppred_arxiv_logger.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     4454 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_nodeproppred_arxiv_mlp.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     2237 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_nodeproppred_arxiv_node2vec.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     1827 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_nodeproppred_mag_README.md.txt
--rw-------   0 jtli      (1007) jtli      (1007)    11163 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_nodeproppred_mag_cluster_gcn.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     6031 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_nodeproppred_mag_gnn.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)    11503 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_nodeproppred_mag_graph_saint.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     1725 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_nodeproppred_mag_logger.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     3507 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_nodeproppred_mag_metapath.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     4289 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_nodeproppred_mag_mlp.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     7323 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_nodeproppred_mag_rgcn.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)    11415 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_nodeproppred_mag_sampler.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     2854 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_nodeproppred_papers100M_README.md.txt
--rw-------   0 jtli      (1007) jtli      (1007)     1732 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_nodeproppred_papers100M_logger.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     6109 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_nodeproppred_papers100M_mlp.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     3850 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_nodeproppred_papers100M_node2vec.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     2469 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_nodeproppred_papers100M_sgc.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     1814 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_nodeproppred_products_README.md.txt
--rw-------   0 jtli      (1007) jtli      (1007)     6567 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_nodeproppred_products_cluster_gcn.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     5696 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_nodeproppred_products_gnn.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     7004 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_nodeproppred_products_graph_saint.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     1730 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_nodeproppred_products_logger.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     4188 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_nodeproppred_products_mlp.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     2129 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_nodeproppred_products_node2vec.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     4471 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_nodeproppred_products_sign.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)      928 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_nodeproppred_proteins_README.md.txt
--rw-------   0 jtli      (1007) jtli      (1007)     5868 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_nodeproppred_proteins_gnn.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     1730 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_nodeproppred_proteins_logger.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     4488 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_nodeproppred_proteins_mlp.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     2129 2022-02-15 14:42:13.000000 ahelper-1.2/ogb/_ogb-master_examples_nodeproppred_proteins_node2vec.py.txt
-drwxrwxr-x   0 jtli      (1007) jtli      (1007)        0 2022-02-15 16:13:21.000000 ahelper-1.2/pyg_ogbn_mag/
--rw-------   0 jtli      (1007) jtli      (1007)      451 2022-02-15 16:09:13.000000 ahelper-1.2/pyg_ogbn_mag/_PyG-ogbn-mag_README.md.txt
--rw-------   0 jtli      (1007) jtli      (1007)     3896 2022-02-15 16:09:13.000000 ahelper-1.2/pyg_ogbn_mag/_PyG-ogbn-mag_rgsn+metapath2vec_README.md.txt
--rw-------   0 jtli      (1007) jtli      (1007)     3413 2022-02-15 16:09:13.000000 ahelper-1.2/pyg_ogbn_mag/_PyG-ogbn-mag_rgsn+metapath2vec_attacks.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     2903 2022-02-15 16:09:13.000000 ahelper-1.2/pyg_ogbn_mag/_PyG-ogbn-mag_rgsn+metapath2vec_logger.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     3526 2022-02-15 16:09:13.000000 ahelper-1.2/pyg_ogbn_mag/_PyG-ogbn-mag_rgsn+metapath2vec_metapath2vec.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)    10547 2022-02-15 16:09:13.000000 ahelper-1.2/pyg_ogbn_mag/_PyG-ogbn-mag_rgsn+metapath2vec_models.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)    12010 2022-02-15 16:09:13.000000 ahelper-1.2/pyg_ogbn_mag/_PyG-ogbn-mag_rgsn+metapath2vec_rgsn.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     3047 2022-02-15 16:09:13.000000 ahelper-1.2/pyg_ogbn_mag/_PyG-ogbn-mag_rgsn+metapath2vec_utils.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     6021 2022-02-15 16:09:13.000000 ahelper-1.2/pyg_ogbn_mag/_PyG-ogbn-mag_saint+metapath2vec+cs_CorrectAndSmooth.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     2824 2022-02-15 16:09:13.000000 ahelper-1.2/pyg_ogbn_mag/_PyG-ogbn-mag_saint+metapath2vec+cs_LabelPropagation.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     1788 2022-02-15 16:09:13.000000 ahelper-1.2/pyg_ogbn_mag/_PyG-ogbn-mag_saint+metapath2vec+cs_README.md.txt
--rw-------   0 jtli      (1007) jtli      (1007)     1909 2022-02-15 16:09:13.000000 ahelper-1.2/pyg_ogbn_mag/_PyG-ogbn-mag_saint+metapath2vec+cs_logger.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     3530 2022-02-15 16:09:13.000000 ahelper-1.2/pyg_ogbn_mag/_PyG-ogbn-mag_saint+metapath2vec+cs_metapath2vec.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)    13715 2022-02-15 16:09:13.000000 ahelper-1.2/pyg_ogbn_mag/_PyG-ogbn-mag_saint+metapath2vec+cs_rgcn_saint_cs.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     1660 2022-02-15 16:09:13.000000 ahelper-1.2/pyg_ogbn_mag/_PyG-ogbn-mag_saint+metapath2vec+flag_README.md.txt
--rw-------   0 jtli      (1007) jtli      (1007)     1911 2022-02-15 16:09:13.000000 ahelper-1.2/pyg_ogbn_mag/_PyG-ogbn-mag_saint+metapath2vec+flag_logger.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     3532 2022-02-15 16:09:13.000000 ahelper-1.2/pyg_ogbn_mag/_PyG-ogbn-mag_saint+metapath2vec+flag_metapath2vec.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)    14116 2022-02-15 16:09:13.000000 ahelper-1.2/pyg_ogbn_mag/_PyG-ogbn-mag_saint+metapath2vec+flag_rgcn_saint_flag.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     1881 2022-02-15 16:09:13.000000 ahelper-1.2/pyg_ogbn_mag/_PyG-ogbn-mag_saint+metapath2vec_README.md.txt
--rw-------   0 jtli      (1007) jtli      (1007)     1906 2022-02-15 16:09:13.000000 ahelper-1.2/pyg_ogbn_mag/_PyG-ogbn-mag_saint+metapath2vec_logger.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     3527 2022-02-15 16:09:13.000000 ahelper-1.2/pyg_ogbn_mag/_PyG-ogbn-mag_saint+metapath2vec_metapath2vec.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)    11998 2022-02-15 16:09:13.000000 ahelper-1.2/pyg_ogbn_mag/_PyG-ogbn-mag_saint+metapath2vec_rgcn_saint.py.txt
-drwxrwxr-x   0 jtli      (1007) jtli      (1007)        0 2022-02-15 16:13:21.000000 ahelper-1.2/pygcl/
--rw-------   0 jtli      (1007) jtli      (1007)      242 2022-02-15 16:05:45.000000 ahelper-1.2/pygcl/_PyGCL1_GCL___init__.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)      865 2022-02-15 16:05:45.000000 ahelper-1.2/pygcl/_PyGCL1_GCL_augmentors___init__.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     1831 2022-02-15 16:05:45.000000 ahelper-1.2/pygcl/_PyGCL1_GCL_augmentors_augmentor.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)      494 2022-02-15 16:05:45.000000 ahelper-1.2/pygcl/_PyGCL1_GCL_augmentors_edge_adding.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)      557 2022-02-15 16:05:45.000000 ahelper-1.2/pygcl/_PyGCL1_GCL_augmentors_edge_attr_masking.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)      540 2022-02-15 16:05:45.000000 ahelper-1.2/pygcl/_PyGCL1_GCL_augmentors_edge_removing.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)      496 2022-02-15 16:05:45.000000 ahelper-1.2/pygcl/_PyGCL1_GCL_augmentors_feature_dropout.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)      490 2022-02-15 16:05:45.000000 ahelper-1.2/pygcl/_PyGCL1_GCL_augmentors_feature_masking.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)    11530 2022-02-15 16:05:45.000000 ahelper-1.2/pygcl/_PyGCL1_GCL_augmentors_functional.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)      243 2022-02-15 16:05:45.000000 ahelper-1.2/pygcl/_PyGCL1_GCL_augmentors_identity.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     1106 2022-02-15 16:05:45.000000 ahelper-1.2/pygcl/_PyGCL1_GCL_augmentors_markov_diffusion.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)      541 2022-02-15 16:05:45.000000 ahelper-1.2/pygcl/_PyGCL1_GCL_augmentors_node_dropping.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)      436 2022-02-15 16:05:45.000000 ahelper-1.2/pygcl/_PyGCL1_GCL_augmentors_node_shuffling.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)      987 2022-02-15 16:05:45.000000 ahelper-1.2/pygcl/_PyGCL1_GCL_augmentors_ppr_diffusion.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)      661 2022-02-15 16:05:45.000000 ahelper-1.2/pygcl/_PyGCL1_GCL_augmentors_rw_sampling.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)      417 2022-02-15 16:05:45.000000 ahelper-1.2/pygcl/_PyGCL1_GCL_eval___init__.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     2664 2022-02-15 16:05:45.000000 ahelper-1.2/pygcl/_PyGCL1_GCL_eval_eval.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     3102 2022-02-15 16:05:45.000000 ahelper-1.2/pygcl/_PyGCL1_GCL_eval_logistic_regression.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)      372 2022-02-15 16:05:45.000000 ahelper-1.2/pygcl/_PyGCL1_GCL_eval_random_forest.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)      467 2022-02-15 16:05:45.000000 ahelper-1.2/pygcl/_PyGCL1_GCL_eval_svm.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)      582 2022-02-15 16:05:45.000000 ahelper-1.2/pygcl/_PyGCL1_GCL_losses___init__.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     1121 2022-02-15 16:05:45.000000 ahelper-1.2/pygcl/_PyGCL1_GCL_losses_barlow_twins.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)      528 2022-02-15 16:05:45.000000 ahelper-1.2/pygcl/_PyGCL1_GCL_losses_bootstrap.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     7310 2022-02-15 16:05:45.000000 ahelper-1.2/pygcl/_PyGCL1_GCL_losses_infonce.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     2676 2022-02-15 16:05:45.000000 ahelper-1.2/pygcl/_PyGCL1_GCL_losses_jsd.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)      437 2022-02-15 16:05:45.000000 ahelper-1.2/pygcl/_PyGCL1_GCL_losses_losses.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     3661 2022-02-15 16:05:45.000000 ahelper-1.2/pygcl/_PyGCL1_GCL_losses_triplet.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     1561 2022-02-15 16:05:45.000000 ahelper-1.2/pygcl/_PyGCL1_GCL_losses_vicreg.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)      419 2022-02-15 16:05:45.000000 ahelper-1.2/pygcl/_PyGCL1_GCL_models___init__.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     6222 2022-02-15 16:05:45.000000 ahelper-1.2/pygcl/_PyGCL1_GCL_models_contrast_model.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     3458 2022-02-15 16:05:45.000000 ahelper-1.2/pygcl/_PyGCL1_GCL_models_samplers.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     2222 2022-02-15 16:05:45.000000 ahelper-1.2/pygcl/_PyGCL1_GCL_utils.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)    14042 2022-02-15 16:05:45.000000 ahelper-1.2/pygcl/_PyGCL1_README.md.txt
--rw-------   0 jtli      (1007) jtli      (1007)     1609 2022-02-15 16:05:45.000000 ahelper-1.2/pygcl/_PyGCL1_docs_conf.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     1166 2022-02-15 16:05:45.000000 ahelper-1.2/pygcl/_PyGCL1_docs_index.md.txt
--rw-------   0 jtli      (1007) jtli      (1007)      446 2022-02-15 16:05:45.000000 ahelper-1.2/pygcl/_PyGCL1_docs_modules_augmentors.md.txt
--rw-------   0 jtli      (1007) jtli      (1007)      438 2022-02-15 16:05:45.000000 ahelper-1.2/pygcl/_PyGCL1_docs_notes_installation.md.txt
--rw-------   0 jtli      (1007) jtli      (1007)      517 2022-02-15 16:05:45.000000 ahelper-1.2/pygcl/_PyGCL1_docs_run_livereload.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     6806 2022-02-15 16:05:45.000000 ahelper-1.2/pygcl/_PyGCL1_examples_BGRL_G2L.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     5547 2022-02-15 16:05:45.000000 ahelper-1.2/pygcl/_PyGCL1_examples_BGRL_L2L.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     4153 2022-02-15 16:05:45.000000 ahelper-1.2/pygcl/_PyGCL1_examples_DGI_inductive.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     3186 2022-02-15 16:05:45.000000 ahelper-1.2/pygcl/_PyGCL1_examples_DGI_transductive.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     3412 2022-02-15 16:05:45.000000 ahelper-1.2/pygcl/_PyGCL1_examples_GBT.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     3679 2022-02-15 16:05:45.000000 ahelper-1.2/pygcl/_PyGCL1_examples_GRACE.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     4601 2022-02-15 16:05:45.000000 ahelper-1.2/pygcl/_PyGCL1_examples_GRACE_SupCon.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     4823 2022-02-15 16:05:45.000000 ahelper-1.2/pygcl/_PyGCL1_examples_GraphCL.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     4692 2022-02-15 16:05:45.000000 ahelper-1.2/pygcl/_PyGCL1_examples_InfoGraph.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     4836 2022-02-15 16:05:45.000000 ahelper-1.2/pygcl/_PyGCL1_examples_MVGRL_graph.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     3975 2022-02-15 16:05:45.000000 ahelper-1.2/pygcl/_PyGCL1_examples_MVGRL_node.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)       55 2022-02-15 16:05:45.000000 ahelper-1.2/pygcl/_PyGCL1_setup.py.txt
-drwxrwxr-x   0 jtli      (1007) jtli      (1007)        0 2022-02-15 16:13:21.000000 ahelper-1.2/pyhgt/
--rw-------   0 jtli      (1007) jtli      (1007)      529 2022-02-15 14:45:17.000000 ahelper-1.2/pyhgt/_pyHGT-master_Docker_README.md.txt
--rw-------   0 jtli      (1007) jtli      (1007)    16216 2022-02-15 14:45:17.000000 ahelper-1.2/pyhgt/_pyHGT-master_OAG_preprocess_OAG.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)       36 2022-02-15 14:45:17.000000 ahelper-1.2/pyhgt/_pyHGT-master_OAG_pyHGT___init__.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)    15079 2022-02-15 14:45:17.000000 ahelper-1.2/pyhgt/_pyHGT-master_OAG_pyHGT_conv.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)    11294 2022-02-15 14:45:17.000000 ahelper-1.2/pyhgt/_pyHGT-master_OAG_pyHGT_data.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     3294 2022-02-15 14:45:17.000000 ahelper-1.2/pyhgt/_pyHGT-master_OAG_pyHGT_model.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     2266 2022-02-15 14:45:17.000000 ahelper-1.2/pyhgt/_pyHGT-master_OAG_pyHGT_utils.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)    16066 2022-02-15 14:45:17.000000 ahelper-1.2/pyhgt/_pyHGT-master_OAG_train_author_disambiguation.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)    13604 2022-02-15 14:45:17.000000 ahelper-1.2/pyhgt/_pyHGT-master_OAG_train_paper_field.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)    13372 2022-02-15 14:45:17.000000 ahelper-1.2/pyhgt/_pyHGT-master_OAG_train_paper_venue.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     4893 2022-02-15 14:45:17.000000 ahelper-1.2/pyhgt/_pyHGT-master_README.md.txt
--rw-------   0 jtli      (1007) jtli      (1007)     2341 2022-02-15 14:45:17.000000 ahelper-1.2/pyhgt/_pyHGT-master_ogbn-mag_README.md.txt
--rw-------   0 jtli      (1007) jtli      (1007)     9268 2022-02-15 14:45:17.000000 ahelper-1.2/pyhgt/_pyHGT-master_ogbn-mag_eval_ogbn_mag.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     4220 2022-02-15 14:45:17.000000 ahelper-1.2/pyhgt/_pyHGT-master_ogbn-mag_preprocess_ogbn_mag.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)       41 2022-02-15 14:45:17.000000 ahelper-1.2/pyhgt/_pyHGT-master_ogbn-mag_pyHGT___init__.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)    15084 2022-02-15 14:45:17.000000 ahelper-1.2/pyhgt/_pyHGT-master_ogbn-mag_pyHGT_conv.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)    10864 2022-02-15 14:45:17.000000 ahelper-1.2/pyhgt/_pyHGT-master_ogbn-mag_pyHGT_data.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     3301 2022-02-15 14:45:17.000000 ahelper-1.2/pyhgt/_pyHGT-master_ogbn-mag_pyHGT_model.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     3189 2022-02-15 14:45:17.000000 ahelper-1.2/pyhgt/_pyHGT-master_ogbn-mag_pyHGT_utils.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     9685 2022-02-15 14:45:17.000000 ahelper-1.2/pyhgt/_pyHGT-master_ogbn-mag_train_ogbn_mag.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)       32 2022-02-15 14:45:17.000000 ahelper-1.2/pyhgt/_pyHGT-master_pyHGT___init__.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)    15075 2022-02-15 14:45:17.000000 ahelper-1.2/pyhgt/_pyHGT-master_pyHGT_conv.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)    11280 2022-02-15 14:45:17.000000 ahelper-1.2/pyhgt/_pyHGT-master_pyHGT_data.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     3292 2022-02-15 14:45:17.000000 ahelper-1.2/pyhgt/_pyHGT-master_pyHGT_model.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     2262 2022-02-15 14:45:17.000000 ahelper-1.2/pyhgt/_pyHGT-master_pyHGT_utils.py.txt
-drwxrwxr-x   0 jtli      (1007) jtli      (1007)        0 2022-02-15 16:13:21.000000 ahelper-1.2/refine/
--rw-------   0 jtli      (1007) jtli      (1007)     5675 2022-02-15 14:43:05.000000 ahelper-1.2/refine/_ReFine-main_README.md.txt
--rw-------   0 jtli      (1007) jtli      (1007)      203 2022-02-15 14:43:05.000000 ahelper-1.2/refine/_ReFine-main_datasets___init__.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     2776 2022-02-15 14:43:05.000000 ahelper-1.2/refine/_ReFine-main_datasets_ba3motif_dataset.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)    18210 2022-02-15 14:43:05.000000 ahelper-1.2/refine/_ReFine-main_datasets_graphss2_dataset.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     3803 2022-02-15 14:43:05.000000 ahelper-1.2/refine/_ReFine-main_datasets_mutag_dataset.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     3204 2022-02-15 14:43:05.000000 ahelper-1.2/refine/_ReFine-main_datasets_vg_dataset.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     3602 2022-02-15 14:43:05.000000 ahelper-1.2/refine/_ReFine-main_evaluate.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     2199 2022-02-15 14:43:05.000000 ahelper-1.2/refine/_ReFine-main_example.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)      426 2022-02-15 14:43:05.000000 ahelper-1.2/refine/_ReFine-main_explainers___init__.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)    20122 2022-02-15 14:43:05.000000 ahelper-1.2/refine/_ReFine-main_explainers_base.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     2237 2022-02-15 14:43:05.000000 ahelper-1.2/refine/_ReFine-main_explainers_common.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     3165 2022-02-15 14:43:05.000000 ahelper-1.2/refine/_ReFine-main_explainers_cxplainer.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     3577 2022-02-15 14:43:05.000000 ahelper-1.2/refine/_ReFine-main_explainers_deeplift.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)      929 2022-02-15 14:43:05.000000 ahelper-1.2/refine/_ReFine-main_explainers_gnnexplainer.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     1096 2022-02-15 14:43:05.000000 ahelper-1.2/refine/_ReFine-main_explainers_gradcam.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     1745 2022-02-15 14:43:05.000000 ahelper-1.2/refine/_ReFine-main_explainers_ig_explainer.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     2656 2022-02-15 14:43:05.000000 ahelper-1.2/refine/_ReFine-main_explainers_meta_gnnexplainer.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     6316 2022-02-15 14:43:05.000000 ahelper-1.2/refine/_ReFine-main_explainers_meta_pgm_explainer.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     5595 2022-02-15 14:43:05.000000 ahelper-1.2/refine/_ReFine-main_explainers_pg_explainer.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     2290 2022-02-15 14:43:05.000000 ahelper-1.2/refine/_ReFine-main_explainers_pgm_explainer.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)      923 2022-02-15 14:43:05.000000 ahelper-1.2/refine/_ReFine-main_explainers_random_caster.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     8743 2022-02-15 14:43:05.000000 ahelper-1.2/refine/_ReFine-main_explainers_refine.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     1066 2022-02-15 14:43:05.000000 ahelper-1.2/refine/_ReFine-main_explainers_sa_explainer.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)    12131 2022-02-15 14:43:05.000000 ahelper-1.2/refine/_ReFine-main_explainers_screener.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     4026 2022-02-15 14:43:05.000000 ahelper-1.2/refine/_ReFine-main_explainers_visual.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)      211 2022-02-15 14:43:05.000000 ahelper-1.2/refine/_ReFine-main_gnns___init__.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     7284 2022-02-15 14:43:05.000000 ahelper-1.2/refine/_ReFine-main_gnns_ba3motif_gnn.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     5702 2022-02-15 14:43:05.000000 ahelper-1.2/refine/_ReFine-main_gnns_mnist_gnn.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     7503 2022-02-15 14:43:05.000000 ahelper-1.2/refine/_ReFine-main_gnns_mutag_gnn.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     1076 2022-02-15 14:43:05.000000 ahelper-1.2/refine/_ReFine-main_gnns_overloader.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     7636 2022-02-15 14:43:05.000000 ahelper-1.2/refine/_ReFine-main_gnns_vg_gnn.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)       31 2022-02-15 14:43:05.000000 ahelper-1.2/refine/_ReFine-main_train___init__.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)       98 2022-02-15 14:43:05.000000 ahelper-1.2/refine/_ReFine-main_train_config.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     6097 2022-02-15 14:43:05.000000 ahelper-1.2/refine/_ReFine-main_train_pg_train.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     6496 2022-02-15 14:43:05.000000 ahelper-1.2/refine/_ReFine-main_train_refine_train.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)      679 2022-02-15 14:43:05.000000 ahelper-1.2/refine/_ReFine-main_train_run.sh.txt
--rw-------   0 jtli      (1007) jtli      (1007)     5576 2022-02-15 14:43:05.000000 ahelper-1.2/refine/_ReFine-main_utils___init__.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     2701 2022-02-15 14:43:05.000000 ahelper-1.2/refine/_ReFine-main_utils_dataset.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     9173 2022-02-15 14:43:05.000000 ahelper-1.2/refine/_ReFine-main_utils_get_subgraph.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     1069 2022-02-15 14:43:05.000000 ahelper-1.2/refine/_ReFine-main_utils_logger.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)      268 2022-02-15 14:43:05.000000 ahelper-1.2/refine/_ReFine-main_utils_parser.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     1526 2022-02-15 14:43:05.000000 ahelper-1.2/refine/_ReFine-main_utils_saver.py.txt
--rw-rw-r--   0 jtli      (1007) jtli      (1007)       38 2022-02-15 16:13:21.000000 ahelper-1.2/setup.cfg
--rw-------   0 jtli      (1007) jtli      (1007)     1485 2022-02-15 16:12:12.000000 ahelper-1.2/setup.py
-drwxrwxr-x   0 jtli      (1007) jtli      (1007)        0 2022-02-15 16:13:21.000000 ahelper-1.2/tencent/
--rw-------   0 jtli      (1007) jtli      (1007)     2220 2022-02-15 16:11:30.000000 ahelper-1.2/tencent/_Tencent2020_Rank1st_BERT_model.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)    27340 2022-02-15 16:11:30.000000 ahelper-1.2/tencent/_Tencent2020_Rank1st_BERT_run.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     5150 2022-02-15 16:11:30.000000 ahelper-1.2/tencent/_Tencent2020_Rank1st_README.md.txt
--rw-------   0 jtli      (1007) jtli      (1007)    11792 2022-02-15 16:11:30.000000 ahelper-1.2/tencent/_Tencent2020_Rank1st_models_ctrNet.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     6463 2022-02-15 16:11:30.000000 ahelper-1.2/tencent/_Tencent2020_Rank1st_models_model.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     7603 2022-02-15 16:11:30.000000 ahelper-1.2/tencent/_Tencent2020_Rank1st_run.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     1142 2022-02-15 16:11:30.000000 ahelper-1.2/tencent/_Tencent2020_Rank1st_run.sh.txt
--rw-------   0 jtli      (1007) jtli      (1007)     3835 2022-02-15 16:11:30.000000 ahelper-1.2/tencent/_Tencent2020_Rank1st_src_data_loader.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)    10606 2022-02-15 16:11:30.000000 ahelper-1.2/tencent/_Tencent2020_Rank1st_src_extract_features.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     1932 2022-02-15 16:11:30.000000 ahelper-1.2/tencent/_Tencent2020_Rank1st_src_merge_submission.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     2179 2022-02-15 16:11:30.000000 ahelper-1.2/tencent/_Tencent2020_Rank1st_src_preprocess.py.txt
--rw-------   0 jtli      (1007) jtli      (1007)     1534 2022-02-15 16:11:30.000000 ahelper-1.2/tencent/_Tencent2020_Rank1st_src_w2v.py.txt
+drwxrwxr-x   0 jtli      (1012) jtli      (1013)        0 2024-04-18 15:32:51.972224 ahelper-1.3/
+-rw-rw-r--   0 jtli      (1012) jtli      (1013)      934 2024-04-18 15:32:51.972224 ahelper-1.3/PKG-INFO
+drwxrwxr-x   0 jtli      (1012) jtli      (1013)        0 2024-04-18 15:32:51.972224 ahelper-1.3/ahelper/
+-rw-------   0 jtli      (1012) jtli      (1013)      957 2024-04-18 15:06:12.000000 ahelper-1.3/ahelper/__init__.py
+-rw-------   0 jtli      (1012) jtli      (1013)     9944 2024-04-18 14:56:41.000000 ahelper-1.3/ahelper/deepwalk.py
+-rw-------   0 jtli      (1012) jtli      (1013)     4074 2024-04-18 14:56:41.000000 ahelper-1.3/ahelper/feature.py
+-rw-------   0 jtli      (1012) jtli      (1013)    15521 2024-04-18 14:56:41.000000 ahelper-1.3/ahelper/layers.py
+-rw-------   0 jtli      (1012) jtli      (1013)      839 2024-04-18 14:56:41.000000 ahelper-1.3/ahelper/links.py
+-rw-rw-r--   0 jtli      (1012) jtli      (1013)    18348 2024-04-18 15:01:07.000000 ahelper-1.3/ahelper/nlu_lora.py
+-rw-------   0 jtli      (1012) jtli      (1013)    12614 2024-04-18 14:56:41.000000 ahelper-1.3/ahelper/snn.py
+-rw-------   0 jtli      (1012) jtli      (1013)    14793 2024-04-18 14:56:41.000000 ahelper-1.3/ahelper/utils.py
+drwxrwxr-x   0 jtli      (1012) jtli      (1013)        0 2024-04-18 15:32:51.972224 ahelper-1.3/ahelper.egg-info/
+-rw-rw-r--   0 jtli      (1012) jtli      (1013)      934 2024-04-18 15:32:51.000000 ahelper-1.3/ahelper.egg-info/PKG-INFO
+-rw-rw-r--   0 jtli      (1012) jtli      (1013)      278 2024-04-18 15:32:51.000000 ahelper-1.3/ahelper.egg-info/SOURCES.txt
+-rw-rw-r--   0 jtli      (1012) jtli      (1013)        1 2024-04-18 15:32:51.000000 ahelper-1.3/ahelper.egg-info/dependency_links.txt
+-rw-rw-r--   0 jtli      (1012) jtli      (1013)        8 2024-04-18 15:32:51.000000 ahelper-1.3/ahelper.egg-info/top_level.txt
+-rw-rw-r--   0 jtli      (1012) jtli      (1013)       38 2024-04-18 15:32:51.972224 ahelper-1.3/setup.cfg
+-rw-------   0 jtli      (1012) jtli      (1013)     1241 2024-04-18 15:32:49.000000 ahelper-1.3/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `ahelper-1.2/PKG-INFO` & `ahelper-1.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: ahelper
-Version: 1.2
+Version: 1.3
 Summary: A helper.
 Home-page: https://gitee.com/EdisonLeeeee/ahelper
 Author: Jintang Li
 Author-email: cnljt@outlook.com
 License: MIT LICENSE
-Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Libraries
@@ -18,7 +17,11 @@
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+
+UNKNOWN
+
```

### Comparing `ahelper-1.2/ahelper/deepwalk.py` & `ahelper-1.3/ahelper/deepwalk.py`

 * *Files identical despite different names*

### Comparing `ahelper-1.2/ahelper/feature.py` & `ahelper-1.3/ahelper/feature.py`

 * *Files identical despite different names*

### Comparing `ahelper-1.2/ahelper/layers.py` & `ahelper-1.3/ahelper/layers.py`

 * *Files identical despite different names*

### Comparing `ahelper-1.2/ahelper/links.py` & `ahelper-1.3/ahelper/links.py`

 * *Files identical despite different names*

### Comparing `ahelper-1.2/ahelper/snn.py` & `ahelper-1.3/ahelper/snn.py`

 * *Files identical despite different names*

### Comparing `ahelper-1.2/ahelper/utils.py` & `ahelper-1.3/ahelper/utils.py`

 * *Files identical despite different names*

### Comparing `ahelper-1.2/ahelper.egg-info/PKG-INFO` & `ahelper-1.3/ahelper.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: ahelper
-Version: 1.2
+Version: 1.3
 Summary: A helper.
 Home-page: https://gitee.com/EdisonLeeeee/ahelper
 Author: Jintang Li
 Author-email: cnljt@outlook.com
 License: MIT LICENSE
-Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Libraries
@@ -18,7 +17,11 @@
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+
+UNKNOWN
+
```

### Comparing `ahelper-1.2/setup.py` & `ahelper-1.3/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,31 +1,26 @@
 from setuptools import setup, find_packages
 
 url='https://gitee.com/EdisonLeeeee/ahelper'
-VERSION = 1.2
-package_data_list = ['ogb/*.txt','refine/*.txt', 
-                     'Graph_Transformer_Networks/*.txt', 
-                     'pyhgt/*.txt', 
-                     'pygcl/*.txt', 
-                     'cogdl/*.txt',
-                    'pyg_ogbn_mag/*.txt',
-                    'tencent/*.txt']
+VERSION = 1.3
 
 setup(
     name='ahelper',
     version=VERSION,
     description='A helper.',
     python_requires='>=3.6',
     license="MIT LICENSE",
     author='Jintang Li',
     author_email='cnljt@outlook.com',
     url='https://gitee.com/EdisonLeeeee/ahelper',
 #     download_url='{}/archive/{}.tar.gz'.format(url, VERSION),
     packages=['ahelper'],
-      package_data={'ahelper': package_data_list},
+      package_data={'ahelper': ['medicalgpt']},
+    long_description_content_type="text/markdown",
+    
   include_package_data=True,
     classifiers=[
         'Development Status :: 3 - Alpha',
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: MIT License",
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
         'Topic :: Scientific/Engineering',
```

