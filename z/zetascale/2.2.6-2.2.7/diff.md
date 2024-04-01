# Comparing `tmp/zetascale-2.2.6.tar.gz` & `tmp/zetascale-2.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zetascale-2.2.6.tar", max compression
+gzip compressed data, was "zetascale-2.2.7.tar", max compression
```

## Comparing `zetascale-2.2.6.tar` & `zetascale-2.2.7.tar`

### file list

```diff
@@ -1,361 +1,362 @@
--rw-r--r--   0        0        0    11342 2023-10-13 21:44:53.585497 zetascale-2.2.6/LICENSE
--rw-r--r--   0        0        0    20231 2024-02-27 06:39:21.932280 zetascale-2.2.6/README.md
--rw-r--r--   0        0        0     1457 2024-03-21 22:09:52.672699 zetascale-2.2.6/pyproject.toml
--rw-r--r--   0        0        0      546 2024-02-20 02:20:54.857337 zetascale-2.2.6/zeta/__init__.py
--rw-r--r--   0        0        0        0 2023-12-19 19:47:39.268788 zetascale-2.2.6/zeta/cli/__init__.py
--rw-r--r--   0        0        0     1937 2024-02-20 02:20:55.165790 zetascale-2.2.6/zeta/cli/main.py
--rw-r--r--   0        0        0      157 2024-02-20 03:07:47.757716 zetascale-2.2.6/zeta/cloud/__init__.py
--rw-r--r--   0        0        0     2071 2024-03-12 17:08:02.038250 zetascale-2.2.6/zeta/cloud/main.py
--rw-r--r--   0        0        0     6217 2024-03-12 17:08:02.120591 zetascale-2.2.6/zeta/cloud/sky_api.py
--rw-r--r--   0        0        0     1809 2024-03-12 17:08:02.079698 zetascale-2.2.6/zeta/models/LongNet.py
--rw-r--r--   0        0        0        0 2023-07-10 01:12:17.230004 zetascale-2.2.6/zeta/models/Magneto.py
--rw-r--r--   0        0        0      603 2024-02-22 19:03:14.806609 zetascale-2.2.6/zeta/models/__init__.py
--rw-r--r--   0        0        0     3308 2024-02-20 02:20:55.572463 zetascale-2.2.6/zeta/models/andromeda.py
--rw-r--r--   0        0        0      135 2023-12-31 05:32:43.412544 zetascale-2.2.6/zeta/models/base.py
--rw-r--r--   0        0        0     3311 2024-03-12 17:08:02.117008 zetascale-2.2.6/zeta/models/beit3.py
--rw-r--r--   0        0        0     6752 2024-02-20 03:07:47.967442 zetascale-2.2.6/zeta/models/gpt4.py
--rw-r--r--   0        0        0     4288 2024-03-12 17:08:02.180350 zetascale-2.2.6/zeta/models/kosmos.py
--rw-r--r--   0        0        0      949 2024-02-20 02:20:55.502345 zetascale-2.2.6/zeta/models/llama.py
--rw-r--r--   0        0        0     3639 2024-03-12 17:08:02.150836 zetascale-2.2.6/zeta/models/max_vit.py
--rw-r--r--   0        0        0     6678 2024-03-12 17:08:02.311937 zetascale-2.2.6/zeta/models/mega_vit.py
--rw-r--r--   0        0        0     6927 2024-02-20 02:20:56.942968 zetascale-2.2.6/zeta/models/mm_mamba.py
--rw-r--r--   0        0        0    12991 2024-03-12 17:08:02.622848 zetascale-2.2.6/zeta/models/navit.py
--rw-r--r--   0        0        0     1884 2024-02-20 03:07:48.030803 zetascale-2.2.6/zeta/models/palme.py
--rw-r--r--   0        0        0     2762 2024-03-12 17:08:02.154861 zetascale-2.2.6/zeta/models/vit.py
--rw-r--r--   0        0        0      219 2024-02-20 03:07:47.976964 zetascale-2.2.6/zeta/nn/__init__.py
--rw-r--r--   0        0        0     1797 2024-03-19 17:05:56.616851 zetascale-2.2.6/zeta/nn/attention/__init__.py
--rw-r--r--   0        0        0     4184 2024-03-12 17:08:02.309118 zetascale-2.2.6/zeta/nn/attention/agent_attn.py
--rw-r--r--   0        0        0    14876 2024-03-12 17:08:02.715767 zetascale-2.2.6/zeta/nn/attention/attend.py
--rw-r--r--   0        0        0      244 2024-02-20 02:20:56.872011 zetascale-2.2.6/zeta/nn/attention/base.py
--rw-r--r--   0        0        0     4050 2024-03-12 17:08:02.358668 zetascale-2.2.6/zeta/nn/attention/cross_attention.py
--rw-r--r--   0        0        0     3236 2023-12-29 17:40:30.936298 zetascale-2.2.6/zeta/nn/attention/cross_attn_images.py
--rw-r--r--   0        0        0    10734 2024-03-12 17:08:02.527291 zetascale-2.2.6/zeta/nn/attention/dilated_attention.py
--rw-r--r--   0        0        0     8803 2024-03-12 17:08:02.448488 zetascale-2.2.6/zeta/nn/attention/flash_attention.py
--rw-r--r--   0        0        0     2161 2024-01-13 18:03:19.763236 zetascale-2.2.6/zeta/nn/attention/linear_attention.py
--rw-r--r--   0        0        0     2370 2024-03-12 17:08:02.307028 zetascale-2.2.6/zeta/nn/attention/linear_attn_l.py
--rw-r--r--   0        0        0     9794 2024-03-12 17:08:02.638502 zetascale-2.2.6/zeta/nn/attention/local_attention.py
--rw-r--r--   0        0        0     1966 2023-12-19 19:26:43.471021 zetascale-2.2.6/zeta/nn/attention/local_attention_mha.py
--rw-r--r--   0        0        0    18990 2024-03-12 17:08:03.268461 zetascale-2.2.6/zeta/nn/attention/mixture_attention.py
--rw-r--r--   0        0        0    12414 2024-03-19 16:54:57.559772 zetascale-2.2.6/zeta/nn/attention/multi_grouped_attn.py
--rw-r--r--   0        0        0     2729 2024-03-12 17:08:02.437305 zetascale-2.2.6/zeta/nn/attention/multi_modal_causal_attention.py
--rw-r--r--   0        0        0     3879 2023-12-29 18:02:53.657706 zetascale-2.2.6/zeta/nn/attention/multi_modal_cross_attn.py
--rw-r--r--   0        0        0     5767 2024-03-12 17:08:02.611227 zetascale-2.2.6/zeta/nn/attention/multihead_attention.py
--rw-r--r--   0        0        0    25390 2024-03-12 17:08:03.886143 zetascale-2.2.6/zeta/nn/attention/multiquery_attention.py
--rw-r--r--   0        0        0     2198 2024-02-20 02:21:01.439585 zetascale-2.2.6/zeta/nn/attention/shaped_attention.py
--rw-r--r--   0        0        0     4672 2024-02-20 02:21:02.943176 zetascale-2.2.6/zeta/nn/attention/sparse_attention.py
--rw-r--r--   0        0        0     1741 2024-03-12 17:08:02.503328 zetascale-2.2.6/zeta/nn/attention/spatial_linear_attention.py
--rw-r--r--   0        0        0     2973 2024-02-20 02:21:01.927064 zetascale-2.2.6/zeta/nn/attention/xc_attention.py
--rw-r--r--   0        0        0      482 2024-02-20 02:21:01.042463 zetascale-2.2.6/zeta/nn/biases/__init__.py
--rw-r--r--   0        0        0     3951 2024-03-12 17:08:02.722676 zetascale-2.2.6/zeta/nn/biases/alibi.py
--rw-r--r--   0        0        0      245 2024-02-20 02:21:01.653481 zetascale-2.2.6/zeta/nn/biases/base.py
--rw-r--r--   0        0        0     1348 2024-02-20 02:21:02.183763 zetascale-2.2.6/zeta/nn/biases/dynamic_position_bias.py
--rw-r--r--   0        0        0     2886 2024-03-12 17:08:02.668729 zetascale-2.2.6/zeta/nn/biases/relative_position_bias.py
--rw-r--r--   0        0        0     2069 2024-03-02 07:30:50.700992 zetascale-2.2.6/zeta/nn/embeddings/__init__.py
--rw-r--r--   0        0        0     1231 2023-12-23 05:23:23.147156 zetascale-2.2.6/zeta/nn/embeddings/abc_pos_emb.py
--rw-r--r--   0        0        0      255 2024-02-20 02:21:02.347272 zetascale-2.2.6/zeta/nn/embeddings/base.py
--rw-r--r--   0        0        0      723 2024-02-20 02:21:02.661920 zetascale-2.2.6/zeta/nn/embeddings/embedding.py
--rw-r--r--   0        0        0     2509 2024-01-07 05:11:05.739698 zetascale-2.2.6/zeta/nn/embeddings/multiway_network.py
--rw-r--r--   0        0        0      358 2024-02-20 02:21:02.600313 zetascale-2.2.6/zeta/nn/embeddings/nominal_embeddings.py
--rw-r--r--   0        0        0      900 2023-10-24 04:07:16.862154 zetascale-2.2.6/zeta/nn/embeddings/patch_embedding.py
--rw-r--r--   0        0        0     3120 2024-02-20 02:21:03.171183 zetascale-2.2.6/zeta/nn/embeddings/pi.md
--rw-r--r--   0        0        0     1996 2024-03-12 17:08:02.654239 zetascale-2.2.6/zeta/nn/embeddings/positional.py
--rw-r--r--   0        0        0     2584 2024-03-12 17:08:02.753885 zetascale-2.2.6/zeta/nn/embeddings/positional_interpolation.py
--rw-r--r--   0        0        0     3021 2024-03-12 17:08:02.747974 zetascale-2.2.6/zeta/nn/embeddings/qfsp_embeddings.py
--rw-r--r--   0        0        0     1668 2024-03-12 17:08:02.722910 zetascale-2.2.6/zeta/nn/embeddings/qft_embeddings.py
--rw-r--r--   0        0        0     2250 2024-02-20 02:21:03.986803 zetascale-2.2.6/zeta/nn/embeddings/rope.py
--rw-r--r--   0        0        0     1570 2024-03-02 07:30:50.701708 zetascale-2.2.6/zeta/nn/embeddings/scaled_sinusoidal_embeddings.py
--rw-r--r--   0        0        0     2345 2024-03-12 17:08:02.798633 zetascale-2.2.6/zeta/nn/embeddings/sine_positional.py
--rw-r--r--   0        0        0     2650 2024-03-12 17:08:02.815289 zetascale-2.2.6/zeta/nn/embeddings/sinusoidal.py
--rw-r--r--   0        0        0     1810 2024-03-12 17:08:02.785699 zetascale-2.2.6/zeta/nn/embeddings/truncated_rope.py
--rw-r--r--   0        0        0     1003 2023-10-24 04:10:28.452387 zetascale-2.2.6/zeta/nn/embeddings/vis_lang_emb.py
--rw-r--r--   0        0        0     3195 2024-03-12 17:08:02.854455 zetascale-2.2.6/zeta/nn/embeddings/vision_emb.py
--rw-r--r--   0        0        0     3208 2023-11-24 07:50:24.220934 zetascale-2.2.6/zeta/nn/embeddings/xpos_relative_position.py
--rw-r--r--   0        0        0     6685 2024-03-12 17:08:03.090171 zetascale-2.2.6/zeta/nn/embeddings/yarn.py
--rw-r--r--   0        0        0     1150 2024-02-20 02:21:04.287040 zetascale-2.2.6/zeta/nn/masks/__init__.py
--rw-r--r--   0        0        0    31987 2024-03-12 17:08:04.258733 zetascale-2.2.6/zeta/nn/masks/attn_masks.py
--rw-r--r--   0        0        0     1248 2024-03-12 17:08:02.883585 zetascale-2.2.6/zeta/nn/masks/block_diagonal.py
--rw-r--r--   0        0        0    15253 2023-09-12 13:55:36.035815 zetascale-2.2.6/zeta/nn/modules/README.md
--rw-r--r--   0        0        0    12591 2024-03-06 07:48:41.914705 zetascale-2.2.6/zeta/nn/modules/__init__.py
--rw-r--r--   0        0        0     7658 2024-03-12 17:08:03.198677 zetascale-2.2.6/zeta/nn/modules/_activations.py
--rw-r--r--   0        0        0     3561 2024-03-12 17:08:03.078712 zetascale-2.2.6/zeta/nn/modules/adaptive_conv.py
--rw-r--r--   0        0        0     1572 2024-02-20 02:21:05.564114 zetascale-2.2.6/zeta/nn/modules/adaptive_layernorm.py
--rw-r--r--   0        0        0     1506 2024-02-20 02:21:05.599056 zetascale-2.2.6/zeta/nn/modules/adaptive_parameter_list.py
--rw-r--r--   0        0        0     2181 2024-03-12 17:08:03.031630 zetascale-2.2.6/zeta/nn/modules/adaptive_rmsnorm.py
--rw-r--r--   0        0        0      465 2024-02-20 02:21:05.714929 zetascale-2.2.6/zeta/nn/modules/add_norm.py
--rw-r--r--   0        0        0     1969 2024-03-12 17:08:03.054998 zetascale-2.2.6/zeta/nn/modules/alr_block.py
--rw-r--r--   0        0        0     1885 2024-02-20 02:21:07.006024 zetascale-2.2.6/zeta/nn/modules/attn.py
--rw-r--r--   0        0        0     1170 2024-02-20 02:21:06.839757 zetascale-2.2.6/zeta/nn/modules/audio_to_text.py
--rw-r--r--   0        0        0     2927 2024-03-12 17:08:03.099808 zetascale-2.2.6/zeta/nn/modules/avg_model_merger.py
--rw-r--r--   0        0        0      200 2023-12-19 19:26:43.426210 zetascale-2.2.6/zeta/nn/modules/batched_dp.py
--rw-r--r--   0        0        0     2355 2024-02-20 02:21:07.701284 zetascale-2.2.6/zeta/nn/modules/block_butterfly_mlp.py
--rw-r--r--   0        0        0    12708 2024-03-12 17:08:03.864220 zetascale-2.2.6/zeta/nn/modules/blockdiag_butterfly.py
--rw-r--r--   0        0        0     7693 2024-03-12 17:08:03.471293 zetascale-2.2.6/zeta/nn/modules/clex.py
--rw-r--r--   0        0        0     2522 2024-03-12 17:08:03.192850 zetascale-2.2.6/zeta/nn/modules/clip_bottleneck.py
--rw-r--r--   0        0        0     1530 2024-03-12 17:08:03.171903 zetascale-2.2.6/zeta/nn/modules/cnn_text.py
--rw-r--r--   0        0        0     4281 2024-03-12 17:08:03.300302 zetascale-2.2.6/zeta/nn/modules/combined_linear.py
--rw-r--r--   0        0        0     1026 2024-02-20 02:21:08.160986 zetascale-2.2.6/zeta/nn/modules/conv_bn_relu.py
--rw-r--r--   0        0        0     2446 2024-03-12 17:08:03.304310 zetascale-2.2.6/zeta/nn/modules/conv_mlp.py
--rw-r--r--   0        0        0      888 2024-02-20 02:21:09.097401 zetascale-2.2.6/zeta/nn/modules/convnet.py
--rw-r--r--   0        0        0     1723 2023-12-29 18:03:56.299433 zetascale-2.2.6/zeta/nn/modules/cross_embed_layer.py
--rw-r--r--   0        0        0     7316 2024-03-12 17:08:03.415262 zetascale-2.2.6/zeta/nn/modules/cross_modal_reparametization.py
--rw-r--r--   0        0        0     3540 2024-03-12 17:08:03.361727 zetascale-2.2.6/zeta/nn/modules/decision_tree.py
--rw-r--r--   0        0        0     2648 2024-02-20 02:21:10.160405 zetascale-2.2.6/zeta/nn/modules/deepseek_moe.py
--rw-r--r--   0        0        0      794 2023-12-25 18:55:47.859671 zetascale-2.2.6/zeta/nn/modules/dense_connect.py
--rw-r--r--   0        0        0     2371 2024-02-20 02:21:09.798586 zetascale-2.2.6/zeta/nn/modules/diffusion.py
--rw-r--r--   0        0        0      532 2024-02-20 02:21:09.698650 zetascale-2.2.6/zeta/nn/modules/droppath.py
--rw-r--r--   0        0        0      796 2023-12-25 19:11:45.652469 zetascale-2.2.6/zeta/nn/modules/dual_path_block.py
--rw-r--r--   0        0        0     4687 2024-02-20 02:21:11.437130 zetascale-2.2.6/zeta/nn/modules/dyna_conv.py
--rw-r--r--   0        0        0     2064 2024-02-20 02:21:10.627986 zetascale-2.2.6/zeta/nn/modules/dynamic_module.py
--rw-r--r--   0        0        0      980 2024-03-12 17:08:03.323481 zetascale-2.2.6/zeta/nn/modules/dynamic_routing_block.py
--rw-r--r--   0        0        0      786 2023-10-24 05:22:56.453163 zetascale-2.2.6/zeta/nn/modules/embedding_to_grid.py
--rw-r--r--   0        0        0    11202 2024-03-12 17:08:03.369914 zetascale-2.2.6/zeta/nn/modules/ether.py
--rw-r--r--   0        0        0     5338 2024-02-20 02:21:10.712472 zetascale-2.2.6/zeta/nn/modules/exo.py
--rw-r--r--   0        0        0      888 2023-10-24 05:22:56.487707 zetascale-2.2.6/zeta/nn/modules/expand_channels.py
--rw-r--r--   0        0        0     1184 2024-01-08 00:23:23.966366 zetascale-2.2.6/zeta/nn/modules/expert.py
--rw-r--r--   0        0        0      678 2024-02-20 02:21:11.125020 zetascale-2.2.6/zeta/nn/modules/fast_text.py
--rw-r--r--   0        0        0     1004 2023-12-25 19:10:00.967347 zetascale-2.2.6/zeta/nn/modules/feedback_block.py
--rw-r--r--   0        0        0     2441 2024-03-12 17:08:03.434115 zetascale-2.2.6/zeta/nn/modules/feedforward.py
--rw-r--r--   0        0        0     4396 2024-03-12 17:08:03.564214 zetascale-2.2.6/zeta/nn/modules/feedforward_network.py
--rw-r--r--   0        0        0     3153 2024-03-12 17:08:03.438496 zetascale-2.2.6/zeta/nn/modules/film.py
--rw-r--r--   0        0        0     2607 2024-01-14 05:11:08.698323 zetascale-2.2.6/zeta/nn/modules/film_conditioning.py
--rw-r--r--   0        0        0     2657 2024-02-20 02:21:12.679701 zetascale-2.2.6/zeta/nn/modules/film_efficient_metb3.py
--rw-r--r--   0        0        0      363 2023-11-18 04:30:04.310707 zetascale-2.2.6/zeta/nn/modules/flash_conv.py
--rw-r--r--   0        0        0      817 2023-12-19 19:26:43.429076 zetascale-2.2.6/zeta/nn/modules/flatten_features.py
--rw-r--r--   0        0        0     3528 2024-03-12 17:08:03.523933 zetascale-2.2.6/zeta/nn/modules/flex_conv.py
--rw-r--r--   0        0        0     2694 2024-03-12 17:08:03.538134 zetascale-2.2.6/zeta/nn/modules/flexible_mlp.py
--rw-r--r--   0        0        0     2552 2024-03-12 17:08:03.528011 zetascale-2.2.6/zeta/nn/modules/fractorial_net.py
--rw-r--r--   0        0        0      769 2024-02-22 19:14:04.770478 zetascale-2.2.6/zeta/nn/modules/freeze_layers.py
--rw-r--r--   0        0        0     2408 2024-03-12 17:08:03.534463 zetascale-2.2.6/zeta/nn/modules/fused_dropout_add.py
--rw-r--r--   0        0        0     1223 2024-02-20 02:21:13.183242 zetascale-2.2.6/zeta/nn/modules/fused_dropout_layernom.py
--rw-r--r--   0        0        0     2268 2024-02-20 02:21:13.592327 zetascale-2.2.6/zeta/nn/modules/fused_gelu_dense.py
--rw-r--r--   0        0        0     1006 2024-02-20 02:21:13.298075 zetascale-2.2.6/zeta/nn/modules/fusion_ffn.py
--rw-r--r--   0        0        0    33392 2024-03-12 17:08:05.481194 zetascale-2.2.6/zeta/nn/modules/g_shard_moe.py
--rw-r--r--   0        0        0      707 2023-12-27 16:22:31.740775 zetascale-2.2.6/zeta/nn/modules/gated_residual_block.py
--rw-r--r--   0        0        0     4104 2024-03-12 17:08:03.702885 zetascale-2.2.6/zeta/nn/modules/gill_mapper.py
--rw-r--r--   0        0        0      920 2024-02-20 03:19:54.342658 zetascale-2.2.6/zeta/nn/modules/glu.py
--rw-r--r--   0        0        0     1826 2024-03-12 17:08:03.620762 zetascale-2.2.6/zeta/nn/modules/gru_gating.py
--rw-r--r--   0        0        0     2634 2023-11-30 08:00:40.761474 zetascale-2.2.6/zeta/nn/modules/h3.py
--rw-r--r--   0        0        0     2078 2024-02-20 02:21:13.917866 zetascale-2.2.6/zeta/nn/modules/hebbian.py
--rw-r--r--   0        0        0      809 2024-02-20 02:21:13.641036 zetascale-2.2.6/zeta/nn/modules/highway_layer.py
--rw-r--r--   0        0        0     3527 2024-03-12 17:08:03.674327 zetascale-2.2.6/zeta/nn/modules/image_projector.py
--rw-r--r--   0        0        0     1049 2024-02-20 02:21:14.054761 zetascale-2.2.6/zeta/nn/modules/image_to_text.py
--rw-r--r--   0        0        0     1385 2024-02-20 02:21:14.700462 zetascale-2.2.6/zeta/nn/modules/img_or_video_to_time.py
--rw-r--r--   0        0        0     1197 2023-12-21 06:04:56.833591 zetascale-2.2.6/zeta/nn/modules/img_patch_embed.py
--rw-r--r--   0        0        0      763 2023-10-24 05:22:56.462573 zetascale-2.2.6/zeta/nn/modules/img_reshape.py
--rw-r--r--   0        0        0     4024 2024-03-12 17:08:03.899369 zetascale-2.2.6/zeta/nn/modules/itca.py
--rw-r--r--   0        0        0     4656 2024-03-12 17:08:03.898644 zetascale-2.2.6/zeta/nn/modules/kv_cache.py
--rw-r--r--   0        0        0     6221 2024-03-12 17:08:04.137958 zetascale-2.2.6/zeta/nn/modules/lambda_mask.py
--rw-r--r--   0        0        0     3504 2024-02-20 02:21:15.562473 zetascale-2.2.6/zeta/nn/modules/lang_conv_module.py
--rw-r--r--   0        0        0     2760 2024-02-20 02:21:15.370804 zetascale-2.2.6/zeta/nn/modules/laser.py
--rw-r--r--   0        0        0     2379 2024-02-20 02:21:15.528047 zetascale-2.2.6/zeta/nn/modules/layernorm.py
--rw-r--r--   0        0        0     1132 2024-02-20 02:21:15.732195 zetascale-2.2.6/zeta/nn/modules/leaky_relu.py
--rw-r--r--   0        0        0    24514 2024-03-12 17:08:04.551145 zetascale-2.2.6/zeta/nn/modules/log_ff.py
--rw-r--r--   0        0        0     1747 2023-12-29 16:19:54.276255 zetascale-2.2.6/zeta/nn/modules/lora.py
--rw-r--r--   0        0        0     3240 2024-03-12 17:08:03.982193 zetascale-2.2.6/zeta/nn/modules/matrix.py
--rw-r--r--   0        0        0     2993 2024-02-05 02:47:16.470298 zetascale-2.2.6/zeta/nn/modules/mbconv.py
--rw-r--r--   0        0        0     2125 2024-02-20 02:21:16.517619 zetascale-2.2.6/zeta/nn/modules/mixtral_expert.py
--rw-r--r--   0        0        0     1884 2024-03-12 17:08:03.941463 zetascale-2.2.6/zeta/nn/modules/mlp.py
--rw-r--r--   0        0        0     3729 2024-03-12 17:08:04.025060 zetascale-2.2.6/zeta/nn/modules/mlp_mixer.py
--rw-r--r--   0        0        0     2435 2024-02-20 02:21:17.308630 zetascale-2.2.6/zeta/nn/modules/mm_adapter.py
--rw-r--r--   0        0        0       87 2024-01-13 18:34:06.474255 zetascale-2.2.6/zeta/nn/modules/mm_fusion.py
--rw-r--r--   0        0        0     2340 2024-02-20 02:21:17.406784 zetascale-2.2.6/zeta/nn/modules/mm_layernorm.py
--rw-r--r--   0        0        0     1405 2024-03-12 17:08:03.947904 zetascale-2.2.6/zeta/nn/modules/mm_ops.py
--rw-r--r--   0        0        0     6234 2024-03-12 17:08:04.186893 zetascale-2.2.6/zeta/nn/modules/modality_adaptive_module.py
--rw-r--r--   0        0        0     2930 2024-01-12 20:34:35.589003 zetascale-2.2.6/zeta/nn/modules/moe.py
--rw-r--r--   0        0        0     3228 2024-03-12 17:08:04.066438 zetascale-2.2.6/zeta/nn/modules/moe_router.py
--rw-r--r--   0        0        0      776 2024-02-20 02:21:17.825560 zetascale-2.2.6/zeta/nn/modules/monarch_mlp.py
--rw-r--r--   0        0        0     1564 2024-03-06 07:48:51.576854 zetascale-2.2.6/zeta/nn/modules/mr_adapter.py
--rw-r--r--   0        0        0     6554 2024-02-20 02:21:19.545623 zetascale-2.2.6/zeta/nn/modules/multi_input_multi_output.py
--rw-r--r--   0        0        0      837 2024-02-20 02:21:18.368530 zetascale-2.2.6/zeta/nn/modules/multi_scale_block.py
--rw-r--r--   0        0        0        2 2023-11-10 22:26:53.685193 zetascale-2.2.6/zeta/nn/modules/multiclass_label.py
--rw-r--r--   0        0        0      225 2023-12-19 19:26:43.445812 zetascale-2.2.6/zeta/nn/modules/multimodal_concat.py
--rw-r--r--   0        0        0      472 2024-02-20 02:21:18.382142 zetascale-2.2.6/zeta/nn/modules/nearest_upsample.py
--rw-r--r--   0        0        0     8309 2024-03-12 17:08:04.427188 zetascale-2.2.6/zeta/nn/modules/nebula.py
--rw-r--r--   0        0        0     2590 2024-02-20 02:21:19.424059 zetascale-2.2.6/zeta/nn/modules/nfn_stem.py
--rw-r--r--   0        0        0     1456 2024-02-20 02:21:18.846159 zetascale-2.2.6/zeta/nn/modules/norm_fractorals.py
--rw-r--r--   0        0        0     2034 2024-01-13 01:44:35.836293 zetascale-2.2.6/zeta/nn/modules/norm_utils.py
--rw-r--r--   0        0        0     2842 2024-02-20 02:21:20.023982 zetascale-2.2.6/zeta/nn/modules/omnimodal_fusion.py
--rw-r--r--   0        0        0     3851 2024-01-13 22:08:51.525372 zetascale-2.2.6/zeta/nn/modules/p_scan.py
--rw-r--r--   0        0        0     2571 2024-02-23 08:38:09.264979 zetascale-2.2.6/zeta/nn/modules/palo_ldp.py
--rw-r--r--   0        0        0      601 2024-01-12 16:28:17.189839 zetascale-2.2.6/zeta/nn/modules/parallel_wrapper.py
--rw-r--r--   0        0        0      200 2024-02-20 02:21:19.576787 zetascale-2.2.6/zeta/nn/modules/patch_img.py
--rw-r--r--   0        0        0      985 2024-01-11 04:33:38.594357 zetascale-2.2.6/zeta/nn/modules/patch_video.py
--rw-r--r--   0        0        0     3180 2024-01-10 07:40:01.644421 zetascale-2.2.6/zeta/nn/modules/perceiver_layer.py
--rw-r--r--   0        0        0     6115 2024-03-12 17:08:04.440415 zetascale-2.2.6/zeta/nn/modules/perceiver_resampler.py
--rw-r--r--   0        0        0     1692 2024-03-12 17:08:04.160718 zetascale-2.2.6/zeta/nn/modules/poly_expert_fusion_network.py
--rw-r--r--   0        0        0     2045 2024-02-20 02:21:20.607131 zetascale-2.2.6/zeta/nn/modules/polymorphic_activation.py
--rw-r--r--   0        0        0     5804 2024-02-20 02:21:21.939907 zetascale-2.2.6/zeta/nn/modules/polymorphic_neuron.py
--rw-r--r--   0        0        0      527 2023-11-29 20:30:23.164354 zetascale-2.2.6/zeta/nn/modules/prenorm.py
--rw-r--r--   0        0        0     1299 2024-03-12 17:08:04.183108 zetascale-2.2.6/zeta/nn/modules/proj_then_softmax.py
--rw-r--r--   0        0        0     7164 2024-03-12 17:08:04.267345 zetascale-2.2.6/zeta/nn/modules/pulsar.py
--rw-r--r--   0        0        0     3451 2024-02-20 02:21:21.996199 zetascale-2.2.6/zeta/nn/modules/pyro.py
--rw-r--r--   0        0        0     9454 2024-03-12 17:08:04.485725 zetascale-2.2.6/zeta/nn/modules/qformer.py
--rw-r--r--   0        0        0      812 2024-01-15 23:55:29.316200 zetascale-2.2.6/zeta/nn/modules/qkv_norm.py
--rw-r--r--   0        0        0     1381 2024-02-20 02:21:22.210314 zetascale-2.2.6/zeta/nn/modules/quantized_layernorm.py
--rw-r--r--   0        0        0     1152 2024-03-12 17:08:04.219236 zetascale-2.2.6/zeta/nn/modules/recurrent_model.py
--rw-r--r--   0        0        0      903 2023-12-25 19:15:44.005559 zetascale-2.2.6/zeta/nn/modules/recursive_block.py
--rw-r--r--   0        0        0      369 2024-03-02 07:30:50.680921 zetascale-2.2.6/zeta/nn/modules/relu_squared.py
--rw-r--r--   0        0        0     5037 2024-03-12 17:08:04.445015 zetascale-2.2.6/zeta/nn/modules/res_net.py
--rw-r--r--   0        0        0      492 2023-10-24 04:20:58.291559 zetascale-2.2.6/zeta/nn/modules/residual.py
--rw-r--r--   0        0        0     2238 2024-02-20 02:21:23.245499 zetascale-2.2.6/zeta/nn/modules/resnet.py
--rw-r--r--   0        0        0      829 2024-02-20 02:21:22.626278 zetascale-2.2.6/zeta/nn/modules/rms_norm.py
--rw-r--r--   0        0        0     1646 2024-02-20 02:21:22.868825 zetascale-2.2.6/zeta/nn/modules/rnn_nlp.py
--rw-r--r--   0        0        0     3106 2024-03-12 17:08:04.350941 zetascale-2.2.6/zeta/nn/modules/s4.py
--rw-r--r--   0        0        0      818 2023-12-19 19:26:43.446233 zetascale-2.2.6/zeta/nn/modules/scale.py
--rw-r--r--   0        0        0      882 2024-03-02 07:30:51.064762 zetascale-2.2.6/zeta/nn/modules/scale_norm.py
--rw-r--r--   0        0        0     1433 2024-02-20 02:21:23.383643 zetascale-2.2.6/zeta/nn/modules/scaled_sinusoidal.py
--rw-r--r--   0        0        0      799 2023-10-24 15:36:34.861776 zetascale-2.2.6/zeta/nn/modules/scalenorm.py
--rw-r--r--   0        0        0     1858 2024-02-20 02:21:23.545588 zetascale-2.2.6/zeta/nn/modules/shift_tokens.py
--rw-r--r--   0        0        0     2877 2024-02-20 02:21:23.721206 zetascale-2.2.6/zeta/nn/modules/shufflenet.py
--rw-r--r--   0        0        0     8939 2024-03-12 17:08:04.608471 zetascale-2.2.6/zeta/nn/modules/sig_lip.py
--rw-r--r--   0        0        0      283 2023-11-09 00:22:32.316816 zetascale-2.2.6/zeta/nn/modules/simple_attention.py
--rw-r--r--   0        0        0      692 2023-11-12 15:13:51.606294 zetascale-2.2.6/zeta/nn/modules/simple_feedforward.py
--rw-r--r--   0        0        0     9680 2024-03-12 17:08:04.644723 zetascale-2.2.6/zeta/nn/modules/simple_mamba.py
--rw-r--r--   0        0        0      764 2023-12-19 19:26:43.436224 zetascale-2.2.6/zeta/nn/modules/simple_res_block.py
--rw-r--r--   0        0        0      978 2023-12-23 05:14:59.170325 zetascale-2.2.6/zeta/nn/modules/simple_resblock.py
--rw-r--r--   0        0        0      638 2023-12-19 19:26:43.443919 zetascale-2.2.6/zeta/nn/modules/simple_rmsnorm.py
--rw-r--r--   0        0        0      509 2023-12-25 18:55:47.862390 zetascale-2.2.6/zeta/nn/modules/skip_connect.py
--rw-r--r--   0        0        0     1194 2024-02-20 02:21:23.914746 zetascale-2.2.6/zeta/nn/modules/skipconnection.py
--rw-r--r--   0        0        0     3553 2024-03-12 17:08:04.540860 zetascale-2.2.6/zeta/nn/modules/slerp_model_merger.py
--rw-r--r--   0        0        0      765 2024-01-16 18:48:36.091054 zetascale-2.2.6/zeta/nn/modules/sp_act.py
--rw-r--r--   0        0        0    22039 2024-03-12 17:08:05.932332 zetascale-2.2.6/zeta/nn/modules/space_time_unet.py
--rw-r--r--   0        0        0     1346 2024-03-12 17:08:04.539605 zetascale-2.2.6/zeta/nn/modules/spacial_transformer.py
--rw-r--r--   0        0        0     4976 2024-02-20 02:21:25.283384 zetascale-2.2.6/zeta/nn/modules/sparq_attn.py
--rw-r--r--   0        0        0     2021 2024-02-20 02:21:24.433522 zetascale-2.2.6/zeta/nn/modules/spatial_downsample.py
--rw-r--r--   0        0        0     1346 2024-03-12 17:08:04.544222 zetascale-2.2.6/zeta/nn/modules/spatial_transformer.py
--rw-r--r--   0        0        0     1041 2024-02-20 02:21:24.810848 zetascale-2.2.6/zeta/nn/modules/squeeze_excitation.py
--rw-r--r--   0        0        0     4334 2024-03-12 17:08:04.701025 zetascale-2.2.6/zeta/nn/modules/ssm.py
--rw-r--r--   0        0        0     7305 2024-03-12 17:08:04.788869 zetascale-2.2.6/zeta/nn/modules/ssm_language.py
--rw-r--r--   0        0        0      942 2024-01-08 00:04:54.571884 zetascale-2.2.6/zeta/nn/modules/stoch_depth.py
--rw-r--r--   0        0        0      958 2023-12-27 16:23:01.966770 zetascale-2.2.6/zeta/nn/modules/stochastic_depth.py
--rw-r--r--   0        0        0     2032 2024-02-20 02:21:25.534554 zetascale-2.2.6/zeta/nn/modules/subln.py
--rw-r--r--   0        0        0      972 2024-02-20 02:21:25.575751 zetascale-2.2.6/zeta/nn/modules/super_resolution.py
--rw-r--r--   0        0        0     5626 2024-03-12 17:08:04.744143 zetascale-2.2.6/zeta/nn/modules/swarmalator.py
--rw-r--r--   0        0        0     1313 2024-02-20 02:21:25.712744 zetascale-2.2.6/zeta/nn/modules/swiglu.py
--rw-r--r--   0        0        0      715 2024-02-20 02:21:25.696562 zetascale-2.2.6/zeta/nn/modules/tensor.py
--rw-r--r--   0        0        0      865 2024-01-09 16:54:56.616879 zetascale-2.2.6/zeta/nn/modules/tensor_to_int.py
--rw-r--r--   0        0        0     3281 2024-03-12 17:08:04.639643 zetascale-2.2.6/zeta/nn/modules/text_scene_fusion.py
--rw-r--r--   0        0        0     2692 2024-03-12 17:08:04.672980 zetascale-2.2.6/zeta/nn/modules/text_video_fuse.py
--rw-r--r--   0        0        0     2104 2024-02-20 02:21:26.347288 zetascale-2.2.6/zeta/nn/modules/time_up_sample.py
--rw-r--r--   0        0        0      631 2024-03-12 17:08:04.667636 zetascale-2.2.6/zeta/nn/modules/to_logits.py
--rw-r--r--   0        0        0     2158 2024-03-12 17:08:04.706429 zetascale-2.2.6/zeta/nn/modules/token_learner.py
--rw-r--r--   0        0        0     1075 2024-02-20 02:21:26.152416 zetascale-2.2.6/zeta/nn/modules/token_mixer.py
--rw-r--r--   0        0        0      189 2023-10-07 02:00:01.902947 zetascale-2.2.6/zeta/nn/modules/token_shift.py
--rw-r--r--   0        0        0    10310 2024-03-12 17:08:05.210522 zetascale-2.2.6/zeta/nn/modules/top_n_gating.py
--rw-r--r--   0        0        0     4363 2024-02-20 02:21:27.101778 zetascale-2.2.6/zeta/nn/modules/transformations.py
--rw-r--r--   0        0        0      921 2024-02-20 02:21:26.371224 zetascale-2.2.6/zeta/nn/modules/triple_skip.py
--rw-r--r--   0        0        0     2193 2024-01-23 14:49:04.463435 zetascale-2.2.6/zeta/nn/modules/triton_rmsnorm.py
--rw-r--r--   0        0        0     4112 2024-01-10 18:04:05.447145 zetascale-2.2.6/zeta/nn/modules/u_mamba.py
--rw-r--r--   0        0        0     4717 2024-03-12 17:08:04.956574 zetascale-2.2.6/zeta/nn/modules/unet.py
--rw-r--r--   0        0        0      974 2024-02-20 02:21:26.656166 zetascale-2.2.6/zeta/nn/modules/v_layernorm.py
--rw-r--r--   0        0        0     1686 2024-03-12 17:08:04.807655 zetascale-2.2.6/zeta/nn/modules/v_pool.py
--rw-r--r--   0        0        0     2809 2024-02-20 02:21:27.251834 zetascale-2.2.6/zeta/nn/modules/video_autoencoder.py
--rw-r--r--   0        0        0     9239 2024-03-12 17:08:05.102603 zetascale-2.2.6/zeta/nn/modules/video_diffusion_modules.py
--rw-r--r--   0        0        0     1497 2024-01-09 02:18:08.376975 zetascale-2.2.6/zeta/nn/modules/video_to_tensor.py
--rw-r--r--   0        0        0     1067 2024-02-20 02:21:27.232331 zetascale-2.2.6/zeta/nn/modules/video_to_text.py
--rw-r--r--   0        0        0     2702 2024-02-20 02:21:27.552948 zetascale-2.2.6/zeta/nn/modules/vision_mamba.py
--rw-r--r--   0        0        0     2018 2024-03-12 17:08:04.833044 zetascale-2.2.6/zeta/nn/modules/vision_weighted_permute_mlp.py
--rw-r--r--   0        0        0     5445 2024-02-20 02:21:27.810272 zetascale-2.2.6/zeta/nn/modules/visual_expert.py
--rw-r--r--   0        0        0     6100 2024-03-12 17:08:05.088354 zetascale-2.2.6/zeta/nn/modules/vit_denoiser.py
--rw-r--r--   0        0        0     3099 2024-02-20 02:21:28.252160 zetascale-2.2.6/zeta/nn/modules/vss_block.py
--rw-r--r--   0        0        0     2775 2024-03-12 17:08:04.893657 zetascale-2.2.6/zeta/nn/modules/ws_conv2d.py
--rw-r--r--   0        0        0       86 2023-07-09 23:46:34.364954 zetascale-2.2.6/zeta/nn/modules/xmoe/__init__.py
--rw-r--r--   0        0        0     2351 2024-03-12 17:08:05.082817 zetascale-2.2.6/zeta/nn/modules/xmoe/global_groups.py
--rw-r--r--   0        0        0    12458 2024-03-12 17:08:05.702507 zetascale-2.2.6/zeta/nn/modules/xmoe/moe_layer.py
--rw-r--r--   0        0        0    18694 2024-03-12 17:08:06.021245 zetascale-2.2.6/zeta/nn/modules/xmoe/routing.py
--rw-r--r--   0        0        0     2302 2024-03-12 17:08:05.160919 zetascale-2.2.6/zeta/nn/modules/yolo.py
--rw-r--r--   0        0        0     2595 2024-02-20 02:21:28.852202 zetascale-2.2.6/zeta/ops/__init__.py
--rw-r--r--   0        0        0      287 2024-01-07 07:16:03.424289 zetascale-2.2.6/zeta/ops/absmax.py
--rw-r--r--   0        0        0     2652 2024-03-12 17:08:05.173619 zetascale-2.2.6/zeta/ops/async_softmax.py
--rw-r--r--   0        0        0     2054 2024-01-07 05:11:53.247763 zetascale-2.2.6/zeta/ops/dilated_attn_ops.py
--rw-r--r--   0        0        0     2017 2024-03-12 17:08:05.321616 zetascale-2.2.6/zeta/ops/einops_from_to.py
--rw-r--r--   0        0        0     1876 2024-03-12 17:08:05.320032 zetascale-2.2.6/zeta/ops/einops_poly.py
--rw-r--r--   0        0        0     2150 2024-03-19 17:49:56.995242 zetascale-2.2.6/zeta/ops/expand.py
--rw-r--r--   0        0        0     1262 2024-03-12 17:08:05.374955 zetascale-2.2.6/zeta/ops/laplace.py
--rw-r--r--   0        0        0    16138 2024-03-12 17:08:05.848451 zetascale-2.2.6/zeta/ops/main.py
--rw-r--r--   0        0        0     1392 2024-02-20 02:21:29.213231 zetascale-2.2.6/zeta/ops/misc_act.py
--rw-r--r--   0        0        0     1671 2023-12-29 21:30:30.265822 zetascale-2.2.6/zeta/ops/mm_rearranges.py
--rw-r--r--   0        0        0      996 2024-02-20 02:21:29.289328 zetascale-2.2.6/zeta/ops/mm_softmax.py
--rw-r--r--   0        0        0     1851 2024-03-12 17:08:05.371465 zetascale-2.2.6/zeta/ops/mos.py
--rw-r--r--   0        0        0      995 2023-10-13 18:22:25.535325 zetascale-2.2.6/zeta/ops/nonlinear.py
--rw-r--r--   0        0        0     5070 2024-03-12 17:08:05.555951 zetascale-2.2.6/zeta/ops/softmax.py
--rw-r--r--   0        0        0     1086 2024-03-12 17:08:05.438443 zetascale-2.2.6/zeta/ops/sparsemax.py
--rw-r--r--   0        0        0      453 2024-03-12 17:08:05.416222 zetascale-2.2.6/zeta/ops/unitwise_norm.py
--rw-r--r--   0        0        0      814 2024-02-20 02:21:29.633384 zetascale-2.2.6/zeta/optim/__init__.py
--rw-r--r--   0        0        0    41198 2024-03-12 17:08:07.066649 zetascale-2.2.6/zeta/optim/batched_optimizer.py
--rw-r--r--   0        0        0    10142 2024-03-12 17:08:05.816147 zetascale-2.2.6/zeta/optim/decoupled_lion.py
--rw-r--r--   0        0        0     6443 2023-11-09 00:22:32.911336 zetascale-2.2.6/zeta/optim/decoupled_optimizer.py
--rw-r--r--   0        0        0    12445 2024-03-12 17:08:05.927362 zetascale-2.2.6/zeta/optim/decoupled_sophia.py
--rw-r--r--   0        0        0     4709 2024-03-12 17:08:05.712989 zetascale-2.2.6/zeta/optim/gradient_ascent.py
--rw-r--r--   0        0        0     2752 2024-02-20 02:21:30.662791 zetascale-2.2.6/zeta/optim/gradient_equillibrum.py
--rw-r--r--   0        0        0    19017 2024-03-12 17:08:06.610046 zetascale-2.2.6/zeta/optim/lion8b.py
--rw-r--r--   0        0        0     3387 2024-03-12 17:20:04.940463 zetascale-2.2.6/zeta/optim/parallel_gradient_descent.py
--rw-r--r--   0        0        0     4536 2024-03-15 15:09:05.079449 zetascale-2.2.6/zeta/optim/stable_adam.py
--rw-r--r--   0        0        0      453 2024-02-20 02:21:30.894505 zetascale-2.2.6/zeta/quant/__init__.py
--rw-r--r--   0        0        0      405 2023-12-27 18:55:30.757913 zetascale-2.2.6/zeta/quant/absmax.py
--rw-r--r--   0        0        0     2098 2024-02-20 02:21:31.386209 zetascale-2.2.6/zeta/quant/bitlinear.py
--rw-r--r--   0        0        0     1947 2024-03-12 17:08:05.865471 zetascale-2.2.6/zeta/quant/half_bit_linear.py
--rw-r--r--   0        0        0    10942 2024-03-12 17:08:06.282121 zetascale-2.2.6/zeta/quant/lfq.py
--rw-r--r--   0        0        0     3126 2024-02-10 02:19:51.497983 zetascale-2.2.6/zeta/quant/niva.py
--rw-r--r--   0        0        0    25173 2024-03-12 17:08:07.085198 zetascale-2.2.6/zeta/quant/qlora.py
--rw-r--r--   0        0        0     6010 2024-03-12 17:08:06.587037 zetascale-2.2.6/zeta/quant/qmoe.py
--rw-r--r--   0        0        0     3785 2024-03-12 17:08:06.081447 zetascale-2.2.6/zeta/quant/quick.py
--rw-r--r--   0        0        0        0 2024-01-03 03:30:55.516534 zetascale-2.2.6/zeta/quant/random_proj_quan.py
--rw-r--r--   0        0        0     1602 2024-03-12 17:08:05.991815 zetascale-2.2.6/zeta/quant/residual_vq.py
--rw-r--r--   0        0        0     1547 2023-10-19 20:04:49.349438 zetascale-2.2.6/zeta/quant/ste.py
--rw-r--r--   0        0        0      522 2024-02-20 03:07:52.541603 zetascale-2.2.6/zeta/rl/__init__.py
--rw-r--r--   0        0        0     4286 2024-03-12 17:08:06.190420 zetascale-2.2.6/zeta/rl/actor_critic.py
--rw-r--r--   0        0        0     2509 2024-02-20 02:21:33.772653 zetascale-2.2.6/zeta/rl/dpo.py
--rw-r--r--   0        0        0     3381 2024-02-20 02:21:33.739053 zetascale-2.2.6/zeta/rl/hindsight_replay.py
--rw-r--r--   0        0        0     2033 2023-11-10 22:26:53.747770 zetascale-2.2.6/zeta/rl/language_reward.py
--rw-r--r--   0        0        0     4130 2024-03-12 17:08:06.213360 zetascale-2.2.6/zeta/rl/ppo.py
--rw-r--r--   0        0        0     4513 2024-03-12 17:08:06.473169 zetascale-2.2.6/zeta/rl/priortized_replay_buffer.py
--rw-r--r--   0        0        0     5765 2024-03-12 17:08:06.471789 zetascale-2.2.6/zeta/rl/priortized_rps.py
--rw-r--r--   0        0        0      128 2023-10-07 01:59:52.333319 zetascale-2.2.6/zeta/rl/rest.py
--rw-r--r--   0        0        0     4585 2024-02-10 02:19:59.618788 zetascale-2.2.6/zeta/rl/reward_model.py
--rw-r--r--   0        0        0     2987 2024-03-12 17:08:06.505750 zetascale-2.2.6/zeta/rl/sumtree.py
--rw-r--r--   0        0        0     3185 2024-03-12 17:08:06.615506 zetascale-2.2.6/zeta/rl/vision_model_rl.py
--rw-r--r--   0        0        0     1227 2024-02-20 03:59:55.774566 zetascale-2.2.6/zeta/structs/__init__.py
--rw-r--r--   0        0        0    11560 2024-03-12 17:08:06.933534 zetascale-2.2.6/zeta/structs/auto_regressive_wrapper.py
--rw-r--r--   0        0        0     3505 2024-03-12 17:08:06.675632 zetascale-2.2.6/zeta/structs/clip_encoder.py
--rw-r--r--   0        0        0     6600 2024-02-20 02:21:38.475830 zetascale-2.2.6/zeta/structs/efficient_net.py
--rw-r--r--   0        0        0     3219 2024-03-12 17:08:06.579407 zetascale-2.2.6/zeta/structs/encoder_decoder.py
--rw-r--r--   0        0        0    28639 2024-03-12 17:08:07.715978 zetascale-2.2.6/zeta/structs/hierarchical_transformer.py
--rw-r--r--   0        0        0     5946 2024-03-12 17:08:06.771710 zetascale-2.2.6/zeta/structs/local_transformer.py
--rw-r--r--   0        0        0     1665 2024-02-20 02:21:37.803384 zetascale-2.2.6/zeta/structs/multi_modal_projector.py
--rw-r--r--   0        0        0    10839 2024-03-12 17:08:07.153852 zetascale-2.2.6/zeta/structs/simple_transformer.py
--rw-r--r--   0        0        0     2468 2024-03-12 17:08:06.698283 zetascale-2.2.6/zeta/structs/simple_vision_encoder.py
--rw-r--r--   0        0        0    68945 2024-03-12 17:08:08.927611 zetascale-2.2.6/zeta/structs/transformer.py
--rw-r--r--   0        0        0     4490 2024-03-12 17:08:06.878786 zetascale-2.2.6/zeta/structs/transformer_block.py
--rw-r--r--   0        0        0      461 2024-02-20 02:21:38.926412 zetascale-2.2.6/zeta/tokenizers/__init__.py
--rw-r--r--   0        0        0     1438 2023-12-23 05:13:40.934254 zetascale-2.2.6/zeta/tokenizers/gptx_tokenizer.py
--rw-r--r--   0        0        0     3079 2024-03-12 17:08:06.850076 zetascale-2.2.6/zeta/tokenizers/llama_sentencepiece.py
--rw-r--r--   0        0        0     3651 2024-03-12 17:08:06.970562 zetascale-2.2.6/zeta/tokenizers/multi_modal_tokenizer.py
--rw-r--r--   0        0        0     3720 2024-03-12 17:08:06.997545 zetascale-2.2.6/zeta/tokenizers/sentence_piece.py
--rw-r--r--   0        0        0     9771 2023-12-19 19:26:43.476444 zetascale-2.2.6/zeta/tokenizers/tokenmonster.py
--rw-r--r--   0        0        0      460 2024-02-20 02:21:39.816336 zetascale-2.2.6/zeta/training/__init__.py
--rw-r--r--   0        0        0     5400 2024-02-20 02:21:40.381513 zetascale-2.2.6/zeta/training/activation_checkpoint.py
--rw-r--r--   0        0        0     2576 2024-03-12 17:08:07.002747 zetascale-2.2.6/zeta/training/dataloader.py
--rw-r--r--   0        0        0     3496 2024-03-12 17:08:07.184296 zetascale-2.2.6/zeta/training/fsdp.py
--rw-r--r--   0        0        0     3186 2024-03-16 00:52:50.202568 zetascale-2.2.6/zeta/training/galore.py
--rw-r--r--   0        0        0     6054 2024-03-12 17:08:07.228332 zetascale-2.2.6/zeta/training/hive_trainer.py
--rw-r--r--   0        0        0     1626 2023-10-23 03:27:31.592537 zetascale-2.2.6/zeta/training/parallel_wrapper.py
--rw-r--r--   0        0        0     2059 2024-03-12 17:08:07.154710 zetascale-2.2.6/zeta/training/scheduler.py
--rw-r--r--   0        0        0     9273 2024-03-12 17:08:07.389221 zetascale-2.2.6/zeta/training/train.py
--rw-r--r--   0        0        0     2347 2024-03-20 20:38:15.450877 zetascale-2.2.6/zeta/utils/__init__.py
--rw-r--r--   0        0        0     3464 2024-03-12 17:08:07.301138 zetascale-2.2.6/zeta/utils/benchmark.py
--rw-r--r--   0        0        0     1347 2024-03-12 17:08:07.197874 zetascale-2.2.6/zeta/utils/cuda_memory_wrapper.py
--rw-r--r--   0        0        0     6424 2024-03-12 17:08:07.321106 zetascale-2.2.6/zeta/utils/cuda_wrapper.py
--rw-r--r--   0        0        0     1337 2024-03-19 17:10:27.077564 zetascale-2.2.6/zeta/utils/disable_logging.py
--rw-r--r--   0        0        0     1184 2024-03-12 17:08:07.232349 zetascale-2.2.6/zeta/utils/enforce_types.py
--rw-r--r--   0        0        0     1110 2024-03-20 21:10:20.934445 zetascale-2.2.6/zeta/utils/img_to_tensor.py
--rw-r--r--   0        0        0     2953 2024-03-12 17:08:07.318804 zetascale-2.2.6/zeta/utils/log_pytorch_op.py
--rw-r--r--   0        0        0    19874 2024-03-12 17:08:07.939241 zetascale-2.2.6/zeta/utils/main.py
--rw-r--r--   0        0        0     1798 2024-03-12 17:08:07.328852 zetascale-2.2.6/zeta/utils/module_device.py
--rw-r--r--   0        0        0      703 2023-12-17 00:28:55.289752 zetascale-2.2.6/zeta/utils/params.py
--rw-r--r--   0        0        0     3966 2024-02-20 02:21:42.476410 zetascale-2.2.6/zeta/utils/save_load_wrapper.py
--rw-r--r--   0        0        0      846 2024-03-20 21:10:20.904725 zetascale-2.2.6/zeta/utils/text_to_tensor.py
--rw-r--r--   0        0        0      751 2024-02-20 02:21:41.805576 zetascale-2.2.6/zeta/utils/verbose_execution.py
--rw-r--r--   0        0        0    25931 2024-03-12 17:08:07.919574 zetascale-2.2.6/zeta/utils/vision_utils.py
--rw-r--r--   0        0        0    22393 1970-01-01 00:00:00.000000 zetascale-2.2.6/setup.py
--rw-r--r--   0        0        0    21789 1970-01-01 00:00:00.000000 zetascale-2.2.6/PKG-INFO
+-rw-r--r--   0        0        0    11342 2023-10-13 21:44:53.585497 zetascale-2.2.7/LICENSE
+-rw-r--r--   0        0        0    20231 2024-02-27 06:39:21.932280 zetascale-2.2.7/README.md
+-rw-r--r--   0        0        0     1457 2024-04-01 18:08:25.665814 zetascale-2.2.7/pyproject.toml
+-rw-r--r--   0        0        0      546 2024-02-20 02:20:54.857337 zetascale-2.2.7/zeta/__init__.py
+-rw-r--r--   0        0        0        0 2023-12-19 19:47:39.268788 zetascale-2.2.7/zeta/cli/__init__.py
+-rw-r--r--   0        0        0     1937 2024-02-20 02:20:55.165790 zetascale-2.2.7/zeta/cli/main.py
+-rw-r--r--   0        0        0      157 2024-02-20 03:07:47.757716 zetascale-2.2.7/zeta/cloud/__init__.py
+-rw-r--r--   0        0        0     2071 2024-03-12 17:08:02.038250 zetascale-2.2.7/zeta/cloud/main.py
+-rw-r--r--   0        0        0     6217 2024-03-12 17:08:02.120591 zetascale-2.2.7/zeta/cloud/sky_api.py
+-rw-r--r--   0        0        0     1809 2024-03-12 17:08:02.079698 zetascale-2.2.7/zeta/models/LongNet.py
+-rw-r--r--   0        0        0        0 2023-07-10 01:12:17.230004 zetascale-2.2.7/zeta/models/Magneto.py
+-rw-r--r--   0        0        0      603 2024-02-22 19:03:14.806609 zetascale-2.2.7/zeta/models/__init__.py
+-rw-r--r--   0        0        0     3308 2024-02-20 02:20:55.572463 zetascale-2.2.7/zeta/models/andromeda.py
+-rw-r--r--   0        0        0      135 2023-12-31 05:32:43.412544 zetascale-2.2.7/zeta/models/base.py
+-rw-r--r--   0        0        0     3311 2024-03-12 17:08:02.117008 zetascale-2.2.7/zeta/models/beit3.py
+-rw-r--r--   0        0        0     6752 2024-02-20 03:07:47.967442 zetascale-2.2.7/zeta/models/gpt4.py
+-rw-r--r--   0        0        0     4288 2024-03-12 17:08:02.180350 zetascale-2.2.7/zeta/models/kosmos.py
+-rw-r--r--   0        0        0      949 2024-02-20 02:20:55.502345 zetascale-2.2.7/zeta/models/llama.py
+-rw-r--r--   0        0        0     3639 2024-03-12 17:08:02.150836 zetascale-2.2.7/zeta/models/max_vit.py
+-rw-r--r--   0        0        0     6678 2024-03-12 17:08:02.311937 zetascale-2.2.7/zeta/models/mega_vit.py
+-rw-r--r--   0        0        0     6927 2024-02-20 02:20:56.942968 zetascale-2.2.7/zeta/models/mm_mamba.py
+-rw-r--r--   0        0        0    12991 2024-03-12 17:08:02.622848 zetascale-2.2.7/zeta/models/navit.py
+-rw-r--r--   0        0        0     1884 2024-02-20 03:07:48.030803 zetascale-2.2.7/zeta/models/palme.py
+-rw-r--r--   0        0        0     2762 2024-03-12 17:08:02.154861 zetascale-2.2.7/zeta/models/vit.py
+-rw-r--r--   0        0        0      219 2024-02-20 03:07:47.976964 zetascale-2.2.7/zeta/nn/__init__.py
+-rw-r--r--   0        0        0     1797 2024-03-19 17:05:56.616851 zetascale-2.2.7/zeta/nn/attention/__init__.py
+-rw-r--r--   0        0        0     4184 2024-03-12 17:08:02.309118 zetascale-2.2.7/zeta/nn/attention/agent_attn.py
+-rw-r--r--   0        0        0    14876 2024-03-12 17:08:02.715767 zetascale-2.2.7/zeta/nn/attention/attend.py
+-rw-r--r--   0        0        0      244 2024-02-20 02:20:56.872011 zetascale-2.2.7/zeta/nn/attention/base.py
+-rw-r--r--   0        0        0     4050 2024-03-12 17:08:02.358668 zetascale-2.2.7/zeta/nn/attention/cross_attention.py
+-rw-r--r--   0        0        0     3236 2023-12-29 17:40:30.936298 zetascale-2.2.7/zeta/nn/attention/cross_attn_images.py
+-rw-r--r--   0        0        0    10734 2024-03-12 17:08:02.527291 zetascale-2.2.7/zeta/nn/attention/dilated_attention.py
+-rw-r--r--   0        0        0     8803 2024-03-12 17:08:02.448488 zetascale-2.2.7/zeta/nn/attention/flash_attention.py
+-rw-r--r--   0        0        0     2161 2024-01-13 18:03:19.763236 zetascale-2.2.7/zeta/nn/attention/linear_attention.py
+-rw-r--r--   0        0        0     2370 2024-03-12 17:08:02.307028 zetascale-2.2.7/zeta/nn/attention/linear_attn_l.py
+-rw-r--r--   0        0        0     9794 2024-03-12 17:08:02.638502 zetascale-2.2.7/zeta/nn/attention/local_attention.py
+-rw-r--r--   0        0        0     1966 2023-12-19 19:26:43.471021 zetascale-2.2.7/zeta/nn/attention/local_attention_mha.py
+-rw-r--r--   0        0        0    18990 2024-03-12 17:08:03.268461 zetascale-2.2.7/zeta/nn/attention/mixture_attention.py
+-rw-r--r--   0        0        0    12414 2024-03-19 16:54:57.559772 zetascale-2.2.7/zeta/nn/attention/multi_grouped_attn.py
+-rw-r--r--   0        0        0     2729 2024-03-12 17:08:02.437305 zetascale-2.2.7/zeta/nn/attention/multi_modal_causal_attention.py
+-rw-r--r--   0        0        0     3879 2023-12-29 18:02:53.657706 zetascale-2.2.7/zeta/nn/attention/multi_modal_cross_attn.py
+-rw-r--r--   0        0        0     5767 2024-03-12 17:08:02.611227 zetascale-2.2.7/zeta/nn/attention/multihead_attention.py
+-rw-r--r--   0        0        0    25390 2024-03-12 17:08:03.886143 zetascale-2.2.7/zeta/nn/attention/multiquery_attention.py
+-rw-r--r--   0        0        0     2198 2024-02-20 02:21:01.439585 zetascale-2.2.7/zeta/nn/attention/shaped_attention.py
+-rw-r--r--   0        0        0     4672 2024-02-20 02:21:02.943176 zetascale-2.2.7/zeta/nn/attention/sparse_attention.py
+-rw-r--r--   0        0        0     1741 2024-03-12 17:08:02.503328 zetascale-2.2.7/zeta/nn/attention/spatial_linear_attention.py
+-rw-r--r--   0        0        0     2973 2024-02-20 02:21:01.927064 zetascale-2.2.7/zeta/nn/attention/xc_attention.py
+-rw-r--r--   0        0        0      482 2024-02-20 02:21:01.042463 zetascale-2.2.7/zeta/nn/biases/__init__.py
+-rw-r--r--   0        0        0     3951 2024-03-12 17:08:02.722676 zetascale-2.2.7/zeta/nn/biases/alibi.py
+-rw-r--r--   0        0        0      245 2024-02-20 02:21:01.653481 zetascale-2.2.7/zeta/nn/biases/base.py
+-rw-r--r--   0        0        0     1348 2024-02-20 02:21:02.183763 zetascale-2.2.7/zeta/nn/biases/dynamic_position_bias.py
+-rw-r--r--   0        0        0     2886 2024-03-12 17:08:02.668729 zetascale-2.2.7/zeta/nn/biases/relative_position_bias.py
+-rw-r--r--   0        0        0     2069 2024-03-02 07:30:50.700992 zetascale-2.2.7/zeta/nn/embeddings/__init__.py
+-rw-r--r--   0        0        0     1231 2023-12-23 05:23:23.147156 zetascale-2.2.7/zeta/nn/embeddings/abc_pos_emb.py
+-rw-r--r--   0        0        0      255 2024-02-20 02:21:02.347272 zetascale-2.2.7/zeta/nn/embeddings/base.py
+-rw-r--r--   0        0        0      723 2024-02-20 02:21:02.661920 zetascale-2.2.7/zeta/nn/embeddings/embedding.py
+-rw-r--r--   0        0        0     2509 2024-01-07 05:11:05.739698 zetascale-2.2.7/zeta/nn/embeddings/multiway_network.py
+-rw-r--r--   0        0        0      358 2024-02-20 02:21:02.600313 zetascale-2.2.7/zeta/nn/embeddings/nominal_embeddings.py
+-rw-r--r--   0        0        0      900 2023-10-24 04:07:16.862154 zetascale-2.2.7/zeta/nn/embeddings/patch_embedding.py
+-rw-r--r--   0        0        0     3120 2024-02-20 02:21:03.171183 zetascale-2.2.7/zeta/nn/embeddings/pi.md
+-rw-r--r--   0        0        0     1996 2024-03-12 17:08:02.654239 zetascale-2.2.7/zeta/nn/embeddings/positional.py
+-rw-r--r--   0        0        0     2584 2024-03-12 17:08:02.753885 zetascale-2.2.7/zeta/nn/embeddings/positional_interpolation.py
+-rw-r--r--   0        0        0     3021 2024-03-12 17:08:02.747974 zetascale-2.2.7/zeta/nn/embeddings/qfsp_embeddings.py
+-rw-r--r--   0        0        0     1668 2024-03-12 17:08:02.722910 zetascale-2.2.7/zeta/nn/embeddings/qft_embeddings.py
+-rw-r--r--   0        0        0     2250 2024-02-20 02:21:03.986803 zetascale-2.2.7/zeta/nn/embeddings/rope.py
+-rw-r--r--   0        0        0     1570 2024-03-02 07:30:50.701708 zetascale-2.2.7/zeta/nn/embeddings/scaled_sinusoidal_embeddings.py
+-rw-r--r--   0        0        0     2345 2024-03-12 17:08:02.798633 zetascale-2.2.7/zeta/nn/embeddings/sine_positional.py
+-rw-r--r--   0        0        0     2650 2024-03-12 17:08:02.815289 zetascale-2.2.7/zeta/nn/embeddings/sinusoidal.py
+-rw-r--r--   0        0        0     1810 2024-03-12 17:08:02.785699 zetascale-2.2.7/zeta/nn/embeddings/truncated_rope.py
+-rw-r--r--   0        0        0     1003 2023-10-24 04:10:28.452387 zetascale-2.2.7/zeta/nn/embeddings/vis_lang_emb.py
+-rw-r--r--   0        0        0     3195 2024-03-12 17:08:02.854455 zetascale-2.2.7/zeta/nn/embeddings/vision_emb.py
+-rw-r--r--   0        0        0     3208 2023-11-24 07:50:24.220934 zetascale-2.2.7/zeta/nn/embeddings/xpos_relative_position.py
+-rw-r--r--   0        0        0     6685 2024-03-12 17:08:03.090171 zetascale-2.2.7/zeta/nn/embeddings/yarn.py
+-rw-r--r--   0        0        0     1150 2024-02-20 02:21:04.287040 zetascale-2.2.7/zeta/nn/masks/__init__.py
+-rw-r--r--   0        0        0    31987 2024-03-12 17:08:04.258733 zetascale-2.2.7/zeta/nn/masks/attn_masks.py
+-rw-r--r--   0        0        0     1248 2024-03-12 17:08:02.883585 zetascale-2.2.7/zeta/nn/masks/block_diagonal.py
+-rw-r--r--   0        0        0    15253 2023-09-12 13:55:36.035815 zetascale-2.2.7/zeta/nn/modules/README.md
+-rw-r--r--   0        0        0    12665 2024-04-01 18:08:13.622360 zetascale-2.2.7/zeta/nn/modules/__init__.py
+-rw-r--r--   0        0        0     7658 2024-03-12 17:08:03.198677 zetascale-2.2.7/zeta/nn/modules/_activations.py
+-rw-r--r--   0        0        0     3561 2024-03-12 17:08:03.078712 zetascale-2.2.7/zeta/nn/modules/adaptive_conv.py
+-rw-r--r--   0        0        0     1572 2024-02-20 02:21:05.564114 zetascale-2.2.7/zeta/nn/modules/adaptive_layernorm.py
+-rw-r--r--   0        0        0     1506 2024-02-20 02:21:05.599056 zetascale-2.2.7/zeta/nn/modules/adaptive_parameter_list.py
+-rw-r--r--   0        0        0     2181 2024-03-12 17:08:03.031630 zetascale-2.2.7/zeta/nn/modules/adaptive_rmsnorm.py
+-rw-r--r--   0        0        0      465 2024-02-20 02:21:05.714929 zetascale-2.2.7/zeta/nn/modules/add_norm.py
+-rw-r--r--   0        0        0     1969 2024-03-12 17:08:03.054998 zetascale-2.2.7/zeta/nn/modules/alr_block.py
+-rw-r--r--   0        0        0     1885 2024-02-20 02:21:07.006024 zetascale-2.2.7/zeta/nn/modules/attn.py
+-rw-r--r--   0        0        0     1170 2024-02-20 02:21:06.839757 zetascale-2.2.7/zeta/nn/modules/audio_to_text.py
+-rw-r--r--   0        0        0     2927 2024-03-12 17:08:03.099808 zetascale-2.2.7/zeta/nn/modules/avg_model_merger.py
+-rw-r--r--   0        0        0      200 2023-12-19 19:26:43.426210 zetascale-2.2.7/zeta/nn/modules/batched_dp.py
+-rw-r--r--   0        0        0     2355 2024-02-20 02:21:07.701284 zetascale-2.2.7/zeta/nn/modules/block_butterfly_mlp.py
+-rw-r--r--   0        0        0    12708 2024-03-12 17:08:03.864220 zetascale-2.2.7/zeta/nn/modules/blockdiag_butterfly.py
+-rw-r--r--   0        0        0     7693 2024-03-12 17:08:03.471293 zetascale-2.2.7/zeta/nn/modules/clex.py
+-rw-r--r--   0        0        0     2522 2024-03-12 17:08:03.192850 zetascale-2.2.7/zeta/nn/modules/clip_bottleneck.py
+-rw-r--r--   0        0        0     1530 2024-03-12 17:08:03.171903 zetascale-2.2.7/zeta/nn/modules/cnn_text.py
+-rw-r--r--   0        0        0     4281 2024-03-12 17:08:03.300302 zetascale-2.2.7/zeta/nn/modules/combined_linear.py
+-rw-r--r--   0        0        0     1026 2024-02-20 02:21:08.160986 zetascale-2.2.7/zeta/nn/modules/conv_bn_relu.py
+-rw-r--r--   0        0        0     2446 2024-03-12 17:08:03.304310 zetascale-2.2.7/zeta/nn/modules/conv_mlp.py
+-rw-r--r--   0        0        0      888 2024-02-20 02:21:09.097401 zetascale-2.2.7/zeta/nn/modules/convnet.py
+-rw-r--r--   0        0        0     1723 2023-12-29 18:03:56.299433 zetascale-2.2.7/zeta/nn/modules/cross_embed_layer.py
+-rw-r--r--   0        0        0     7316 2024-03-12 17:08:03.415262 zetascale-2.2.7/zeta/nn/modules/cross_modal_reparametization.py
+-rw-r--r--   0        0        0     3540 2024-03-12 17:08:03.361727 zetascale-2.2.7/zeta/nn/modules/decision_tree.py
+-rw-r--r--   0        0        0     2648 2024-02-20 02:21:10.160405 zetascale-2.2.7/zeta/nn/modules/deepseek_moe.py
+-rw-r--r--   0        0        0      794 2023-12-25 18:55:47.859671 zetascale-2.2.7/zeta/nn/modules/dense_connect.py
+-rw-r--r--   0        0        0     2371 2024-02-20 02:21:09.798586 zetascale-2.2.7/zeta/nn/modules/diffusion.py
+-rw-r--r--   0        0        0      532 2024-02-20 02:21:09.698650 zetascale-2.2.7/zeta/nn/modules/droppath.py
+-rw-r--r--   0        0        0      796 2023-12-25 19:11:45.652469 zetascale-2.2.7/zeta/nn/modules/dual_path_block.py
+-rw-r--r--   0        0        0     4687 2024-02-20 02:21:11.437130 zetascale-2.2.7/zeta/nn/modules/dyna_conv.py
+-rw-r--r--   0        0        0     2064 2024-02-20 02:21:10.627986 zetascale-2.2.7/zeta/nn/modules/dynamic_module.py
+-rw-r--r--   0        0        0      980 2024-03-12 17:08:03.323481 zetascale-2.2.7/zeta/nn/modules/dynamic_routing_block.py
+-rw-r--r--   0        0        0      786 2023-10-24 05:22:56.453163 zetascale-2.2.7/zeta/nn/modules/embedding_to_grid.py
+-rw-r--r--   0        0        0    11202 2024-03-12 17:08:03.369914 zetascale-2.2.7/zeta/nn/modules/ether.py
+-rw-r--r--   0        0        0     5338 2024-02-20 02:21:10.712472 zetascale-2.2.7/zeta/nn/modules/exo.py
+-rw-r--r--   0        0        0      888 2023-10-24 05:22:56.487707 zetascale-2.2.7/zeta/nn/modules/expand_channels.py
+-rw-r--r--   0        0        0     1184 2024-01-08 00:23:23.966366 zetascale-2.2.7/zeta/nn/modules/expert.py
+-rw-r--r--   0        0        0      678 2024-02-20 02:21:11.125020 zetascale-2.2.7/zeta/nn/modules/fast_text.py
+-rw-r--r--   0        0        0     1004 2023-12-25 19:10:00.967347 zetascale-2.2.7/zeta/nn/modules/feedback_block.py
+-rw-r--r--   0        0        0     2441 2024-03-12 17:08:03.434115 zetascale-2.2.7/zeta/nn/modules/feedforward.py
+-rw-r--r--   0        0        0     4396 2024-03-12 17:08:03.564214 zetascale-2.2.7/zeta/nn/modules/feedforward_network.py
+-rw-r--r--   0        0        0     3153 2024-03-12 17:08:03.438496 zetascale-2.2.7/zeta/nn/modules/film.py
+-rw-r--r--   0        0        0     2607 2024-01-14 05:11:08.698323 zetascale-2.2.7/zeta/nn/modules/film_conditioning.py
+-rw-r--r--   0        0        0     2657 2024-02-20 02:21:12.679701 zetascale-2.2.7/zeta/nn/modules/film_efficient_metb3.py
+-rw-r--r--   0        0        0      363 2023-11-18 04:30:04.310707 zetascale-2.2.7/zeta/nn/modules/flash_conv.py
+-rw-r--r--   0        0        0      817 2023-12-19 19:26:43.429076 zetascale-2.2.7/zeta/nn/modules/flatten_features.py
+-rw-r--r--   0        0        0     3528 2024-03-12 17:08:03.523933 zetascale-2.2.7/zeta/nn/modules/flex_conv.py
+-rw-r--r--   0        0        0     2694 2024-03-12 17:08:03.538134 zetascale-2.2.7/zeta/nn/modules/flexible_mlp.py
+-rw-r--r--   0        0        0     2552 2024-03-12 17:08:03.528011 zetascale-2.2.7/zeta/nn/modules/fractorial_net.py
+-rw-r--r--   0        0        0      769 2024-02-22 19:14:04.770478 zetascale-2.2.7/zeta/nn/modules/freeze_layers.py
+-rw-r--r--   0        0        0     2408 2024-03-12 17:08:03.534463 zetascale-2.2.7/zeta/nn/modules/fused_dropout_add.py
+-rw-r--r--   0        0        0     1223 2024-02-20 02:21:13.183242 zetascale-2.2.7/zeta/nn/modules/fused_dropout_layernom.py
+-rw-r--r--   0        0        0     2268 2024-02-20 02:21:13.592327 zetascale-2.2.7/zeta/nn/modules/fused_gelu_dense.py
+-rw-r--r--   0        0        0     1006 2024-02-20 02:21:13.298075 zetascale-2.2.7/zeta/nn/modules/fusion_ffn.py
+-rw-r--r--   0        0        0    33392 2024-03-12 17:08:05.481194 zetascale-2.2.7/zeta/nn/modules/g_shard_moe.py
+-rw-r--r--   0        0        0      707 2023-12-27 16:22:31.740775 zetascale-2.2.7/zeta/nn/modules/gated_residual_block.py
+-rw-r--r--   0        0        0     4104 2024-03-12 17:08:03.702885 zetascale-2.2.7/zeta/nn/modules/gill_mapper.py
+-rw-r--r--   0        0        0      920 2024-02-20 03:19:54.342658 zetascale-2.2.7/zeta/nn/modules/glu.py
+-rw-r--r--   0        0        0     1826 2024-03-12 17:08:03.620762 zetascale-2.2.7/zeta/nn/modules/gru_gating.py
+-rw-r--r--   0        0        0     2634 2023-11-30 08:00:40.761474 zetascale-2.2.7/zeta/nn/modules/h3.py
+-rw-r--r--   0        0        0     2078 2024-02-20 02:21:13.917866 zetascale-2.2.7/zeta/nn/modules/hebbian.py
+-rw-r--r--   0        0        0      809 2024-02-20 02:21:13.641036 zetascale-2.2.7/zeta/nn/modules/highway_layer.py
+-rw-r--r--   0        0        0     3527 2024-03-12 17:08:03.674327 zetascale-2.2.7/zeta/nn/modules/image_projector.py
+-rw-r--r--   0        0        0     1049 2024-02-20 02:21:14.054761 zetascale-2.2.7/zeta/nn/modules/image_to_text.py
+-rw-r--r--   0        0        0     1385 2024-02-20 02:21:14.700462 zetascale-2.2.7/zeta/nn/modules/img_or_video_to_time.py
+-rw-r--r--   0        0        0     1197 2023-12-21 06:04:56.833591 zetascale-2.2.7/zeta/nn/modules/img_patch_embed.py
+-rw-r--r--   0        0        0      763 2023-10-24 05:22:56.462573 zetascale-2.2.7/zeta/nn/modules/img_reshape.py
+-rw-r--r--   0        0        0     4024 2024-03-12 17:08:03.899369 zetascale-2.2.7/zeta/nn/modules/itca.py
+-rw-r--r--   0        0        0     4656 2024-03-12 17:08:03.898644 zetascale-2.2.7/zeta/nn/modules/kv_cache.py
+-rw-r--r--   0        0        0     6221 2024-03-12 17:08:04.137958 zetascale-2.2.7/zeta/nn/modules/lambda_mask.py
+-rw-r--r--   0        0        0     3504 2024-02-20 02:21:15.562473 zetascale-2.2.7/zeta/nn/modules/lang_conv_module.py
+-rw-r--r--   0        0        0     2760 2024-02-20 02:21:15.370804 zetascale-2.2.7/zeta/nn/modules/laser.py
+-rw-r--r--   0        0        0     2379 2024-02-20 02:21:15.528047 zetascale-2.2.7/zeta/nn/modules/layernorm.py
+-rw-r--r--   0        0        0     1132 2024-02-20 02:21:15.732195 zetascale-2.2.7/zeta/nn/modules/leaky_relu.py
+-rw-r--r--   0        0        0    24514 2024-03-12 17:08:04.551145 zetascale-2.2.7/zeta/nn/modules/log_ff.py
+-rw-r--r--   0        0        0     1747 2023-12-29 16:19:54.276255 zetascale-2.2.7/zeta/nn/modules/lora.py
+-rw-r--r--   0        0        0     3240 2024-03-12 17:08:03.982193 zetascale-2.2.7/zeta/nn/modules/matrix.py
+-rw-r--r--   0        0        0     2993 2024-02-05 02:47:16.470298 zetascale-2.2.7/zeta/nn/modules/mbconv.py
+-rw-r--r--   0        0        0     2125 2024-02-20 02:21:16.517619 zetascale-2.2.7/zeta/nn/modules/mixtral_expert.py
+-rw-r--r--   0        0        0     1884 2024-03-12 17:08:03.941463 zetascale-2.2.7/zeta/nn/modules/mlp.py
+-rw-r--r--   0        0        0     3729 2024-03-12 17:08:04.025060 zetascale-2.2.7/zeta/nn/modules/mlp_mixer.py
+-rw-r--r--   0        0        0     2435 2024-02-20 02:21:17.308630 zetascale-2.2.7/zeta/nn/modules/mm_adapter.py
+-rw-r--r--   0        0        0       87 2024-01-13 18:34:06.474255 zetascale-2.2.7/zeta/nn/modules/mm_fusion.py
+-rw-r--r--   0        0        0     2340 2024-02-20 02:21:17.406784 zetascale-2.2.7/zeta/nn/modules/mm_layernorm.py
+-rw-r--r--   0        0        0     1405 2024-03-12 17:08:03.947904 zetascale-2.2.7/zeta/nn/modules/mm_ops.py
+-rw-r--r--   0        0        0     6234 2024-03-12 17:08:04.186893 zetascale-2.2.7/zeta/nn/modules/modality_adaptive_module.py
+-rw-r--r--   0        0        0     2930 2024-01-12 20:34:35.589003 zetascale-2.2.7/zeta/nn/modules/moe.py
+-rw-r--r--   0        0        0     3228 2024-03-12 17:08:04.066438 zetascale-2.2.7/zeta/nn/modules/moe_router.py
+-rw-r--r--   0        0        0      776 2024-02-20 02:21:17.825560 zetascale-2.2.7/zeta/nn/modules/monarch_mlp.py
+-rw-r--r--   0        0        0     1564 2024-03-06 07:48:51.576854 zetascale-2.2.7/zeta/nn/modules/mr_adapter.py
+-rw-r--r--   0        0        0     6554 2024-02-20 02:21:19.545623 zetascale-2.2.7/zeta/nn/modules/multi_input_multi_output.py
+-rw-r--r--   0        0        0      837 2024-02-20 02:21:18.368530 zetascale-2.2.7/zeta/nn/modules/multi_scale_block.py
+-rw-r--r--   0        0        0        2 2023-11-10 22:26:53.685193 zetascale-2.2.7/zeta/nn/modules/multiclass_label.py
+-rw-r--r--   0        0        0      225 2023-12-19 19:26:43.445812 zetascale-2.2.7/zeta/nn/modules/multimodal_concat.py
+-rw-r--r--   0        0        0      472 2024-02-20 02:21:18.382142 zetascale-2.2.7/zeta/nn/modules/nearest_upsample.py
+-rw-r--r--   0        0        0     8309 2024-03-12 17:08:04.427188 zetascale-2.2.7/zeta/nn/modules/nebula.py
+-rw-r--r--   0        0        0     2590 2024-02-20 02:21:19.424059 zetascale-2.2.7/zeta/nn/modules/nfn_stem.py
+-rw-r--r--   0        0        0     1456 2024-02-20 02:21:18.846159 zetascale-2.2.7/zeta/nn/modules/norm_fractorals.py
+-rw-r--r--   0        0        0     2034 2024-01-13 01:44:35.836293 zetascale-2.2.7/zeta/nn/modules/norm_utils.py
+-rw-r--r--   0        0        0     2842 2024-02-20 02:21:20.023982 zetascale-2.2.7/zeta/nn/modules/omnimodal_fusion.py
+-rw-r--r--   0        0        0     3851 2024-01-13 22:08:51.525372 zetascale-2.2.7/zeta/nn/modules/p_scan.py
+-rw-r--r--   0        0        0     2571 2024-02-23 08:38:09.264979 zetascale-2.2.7/zeta/nn/modules/palo_ldp.py
+-rw-r--r--   0        0        0      601 2024-01-12 16:28:17.189839 zetascale-2.2.7/zeta/nn/modules/parallel_wrapper.py
+-rw-r--r--   0        0        0      200 2024-02-20 02:21:19.576787 zetascale-2.2.7/zeta/nn/modules/patch_img.py
+-rw-r--r--   0        0        0      985 2024-01-11 04:33:38.594357 zetascale-2.2.7/zeta/nn/modules/patch_video.py
+-rw-r--r--   0        0        0     3180 2024-01-10 07:40:01.644421 zetascale-2.2.7/zeta/nn/modules/perceiver_layer.py
+-rw-r--r--   0        0        0     6115 2024-03-12 17:08:04.440415 zetascale-2.2.7/zeta/nn/modules/perceiver_resampler.py
+-rw-r--r--   0        0        0     1692 2024-03-12 17:08:04.160718 zetascale-2.2.7/zeta/nn/modules/poly_expert_fusion_network.py
+-rw-r--r--   0        0        0     2045 2024-02-20 02:21:20.607131 zetascale-2.2.7/zeta/nn/modules/polymorphic_activation.py
+-rw-r--r--   0        0        0     5804 2024-02-20 02:21:21.939907 zetascale-2.2.7/zeta/nn/modules/polymorphic_neuron.py
+-rw-r--r--   0        0        0      527 2023-11-29 20:30:23.164354 zetascale-2.2.7/zeta/nn/modules/prenorm.py
+-rw-r--r--   0        0        0     1299 2024-03-12 17:08:04.183108 zetascale-2.2.7/zeta/nn/modules/proj_then_softmax.py
+-rw-r--r--   0        0        0     7164 2024-03-12 17:08:04.267345 zetascale-2.2.7/zeta/nn/modules/pulsar.py
+-rw-r--r--   0        0        0     3451 2024-02-20 02:21:21.996199 zetascale-2.2.7/zeta/nn/modules/pyro.py
+-rw-r--r--   0        0        0     9454 2024-03-12 17:08:04.485725 zetascale-2.2.7/zeta/nn/modules/qformer.py
+-rw-r--r--   0        0        0      812 2024-01-15 23:55:29.316200 zetascale-2.2.7/zeta/nn/modules/qkv_norm.py
+-rw-r--r--   0        0        0     1381 2024-02-20 02:21:22.210314 zetascale-2.2.7/zeta/nn/modules/quantized_layernorm.py
+-rw-r--r--   0        0        0     1152 2024-03-12 17:08:04.219236 zetascale-2.2.7/zeta/nn/modules/recurrent_model.py
+-rw-r--r--   0        0        0      903 2023-12-25 19:15:44.005559 zetascale-2.2.7/zeta/nn/modules/recursive_block.py
+-rw-r--r--   0        0        0      369 2024-03-02 07:30:50.680921 zetascale-2.2.7/zeta/nn/modules/relu_squared.py
+-rw-r--r--   0        0        0     5037 2024-03-12 17:08:04.445015 zetascale-2.2.7/zeta/nn/modules/res_net.py
+-rw-r--r--   0        0        0      492 2023-10-24 04:20:58.291559 zetascale-2.2.7/zeta/nn/modules/residual.py
+-rw-r--r--   0        0        0     2238 2024-02-20 02:21:23.245499 zetascale-2.2.7/zeta/nn/modules/resnet.py
+-rw-r--r--   0        0        0      829 2024-02-20 02:21:22.626278 zetascale-2.2.7/zeta/nn/modules/rms_norm.py
+-rw-r--r--   0        0        0     1646 2024-02-20 02:21:22.868825 zetascale-2.2.7/zeta/nn/modules/rnn_nlp.py
+-rw-r--r--   0        0        0     3106 2024-03-12 17:08:04.350941 zetascale-2.2.7/zeta/nn/modules/s4.py
+-rw-r--r--   0        0        0      818 2023-12-19 19:26:43.446233 zetascale-2.2.7/zeta/nn/modules/scale.py
+-rw-r--r--   0        0        0      882 2024-03-02 07:30:51.064762 zetascale-2.2.7/zeta/nn/modules/scale_norm.py
+-rw-r--r--   0        0        0     1433 2024-02-20 02:21:23.383643 zetascale-2.2.7/zeta/nn/modules/scaled_sinusoidal.py
+-rw-r--r--   0        0        0      799 2023-10-24 15:36:34.861776 zetascale-2.2.7/zeta/nn/modules/scalenorm.py
+-rw-r--r--   0        0        0     1858 2024-02-20 02:21:23.545588 zetascale-2.2.7/zeta/nn/modules/shift_tokens.py
+-rw-r--r--   0        0        0     2877 2024-02-20 02:21:23.721206 zetascale-2.2.7/zeta/nn/modules/shufflenet.py
+-rw-r--r--   0        0        0     8939 2024-03-12 17:08:04.608471 zetascale-2.2.7/zeta/nn/modules/sig_lip.py
+-rw-r--r--   0        0        0      283 2023-11-09 00:22:32.316816 zetascale-2.2.7/zeta/nn/modules/simple_attention.py
+-rw-r--r--   0        0        0      692 2023-11-12 15:13:51.606294 zetascale-2.2.7/zeta/nn/modules/simple_feedforward.py
+-rw-r--r--   0        0        0     9680 2024-03-12 17:08:04.644723 zetascale-2.2.7/zeta/nn/modules/simple_mamba.py
+-rw-r--r--   0        0        0      764 2023-12-19 19:26:43.436224 zetascale-2.2.7/zeta/nn/modules/simple_res_block.py
+-rw-r--r--   0        0        0      978 2023-12-23 05:14:59.170325 zetascale-2.2.7/zeta/nn/modules/simple_resblock.py
+-rw-r--r--   0        0        0      638 2023-12-19 19:26:43.443919 zetascale-2.2.7/zeta/nn/modules/simple_rmsnorm.py
+-rw-r--r--   0        0        0      509 2023-12-25 18:55:47.862390 zetascale-2.2.7/zeta/nn/modules/skip_connect.py
+-rw-r--r--   0        0        0     1194 2024-02-20 02:21:23.914746 zetascale-2.2.7/zeta/nn/modules/skipconnection.py
+-rw-r--r--   0        0        0     3553 2024-03-12 17:08:04.540860 zetascale-2.2.7/zeta/nn/modules/slerp_model_merger.py
+-rw-r--r--   0        0        0      765 2024-01-16 18:48:36.091054 zetascale-2.2.7/zeta/nn/modules/sp_act.py
+-rw-r--r--   0        0        0    22039 2024-03-12 17:08:05.932332 zetascale-2.2.7/zeta/nn/modules/space_time_unet.py
+-rw-r--r--   0        0        0     1346 2024-03-12 17:08:04.539605 zetascale-2.2.7/zeta/nn/modules/spacial_transformer.py
+-rw-r--r--   0        0        0     4976 2024-02-20 02:21:25.283384 zetascale-2.2.7/zeta/nn/modules/sparq_attn.py
+-rw-r--r--   0        0        0    13865 2024-04-01 18:08:14.050713 zetascale-2.2.7/zeta/nn/modules/sparse_moe.py
+-rw-r--r--   0        0        0     2021 2024-02-20 02:21:24.433522 zetascale-2.2.7/zeta/nn/modules/spatial_downsample.py
+-rw-r--r--   0        0        0     1346 2024-03-12 17:08:04.544222 zetascale-2.2.7/zeta/nn/modules/spatial_transformer.py
+-rw-r--r--   0        0        0     1041 2024-02-20 02:21:24.810848 zetascale-2.2.7/zeta/nn/modules/squeeze_excitation.py
+-rw-r--r--   0        0        0     4334 2024-03-12 17:08:04.701025 zetascale-2.2.7/zeta/nn/modules/ssm.py
+-rw-r--r--   0        0        0     7305 2024-03-12 17:08:04.788869 zetascale-2.2.7/zeta/nn/modules/ssm_language.py
+-rw-r--r--   0        0        0      942 2024-01-08 00:04:54.571884 zetascale-2.2.7/zeta/nn/modules/stoch_depth.py
+-rw-r--r--   0        0        0      958 2023-12-27 16:23:01.966770 zetascale-2.2.7/zeta/nn/modules/stochastic_depth.py
+-rw-r--r--   0        0        0     2032 2024-02-20 02:21:25.534554 zetascale-2.2.7/zeta/nn/modules/subln.py
+-rw-r--r--   0        0        0      972 2024-02-20 02:21:25.575751 zetascale-2.2.7/zeta/nn/modules/super_resolution.py
+-rw-r--r--   0        0        0     5626 2024-03-12 17:08:04.744143 zetascale-2.2.7/zeta/nn/modules/swarmalator.py
+-rw-r--r--   0        0        0     1313 2024-02-20 02:21:25.712744 zetascale-2.2.7/zeta/nn/modules/swiglu.py
+-rw-r--r--   0        0        0      715 2024-02-20 02:21:25.696562 zetascale-2.2.7/zeta/nn/modules/tensor.py
+-rw-r--r--   0        0        0      865 2024-01-09 16:54:56.616879 zetascale-2.2.7/zeta/nn/modules/tensor_to_int.py
+-rw-r--r--   0        0        0     3281 2024-03-12 17:08:04.639643 zetascale-2.2.7/zeta/nn/modules/text_scene_fusion.py
+-rw-r--r--   0        0        0     2692 2024-03-12 17:08:04.672980 zetascale-2.2.7/zeta/nn/modules/text_video_fuse.py
+-rw-r--r--   0        0        0     2104 2024-02-20 02:21:26.347288 zetascale-2.2.7/zeta/nn/modules/time_up_sample.py
+-rw-r--r--   0        0        0      631 2024-03-12 17:08:04.667636 zetascale-2.2.7/zeta/nn/modules/to_logits.py
+-rw-r--r--   0        0        0     2158 2024-03-12 17:08:04.706429 zetascale-2.2.7/zeta/nn/modules/token_learner.py
+-rw-r--r--   0        0        0     1075 2024-02-20 02:21:26.152416 zetascale-2.2.7/zeta/nn/modules/token_mixer.py
+-rw-r--r--   0        0        0      189 2023-10-07 02:00:01.902947 zetascale-2.2.7/zeta/nn/modules/token_shift.py
+-rw-r--r--   0        0        0    10310 2024-03-12 17:08:05.210522 zetascale-2.2.7/zeta/nn/modules/top_n_gating.py
+-rw-r--r--   0        0        0     4363 2024-02-20 02:21:27.101778 zetascale-2.2.7/zeta/nn/modules/transformations.py
+-rw-r--r--   0        0        0      921 2024-02-20 02:21:26.371224 zetascale-2.2.7/zeta/nn/modules/triple_skip.py
+-rw-r--r--   0        0        0     2193 2024-01-23 14:49:04.463435 zetascale-2.2.7/zeta/nn/modules/triton_rmsnorm.py
+-rw-r--r--   0        0        0     4112 2024-01-10 18:04:05.447145 zetascale-2.2.7/zeta/nn/modules/u_mamba.py
+-rw-r--r--   0        0        0     4717 2024-03-12 17:08:04.956574 zetascale-2.2.7/zeta/nn/modules/unet.py
+-rw-r--r--   0        0        0      974 2024-02-20 02:21:26.656166 zetascale-2.2.7/zeta/nn/modules/v_layernorm.py
+-rw-r--r--   0        0        0     1686 2024-03-12 17:08:04.807655 zetascale-2.2.7/zeta/nn/modules/v_pool.py
+-rw-r--r--   0        0        0     2809 2024-02-20 02:21:27.251834 zetascale-2.2.7/zeta/nn/modules/video_autoencoder.py
+-rw-r--r--   0        0        0     9239 2024-03-12 17:08:05.102603 zetascale-2.2.7/zeta/nn/modules/video_diffusion_modules.py
+-rw-r--r--   0        0        0     1497 2024-01-09 02:18:08.376975 zetascale-2.2.7/zeta/nn/modules/video_to_tensor.py
+-rw-r--r--   0        0        0     1067 2024-02-20 02:21:27.232331 zetascale-2.2.7/zeta/nn/modules/video_to_text.py
+-rw-r--r--   0        0        0     2702 2024-02-20 02:21:27.552948 zetascale-2.2.7/zeta/nn/modules/vision_mamba.py
+-rw-r--r--   0        0        0     2018 2024-03-12 17:08:04.833044 zetascale-2.2.7/zeta/nn/modules/vision_weighted_permute_mlp.py
+-rw-r--r--   0        0        0     5445 2024-02-20 02:21:27.810272 zetascale-2.2.7/zeta/nn/modules/visual_expert.py
+-rw-r--r--   0        0        0     6100 2024-03-12 17:08:05.088354 zetascale-2.2.7/zeta/nn/modules/vit_denoiser.py
+-rw-r--r--   0        0        0     3099 2024-02-20 02:21:28.252160 zetascale-2.2.7/zeta/nn/modules/vss_block.py
+-rw-r--r--   0        0        0     2775 2024-03-12 17:08:04.893657 zetascale-2.2.7/zeta/nn/modules/ws_conv2d.py
+-rw-r--r--   0        0        0       86 2023-07-09 23:46:34.364954 zetascale-2.2.7/zeta/nn/modules/xmoe/__init__.py
+-rw-r--r--   0        0        0     2351 2024-03-12 17:08:05.082817 zetascale-2.2.7/zeta/nn/modules/xmoe/global_groups.py
+-rw-r--r--   0        0        0    12458 2024-03-12 17:08:05.702507 zetascale-2.2.7/zeta/nn/modules/xmoe/moe_layer.py
+-rw-r--r--   0        0        0    18694 2024-03-12 17:08:06.021245 zetascale-2.2.7/zeta/nn/modules/xmoe/routing.py
+-rw-r--r--   0        0        0     2302 2024-03-12 17:08:05.160919 zetascale-2.2.7/zeta/nn/modules/yolo.py
+-rw-r--r--   0        0        0     2595 2024-02-20 02:21:28.852202 zetascale-2.2.7/zeta/ops/__init__.py
+-rw-r--r--   0        0        0      287 2024-01-07 07:16:03.424289 zetascale-2.2.7/zeta/ops/absmax.py
+-rw-r--r--   0        0        0     2652 2024-03-12 17:08:05.173619 zetascale-2.2.7/zeta/ops/async_softmax.py
+-rw-r--r--   0        0        0     2054 2024-01-07 05:11:53.247763 zetascale-2.2.7/zeta/ops/dilated_attn_ops.py
+-rw-r--r--   0        0        0     2017 2024-03-12 17:08:05.321616 zetascale-2.2.7/zeta/ops/einops_from_to.py
+-rw-r--r--   0        0        0     1876 2024-03-12 17:08:05.320032 zetascale-2.2.7/zeta/ops/einops_poly.py
+-rw-r--r--   0        0        0     2150 2024-03-19 17:49:56.995242 zetascale-2.2.7/zeta/ops/expand.py
+-rw-r--r--   0        0        0     1262 2024-03-12 17:08:05.374955 zetascale-2.2.7/zeta/ops/laplace.py
+-rw-r--r--   0        0        0    16138 2024-03-12 17:08:05.848451 zetascale-2.2.7/zeta/ops/main.py
+-rw-r--r--   0        0        0     1392 2024-02-20 02:21:29.213231 zetascale-2.2.7/zeta/ops/misc_act.py
+-rw-r--r--   0        0        0     1671 2023-12-29 21:30:30.265822 zetascale-2.2.7/zeta/ops/mm_rearranges.py
+-rw-r--r--   0        0        0      996 2024-02-20 02:21:29.289328 zetascale-2.2.7/zeta/ops/mm_softmax.py
+-rw-r--r--   0        0        0     1851 2024-03-12 17:08:05.371465 zetascale-2.2.7/zeta/ops/mos.py
+-rw-r--r--   0        0        0      995 2023-10-13 18:22:25.535325 zetascale-2.2.7/zeta/ops/nonlinear.py
+-rw-r--r--   0        0        0     5070 2024-03-12 17:08:05.555951 zetascale-2.2.7/zeta/ops/softmax.py
+-rw-r--r--   0        0        0     1086 2024-03-12 17:08:05.438443 zetascale-2.2.7/zeta/ops/sparsemax.py
+-rw-r--r--   0        0        0      453 2024-03-12 17:08:05.416222 zetascale-2.2.7/zeta/ops/unitwise_norm.py
+-rw-r--r--   0        0        0      814 2024-02-20 02:21:29.633384 zetascale-2.2.7/zeta/optim/__init__.py
+-rw-r--r--   0        0        0    41198 2024-03-12 17:08:07.066649 zetascale-2.2.7/zeta/optim/batched_optimizer.py
+-rw-r--r--   0        0        0    10142 2024-03-12 17:08:05.816147 zetascale-2.2.7/zeta/optim/decoupled_lion.py
+-rw-r--r--   0        0        0     6443 2023-11-09 00:22:32.911336 zetascale-2.2.7/zeta/optim/decoupled_optimizer.py
+-rw-r--r--   0        0        0    12445 2024-03-12 17:08:05.927362 zetascale-2.2.7/zeta/optim/decoupled_sophia.py
+-rw-r--r--   0        0        0     4709 2024-03-12 17:08:05.712989 zetascale-2.2.7/zeta/optim/gradient_ascent.py
+-rw-r--r--   0        0        0     2752 2024-02-20 02:21:30.662791 zetascale-2.2.7/zeta/optim/gradient_equillibrum.py
+-rw-r--r--   0        0        0    19017 2024-03-12 17:08:06.610046 zetascale-2.2.7/zeta/optim/lion8b.py
+-rw-r--r--   0        0        0     3387 2024-03-12 17:20:04.940463 zetascale-2.2.7/zeta/optim/parallel_gradient_descent.py
+-rw-r--r--   0        0        0     4536 2024-03-15 15:09:05.079449 zetascale-2.2.7/zeta/optim/stable_adam.py
+-rw-r--r--   0        0        0      453 2024-02-20 02:21:30.894505 zetascale-2.2.7/zeta/quant/__init__.py
+-rw-r--r--   0        0        0      405 2023-12-27 18:55:30.757913 zetascale-2.2.7/zeta/quant/absmax.py
+-rw-r--r--   0        0        0     2098 2024-02-20 02:21:31.386209 zetascale-2.2.7/zeta/quant/bitlinear.py
+-rw-r--r--   0        0        0     1947 2024-03-12 17:08:05.865471 zetascale-2.2.7/zeta/quant/half_bit_linear.py
+-rw-r--r--   0        0        0    10942 2024-03-12 17:08:06.282121 zetascale-2.2.7/zeta/quant/lfq.py
+-rw-r--r--   0        0        0     3126 2024-02-10 02:19:51.497983 zetascale-2.2.7/zeta/quant/niva.py
+-rw-r--r--   0        0        0    25173 2024-03-12 17:08:07.085198 zetascale-2.2.7/zeta/quant/qlora.py
+-rw-r--r--   0        0        0     6010 2024-03-12 17:08:06.587037 zetascale-2.2.7/zeta/quant/qmoe.py
+-rw-r--r--   0        0        0     3785 2024-03-12 17:08:06.081447 zetascale-2.2.7/zeta/quant/quick.py
+-rw-r--r--   0        0        0        0 2024-01-03 03:30:55.516534 zetascale-2.2.7/zeta/quant/random_proj_quan.py
+-rw-r--r--   0        0        0     1602 2024-03-12 17:08:05.991815 zetascale-2.2.7/zeta/quant/residual_vq.py
+-rw-r--r--   0        0        0     1547 2023-10-19 20:04:49.349438 zetascale-2.2.7/zeta/quant/ste.py
+-rw-r--r--   0        0        0      522 2024-02-20 03:07:52.541603 zetascale-2.2.7/zeta/rl/__init__.py
+-rw-r--r--   0        0        0     4286 2024-03-12 17:08:06.190420 zetascale-2.2.7/zeta/rl/actor_critic.py
+-rw-r--r--   0        0        0     2509 2024-02-20 02:21:33.772653 zetascale-2.2.7/zeta/rl/dpo.py
+-rw-r--r--   0        0        0     3381 2024-02-20 02:21:33.739053 zetascale-2.2.7/zeta/rl/hindsight_replay.py
+-rw-r--r--   0        0        0     2033 2023-11-10 22:26:53.747770 zetascale-2.2.7/zeta/rl/language_reward.py
+-rw-r--r--   0        0        0     4130 2024-03-12 17:08:06.213360 zetascale-2.2.7/zeta/rl/ppo.py
+-rw-r--r--   0        0        0     4513 2024-03-12 17:08:06.473169 zetascale-2.2.7/zeta/rl/priortized_replay_buffer.py
+-rw-r--r--   0        0        0     5765 2024-03-12 17:08:06.471789 zetascale-2.2.7/zeta/rl/priortized_rps.py
+-rw-r--r--   0        0        0      128 2023-10-07 01:59:52.333319 zetascale-2.2.7/zeta/rl/rest.py
+-rw-r--r--   0        0        0     4585 2024-02-10 02:19:59.618788 zetascale-2.2.7/zeta/rl/reward_model.py
+-rw-r--r--   0        0        0     2987 2024-03-12 17:08:06.505750 zetascale-2.2.7/zeta/rl/sumtree.py
+-rw-r--r--   0        0        0     3185 2024-03-12 17:08:06.615506 zetascale-2.2.7/zeta/rl/vision_model_rl.py
+-rw-r--r--   0        0        0     1227 2024-02-20 03:59:55.774566 zetascale-2.2.7/zeta/structs/__init__.py
+-rw-r--r--   0        0        0    11560 2024-03-12 17:08:06.933534 zetascale-2.2.7/zeta/structs/auto_regressive_wrapper.py
+-rw-r--r--   0        0        0     3505 2024-03-12 17:08:06.675632 zetascale-2.2.7/zeta/structs/clip_encoder.py
+-rw-r--r--   0        0        0     6600 2024-02-20 02:21:38.475830 zetascale-2.2.7/zeta/structs/efficient_net.py
+-rw-r--r--   0        0        0     3219 2024-03-12 17:08:06.579407 zetascale-2.2.7/zeta/structs/encoder_decoder.py
+-rw-r--r--   0        0        0    28639 2024-03-12 17:08:07.715978 zetascale-2.2.7/zeta/structs/hierarchical_transformer.py
+-rw-r--r--   0        0        0     5946 2024-03-12 17:08:06.771710 zetascale-2.2.7/zeta/structs/local_transformer.py
+-rw-r--r--   0        0        0     1665 2024-02-20 02:21:37.803384 zetascale-2.2.7/zeta/structs/multi_modal_projector.py
+-rw-r--r--   0        0        0    10839 2024-03-12 17:08:07.153852 zetascale-2.2.7/zeta/structs/simple_transformer.py
+-rw-r--r--   0        0        0     2468 2024-03-12 17:08:06.698283 zetascale-2.2.7/zeta/structs/simple_vision_encoder.py
+-rw-r--r--   0        0        0    68945 2024-03-12 17:08:08.927611 zetascale-2.2.7/zeta/structs/transformer.py
+-rw-r--r--   0        0        0     4490 2024-03-12 17:08:06.878786 zetascale-2.2.7/zeta/structs/transformer_block.py
+-rw-r--r--   0        0        0      461 2024-02-20 02:21:38.926412 zetascale-2.2.7/zeta/tokenizers/__init__.py
+-rw-r--r--   0        0        0     1438 2023-12-23 05:13:40.934254 zetascale-2.2.7/zeta/tokenizers/gptx_tokenizer.py
+-rw-r--r--   0        0        0     3079 2024-03-12 17:08:06.850076 zetascale-2.2.7/zeta/tokenizers/llama_sentencepiece.py
+-rw-r--r--   0        0        0     3651 2024-03-12 17:08:06.970562 zetascale-2.2.7/zeta/tokenizers/multi_modal_tokenizer.py
+-rw-r--r--   0        0        0     3720 2024-03-12 17:08:06.997545 zetascale-2.2.7/zeta/tokenizers/sentence_piece.py
+-rw-r--r--   0        0        0     9771 2023-12-19 19:26:43.476444 zetascale-2.2.7/zeta/tokenizers/tokenmonster.py
+-rw-r--r--   0        0        0      460 2024-02-20 02:21:39.816336 zetascale-2.2.7/zeta/training/__init__.py
+-rw-r--r--   0        0        0     5400 2024-02-20 02:21:40.381513 zetascale-2.2.7/zeta/training/activation_checkpoint.py
+-rw-r--r--   0        0        0     2576 2024-03-12 17:08:07.002747 zetascale-2.2.7/zeta/training/dataloader.py
+-rw-r--r--   0        0        0     3496 2024-03-12 17:08:07.184296 zetascale-2.2.7/zeta/training/fsdp.py
+-rw-r--r--   0        0        0     3186 2024-03-16 00:52:50.202568 zetascale-2.2.7/zeta/training/galore.py
+-rw-r--r--   0        0        0     6054 2024-03-12 17:08:07.228332 zetascale-2.2.7/zeta/training/hive_trainer.py
+-rw-r--r--   0        0        0     1626 2023-10-23 03:27:31.592537 zetascale-2.2.7/zeta/training/parallel_wrapper.py
+-rw-r--r--   0        0        0     2059 2024-03-12 17:08:07.154710 zetascale-2.2.7/zeta/training/scheduler.py
+-rw-r--r--   0        0        0     9273 2024-03-12 17:08:07.389221 zetascale-2.2.7/zeta/training/train.py
+-rw-r--r--   0        0        0     2347 2024-03-20 20:38:15.450877 zetascale-2.2.7/zeta/utils/__init__.py
+-rw-r--r--   0        0        0     3464 2024-03-12 17:08:07.301138 zetascale-2.2.7/zeta/utils/benchmark.py
+-rw-r--r--   0        0        0     1347 2024-03-12 17:08:07.197874 zetascale-2.2.7/zeta/utils/cuda_memory_wrapper.py
+-rw-r--r--   0        0        0     6424 2024-03-12 17:08:07.321106 zetascale-2.2.7/zeta/utils/cuda_wrapper.py
+-rw-r--r--   0        0        0     1337 2024-03-19 17:10:27.077564 zetascale-2.2.7/zeta/utils/disable_logging.py
+-rw-r--r--   0        0        0     1184 2024-03-12 17:08:07.232349 zetascale-2.2.7/zeta/utils/enforce_types.py
+-rw-r--r--   0        0        0     1110 2024-03-20 21:10:20.934445 zetascale-2.2.7/zeta/utils/img_to_tensor.py
+-rw-r--r--   0        0        0     2953 2024-03-12 17:08:07.318804 zetascale-2.2.7/zeta/utils/log_pytorch_op.py
+-rw-r--r--   0        0        0    19874 2024-03-12 17:08:07.939241 zetascale-2.2.7/zeta/utils/main.py
+-rw-r--r--   0        0        0     1798 2024-03-12 17:08:07.328852 zetascale-2.2.7/zeta/utils/module_device.py
+-rw-r--r--   0        0        0      703 2023-12-17 00:28:55.289752 zetascale-2.2.7/zeta/utils/params.py
+-rw-r--r--   0        0        0     3966 2024-02-20 02:21:42.476410 zetascale-2.2.7/zeta/utils/save_load_wrapper.py
+-rw-r--r--   0        0        0      846 2024-03-20 21:10:20.904725 zetascale-2.2.7/zeta/utils/text_to_tensor.py
+-rw-r--r--   0        0        0      751 2024-02-20 02:21:41.805576 zetascale-2.2.7/zeta/utils/verbose_execution.py
+-rw-r--r--   0        0        0    25931 2024-03-12 17:08:07.919574 zetascale-2.2.7/zeta/utils/vision_utils.py
+-rw-r--r--   0        0        0    22393 1970-01-01 00:00:00.000000 zetascale-2.2.7/setup.py
+-rw-r--r--   0        0        0    21789 1970-01-01 00:00:00.000000 zetascale-2.2.7/PKG-INFO
```

### Comparing `zetascale-2.2.6/LICENSE` & `zetascale-2.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/README.md` & `zetascale-2.2.7/README.md`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/pyproject.toml` & `zetascale-2.2.7/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zetascale"
-version = "2.2.6"
+version = "2.2.7"
 description = "Transformers at zeta scales"
 authors = ["Zeta Team <kye@apac.ai>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/kyegomez/zeta"
 keywords = ["Transformers", "zeta scale"]
 classifiers = [
```

### Comparing `zetascale-2.2.6/zeta/__init__.py` & `zetascale-2.2.7/zeta/__init__.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/cli/main.py` & `zetascale-2.2.7/zeta/cli/main.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/cloud/main.py` & `zetascale-2.2.7/zeta/cloud/main.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/cloud/sky_api.py` & `zetascale-2.2.7/zeta/cloud/sky_api.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/models/LongNet.py` & `zetascale-2.2.7/zeta/models/LongNet.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/models/__init__.py` & `zetascale-2.2.7/zeta/models/__init__.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/models/andromeda.py` & `zetascale-2.2.7/zeta/models/andromeda.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/models/beit3.py` & `zetascale-2.2.7/zeta/models/beit3.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/models/gpt4.py` & `zetascale-2.2.7/zeta/models/gpt4.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/models/kosmos.py` & `zetascale-2.2.7/zeta/models/kosmos.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/models/llama.py` & `zetascale-2.2.7/zeta/models/llama.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/models/max_vit.py` & `zetascale-2.2.7/zeta/models/max_vit.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/models/mega_vit.py` & `zetascale-2.2.7/zeta/models/mega_vit.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/models/mm_mamba.py` & `zetascale-2.2.7/zeta/models/mm_mamba.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/models/navit.py` & `zetascale-2.2.7/zeta/models/navit.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/models/palme.py` & `zetascale-2.2.7/zeta/models/palme.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/models/vit.py` & `zetascale-2.2.7/zeta/models/vit.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/attention/__init__.py` & `zetascale-2.2.7/zeta/nn/attention/__init__.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/attention/agent_attn.py` & `zetascale-2.2.7/zeta/nn/attention/agent_attn.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/attention/attend.py` & `zetascale-2.2.7/zeta/nn/attention/attend.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/attention/cross_attention.py` & `zetascale-2.2.7/zeta/nn/attention/cross_attention.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/attention/cross_attn_images.py` & `zetascale-2.2.7/zeta/nn/attention/cross_attn_images.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/attention/dilated_attention.py` & `zetascale-2.2.7/zeta/nn/attention/dilated_attention.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/attention/flash_attention.py` & `zetascale-2.2.7/zeta/nn/attention/flash_attention.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/attention/linear_attention.py` & `zetascale-2.2.7/zeta/nn/attention/linear_attention.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/attention/linear_attn_l.py` & `zetascale-2.2.7/zeta/nn/attention/linear_attn_l.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/attention/local_attention.py` & `zetascale-2.2.7/zeta/nn/attention/local_attention.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/attention/local_attention_mha.py` & `zetascale-2.2.7/zeta/nn/attention/local_attention_mha.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/attention/mixture_attention.py` & `zetascale-2.2.7/zeta/nn/attention/mixture_attention.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/attention/multi_grouped_attn.py` & `zetascale-2.2.7/zeta/nn/attention/multi_grouped_attn.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/attention/multi_modal_causal_attention.py` & `zetascale-2.2.7/zeta/nn/attention/multi_modal_causal_attention.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/attention/multi_modal_cross_attn.py` & `zetascale-2.2.7/zeta/nn/attention/multi_modal_cross_attn.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/attention/multihead_attention.py` & `zetascale-2.2.7/zeta/nn/attention/multihead_attention.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/attention/multiquery_attention.py` & `zetascale-2.2.7/zeta/nn/attention/multiquery_attention.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/attention/shaped_attention.py` & `zetascale-2.2.7/zeta/nn/attention/shaped_attention.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/attention/sparse_attention.py` & `zetascale-2.2.7/zeta/nn/attention/sparse_attention.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/attention/spatial_linear_attention.py` & `zetascale-2.2.7/zeta/nn/attention/spatial_linear_attention.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/attention/xc_attention.py` & `zetascale-2.2.7/zeta/nn/attention/xc_attention.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/biases/alibi.py` & `zetascale-2.2.7/zeta/nn/biases/alibi.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/biases/dynamic_position_bias.py` & `zetascale-2.2.7/zeta/nn/biases/dynamic_position_bias.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/biases/relative_position_bias.py` & `zetascale-2.2.7/zeta/nn/biases/relative_position_bias.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/embeddings/__init__.py` & `zetascale-2.2.7/zeta/nn/embeddings/__init__.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/embeddings/abc_pos_emb.py` & `zetascale-2.2.7/zeta/nn/embeddings/abc_pos_emb.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/embeddings/embedding.py` & `zetascale-2.2.7/zeta/nn/embeddings/embedding.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/embeddings/multiway_network.py` & `zetascale-2.2.7/zeta/nn/embeddings/multiway_network.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/embeddings/patch_embedding.py` & `zetascale-2.2.7/zeta/nn/embeddings/patch_embedding.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/embeddings/pi.md` & `zetascale-2.2.7/zeta/nn/embeddings/pi.md`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/embeddings/positional.py` & `zetascale-2.2.7/zeta/nn/embeddings/positional.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/embeddings/positional_interpolation.py` & `zetascale-2.2.7/zeta/nn/embeddings/positional_interpolation.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/embeddings/qfsp_embeddings.py` & `zetascale-2.2.7/zeta/nn/embeddings/qfsp_embeddings.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/embeddings/qft_embeddings.py` & `zetascale-2.2.7/zeta/nn/embeddings/qft_embeddings.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/embeddings/rope.py` & `zetascale-2.2.7/zeta/nn/embeddings/rope.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/embeddings/scaled_sinusoidal_embeddings.py` & `zetascale-2.2.7/zeta/nn/embeddings/scaled_sinusoidal_embeddings.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/embeddings/sine_positional.py` & `zetascale-2.2.7/zeta/nn/embeddings/sine_positional.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/embeddings/sinusoidal.py` & `zetascale-2.2.7/zeta/nn/embeddings/sinusoidal.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/embeddings/truncated_rope.py` & `zetascale-2.2.7/zeta/nn/embeddings/truncated_rope.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/embeddings/vis_lang_emb.py` & `zetascale-2.2.7/zeta/nn/embeddings/vis_lang_emb.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/embeddings/vision_emb.py` & `zetascale-2.2.7/zeta/nn/embeddings/vision_emb.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/embeddings/xpos_relative_position.py` & `zetascale-2.2.7/zeta/nn/embeddings/xpos_relative_position.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/embeddings/yarn.py` & `zetascale-2.2.7/zeta/nn/embeddings/yarn.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/masks/__init__.py` & `zetascale-2.2.7/zeta/nn/masks/__init__.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/masks/attn_masks.py` & `zetascale-2.2.7/zeta/nn/masks/attn_masks.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/masks/block_diagonal.py` & `zetascale-2.2.7/zeta/nn/masks/block_diagonal.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/README.md` & `zetascale-2.2.7/zeta/nn/modules/README.md`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/__init__.py` & `zetascale-2.2.7/zeta/nn/modules/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -187,20 +187,19 @@
 )
 from zeta.nn.modules.ws_conv2d import WSConv2d
 from zeta.nn.modules.yolo import yolo
 from zeta.nn.modules.palo_ldp import PaloLDP
 from zeta.nn.modules.relu_squared import ReluSquared
 from zeta.nn.modules.scale_norm import ScaleNorm
 from zeta.nn.modules.mr_adapter import MRAdapter
-
-# from zeta.nn.modules.g_shard_moe import (
-#     Top1Gate,
-#     Top2Gate,
-#     GShardMoELayer,
-# )
+from zeta.nn.modules.sparse_moe import (
+    Top2Gating,
+    NormalSparseMoE,
+    HeirarchicalSparseMoE,
+)
 
 # from zeta.nn.modules.img_reshape import image_reshape
 # from zeta.nn.modules.flatten_features import flatten_features
 # from zeta.nn.modules.scaled_sinusoidal import ScaledSinuosidalEmbedding
 # from zeta.nn.modules.scale import Scale
 # from zeta.nn.modules.scalenorm import ScaleNorm
 # from zeta.nn.modules.simple_rmsnorm import SimpleRMSNorm
@@ -388,8 +387,11 @@
     "DynamicOutputDecoder",
     "DynamicInputChannels",
     "OutputDecoders",
     "PaloLDP",
     "ReluSquared",
     "ScaleNorm",
     "MRAdapter",
+    "Top2Gating",
+    "NormalSparseMoE",
+    "HeirarchicalSparseMoE",
 ]
```

### Comparing `zetascale-2.2.6/zeta/nn/modules/_activations.py` & `zetascale-2.2.7/zeta/nn/modules/_activations.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/adaptive_conv.py` & `zetascale-2.2.7/zeta/nn/modules/adaptive_conv.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/adaptive_layernorm.py` & `zetascale-2.2.7/zeta/nn/modules/adaptive_layernorm.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/adaptive_parameter_list.py` & `zetascale-2.2.7/zeta/nn/modules/adaptive_parameter_list.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/adaptive_rmsnorm.py` & `zetascale-2.2.7/zeta/nn/modules/adaptive_rmsnorm.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/alr_block.py` & `zetascale-2.2.7/zeta/nn/modules/alr_block.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/attn.py` & `zetascale-2.2.7/zeta/nn/modules/attn.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/audio_to_text.py` & `zetascale-2.2.7/zeta/nn/modules/audio_to_text.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/avg_model_merger.py` & `zetascale-2.2.7/zeta/nn/modules/avg_model_merger.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/block_butterfly_mlp.py` & `zetascale-2.2.7/zeta/nn/modules/block_butterfly_mlp.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/blockdiag_butterfly.py` & `zetascale-2.2.7/zeta/nn/modules/blockdiag_butterfly.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/clex.py` & `zetascale-2.2.7/zeta/nn/modules/clex.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/clip_bottleneck.py` & `zetascale-2.2.7/zeta/nn/modules/clip_bottleneck.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/cnn_text.py` & `zetascale-2.2.7/zeta/nn/modules/cnn_text.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/combined_linear.py` & `zetascale-2.2.7/zeta/nn/modules/combined_linear.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/conv_bn_relu.py` & `zetascale-2.2.7/zeta/nn/modules/conv_bn_relu.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/conv_mlp.py` & `zetascale-2.2.7/zeta/nn/modules/conv_mlp.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/convnet.py` & `zetascale-2.2.7/zeta/nn/modules/convnet.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/cross_embed_layer.py` & `zetascale-2.2.7/zeta/nn/modules/cross_embed_layer.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/cross_modal_reparametization.py` & `zetascale-2.2.7/zeta/nn/modules/cross_modal_reparametization.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/decision_tree.py` & `zetascale-2.2.7/zeta/nn/modules/decision_tree.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/deepseek_moe.py` & `zetascale-2.2.7/zeta/nn/modules/deepseek_moe.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/dense_connect.py` & `zetascale-2.2.7/zeta/nn/modules/dense_connect.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/diffusion.py` & `zetascale-2.2.7/zeta/nn/modules/diffusion.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/droppath.py` & `zetascale-2.2.7/zeta/nn/modules/droppath.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/dual_path_block.py` & `zetascale-2.2.7/zeta/nn/modules/dual_path_block.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/dyna_conv.py` & `zetascale-2.2.7/zeta/nn/modules/dyna_conv.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/dynamic_module.py` & `zetascale-2.2.7/zeta/nn/modules/dynamic_module.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/dynamic_routing_block.py` & `zetascale-2.2.7/zeta/nn/modules/dynamic_routing_block.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/embedding_to_grid.py` & `zetascale-2.2.7/zeta/nn/modules/embedding_to_grid.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/ether.py` & `zetascale-2.2.7/zeta/nn/modules/ether.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/exo.py` & `zetascale-2.2.7/zeta/nn/modules/exo.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/expand_channels.py` & `zetascale-2.2.7/zeta/nn/modules/expand_channels.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/expert.py` & `zetascale-2.2.7/zeta/nn/modules/expert.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/fast_text.py` & `zetascale-2.2.7/zeta/nn/modules/fast_text.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/feedback_block.py` & `zetascale-2.2.7/zeta/nn/modules/feedback_block.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/feedforward.py` & `zetascale-2.2.7/zeta/nn/modules/feedforward.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/feedforward_network.py` & `zetascale-2.2.7/zeta/nn/modules/feedforward_network.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/film.py` & `zetascale-2.2.7/zeta/nn/modules/film.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/film_conditioning.py` & `zetascale-2.2.7/zeta/nn/modules/film_conditioning.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/film_efficient_metb3.py` & `zetascale-2.2.7/zeta/nn/modules/film_efficient_metb3.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/flatten_features.py` & `zetascale-2.2.7/zeta/nn/modules/flatten_features.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/flex_conv.py` & `zetascale-2.2.7/zeta/nn/modules/flex_conv.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/flexible_mlp.py` & `zetascale-2.2.7/zeta/nn/modules/flexible_mlp.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/fractorial_net.py` & `zetascale-2.2.7/zeta/nn/modules/fractorial_net.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/freeze_layers.py` & `zetascale-2.2.7/zeta/nn/modules/freeze_layers.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/fused_dropout_add.py` & `zetascale-2.2.7/zeta/nn/modules/fused_dropout_add.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/fused_dropout_layernom.py` & `zetascale-2.2.7/zeta/nn/modules/fused_dropout_layernom.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/fused_gelu_dense.py` & `zetascale-2.2.7/zeta/nn/modules/fused_gelu_dense.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/fusion_ffn.py` & `zetascale-2.2.7/zeta/nn/modules/fusion_ffn.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/g_shard_moe.py` & `zetascale-2.2.7/zeta/nn/modules/g_shard_moe.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/gated_residual_block.py` & `zetascale-2.2.7/zeta/nn/modules/gated_residual_block.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/gill_mapper.py` & `zetascale-2.2.7/zeta/nn/modules/gill_mapper.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/glu.py` & `zetascale-2.2.7/zeta/nn/modules/glu.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/gru_gating.py` & `zetascale-2.2.7/zeta/nn/modules/gru_gating.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/h3.py` & `zetascale-2.2.7/zeta/nn/modules/h3.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/hebbian.py` & `zetascale-2.2.7/zeta/nn/modules/hebbian.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/highway_layer.py` & `zetascale-2.2.7/zeta/nn/modules/highway_layer.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/image_projector.py` & `zetascale-2.2.7/zeta/nn/modules/image_projector.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/image_to_text.py` & `zetascale-2.2.7/zeta/nn/modules/image_to_text.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/img_or_video_to_time.py` & `zetascale-2.2.7/zeta/nn/modules/img_or_video_to_time.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/img_patch_embed.py` & `zetascale-2.2.7/zeta/nn/modules/img_patch_embed.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/img_reshape.py` & `zetascale-2.2.7/zeta/nn/modules/img_reshape.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/itca.py` & `zetascale-2.2.7/zeta/nn/modules/itca.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/kv_cache.py` & `zetascale-2.2.7/zeta/nn/modules/kv_cache.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/lambda_mask.py` & `zetascale-2.2.7/zeta/nn/modules/lambda_mask.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/lang_conv_module.py` & `zetascale-2.2.7/zeta/nn/modules/lang_conv_module.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/laser.py` & `zetascale-2.2.7/zeta/nn/modules/laser.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/layernorm.py` & `zetascale-2.2.7/zeta/nn/modules/layernorm.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/leaky_relu.py` & `zetascale-2.2.7/zeta/nn/modules/leaky_relu.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/log_ff.py` & `zetascale-2.2.7/zeta/nn/modules/log_ff.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/lora.py` & `zetascale-2.2.7/zeta/nn/modules/lora.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/matrix.py` & `zetascale-2.2.7/zeta/nn/modules/matrix.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/mbconv.py` & `zetascale-2.2.7/zeta/nn/modules/mbconv.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/mixtral_expert.py` & `zetascale-2.2.7/zeta/nn/modules/mixtral_expert.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/mlp.py` & `zetascale-2.2.7/zeta/nn/modules/mlp.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/mlp_mixer.py` & `zetascale-2.2.7/zeta/nn/modules/mlp_mixer.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/mm_adapter.py` & `zetascale-2.2.7/zeta/nn/modules/mm_adapter.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/mm_layernorm.py` & `zetascale-2.2.7/zeta/nn/modules/mm_layernorm.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/mm_ops.py` & `zetascale-2.2.7/zeta/nn/modules/mm_ops.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/modality_adaptive_module.py` & `zetascale-2.2.7/zeta/nn/modules/modality_adaptive_module.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/moe.py` & `zetascale-2.2.7/zeta/nn/modules/moe.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/moe_router.py` & `zetascale-2.2.7/zeta/nn/modules/moe_router.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/monarch_mlp.py` & `zetascale-2.2.7/zeta/nn/modules/monarch_mlp.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/mr_adapter.py` & `zetascale-2.2.7/zeta/nn/modules/mr_adapter.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/multi_input_multi_output.py` & `zetascale-2.2.7/zeta/nn/modules/multi_input_multi_output.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/multi_scale_block.py` & `zetascale-2.2.7/zeta/nn/modules/multi_scale_block.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/nebula.py` & `zetascale-2.2.7/zeta/nn/modules/nebula.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/nfn_stem.py` & `zetascale-2.2.7/zeta/nn/modules/nfn_stem.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/norm_fractorals.py` & `zetascale-2.2.7/zeta/nn/modules/norm_fractorals.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/norm_utils.py` & `zetascale-2.2.7/zeta/nn/modules/norm_utils.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/omnimodal_fusion.py` & `zetascale-2.2.7/zeta/nn/modules/omnimodal_fusion.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/p_scan.py` & `zetascale-2.2.7/zeta/nn/modules/p_scan.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/palo_ldp.py` & `zetascale-2.2.7/zeta/nn/modules/palo_ldp.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/parallel_wrapper.py` & `zetascale-2.2.7/zeta/nn/modules/parallel_wrapper.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/patch_video.py` & `zetascale-2.2.7/zeta/nn/modules/patch_video.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/perceiver_layer.py` & `zetascale-2.2.7/zeta/nn/modules/perceiver_layer.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/perceiver_resampler.py` & `zetascale-2.2.7/zeta/nn/modules/perceiver_resampler.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/poly_expert_fusion_network.py` & `zetascale-2.2.7/zeta/nn/modules/poly_expert_fusion_network.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/polymorphic_activation.py` & `zetascale-2.2.7/zeta/nn/modules/polymorphic_activation.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/polymorphic_neuron.py` & `zetascale-2.2.7/zeta/nn/modules/polymorphic_neuron.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/prenorm.py` & `zetascale-2.2.7/zeta/nn/modules/prenorm.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/proj_then_softmax.py` & `zetascale-2.2.7/zeta/nn/modules/proj_then_softmax.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/pulsar.py` & `zetascale-2.2.7/zeta/nn/modules/pulsar.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/pyro.py` & `zetascale-2.2.7/zeta/nn/modules/pyro.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/qformer.py` & `zetascale-2.2.7/zeta/nn/modules/qformer.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/qkv_norm.py` & `zetascale-2.2.7/zeta/nn/modules/qkv_norm.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/quantized_layernorm.py` & `zetascale-2.2.7/zeta/nn/modules/quantized_layernorm.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/recurrent_model.py` & `zetascale-2.2.7/zeta/nn/modules/recurrent_model.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/recursive_block.py` & `zetascale-2.2.7/zeta/nn/modules/recursive_block.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/res_net.py` & `zetascale-2.2.7/zeta/nn/modules/res_net.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/resnet.py` & `zetascale-2.2.7/zeta/nn/modules/resnet.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/rms_norm.py` & `zetascale-2.2.7/zeta/nn/modules/rms_norm.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/rnn_nlp.py` & `zetascale-2.2.7/zeta/nn/modules/rnn_nlp.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/s4.py` & `zetascale-2.2.7/zeta/nn/modules/s4.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/scale.py` & `zetascale-2.2.7/zeta/nn/modules/scale.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/scale_norm.py` & `zetascale-2.2.7/zeta/nn/modules/scale_norm.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/scaled_sinusoidal.py` & `zetascale-2.2.7/zeta/nn/modules/scaled_sinusoidal.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/scalenorm.py` & `zetascale-2.2.7/zeta/nn/modules/scalenorm.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/shift_tokens.py` & `zetascale-2.2.7/zeta/nn/modules/shift_tokens.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/shufflenet.py` & `zetascale-2.2.7/zeta/nn/modules/shufflenet.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/sig_lip.py` & `zetascale-2.2.7/zeta/nn/modules/sig_lip.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/simple_feedforward.py` & `zetascale-2.2.7/zeta/nn/modules/simple_feedforward.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/simple_mamba.py` & `zetascale-2.2.7/zeta/nn/modules/simple_mamba.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/simple_res_block.py` & `zetascale-2.2.7/zeta/nn/modules/simple_res_block.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/simple_resblock.py` & `zetascale-2.2.7/zeta/nn/modules/simple_resblock.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/simple_rmsnorm.py` & `zetascale-2.2.7/zeta/nn/modules/simple_rmsnorm.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/skipconnection.py` & `zetascale-2.2.7/zeta/nn/modules/skipconnection.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/slerp_model_merger.py` & `zetascale-2.2.7/zeta/nn/modules/slerp_model_merger.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/sp_act.py` & `zetascale-2.2.7/zeta/nn/modules/sp_act.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/space_time_unet.py` & `zetascale-2.2.7/zeta/nn/modules/space_time_unet.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/spacial_transformer.py` & `zetascale-2.2.7/zeta/nn/modules/spacial_transformer.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/sparq_attn.py` & `zetascale-2.2.7/zeta/nn/modules/sparq_attn.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/spatial_downsample.py` & `zetascale-2.2.7/zeta/nn/modules/spatial_downsample.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/spatial_transformer.py` & `zetascale-2.2.7/zeta/nn/modules/spatial_transformer.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/squeeze_excitation.py` & `zetascale-2.2.7/zeta/nn/modules/squeeze_excitation.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/ssm.py` & `zetascale-2.2.7/zeta/nn/modules/ssm.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/ssm_language.py` & `zetascale-2.2.7/zeta/nn/modules/ssm_language.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/stoch_depth.py` & `zetascale-2.2.7/zeta/nn/modules/stoch_depth.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/stochastic_depth.py` & `zetascale-2.2.7/zeta/nn/modules/stochastic_depth.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/subln.py` & `zetascale-2.2.7/zeta/nn/modules/subln.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/super_resolution.py` & `zetascale-2.2.7/zeta/nn/modules/super_resolution.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/swarmalator.py` & `zetascale-2.2.7/zeta/nn/modules/swarmalator.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/swiglu.py` & `zetascale-2.2.7/zeta/nn/modules/swiglu.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/tensor.py` & `zetascale-2.2.7/zeta/nn/modules/tensor.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/tensor_to_int.py` & `zetascale-2.2.7/zeta/nn/modules/tensor_to_int.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/text_scene_fusion.py` & `zetascale-2.2.7/zeta/nn/modules/text_scene_fusion.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/text_video_fuse.py` & `zetascale-2.2.7/zeta/nn/modules/text_video_fuse.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/time_up_sample.py` & `zetascale-2.2.7/zeta/nn/modules/time_up_sample.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/to_logits.py` & `zetascale-2.2.7/zeta/nn/modules/to_logits.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/token_learner.py` & `zetascale-2.2.7/zeta/nn/modules/token_learner.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/token_mixer.py` & `zetascale-2.2.7/zeta/nn/modules/token_mixer.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/top_n_gating.py` & `zetascale-2.2.7/zeta/nn/modules/top_n_gating.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/transformations.py` & `zetascale-2.2.7/zeta/nn/modules/transformations.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/triple_skip.py` & `zetascale-2.2.7/zeta/nn/modules/triple_skip.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/triton_rmsnorm.py` & `zetascale-2.2.7/zeta/nn/modules/triton_rmsnorm.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/u_mamba.py` & `zetascale-2.2.7/zeta/nn/modules/u_mamba.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/unet.py` & `zetascale-2.2.7/zeta/nn/modules/unet.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/v_layernorm.py` & `zetascale-2.2.7/zeta/nn/modules/v_layernorm.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/v_pool.py` & `zetascale-2.2.7/zeta/nn/modules/v_pool.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/video_autoencoder.py` & `zetascale-2.2.7/zeta/nn/modules/video_autoencoder.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/video_diffusion_modules.py` & `zetascale-2.2.7/zeta/nn/modules/video_diffusion_modules.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/video_to_tensor.py` & `zetascale-2.2.7/zeta/nn/modules/video_to_tensor.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/video_to_text.py` & `zetascale-2.2.7/zeta/nn/modules/video_to_text.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/vision_mamba.py` & `zetascale-2.2.7/zeta/nn/modules/vision_mamba.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/vision_weighted_permute_mlp.py` & `zetascale-2.2.7/zeta/nn/modules/vision_weighted_permute_mlp.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/visual_expert.py` & `zetascale-2.2.7/zeta/nn/modules/visual_expert.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/vit_denoiser.py` & `zetascale-2.2.7/zeta/nn/modules/vit_denoiser.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/vss_block.py` & `zetascale-2.2.7/zeta/nn/modules/vss_block.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/ws_conv2d.py` & `zetascale-2.2.7/zeta/nn/modules/ws_conv2d.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/xmoe/global_groups.py` & `zetascale-2.2.7/zeta/nn/modules/xmoe/global_groups.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/xmoe/moe_layer.py` & `zetascale-2.2.7/zeta/nn/modules/xmoe/moe_layer.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/xmoe/routing.py` & `zetascale-2.2.7/zeta/nn/modules/xmoe/routing.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/nn/modules/yolo.py` & `zetascale-2.2.7/zeta/nn/modules/yolo.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/ops/__init__.py` & `zetascale-2.2.7/zeta/ops/__init__.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/ops/async_softmax.py` & `zetascale-2.2.7/zeta/ops/async_softmax.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/ops/dilated_attn_ops.py` & `zetascale-2.2.7/zeta/ops/dilated_attn_ops.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/ops/einops_from_to.py` & `zetascale-2.2.7/zeta/ops/einops_from_to.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/ops/einops_poly.py` & `zetascale-2.2.7/zeta/ops/einops_poly.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/ops/expand.py` & `zetascale-2.2.7/zeta/ops/expand.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/ops/laplace.py` & `zetascale-2.2.7/zeta/ops/laplace.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/ops/main.py` & `zetascale-2.2.7/zeta/ops/main.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/ops/misc_act.py` & `zetascale-2.2.7/zeta/ops/misc_act.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/ops/mm_rearranges.py` & `zetascale-2.2.7/zeta/ops/mm_rearranges.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/ops/mm_softmax.py` & `zetascale-2.2.7/zeta/ops/mm_softmax.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/ops/mos.py` & `zetascale-2.2.7/zeta/ops/mos.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/ops/nonlinear.py` & `zetascale-2.2.7/zeta/ops/nonlinear.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/ops/softmax.py` & `zetascale-2.2.7/zeta/ops/softmax.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/ops/sparsemax.py` & `zetascale-2.2.7/zeta/ops/sparsemax.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/optim/__init__.py` & `zetascale-2.2.7/zeta/optim/__init__.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/optim/batched_optimizer.py` & `zetascale-2.2.7/zeta/optim/batched_optimizer.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/optim/decoupled_lion.py` & `zetascale-2.2.7/zeta/optim/decoupled_lion.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/optim/decoupled_optimizer.py` & `zetascale-2.2.7/zeta/optim/decoupled_optimizer.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/optim/decoupled_sophia.py` & `zetascale-2.2.7/zeta/optim/decoupled_sophia.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/optim/gradient_ascent.py` & `zetascale-2.2.7/zeta/optim/gradient_ascent.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/optim/gradient_equillibrum.py` & `zetascale-2.2.7/zeta/optim/gradient_equillibrum.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/optim/lion8b.py` & `zetascale-2.2.7/zeta/optim/lion8b.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/optim/parallel_gradient_descent.py` & `zetascale-2.2.7/zeta/optim/parallel_gradient_descent.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/optim/stable_adam.py` & `zetascale-2.2.7/zeta/optim/stable_adam.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/quant/bitlinear.py` & `zetascale-2.2.7/zeta/quant/bitlinear.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/quant/half_bit_linear.py` & `zetascale-2.2.7/zeta/quant/half_bit_linear.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/quant/lfq.py` & `zetascale-2.2.7/zeta/quant/lfq.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/quant/niva.py` & `zetascale-2.2.7/zeta/quant/niva.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/quant/qlora.py` & `zetascale-2.2.7/zeta/quant/qlora.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/quant/qmoe.py` & `zetascale-2.2.7/zeta/quant/qmoe.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/quant/quick.py` & `zetascale-2.2.7/zeta/quant/quick.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/quant/residual_vq.py` & `zetascale-2.2.7/zeta/quant/residual_vq.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/quant/ste.py` & `zetascale-2.2.7/zeta/quant/ste.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/rl/__init__.py` & `zetascale-2.2.7/zeta/rl/__init__.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/rl/actor_critic.py` & `zetascale-2.2.7/zeta/rl/actor_critic.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/rl/dpo.py` & `zetascale-2.2.7/zeta/rl/dpo.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/rl/hindsight_replay.py` & `zetascale-2.2.7/zeta/rl/hindsight_replay.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/rl/language_reward.py` & `zetascale-2.2.7/zeta/rl/language_reward.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/rl/ppo.py` & `zetascale-2.2.7/zeta/rl/ppo.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/rl/priortized_replay_buffer.py` & `zetascale-2.2.7/zeta/rl/priortized_replay_buffer.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/rl/priortized_rps.py` & `zetascale-2.2.7/zeta/rl/priortized_rps.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/rl/reward_model.py` & `zetascale-2.2.7/zeta/rl/reward_model.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/rl/sumtree.py` & `zetascale-2.2.7/zeta/rl/sumtree.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/rl/vision_model_rl.py` & `zetascale-2.2.7/zeta/rl/vision_model_rl.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/structs/__init__.py` & `zetascale-2.2.7/zeta/structs/__init__.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/structs/auto_regressive_wrapper.py` & `zetascale-2.2.7/zeta/structs/auto_regressive_wrapper.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/structs/clip_encoder.py` & `zetascale-2.2.7/zeta/structs/clip_encoder.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/structs/efficient_net.py` & `zetascale-2.2.7/zeta/structs/efficient_net.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/structs/encoder_decoder.py` & `zetascale-2.2.7/zeta/structs/encoder_decoder.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/structs/hierarchical_transformer.py` & `zetascale-2.2.7/zeta/structs/hierarchical_transformer.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/structs/local_transformer.py` & `zetascale-2.2.7/zeta/structs/local_transformer.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/structs/multi_modal_projector.py` & `zetascale-2.2.7/zeta/structs/multi_modal_projector.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/structs/simple_transformer.py` & `zetascale-2.2.7/zeta/structs/simple_transformer.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/structs/simple_vision_encoder.py` & `zetascale-2.2.7/zeta/structs/simple_vision_encoder.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/structs/transformer.py` & `zetascale-2.2.7/zeta/structs/transformer.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/structs/transformer_block.py` & `zetascale-2.2.7/zeta/structs/transformer_block.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/tokenizers/gptx_tokenizer.py` & `zetascale-2.2.7/zeta/tokenizers/gptx_tokenizer.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/tokenizers/llama_sentencepiece.py` & `zetascale-2.2.7/zeta/tokenizers/llama_sentencepiece.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/tokenizers/multi_modal_tokenizer.py` & `zetascale-2.2.7/zeta/tokenizers/multi_modal_tokenizer.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/tokenizers/sentence_piece.py` & `zetascale-2.2.7/zeta/tokenizers/sentence_piece.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/tokenizers/tokenmonster.py` & `zetascale-2.2.7/zeta/tokenizers/tokenmonster.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/training/activation_checkpoint.py` & `zetascale-2.2.7/zeta/training/activation_checkpoint.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/training/dataloader.py` & `zetascale-2.2.7/zeta/training/dataloader.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/training/fsdp.py` & `zetascale-2.2.7/zeta/training/fsdp.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/training/galore.py` & `zetascale-2.2.7/zeta/training/galore.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/training/hive_trainer.py` & `zetascale-2.2.7/zeta/training/hive_trainer.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/training/parallel_wrapper.py` & `zetascale-2.2.7/zeta/training/parallel_wrapper.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/training/scheduler.py` & `zetascale-2.2.7/zeta/training/scheduler.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/training/train.py` & `zetascale-2.2.7/zeta/training/train.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/utils/__init__.py` & `zetascale-2.2.7/zeta/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/utils/benchmark.py` & `zetascale-2.2.7/zeta/utils/benchmark.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/utils/cuda_memory_wrapper.py` & `zetascale-2.2.7/zeta/utils/cuda_memory_wrapper.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/utils/cuda_wrapper.py` & `zetascale-2.2.7/zeta/utils/cuda_wrapper.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/utils/disable_logging.py` & `zetascale-2.2.7/zeta/utils/disable_logging.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/utils/enforce_types.py` & `zetascale-2.2.7/zeta/utils/enforce_types.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/utils/img_to_tensor.py` & `zetascale-2.2.7/zeta/utils/img_to_tensor.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/utils/log_pytorch_op.py` & `zetascale-2.2.7/zeta/utils/log_pytorch_op.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/utils/main.py` & `zetascale-2.2.7/zeta/utils/main.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/utils/module_device.py` & `zetascale-2.2.7/zeta/utils/module_device.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/utils/params.py` & `zetascale-2.2.7/zeta/utils/params.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/utils/save_load_wrapper.py` & `zetascale-2.2.7/zeta/utils/save_load_wrapper.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/utils/text_to_tensor.py` & `zetascale-2.2.7/zeta/utils/text_to_tensor.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/utils/verbose_execution.py` & `zetascale-2.2.7/zeta/utils/verbose_execution.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/zeta/utils/vision_utils.py` & `zetascale-2.2.7/zeta/utils/vision_utils.py`

 * *Files identical despite different names*

### Comparing `zetascale-2.2.6/setup.py` & `zetascale-2.2.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
  'vector-quantize-pytorch==1.14.1']
 
 entry_points = \
 {'console_scripts': ['zeta = zeta.cli.main:main']}
 
 setup_kwargs = {
     'name': 'zetascale',
-    'version': '2.2.6',
+    'version': '2.2.7',
     'description': 'Transformers at zeta scales',
     'long_description': '[![Multi-Modality](images/agorabanner.png)](https://discord.gg/qUtxnK2NMf)\n\n![Zeta banner](images/zeta.png)\nBuild SOTA AI Models 80% faster with modular, high-performance, and scalable building blocks!\n\n[![Docs](https://readthedocs.org/projects/zeta/badge/)](https://zeta.readthedocs.io)\n\n<p>\n  <a href="https://github.com/kyegomez/zeta/blob/main/LICENSE"><img alt="MIT License" src="https://img.shields.io/badge/license-MIT-blue.svg" /></a>\n  <a href="https://pypi.org/project/zetascale"><img alt="MIT License" src="https://badge.fury.io/py/zetascale.svg" /></a>\n</p>\n\n[![GitHub issues](https://img.shields.io/github/issues/kyegomez/zeta)](https://github.com/kyegomez/zeta/issues) [![GitHub forks](https://img.shields.io/github/forks/kyegomez/zeta)](https://github.com/kyegomez/zeta/network) [![GitHub stars](https://img.shields.io/github/stars/kyegomez/zeta)](https://github.com/kyegomez/zeta/stargazers) [![GitHub license](https://img.shields.io/github/license/kyegomez/zeta)](https://github.com/kyegomez/zeta/blob/main/LICENSE)[![GitHub star chart](https://img.shields.io/github/stars/kyegomez/zeta?style=social)](https://star-history.com/#kyegomez/zeta)[![Dependency Status](https://img.shields.io/librariesio/github/kyegomez/zeta)](https://libraries.io/github/kyegomez/zeta) [![Downloads](https://static.pepy.tech/badge/zeta/month)](https://pepy.tech/project/zeta)\n\n[![Join the Agora discord](https://img.shields.io/discord/1110910277110743103?label=Discord&logo=discord&logoColor=white&style=plastic&color=d7b023)![Share on Twitter](https://img.shields.io/twitter/url/https/twitter.com/cloudposse.svg?style=social&label=Share%20%40kyegomez/zeta)](https://twitter.com/intent/tweet?text=Check%20out%20this%20amazing%20AI%20project:%20&url=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fzeta) [![Share on Facebook](https://img.shields.io/badge/Share-%20facebook-blue)](https://www.facebook.com/sharer/sharer.php?u=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fzeta) [![Share on LinkedIn](https://img.shields.io/badge/Share-%20linkedin-blue)](https://www.linkedin.com/shareArticle?mini=true&url=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fzeta&title=&summary=&source=)\n\n[![Share on Reddit](https://img.shields.io/badge/-Share%20on%20Reddit-orange)](https://www.reddit.com/submit?url=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fzeta&title=zeta%20-%20the%20future%20of%20AI) [![Share on Hacker News](https://img.shields.io/badge/-Share%20on%20Hacker%20News-orange)](https://news.ycombinator.com/submitlink?u=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fzeta&t=zeta%20-%20the%20future%20of%20AI) [![Share on Pinterest](https://img.shields.io/badge/-Share%20on%20Pinterest-red)](https://pinterest.com/pin/create/button/?url=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fzeta&media=https%3A%2F%2Fexample.com%2Fimage.jpg&description=zeta%20-%20the%20future%20of%20AI) [![Share on WhatsApp](https://img.shields.io/badge/-Share%20on%20WhatsApp-green)](https://api.whatsapp.com/send?text=Check%20out%20zeta%20-%20the%20future%20of%20AI%20%23zeta%20%23AI%0A%0Ahttps%3A%2F%2Fgithub.com%2Fkyegomez%2Fzeta)\n\nAfter building out thousands of neural nets and facing the same annoying bottlenecks of chaotic codebases with no modularity and low performance modules, Zeta needed to be born to enable me and others to quickly prototype, train, and optimize the latest SOTA neural nets and deploy them into production. \n\nZeta places a radical emphasis on useability, modularity, and performance. Zeta is now currently employed in 100s of models across my github and across others. \nGet started below and LMK if you want my help building any model, I\'m here for you 😊 💜 \n\n\n# Install\n\n`$ pip3 install -U zetascale`\n\n# Usage\n\n## Starting Your Journey\n\nCreating a model empowered with the aforementioned breakthrough research features is a breeze. Here\'s how to quickly materialize the renowned Flash Attention\n\n```python\nimport torch\n\nfrom zeta.nn import FlashAttention\n\nq = torch.randn(2, 4, 6, 8)\nk = torch.randn(2, 4, 10, 8)\nv = torch.randn(2, 4, 10, 8)\n\nattention = FlashAttention(causal=False, dropout=0.1, flash=True)\noutput = attention(q, k, v)\n\nprint(output.shape)\n```\n\n\n\n### `SwiGLU`\n- Powers Transformer models\n```python\nimport torch\n\nfrom zeta.nn import SwiGLUStacked\n\nx = torch.randn(5, 10)\nswiglu = SwiGLUStacked(10, 20)\nswiglu(x).shape\n```\n\n### ```RelativePositionBias```\n- ```RelativePositionBias``` quantizes the distance between two positions into a certain number of buckets and then uses an embedding to get the relative position bias. This mechanism aids in the attention mechanism by providing biases based on relative positions between the query and key, rather than relying solely on their absolute positions.\n```python\nimport torch\nfrom torch import nn\n\nfrom zeta.nn import RelativePositionBias\n\n# Initialize the RelativePositionBias module\nrel_pos_bias = RelativePositionBias()\n\n# Example 1: Compute bias for a single batch\nbias_matrix = rel_pos_bias(1, 10, 10)\n\n\n# Example 2: Utilize in conjunction with an attention mechanism\n# NOTE: This is a mock example, and may not represent an actual attention mechanism\'s complete implementation.\nclass MockAttention(nn.Module):\n    def __init__(self):\n        super().__init__()\n        self.rel_pos_bias = RelativePositionBias()\n\n    def forward(self, queries, keys):\n        bias = self.rel_pos_bias(queries.size(0), queries.size(1), keys.size(1))\n        # Further computations with bias in the attention mechanism...\n        return None  # Placeholder\n\n\n# Example 3: Modify default configurations\ncustom_rel_pos_bias = RelativePositionBias(\n    bidirectional=False, num_buckets=64, max_distance=256, num_heads=8\n)\n```\n\n### `FeedForward`\nThe FeedForward module performs a feedforward operation on the input tensor x. It consists of a multi-layer perceptron (MLP) with an optional activation function and LayerNorm. \nUsed in most language, multi-modal, and modern neural networks.\n\n```python\nimport torch\n\nfrom zeta.nn import FeedForward\n\nmodel = FeedForward(256, 512, glu=True, post_act_ln=True, dropout=0.2)\n\nx = torch.randn(1, 256)\n\noutput = model(x)\nprint(output.shape)\n```\n\n### `BitLinear`\n- The BitLinear module performs linear transformation on the input data, followed by quantization and dequantization. The quantization process is performed using the absmax_quantize function, which quantizes the input tensor based on the absolute maximum value, [from the paper](https://arxiv.org/abs/2310.11453)\n```python\nimport torch\nfrom torch import nn\n\nimport zeta.quant as qt\n\n\nclass MyModel(nn.Module):\n    def __init__(self):\n        super().__init__()\n        self.linear = qt.BitLinear(10, 20)\n\n    def forward(self, x):\n        return self.linear(x)\n\n\n# Initialize the model\nmodel = MyModel()\n\n# Create a random tensor of size (128, 10)\ninput = torch.randn(128, 10)\n\n# Perform the forward pass\noutput = model(input)\n\n# Print the size of the output\nprint(output.size())  # torch.Size([128, 20])\n```\n\n### `PalmE`\n- This is an implementation of the multi-modal Palm-E model using a decoder llm as the backbone with an VIT image encoder to process vision, it\'s very similiar to GPT4, Kosmos, RTX2, and many other multi-modality model architectures\n\n```python\nimport torch\n\nfrom zeta.structs import (\n    AutoregressiveWrapper,\n    Decoder,\n    Encoder,\n    Transformer,\n    ViTransformerWrapper,\n)\n\n\nclass PalmE(torch.nn.Module):\n    """\n        PalmE is a transformer architecture that uses a ViT encoder and a transformer decoder.\n\n        Args:\n\n            image_size (int): Size of the image.\n            patch_size (int): Size of the patch.\n            encoder_dim (int): Dimension of the encoder.\n            encoder_depth (int): Depth of the encoder.\n            encoder_heads (int): Number of heads in the encoder.\n            num_tokens (int): Number of tokens.\n            max_seq_len (int): Maximum sequence length.\n            decoder_dim (int): Dimension of the decoder.\n            decoder_depth (int): Depth of the decoder.\n            decoder_heads (int): Number of heads in the decoder.\n            alibi_num_heads (int): Number of heads in the alibi attention.\n            attn_kv_heads (int): Number of heads in the attention key-value projection.\n            use_abs_pos_emb (bool): Whether to use absolute positional embeddings.\n            cross_attend (bool): Whether to cross attend in the decoder.\n            alibi_pos_bias (bool): Whether to use positional bias in the alibi attention.\n            rotary_xpos (bool): Whether to use rotary positional embeddings.\n            attn_flash (bool): Whether to use attention flash.\n            qk_norm (bool): Whether to normalize the query and key in the attention layer.\n\n        Returns:\n\n                torch.Tensor: The output of the model.\n\n        Usage:\n\n    img = torch.randn(1, 3, 256, 256)\n    text = torch.randint(0, 20000, (1, 1024))\n    model = PalmE()\n    output = model(img, text)\n    print(output)\n\n    """\n\n    def __init__(\n        self,\n        image_size=256,\n        patch_size=32,\n        encoder_dim=512,\n        encoder_depth=6,\n        encoder_heads=8,\n        num_tokens=20000,\n        max_seq_len=1024,\n        decoder_dim=512,\n        decoder_depth=6,\n        decoder_heads=8,\n        alibi_num_heads=4,\n        attn_kv_heads=2,\n        use_abs_pos_emb=False,\n        cross_attend=True,\n        alibi_pos_bias=True,\n        rotary_xpos=True,\n        attn_flash=True,\n        qk_norm=True,\n    ):\n        super().__init__()\n\n        # vit architecture\n        self.encoder = ViTransformerWrapper(\n            image_size=image_size,\n            patch_size=patch_size,\n            attn_layers=Encoder(\n                dim=encoder_dim, depth=encoder_depth, heads=encoder_heads\n            ),\n        )\n\n        # palm model architecture\n        self.decoder = Transformer(\n            num_tokens=num_tokens,\n            max_seq_len=max_seq_len,\n            use_abs_pos_emb=use_abs_pos_emb,\n            attn_layers=Decoder(\n                dim=decoder_dim,\n                depth=decoder_depth,\n                heads=decoder_heads,\n                cross_attend=cross_attend,\n                alibi_pos_bias=alibi_pos_bias,\n                alibi_num_heads=alibi_num_heads,\n                rotary_xpos=rotary_xpos,\n                attn_kv_heads=attn_kv_heads,\n                attn_flash=attn_flash,\n                qk_norm=qk_norm,\n            ),\n        )\n\n        # autoregressive wrapper to enable generation of tokens\n        self.decoder = AutoregressiveWrapper(self.decoder)\n\n    def forward(self, img: torch.Tensor, text: torch.Tensor):\n        """Forward pass of the model."""\n        try:\n            encoded = self.encoder(img, return_embeddings=True)\n            return self.decoder(text, context=encoded)\n        except Exception as error:\n            print(f"Failed in forward method: {error}")\n            raise\n\n\n# Usage with random inputs\nimg = torch.randn(1, 3, 256, 256)\ntext = torch.randint(0, 20000, (1, 1024))\n\n# Initiliaze the model\nmodel = PalmE()\noutput = model(img, text)\nprint(output)\n```\n\n\n### `Unet`\nUnet is a famous convolutional neural network architecture originally used for biomedical image segmentation but soon became the backbone of the generative AI Mega-revolution. The architecture comprises two primary pathways: downsampling and upsampling, followed by an output convolution. Due to its U-shape, the architecture is named U-Net. Its symmetric architecture ensures that the context (from downsampling) and the localization (from upsampling) are captured effectively.\n\n```python\nimport torch\n\nfrom zeta.nn import Unet\n\n# Initialize the U-Net model\nmodel = Unet(n_channels=1, n_classes=2)\n\n# Random input tensor with dimensions [batch_size, channels, height, width]\nx = torch.randn(1, 1, 572, 572)\n\n# Forward pass through the model\ny = model(x)\n\n# Output\nprint(f"Input shape: {x.shape}")\nprint(f"Output shape: {y.shape}")\n```\n\n\n### `VisionEmbeddings`\nThe VisionEmbedding class is designed for converting images into patch embeddings, making them suitable for processing by transformer-based models. This class plays a crucial role in various computer vision tasks and enables the integration of vision data into transformer architectures!\n\n```python\nimport torch\n\nfrom zeta.nn import VisionEmbedding\n\n# Create an instance of VisionEmbedding\nvision_embedding = VisionEmbedding(\n    img_size=224,\n    patch_size=16,\n    in_chans=3,\n    embed_dim=768,\n    contain_mask_token=True,\n    prepend_cls_token=True,\n)\n\n# Load an example image (3 channels, 224x224)\ninput_image = torch.rand(1, 3, 224, 224)\n\n# Perform image-to-patch embedding\noutput = vision_embedding(input_image)\n\n# The output now contains patch embeddings, ready for input to a transformer model\n```\n\n\n### `niva`\n- Niva focuses on weights of certain layers (specified by quantize_layers). Ideal for models where runtime activation is variable. 👁️ Example Layers: nn.Embedding, nn.LSTM. \n\n```python\nimport torch\n\nfrom zeta import niva\n\n# Load a pre-trained model\nmodel = YourModelClass()\n\n# Quantize the model dynamically, specifying layers to quantize\nniva(\n    model=model,\n    model_path="path_to_pretrained_model_weights.pt",\n    output_path="quantized_model.pt",\n    quant_type="dynamic",\n    quantize_layers=[nn.Linear, nn.Conv2d],\n    dtype=torch.qint8,\n)\n```\n\n\n### `FusedDenseGELUDense`\n- Increase model speed by 2x with this module that fuses together 2 hyper-optimized dense ops from bits and bytes and a gelu together!\n\n```python\nimport torch\n\nfrom zeta.nn import FusedDenseGELUDense\n\nx = torch.randn(1, 512)\nmodel = FusedDenseGELUDense(512, 1024)\nout = model(x)\nout.shape\n```\n\n\n### `FusedDropoutLayerNorm`\n- FusedDropoutLayerNorm is a fused kernel of dropout and layernorm to speed up FFNs or MLPS by 2X\n\n```python\nimport torch\nfrom torch import nn\n\nfrom zeta.nn import FusedDropoutLayerNorm\n\n# Initialize the module\nmodel = FusedDropoutLayerNorm(dim=512)\n\n# Create a sample input tensor\nx = torch.randn(1, 512)\n\n# Forward pass\noutput = model(x)\n\n# Check output shape\nprint(output.shape)  # Expected: torch.Size([1, 512])\n```\n\n\n### `Mamba`\n- Pytorch implementation of the new SSM model architecture Mamba\n\n```python\nimport torch\n\nfrom zeta.nn import MambaBlock\n\n# Initialize Mamba\nblock = MambaBlock(dim=64, depth=1)\n\n# Random input\nx = torch.randn(1, 10, 64)\n\n# Apply the model to the block\ny = block(x)\n\nprint(y.shape)\n# torch.Size([1, 10, 64])\n```\n\n### `FiLM`\n\n```python\nimport torch\n\nfrom zeta.nn import Film\n\n# Initialize the Film layer\nfilm_layer = Film(dim=128, hidden_dim=64, expanse_ratio=4)\n\n# Create some dummy data for conditions and hiddens\nconditions = torch.randn(10, 128)  # Batch size is 10, feature size is 128\nhiddens = torch.randn(\n    10, 1, 128\n)  # Batch size is 10, sequence length is 1, feature size is 128\n\n# Pass the data through the Film layer\nmodulated_features = film_layer(conditions, hiddens)\n\n# Print the shape of the output\nprint(modulated_features.shape)  # Should be [10, 1, 128]\n```\n\n### `hyper_optimize`\n- A single wrapper for torch.fx, torch.script, torch.compile, dynamic quantization, mixed precision through torch.amp, with execution time metrics all in once place!\n```python\nimport torch\n\nfrom zeta.nn import hyper_optimize\n\n\n@hyper_optimize(\n    torch_fx=False,\n    torch_script=False,\n    torch_compile=True,\n    quantize=True,\n    mixed_precision=True,\n    enable_metrics=True,\n)\ndef model(x):\n    return x @ x\n\n\nout = model(torch.randn(1, 3, 32, 32))\nprint(out)\n```\n\n\n### DPO - Direct Policy Optimization\nDirect Policy Optimization employed for many RLHF applications for LLMs.\n\n```python\nimport torch\nfrom torch import nn\n\nfrom zeta.rl import DPO\n\n\n# Define a simple policy model\nclass PolicyModel(nn.Module):\n    def __init__(self, input_dim, output_dim):\n        super().__init__()\n        self.fc = nn.Linear(input_dim, output_dim)\n\n    def forward(self, x):\n        return self.fc(x)\n\n\ninput_dim = 10\noutput_dim = 5\npolicy_model = PolicyModel(input_dim, output_dim)\n\n# Initialize DPO with the policy model\ndpo_model = DPO(model=policy_model, beta=0.1)\n\n# Sample preferred and unpreferred sequences\npreferred_seq = torch.randint(0, output_dim, (3, input_dim))\nunpreferred_seq = torch.randint(0, output_dim, (3, input_dim))\n\n# Compute loss\nloss = dpo_model(preferred_seq, unpreferred_seq)\nprint(loss)\n```\n\n\n### ZetaCloud\nTrain or finetune any model on any cluster in 1 click with zetacloud, just pass in your file and the GPU type and quantity you want! To gain access first `pip install zetascale` then run `zeta -h` in the terminal. [Here is the docs for more](https://zeta.apac.ai/en/latest/zeta/cloud/main/)\n\n- Flexible Pricing with pooling from many clouds\n- Easy Deployment with 1 click\n- Various options for cloud providers!\n\n```bash\nZetacloud CLI\n\noptions:\n  -h, --help            show this help message and exit\n  -t TASK_NAME, --task_name TASK_NAME\n                        Task name\n  -c CLUSTER_NAME, --cluster_name CLUSTER_NAME\n                        Cluster name\n  -cl CLOUD, --cloud CLOUD\n                        Cloud provider\n  -g GPUS, --gpus GPUS  GPUs\n  -f FILENAME, --filename FILENAME\n                        Filename\n  -s, --stop            Stop flag\n  -d, --down            Down flag\n  -sr, --status_report  Status report flag\n\n```\n\n- A simple run example code would be like:\n\n```bash\nzeta -f train.py -g A100:8\n```\n----\n\n\n# Documentation\nAll classes must have documentation if you see a class or function without documentation then please report it to me at kye@apac.ai,\n\nDocumentation is at [zeta.apac.ai](https://zeta.apac.ai/)\n\n\n-------\n\n\n# Running tests\nYou should install the pre-commit hooks with pre-commit install. This will run the linter, mypy, and a subset of the tests on every commit.\n\nFor more examples on how to run the full test suite please refer to the CI workflow.\n\nSome examples of running tests locally:\n\n```bash\npython3 -m pip install -e \'.[testing]\'  # install extra deps for testing\npython3 -m pytest tests/                 # whole test suite\n```\n----\n\n## Community\n\nJoin our growing community around the world, for real-time support, ideas, and discussions on how to build better models 😊 \n\n- View our official [Docs](https://zeta.apac.ai)\n- Chat live with us on [Discord](https://discord.gg/kS3rwKs3ZC)\n- Follow us on [Twitter](https://twitter.com/kyegomez)\n- Connect with us on [LinkedIn](https://www.linkedin.com/company/the-swarm-corporation)\n- Visit us on [YouTube](https://www.youtube.com/channel/UC9yXyitkbU_WSy7bd_41SqQ)\n- [Join the Swarms community on Discord!](https://discord.gg/AJazBmhKnr)\n\n---\n\n# 🤝 Schedule a 1-on-1 Session\nWant to train a custom AI model for a real-world task like General Multi-Modal Models, Facial Recognitions, Drug Discovery, Humanoid Robotics? I\'ll help you create the model architecture then train the model and then optimize it to meet your quality assurance standards.\n\nBook a [1-on-1 Session with Kye here.](https://calendly.com/apacai/agora), the Creator, to discuss any issues, provide feedback, or explore how we can improve Zeta for you or help you build your own custom models!\n\n## 🫶 Contributions:\n\nThe easiest way to contribute is to pick any issue with the `good first issue` tag 💪. Read the Contributing guidelines [here](/CONTRIBUTING.md). Bug Report? [File here](https://github.com/kyegomez/zeta/issues/new/choose) | Feature Request? [File here](https://github.com/kyegomez/zeta/issues/new/choose)\n\nZeta is an open-source project, and contributions are VERY welcome. If you want to contribute, you can create new features, fix bugs, or improve the infrastructure. Please refer to the [CONTRIBUTING.md](https://github.com/kyegomez/zeta/blob/master/CONTRIBUTING.md) and our [contributing board](https://github.com/users/kyegomez/projects/1) to participate in Roadmap discussions!\n\n<a href="https://github.com/kyegomez/zeta/graphs/contributors">\n  <img src="https://contrib.rocks/image?repo=kyegomez/zeta" />\n</a>\n\n----\n\n## Accelerate Backlog\nHelp us accelerate our backlog by supporting us financially! Note, we\'re an open source corporation and so all the revenue we generate is through donations at the moment ;)\n\n<a href="https://polar.sh/kyegomez"><img src="https://polar.sh/embed/fund-our-backlog.svg?org=kyegomez" /></a>\n\n\n# License \n- Apache\n',
     'author': 'Zeta Team',
     'author_email': 'kye@apac.ai',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/kyegomez/zeta',
```

#### html2text {}

```diff
@@ -8,15 +8,15 @@
 attention', 'datasets', 'einops-exts==0.0.4', 'einops==0.7.0', 'lion-
 pytorch==0.1.2', 'loguru', 'numexpr', 'pytest==8.0.2', 'rich==13.7.0',
 'scipy==1.9.3', 'sentencepiece==0.2.0', 'skypilot==0.4.1', 'tiktoken==0.6.0',
 'timm==0.9.16', 'tokenmonster==1.1.12', 'torch==2.2.0', 'torchdiffeq==0.2.3',
 'torchfix', 'torchvision==0.17.0', 'tqdm==4.66.2', 'transformers==4.38.2',
 'typing==3.7.4.3', 'vector-quantize-pytorch==1.14.1'] entry_points = \
 {'console_scripts': ['zeta = zeta.cli.main:main']} setup_kwargs = { 'name':
-'zetascale', 'version': '2.2.6', 'description': 'Transformers at zeta scales',
+'zetascale', 'version': '2.2.7', 'description': 'Transformers at zeta scales',
 'long_description': '[![Multi-Modality](images/agorabanner.png)](https://
 discord.gg/qUtxnK2NMf)\n\n![Zeta banner](images/zeta.png)\nBuild SOTA AI Models
 80% faster with modular, high-performance, and scalable building blocks!\n\n[!
 [Docs](https://readthedocs.org/projects/zeta/badge/)](https://
 zeta.readthedocs.io)\n\n
 \n _[_M_I_T_ _L_i_c_e_n_s_e_]\n _[_M_I_T_ _L_i_c_e_n_s_e_]\n
 \n\n[![GitHub issues](https://img.shields.io/github/issues/kyegomez/zeta)]
```

### Comparing `zetascale-2.2.6/PKG-INFO` & `zetascale-2.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zetascale
-Version: 2.2.6
+Version: 2.2.7
 Summary: Transformers at zeta scales
 Home-page: https://github.com/kyegomez/zeta
 License: MIT
 Keywords: Transformers,zeta scale
 Author: Zeta Team
 Author-email: kye@apac.ai
 Requires-Python: >=3.8,<4.0
```

