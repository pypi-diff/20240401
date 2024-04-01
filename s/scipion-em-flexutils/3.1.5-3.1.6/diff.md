# Comparing `tmp/scipion-em-flexutils-3.1.5.tar.gz` & `tmp/scipion-em-flexutils-3.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scipion-em-flexutils-3.1.5.tar", last modified: Tue Mar 19 11:31:42 2024, max compression
+gzip compressed data, was "scipion-em-flexutils-3.1.6.tar", last modified: Mon Apr  1 10:23:12 2024, max compression
```

## Comparing `scipion-em-flexutils-3.1.5.tar` & `scipion-em-flexutils-3.1.6.tar`

### file list

```diff
@@ -1,118 +1,118 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 11:31:42.069918 scipion-em-flexutils-3.1.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-03-19 11:31:06.000000 scipion-em-flexutils-3.1.5/CHANGES.txt
--rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-03-19 11:31:06.000000 scipion-em-flexutils-3.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-19 11:31:06.000000 scipion-em-flexutils-3.1.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3384 2024-03-19 11:31:42.069918 scipion-em-flexutils-3.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-03-19 11:31:06.000000 scipion-em-flexutils-3.1.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 11:31:42.053918 scipion-em-flexutils-3.1.5/flexutils/
--rw-r--r--   0 runner    (1001) docker     (127)     7572 2024-03-19 11:31:06.000000 scipion-em-flexutils-3.1.5/flexutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-03-19 11:31:06.000000 scipion-em-flexutils-3.1.5/flexutils/bibtex.py
--rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-03-19 11:31:06.000000 scipion-em-flexutils-3.1.5/flexutils/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)   115652 2024-03-19 11:31:06.000000 scipion-em-flexutils-3.1.5/flexutils/icon.png
--rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-03-19 11:31:06.000000 scipion-em-flexutils-3.1.5/flexutils/icon_square.png
--rw-r--r--   0 runner    (1001) docker     (127)     9559 2024-03-19 11:31:06.000000 scipion-em-flexutils-3.1.5/flexutils/loading.gif
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 11:31:42.053918 scipion-em-flexutils-3.1.5/flexutils/protocols/
--rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-03-19 11:31:06.000000 scipion-em-flexutils-3.1.5/flexutils/protocols/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 11:31:42.057918 scipion-em-flexutils-3.1.5/flexutils/protocols/deprecated/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 11:31:06.000000 scipion-em-flexutils-3.1.5/flexutils/protocols/deprecated/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 11:31:42.057918 scipion-em-flexutils-3.1.5/flexutils/protocols/deprecated/annotation_2d_tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 11:31:06.000000 scipion-em-flexutils-3.1.5/flexutils/protocols/deprecated/annotation_2d_tools/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    26446 2024-03-19 11:31:06.000000 scipion-em-flexutils-3.1.5/flexutils/protocols/deprecated/annotation_2d_tools/viewer_interactive_2d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 11:31:42.057918 scipion-em-flexutils-3.1.5/flexutils/protocols/deprecated/annotation_3d_tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 11:31:06.000000 scipion-em-flexutils-3.1.5/flexutils/protocols/deprecated/annotation_3d_tools/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    23739 2024-03-19 11:31:06.000000 scipion-em-flexutils-3.1.5/flexutils/protocols/deprecated/annotation_3d_tools/viewer_3d_pc.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    30759 2024-03-19 11:31:06.000000 scipion-em-flexutils-3.1.5/flexutils/protocols/deprecated/annotation_3d_tools/viewer_3d_slicer.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    40075 2024-03-19 11:31:06.000000 scipion-em-flexutils-3.1.5/flexutils/protocols/deprecated/annotation_3d_tools/viewer_interactive_2d_3d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 11:31:42.057918 scipion-em-flexutils-3.1.5/flexutils/protocols/deprecated/chimera_viewers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 11:31:06.000000 scipion-em-flexutils-3.1.5/flexutils/protocols/deprecated/chimera_viewers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5983 2024-03-19 11:31:06.000000 scipion-em-flexutils-3.1.5/flexutils/protocols/deprecated/chimera_viewers/viewer_morph_salesman_old.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 11:31:42.057918 scipion-em-flexutils-3.1.5/flexutils/protocols/deprecated/point_cloud_viewers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 11:31:06.000000 scipion-em-flexutils-3.1.5/flexutils/protocols/deprecated/point_cloud_viewers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-03-19 11:31:06.000000 scipion-em-flexutils-3.1.5/flexutils/protocols/deprecated/point_cloud_viewers/viewer_point_cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)    23716 2024-03-19 11:31:06.000000 scipion-em-flexutils-3.1.5/flexutils/protocols/deprecated/protocol_angular_align_deep_nma.py
--rw-r--r--   0 runner    (1001) docker     (127)    17276 2024-03-19 11:31:06.000000 scipion-em-flexutils-3.1.5/flexutils/protocols/deprecated/protocol_cluster_space.py
--rw-r--r--   0 runner    (1001) docker     (127)    12039 2024-03-19 11:31:06.000000 scipion-em-flexutils-3.1.5/flexutils/protocols/deprecated/protocol_predict_deep_nma.py
--rw-r--r--   0 runner    (1001) docker     (127)    19846 2024-03-19 11:31:06.000000 scipion-em-flexutils-3.1.5/flexutils/protocols/protocol_annotate_space.py
--rw-r--r--   0 runner    (1001) docker     (127)     3907 2024-03-19 11:31:06.000000 scipion-em-flexutils-3.1.5/flexutils/protocols/protocol_associate_flex_space_to_particles.py
--rw-r--r--   0 runner    (1001) docker     (127)     7517 2024-03-19 11:31:06.000000 scipion-em-flexutils-3.1.5/flexutils/protocols/protocol_auto_reference.py
--rw-r--r--   0 runner    (1001) docker     (127)    11418 2024-03-19 11:31:06.000000 scipion-em-flexutils-3.1.5/flexutils/protocols/protocol_dimred.py
--rw-r--r--   0 runner    (1001) docker     (127)     7796 2024-03-19 11:31:06.000000 scipion-em-flexutils-3.1.5/flexutils/protocols/protocol_filter_pca.py
--rw-r--r--   0 runner    (1001) docker     (127)     4709 2024-03-19 11:31:06.000000 scipion-em-flexutils-3.1.5/flexutils/protocols/protocol_find_optimal_clusters.py
--rw-r--r--   0 runner    (1001) docker     (127)     8260 2024-03-19 11:31:06.000000 scipion-em-flexutils-3.1.5/flexutils/protocols/protocol_order_volumes.py
--rw-r--r--   0 runner    (1001) docker     (127)     6320 2024-03-19 11:31:06.000000 scipion-em-flexutils-3.1.5/flexutils/protocols/protocol_score_landscape.py
--rw-r--r--   0 runner    (1001) docker     (127)    11216 2024-03-19 11:31:06.000000 scipion-em-flexutils-3.1.5/flexutils/protocols/protocol_select_views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 11:31:42.061918 scipion-em-flexutils-3.1.5/flexutils/protocols/xmipp/
--rw-r--r--   0 runner    (1001) docker     (127)     3820 2024-03-19 11:31:06.000000 scipion-em-flexutils-3.1.5/flexutils/protocols/xmipp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26355 2024-03-19 11:31:06.000000 scipion-em-flexutils-3.1.5/flexutils/protocols/xmipp/protocol_angular_align_deep_pose.py
--rw-r--r--   0 runner    (1001) docker     (127)    34052 2024-03-19 11:31:06.000000 scipion-em-flexutils-3.1.5/flexutils/protocols/xmipp/protocol_angular_align_het_siren.py
--rw-r--r--   0 runner    (1001) docker     (127)    27232 2024-03-19 11:31:06.000000 scipion-em-flexutils-3.1.5/flexutils/protocols/xmipp/protocol_angular_align_homo_siren.py
--rw-r--r--   0 runner    (1001) docker     (127)    34010 2024-03-19 11:31:06.000000 scipion-em-flexutils-3.1.5/flexutils/protocols/xmipp/protocol_angular_align_zernike3deep.py
--rw-r--r--   0 runner    (1001) docker     (127)    16225 2024-03-19 11:31:06.000000 scipion-em-flexutils-3.1.5/flexutils/protocols/xmipp/protocol_angular_alignment_zernike3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     8343 2024-03-19 11:31:06.000000 scipion-em-flexutils-3.1.5/flexutils/protocols/xmipp/protocol_apply_field_nma.py
--rw-r--r--   0 runner    (1001) docker     (127)    13801 2024-03-19 11:31:06.000000 scipion-em-flexutils-3.1.5/flexutils/protocols/xmipp/protocol_apply_field_zernike3d.py
--rw-r--r--   0 runner    (1001) docker     (127)    14913 2024-03-19 11:31:06.000000 scipion-em-flexutils-3.1.5/flexutils/protocols/xmipp/protocol_assign_heterogeneity_priors_zernike3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     7424 2024-03-19 11:31:06.000000 scipion-em-flexutils-3.1.5/flexutils/protocols/xmipp/protocol_cluster_structures_zernike3d.py
--rw-r--r--   0 runner    (1001) docker     (127)    10229 2024-03-19 11:31:06.000000 scipion-em-flexutils-3.1.5/flexutils/protocols/xmipp/protocol_compute_priors_zernike3d.py
--rw-r--r--   0 runner    (1001) docker     (127)    11407 2024-03-19 11:31:06.000000 scipion-em-flexutils-3.1.5/flexutils/protocols/xmipp/protocol_deform_map_zernike3d.py
--rw-r--r--   0 runner    (1001) docker     (127)    14718 2024-03-19 11:31:06.000000 scipion-em-flexutils-3.1.5/flexutils/protocols/xmipp/protocol_denoise_particles_het_siren.py
--rw-r--r--   0 runner    (1001) docker     (127)     7691 2024-03-19 11:31:06.000000 scipion-em-flexutils-3.1.5/flexutils/protocols/xmipp/protocol_focus_zernike3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     7140 2024-03-19 11:31:06.000000 scipion-em-flexutils-3.1.5/flexutils/protocols/xmipp/protocol_interactive_flex_consensus.py
--rw-r--r--   0 runner    (1001) docker     (127)     5518 2024-03-19 11:31:06.000000 scipion-em-flexutils-3.1.5/flexutils/protocols/xmipp/protocol_match_and_deform_map_zernike3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     8354 2024-03-19 11:31:06.000000 scipion-em-flexutils-3.1.5/flexutils/protocols/xmipp/protocol_match_and_deform_structure_zernike3d.py
--rw-r--r--   0 runner    (1001) docker     (127)    12552 2024-03-19 11:31:06.000000 scipion-em-flexutils-3.1.5/flexutils/protocols/xmipp/protocol_predict_deep_pose.py
--rw-r--r--   0 runner    (1001) docker     (127)    16765 2024-03-19 11:31:06.000000 scipion-em-flexutils-3.1.5/flexutils/protocols/xmipp/protocol_predict_het_siren.py
--rw-r--r--   0 runner    (1001) docker     (127)    13241 2024-03-19 11:31:06.000000 scipion-em-flexutils-3.1.5/flexutils/protocols/xmipp/protocol_predict_homo_siren.py
--rw-r--r--   0 runner    (1001) docker     (127)    16635 2024-03-19 11:31:06.000000 scipion-em-flexutils-3.1.5/flexutils/protocols/xmipp/protocol_predict_zernike3deep.py
--rw-r--r--   0 runner    (1001) docker     (127)    16807 2024-03-19 11:31:06.000000 scipion-em-flexutils-3.1.5/flexutils/protocols/xmipp/protocol_prepare_volumes_zernike3deep.py
--rw-r--r--   0 runner    (1001) docker     (127)     8272 2024-03-19 11:31:06.000000 scipion-em-flexutils-3.1.5/flexutils/protocols/xmipp/protocol_reassign_reference_zernike3d.py
--rw-r--r--   0 runner    (1001) docker     (127)    20570 2024-03-19 11:31:06.000000 scipion-em-flexutils-3.1.5/flexutils/protocols/xmipp/protocol_reconstruct_zart.py
--rw-r--r--   0 runner    (1001) docker     (127)    15928 2024-03-19 11:31:06.000000 scipion-em-flexutils-3.1.5/flexutils/protocols/xmipp/protocol_resize_zernike_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     5430 2024-03-19 11:31:06.000000 scipion-em-flexutils-3.1.5/flexutils/protocols/xmipp/protocol_statistics_zernike3d.py
--rw-r--r--   0 runner    (1001) docker     (127)    14571 2024-03-19 11:31:06.000000 scipion-em-flexutils-3.1.5/flexutils/protocols/xmipp/protocol_structure_landscape.py
--rw-r--r--   0 runner    (1001) docker     (127)     8207 2024-03-19 11:31:06.000000 scipion-em-flexutils-3.1.5/flexutils/protocols/xmipp/protocol_train_flex_consensus.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 11:31:42.061918 scipion-em-flexutils-3.1.5/flexutils/protocols/xmipp/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-03-19 11:31:06.000000 scipion-em-flexutils-3.1.5/flexutils/protocols/xmipp/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6524 2024-03-19 11:31:06.000000 scipion-em-flexutils-3.1.5/flexutils/protocols/xmipp/utils/custom_pdb_parser.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    53807 2024-03-19 11:31:06.000000 scipion-em-flexutils-3.1.5/flexutils/protocols/xmipp/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5554 2024-03-19 11:31:06.000000 scipion-em-flexutils-3.1.5/flexutils/protocols.conf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 11:31:42.065918 scipion-em-flexutils-3.1.5/flexutils/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-03-19 11:31:06.000000 scipion-em-flexutils-3.1.5/flexutils/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4802 2024-03-19 11:31:06.000000 scipion-em-flexutils-3.1.5/flexutils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 11:31:42.065918 scipion-em-flexutils-3.1.5/flexutils/viewers/
--rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-03-19 11:31:06.000000 scipion-em-flexutils-3.1.5/flexutils/viewers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 11:31:42.065918 scipion-em-flexutils-3.1.5/flexutils/viewers/clustering_viewers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 11:31:06.000000 scipion-em-flexutils-3.1.5/flexutils/viewers/clustering_viewers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4071 2024-03-19 11:31:06.000000 scipion-em-flexutils-3.1.5/flexutils/viewers/clustering_viewers/viewer_optimal_clusters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 11:31:42.065918 scipion-em-flexutils-3.1.5/flexutils/viewers/consensus_viewers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 11:31:06.000000 scipion-em-flexutils-3.1.5/flexutils/viewers/consensus_viewers/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3262 2024-03-19 11:31:06.000000 scipion-em-flexutils-3.1.5/flexutils/viewers/consensus_viewers/viewer_interactive_hist.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 11:31:42.065918 scipion-em-flexutils-3.1.5/flexutils/viewers/imagej_viewers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 11:31:06.000000 scipion-em-flexutils-3.1.5/flexutils/viewers/imagej_viewers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7039 2024-03-19 11:31:06.000000 scipion-em-flexutils-3.1.5/flexutils/viewers/imagej_viewers/viewer_ij.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 11:31:42.065918 scipion-em-flexutils-3.1.5/flexutils/viewers/map_model_viewers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 11:31:06.000000 scipion-em-flexutils-3.1.5/flexutils/viewers/map_model_viewers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-03-19 11:31:06.000000 scipion-em-flexutils-3.1.5/flexutils/viewers/map_model_viewers/viewer_show_maps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 11:31:42.065918 scipion-em-flexutils-3.1.5/flexutils/viewers/tensorboard/
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-03-19 11:31:06.000000 scipion-em-flexutils-3.1.5/flexutils/viewers/tensorboard/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5041 2024-03-19 11:31:06.000000 scipion-em-flexutils-3.1.5/flexutils/viewers/tensorboard/setup_tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-03-19 11:31:06.000000 scipion-em-flexutils-3.1.5/flexutils/viewers/tensorboard/viewer_tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     2695 2024-03-19 11:31:06.000000 scipion-em-flexutils-3.1.5/flexutils/viewers/viewer_show_structures.py
--rw-r--r--   0 runner    (1001) docker     (127)     2763 2024-03-19 11:31:06.000000 scipion-em-flexutils-3.1.5/flexutils/viewers/viewers_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 11:31:42.065918 scipion-em-flexutils-3.1.5/flexutils/viewers/xmipp/
--rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-03-19 11:31:06.000000 scipion-em-flexutils-3.1.5/flexutils/viewers/xmipp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6272 2024-03-19 11:31:06.000000 scipion-em-flexutils-3.1.5/flexutils/viewers/xmipp/viewer_apply_field_nma.py
--rw-r--r--   0 runner    (1001) docker     (127)    12441 2024-03-19 11:31:06.000000 scipion-em-flexutils-3.1.5/flexutils/viewers/xmipp/viewer_apply_field_zernike3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3341 2024-03-19 11:31:06.000000 scipion-em-flexutils-3.1.5/flexutils/viewers/xmipp/viewer_flex_consensus.py
--rw-r--r--   0 runner    (1001) docker     (127)     8139 2024-03-19 11:31:06.000000 scipion-em-flexutils-3.1.5/flexutils/viewers/xmipp/viewer_landscape.py
--rw-r--r--   0 runner    (1001) docker     (127)     4026 2024-03-19 11:31:06.000000 scipion-em-flexutils-3.1.5/flexutils/viewers/xmipp/viewer_reduced_space.py
--rw-r--r--   0 runner    (1001) docker     (127)    14036 2024-03-19 11:31:06.000000 scipion-em-flexutils-3.1.5/flexutils/viewers/xmipp/viewer_structure_map_zernike3d.py
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-03-19 11:31:06.000000 scipion-em-flexutils-3.1.5/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 11:31:42.069918 scipion-em-flexutils-3.1.5/scipion_em_flexutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3384 2024-03-19 11:31:42.000000 scipion-em-flexutils-3.1.5/scipion_em_flexutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4787 2024-03-19 11:31:42.000000 scipion-em-flexutils-3.1.5/scipion_em_flexutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-19 11:31:42.000000 scipion-em-flexutils-3.1.5/scipion_em_flexutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-19 11:31:42.000000 scipion-em-flexutils-3.1.5/scipion_em_flexutils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-03-19 11:31:42.000000 scipion-em-flexutils-3.1.5/scipion_em_flexutils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-19 11:31:42.000000 scipion-em-flexutils-3.1.5/scipion_em_flexutils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-19 11:31:42.069918 scipion-em-flexutils-3.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-03-19 11:31:06.000000 scipion-em-flexutils-3.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 10:23:12.659666 scipion-em-flexutils-3.1.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-04-01 10:22:39.000000 scipion-em-flexutils-3.1.6/CHANGES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-04-01 10:22:39.000000 scipion-em-flexutils-3.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-01 10:22:39.000000 scipion-em-flexutils-3.1.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3384 2024-04-01 10:23:12.659666 scipion-em-flexutils-3.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-04-01 10:22:39.000000 scipion-em-flexutils-3.1.6/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 10:23:12.647666 scipion-em-flexutils-3.1.6/flexutils/
+-rw-r--r--   0 runner    (1001) docker     (127)     7615 2024-04-01 10:22:39.000000 scipion-em-flexutils-3.1.6/flexutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-04-01 10:22:39.000000 scipion-em-flexutils-3.1.6/flexutils/bibtex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-04-01 10:22:39.000000 scipion-em-flexutils-3.1.6/flexutils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)   115652 2024-04-01 10:22:39.000000 scipion-em-flexutils-3.1.6/flexutils/icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-04-01 10:22:39.000000 scipion-em-flexutils-3.1.6/flexutils/icon_square.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9559 2024-04-01 10:22:39.000000 scipion-em-flexutils-3.1.6/flexutils/loading.gif
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 10:23:12.647666 scipion-em-flexutils-3.1.6/flexutils/protocols/
+-rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-04-01 10:22:39.000000 scipion-em-flexutils-3.1.6/flexutils/protocols/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 10:23:12.647666 scipion-em-flexutils-3.1.6/flexutils/protocols/deprecated/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 10:22:39.000000 scipion-em-flexutils-3.1.6/flexutils/protocols/deprecated/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 10:23:12.647666 scipion-em-flexutils-3.1.6/flexutils/protocols/deprecated/annotation_2d_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 10:22:39.000000 scipion-em-flexutils-3.1.6/flexutils/protocols/deprecated/annotation_2d_tools/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    26446 2024-04-01 10:22:39.000000 scipion-em-flexutils-3.1.6/flexutils/protocols/deprecated/annotation_2d_tools/viewer_interactive_2d.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 10:23:12.647666 scipion-em-flexutils-3.1.6/flexutils/protocols/deprecated/annotation_3d_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 10:22:39.000000 scipion-em-flexutils-3.1.6/flexutils/protocols/deprecated/annotation_3d_tools/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    23739 2024-04-01 10:22:39.000000 scipion-em-flexutils-3.1.6/flexutils/protocols/deprecated/annotation_3d_tools/viewer_3d_pc.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    30759 2024-04-01 10:22:39.000000 scipion-em-flexutils-3.1.6/flexutils/protocols/deprecated/annotation_3d_tools/viewer_3d_slicer.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    40075 2024-04-01 10:22:39.000000 scipion-em-flexutils-3.1.6/flexutils/protocols/deprecated/annotation_3d_tools/viewer_interactive_2d_3d.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 10:23:12.647666 scipion-em-flexutils-3.1.6/flexutils/protocols/deprecated/chimera_viewers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 10:22:39.000000 scipion-em-flexutils-3.1.6/flexutils/protocols/deprecated/chimera_viewers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5983 2024-04-01 10:22:39.000000 scipion-em-flexutils-3.1.6/flexutils/protocols/deprecated/chimera_viewers/viewer_morph_salesman_old.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 10:23:12.651666 scipion-em-flexutils-3.1.6/flexutils/protocols/deprecated/point_cloud_viewers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 10:22:39.000000 scipion-em-flexutils-3.1.6/flexutils/protocols/deprecated/point_cloud_viewers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-04-01 10:22:39.000000 scipion-em-flexutils-3.1.6/flexutils/protocols/deprecated/point_cloud_viewers/viewer_point_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23716 2024-04-01 10:22:39.000000 scipion-em-flexutils-3.1.6/flexutils/protocols/deprecated/protocol_angular_align_deep_nma.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17276 2024-04-01 10:22:39.000000 scipion-em-flexutils-3.1.6/flexutils/protocols/deprecated/protocol_cluster_space.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12039 2024-04-01 10:22:39.000000 scipion-em-flexutils-3.1.6/flexutils/protocols/deprecated/protocol_predict_deep_nma.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19846 2024-04-01 10:22:39.000000 scipion-em-flexutils-3.1.6/flexutils/protocols/protocol_annotate_space.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3907 2024-04-01 10:22:39.000000 scipion-em-flexutils-3.1.6/flexutils/protocols/protocol_associate_flex_space_to_particles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7517 2024-04-01 10:22:39.000000 scipion-em-flexutils-3.1.6/flexutils/protocols/protocol_auto_reference.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11418 2024-04-01 10:22:39.000000 scipion-em-flexutils-3.1.6/flexutils/protocols/protocol_dimred.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7796 2024-04-01 10:22:39.000000 scipion-em-flexutils-3.1.6/flexutils/protocols/protocol_filter_pca.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4709 2024-04-01 10:22:39.000000 scipion-em-flexutils-3.1.6/flexutils/protocols/protocol_find_optimal_clusters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8260 2024-04-01 10:22:39.000000 scipion-em-flexutils-3.1.6/flexutils/protocols/protocol_order_volumes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6320 2024-04-01 10:22:39.000000 scipion-em-flexutils-3.1.6/flexutils/protocols/protocol_score_landscape.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11216 2024-04-01 10:22:39.000000 scipion-em-flexutils-3.1.6/flexutils/protocols/protocol_select_views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 10:23:12.655666 scipion-em-flexutils-3.1.6/flexutils/protocols/xmipp/
+-rw-r--r--   0 runner    (1001) docker     (127)     3820 2024-04-01 10:22:39.000000 scipion-em-flexutils-3.1.6/flexutils/protocols/xmipp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26355 2024-04-01 10:22:39.000000 scipion-em-flexutils-3.1.6/flexutils/protocols/xmipp/protocol_angular_align_deep_pose.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34038 2024-04-01 10:22:39.000000 scipion-em-flexutils-3.1.6/flexutils/protocols/xmipp/protocol_angular_align_het_siren.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27232 2024-04-01 10:22:39.000000 scipion-em-flexutils-3.1.6/flexutils/protocols/xmipp/protocol_angular_align_homo_siren.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34010 2024-04-01 10:22:39.000000 scipion-em-flexutils-3.1.6/flexutils/protocols/xmipp/protocol_angular_align_zernike3deep.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16225 2024-04-01 10:22:39.000000 scipion-em-flexutils-3.1.6/flexutils/protocols/xmipp/protocol_angular_alignment_zernike3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8343 2024-04-01 10:22:39.000000 scipion-em-flexutils-3.1.6/flexutils/protocols/xmipp/protocol_apply_field_nma.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13801 2024-04-01 10:22:39.000000 scipion-em-flexutils-3.1.6/flexutils/protocols/xmipp/protocol_apply_field_zernike3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14913 2024-04-01 10:22:39.000000 scipion-em-flexutils-3.1.6/flexutils/protocols/xmipp/protocol_assign_heterogeneity_priors_zernike3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7424 2024-04-01 10:22:39.000000 scipion-em-flexutils-3.1.6/flexutils/protocols/xmipp/protocol_cluster_structures_zernike3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10229 2024-04-01 10:22:39.000000 scipion-em-flexutils-3.1.6/flexutils/protocols/xmipp/protocol_compute_priors_zernike3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11407 2024-04-01 10:22:39.000000 scipion-em-flexutils-3.1.6/flexutils/protocols/xmipp/protocol_deform_map_zernike3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14718 2024-04-01 10:22:39.000000 scipion-em-flexutils-3.1.6/flexutils/protocols/xmipp/protocol_denoise_particles_het_siren.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7691 2024-04-01 10:22:39.000000 scipion-em-flexutils-3.1.6/flexutils/protocols/xmipp/protocol_focus_zernike3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7140 2024-04-01 10:22:39.000000 scipion-em-flexutils-3.1.6/flexutils/protocols/xmipp/protocol_interactive_flex_consensus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5518 2024-04-01 10:22:39.000000 scipion-em-flexutils-3.1.6/flexutils/protocols/xmipp/protocol_match_and_deform_map_zernike3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8354 2024-04-01 10:22:39.000000 scipion-em-flexutils-3.1.6/flexutils/protocols/xmipp/protocol_match_and_deform_structure_zernike3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12552 2024-04-01 10:22:39.000000 scipion-em-flexutils-3.1.6/flexutils/protocols/xmipp/protocol_predict_deep_pose.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16765 2024-04-01 10:22:39.000000 scipion-em-flexutils-3.1.6/flexutils/protocols/xmipp/protocol_predict_het_siren.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13241 2024-04-01 10:22:39.000000 scipion-em-flexutils-3.1.6/flexutils/protocols/xmipp/protocol_predict_homo_siren.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16635 2024-04-01 10:22:39.000000 scipion-em-flexutils-3.1.6/flexutils/protocols/xmipp/protocol_predict_zernike3deep.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16807 2024-04-01 10:22:39.000000 scipion-em-flexutils-3.1.6/flexutils/protocols/xmipp/protocol_prepare_volumes_zernike3deep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8272 2024-04-01 10:22:39.000000 scipion-em-flexutils-3.1.6/flexutils/protocols/xmipp/protocol_reassign_reference_zernike3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20570 2024-04-01 10:22:39.000000 scipion-em-flexutils-3.1.6/flexutils/protocols/xmipp/protocol_reconstruct_zart.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15928 2024-04-01 10:22:39.000000 scipion-em-flexutils-3.1.6/flexutils/protocols/xmipp/protocol_resize_zernike_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5430 2024-04-01 10:22:39.000000 scipion-em-flexutils-3.1.6/flexutils/protocols/xmipp/protocol_statistics_zernike3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14571 2024-04-01 10:22:39.000000 scipion-em-flexutils-3.1.6/flexutils/protocols/xmipp/protocol_structure_landscape.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8207 2024-04-01 10:22:39.000000 scipion-em-flexutils-3.1.6/flexutils/protocols/xmipp/protocol_train_flex_consensus.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 10:23:12.655666 scipion-em-flexutils-3.1.6/flexutils/protocols/xmipp/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-01 10:22:39.000000 scipion-em-flexutils-3.1.6/flexutils/protocols/xmipp/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6524 2024-04-01 10:22:39.000000 scipion-em-flexutils-3.1.6/flexutils/protocols/xmipp/utils/custom_pdb_parser.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    53807 2024-04-01 10:22:39.000000 scipion-em-flexutils-3.1.6/flexutils/protocols/xmipp/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5554 2024-04-01 10:22:39.000000 scipion-em-flexutils-3.1.6/flexutils/protocols.conf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 10:23:12.655666 scipion-em-flexutils-3.1.6/flexutils/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-04-01 10:22:39.000000 scipion-em-flexutils-3.1.6/flexutils/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4802 2024-04-01 10:22:39.000000 scipion-em-flexutils-3.1.6/flexutils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 10:23:12.655666 scipion-em-flexutils-3.1.6/flexutils/viewers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-04-01 10:22:39.000000 scipion-em-flexutils-3.1.6/flexutils/viewers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 10:23:12.655666 scipion-em-flexutils-3.1.6/flexutils/viewers/clustering_viewers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 10:22:39.000000 scipion-em-flexutils-3.1.6/flexutils/viewers/clustering_viewers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4071 2024-04-01 10:22:39.000000 scipion-em-flexutils-3.1.6/flexutils/viewers/clustering_viewers/viewer_optimal_clusters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 10:23:12.655666 scipion-em-flexutils-3.1.6/flexutils/viewers/consensus_viewers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 10:22:39.000000 scipion-em-flexutils-3.1.6/flexutils/viewers/consensus_viewers/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3262 2024-04-01 10:22:39.000000 scipion-em-flexutils-3.1.6/flexutils/viewers/consensus_viewers/viewer_interactive_hist.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 10:23:12.655666 scipion-em-flexutils-3.1.6/flexutils/viewers/imagej_viewers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 10:22:39.000000 scipion-em-flexutils-3.1.6/flexutils/viewers/imagej_viewers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7039 2024-04-01 10:22:39.000000 scipion-em-flexutils-3.1.6/flexutils/viewers/imagej_viewers/viewer_ij.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 10:23:12.655666 scipion-em-flexutils-3.1.6/flexutils/viewers/map_model_viewers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 10:22:39.000000 scipion-em-flexutils-3.1.6/flexutils/viewers/map_model_viewers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-04-01 10:22:39.000000 scipion-em-flexutils-3.1.6/flexutils/viewers/map_model_viewers/viewer_show_maps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 10:23:12.659666 scipion-em-flexutils-3.1.6/flexutils/viewers/tensorboard/
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-01 10:22:39.000000 scipion-em-flexutils-3.1.6/flexutils/viewers/tensorboard/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5041 2024-04-01 10:22:39.000000 scipion-em-flexutils-3.1.6/flexutils/viewers/tensorboard/setup_tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-04-01 10:22:39.000000 scipion-em-flexutils-3.1.6/flexutils/viewers/tensorboard/viewer_tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2695 2024-04-01 10:22:39.000000 scipion-em-flexutils-3.1.6/flexutils/viewers/viewer_show_structures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2763 2024-04-01 10:22:39.000000 scipion-em-flexutils-3.1.6/flexutils/viewers/viewers_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 10:23:12.659666 scipion-em-flexutils-3.1.6/flexutils/viewers/xmipp/
+-rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-04-01 10:22:39.000000 scipion-em-flexutils-3.1.6/flexutils/viewers/xmipp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6272 2024-04-01 10:22:39.000000 scipion-em-flexutils-3.1.6/flexutils/viewers/xmipp/viewer_apply_field_nma.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12441 2024-04-01 10:22:39.000000 scipion-em-flexutils-3.1.6/flexutils/viewers/xmipp/viewer_apply_field_zernike3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3341 2024-04-01 10:22:39.000000 scipion-em-flexutils-3.1.6/flexutils/viewers/xmipp/viewer_flex_consensus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8139 2024-04-01 10:22:39.000000 scipion-em-flexutils-3.1.6/flexutils/viewers/xmipp/viewer_landscape.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4258 2024-04-01 10:22:39.000000 scipion-em-flexutils-3.1.6/flexutils/viewers/xmipp/viewer_reduced_space.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14036 2024-04-01 10:22:39.000000 scipion-em-flexutils-3.1.6/flexutils/viewers/xmipp/viewer_structure_map_zernike3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-01 10:22:39.000000 scipion-em-flexutils-3.1.6/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 10:23:12.659666 scipion-em-flexutils-3.1.6/scipion_em_flexutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3384 2024-04-01 10:23:12.000000 scipion-em-flexutils-3.1.6/scipion_em_flexutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4787 2024-04-01 10:23:12.000000 scipion-em-flexutils-3.1.6/scipion_em_flexutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 10:23:12.000000 scipion-em-flexutils-3.1.6/scipion_em_flexutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-01 10:23:12.000000 scipion-em-flexutils-3.1.6/scipion_em_flexutils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-01 10:23:12.000000 scipion-em-flexutils-3.1.6/scipion_em_flexutils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-01 10:23:12.000000 scipion-em-flexutils-3.1.6/scipion_em_flexutils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 10:23:12.659666 scipion-em-flexutils-3.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-04-01 10:22:39.000000 scipion-em-flexutils-3.1.6/setup.py
```

### Comparing `scipion-em-flexutils-3.1.5/CHANGES.txt` & `scipion-em-flexutils-3.1.6/CHANGES.txt`

 * *Files identical despite different names*

### Comparing `scipion-em-flexutils-3.1.5/LICENSE` & `scipion-em-flexutils-3.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `scipion-em-flexutils-3.1.5/PKG-INFO` & `scipion-em-flexutils-3.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: scipion-em-flexutils
-Version: 3.1.5
+Version: 3.1.6
 Summary: Tools for 3D visualization and manipulation of flexibility data
 Home-page: https://github.com/scipion-em/scipion-em-flexutils
 Author: David Herreros
 Author-email: dherreros@cnb.csic.es
 License: UNKNOWN
 Description: ==========================
         Scipion flexutils plugin
```

### Comparing `scipion-em-flexutils-3.1.5/README.rst` & `scipion-em-flexutils-3.1.6/README.rst`

 * *Files identical despite different names*

### Comparing `scipion-em-flexutils-3.1.5/flexutils/__init__.py` & `scipion-em-flexutils-3.1.6/flexutils/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
 from pwem import Config as emConfig
 
 import flexutils
 from flexutils.constants import CONDA_YML
 
 
-__version__ = "3.1.5"
+__version__ = "3.1.6"
 _logo = "icon.png"
 _references = []
 
 
 class Plugin(pwplugin.Plugin):
 
     @classmethod
@@ -116,15 +116,15 @@
             return installationCmd
 
         def getCondaInstallationTensorflow():
             conda_init = cls.getCondaActivationCmd()
             branch = "devel" if cls.inDevelMode() else "master"
             installationCmd = f'if [ $(basename "$PWD") = flexutils-{__version__} ]; then cd ..; fi && '
             installationCmd += f"{conda_init} conda activate flexutils && " \
-                               f"git clone -b {branch} https://github.com/I2PC/Flexutils-Toolkit.git && " \
+                               f' if [ ! -d "Flexutils-Toolkit" ]; then git clone -b {branch} https://github.com/I2PC/Flexutils-Toolkit.git; fi && ' \
                                f"cd Flexutils-Toolkit && " \
                                f"bash install.sh && touch flexutils_tensorflow_installed && cd .."
             return installationCmd
 
         def getUpdateCommands():
             conda_init = cls.getCondaActivationCmd()
             updateCmd = f'if [ $(basename "$PWD") = flexutils-{__version__} ]; then cd ..; fi && '
```

### Comparing `scipion-em-flexutils-3.1.5/flexutils/bibtex.py` & `scipion-em-flexutils-3.1.6/flexutils/bibtex.py`

 * *Files identical despite different names*

### Comparing `scipion-em-flexutils-3.1.5/flexutils/constants.py` & `scipion-em-flexutils-3.1.6/flexutils/constants.py`

 * *Files identical despite different names*

### Comparing `scipion-em-flexutils-3.1.5/flexutils/icon.png` & `scipion-em-flexutils-3.1.6/flexutils/icon.png`

 * *Files identical despite different names*

### Comparing `scipion-em-flexutils-3.1.5/flexutils/icon_square.png` & `scipion-em-flexutils-3.1.6/flexutils/icon_square.png`

 * *Files identical despite different names*

### Comparing `scipion-em-flexutils-3.1.5/flexutils/loading.gif` & `scipion-em-flexutils-3.1.6/flexutils/loading.gif`

 * *Files identical despite different names*

### Comparing `scipion-em-flexutils-3.1.5/flexutils/protocols/__init__.py` & `scipion-em-flexutils-3.1.6/flexutils/protocols/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-flexutils-3.1.5/flexutils/protocols/deprecated/annotation_2d_tools/viewer_interactive_2d.py` & `scipion-em-flexutils-3.1.6/flexutils/protocols/deprecated/annotation_2d_tools/viewer_interactive_2d.py`

 * *Files identical despite different names*

### Comparing `scipion-em-flexutils-3.1.5/flexutils/protocols/deprecated/annotation_3d_tools/viewer_3d_pc.py` & `scipion-em-flexutils-3.1.6/flexutils/protocols/deprecated/annotation_3d_tools/viewer_3d_pc.py`

 * *Files identical despite different names*

### Comparing `scipion-em-flexutils-3.1.5/flexutils/protocols/deprecated/annotation_3d_tools/viewer_3d_slicer.py` & `scipion-em-flexutils-3.1.6/flexutils/protocols/deprecated/annotation_3d_tools/viewer_3d_slicer.py`

 * *Files identical despite different names*

### Comparing `scipion-em-flexutils-3.1.5/flexutils/protocols/deprecated/annotation_3d_tools/viewer_interactive_2d_3d.py` & `scipion-em-flexutils-3.1.6/flexutils/protocols/deprecated/annotation_3d_tools/viewer_interactive_2d_3d.py`

 * *Files identical despite different names*

### Comparing `scipion-em-flexutils-3.1.5/flexutils/protocols/deprecated/chimera_viewers/viewer_morph_salesman_old.py` & `scipion-em-flexutils-3.1.6/flexutils/protocols/deprecated/chimera_viewers/viewer_morph_salesman_old.py`

 * *Files identical despite different names*

### Comparing `scipion-em-flexutils-3.1.5/flexutils/protocols/deprecated/point_cloud_viewers/viewer_point_cloud.py` & `scipion-em-flexutils-3.1.6/flexutils/protocols/deprecated/point_cloud_viewers/viewer_point_cloud.py`

 * *Files identical despite different names*

### Comparing `scipion-em-flexutils-3.1.5/flexutils/protocols/deprecated/protocol_angular_align_deep_nma.py` & `scipion-em-flexutils-3.1.6/flexutils/protocols/deprecated/protocol_angular_align_deep_nma.py`

 * *Files identical despite different names*

### Comparing `scipion-em-flexutils-3.1.5/flexutils/protocols/deprecated/protocol_cluster_space.py` & `scipion-em-flexutils-3.1.6/flexutils/protocols/deprecated/protocol_cluster_space.py`

 * *Files identical despite different names*

### Comparing `scipion-em-flexutils-3.1.5/flexutils/protocols/deprecated/protocol_predict_deep_nma.py` & `scipion-em-flexutils-3.1.6/flexutils/protocols/deprecated/protocol_predict_deep_nma.py`

 * *Files identical despite different names*

### Comparing `scipion-em-flexutils-3.1.5/flexutils/protocols/protocol_annotate_space.py` & `scipion-em-flexutils-3.1.6/flexutils/protocols/protocol_annotate_space.py`

 * *Files identical despite different names*

### Comparing `scipion-em-flexutils-3.1.5/flexutils/protocols/protocol_associate_flex_space_to_particles.py` & `scipion-em-flexutils-3.1.6/flexutils/protocols/protocol_associate_flex_space_to_particles.py`

 * *Files identical despite different names*

### Comparing `scipion-em-flexutils-3.1.5/flexutils/protocols/protocol_auto_reference.py` & `scipion-em-flexutils-3.1.6/flexutils/protocols/protocol_auto_reference.py`

 * *Files identical despite different names*

### Comparing `scipion-em-flexutils-3.1.5/flexutils/protocols/protocol_dimred.py` & `scipion-em-flexutils-3.1.6/flexutils/protocols/protocol_dimred.py`

 * *Files identical despite different names*

### Comparing `scipion-em-flexutils-3.1.5/flexutils/protocols/protocol_filter_pca.py` & `scipion-em-flexutils-3.1.6/flexutils/protocols/protocol_filter_pca.py`

 * *Files identical despite different names*

### Comparing `scipion-em-flexutils-3.1.5/flexutils/protocols/protocol_find_optimal_clusters.py` & `scipion-em-flexutils-3.1.6/flexutils/protocols/protocol_find_optimal_clusters.py`

 * *Files identical despite different names*

### Comparing `scipion-em-flexutils-3.1.5/flexutils/protocols/protocol_order_volumes.py` & `scipion-em-flexutils-3.1.6/flexutils/protocols/protocol_order_volumes.py`

 * *Files identical despite different names*

### Comparing `scipion-em-flexutils-3.1.5/flexutils/protocols/protocol_score_landscape.py` & `scipion-em-flexutils-3.1.6/flexutils/protocols/protocol_score_landscape.py`

 * *Files identical despite different names*

### Comparing `scipion-em-flexutils-3.1.5/flexutils/protocols/protocol_select_views.py` & `scipion-em-flexutils-3.1.6/flexutils/protocols/protocol_select_views.py`

 * *Files identical despite different names*

### Comparing `scipion-em-flexutils-3.1.5/flexutils/protocols/xmipp/__init__.py` & `scipion-em-flexutils-3.1.6/flexutils/protocols/xmipp/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-flexutils-3.1.5/flexutils/protocols/xmipp/protocol_angular_align_deep_pose.py` & `scipion-em-flexutils-3.1.6/flexutils/protocols/xmipp/protocol_angular_align_deep_pose.py`

 * *Files identical despite different names*

### Comparing `scipion-em-flexutils-3.1.5/flexutils/protocols/xmipp/protocol_angular_align_het_siren.py` & `scipion-em-flexutils-3.1.6/flexutils/protocols/xmipp/protocol_angular_align_het_siren.py`

 * *Files 0% similar despite different names*

```diff
@@ -410,15 +410,15 @@
         sr = correctionFactor * self.inputParticles.get().getSamplingRate()
         trainSize = self.trainSize.get() if self.trainSize.get() is not None else self.newXdim
         if isinstance(inputParticles, SetOfParticlesFlex) and hasattr(inputParticles.getFlexInfo(), "outSize"):
             outSize = inputParticles.getFlexInfo().outSize.get()
         else:
             outSize = self.outSize.get() if self.outSize.get() is not None else self.newXdim
         applyCTF = self.applyCTF.get()
-        args = "--md_file %s --weigths_file %s --pad %d --refine_pose --sr %f " \
+        args = "--md_file %s --weigths_file %s --pad %d --sr %f " \
                "--apply_ctf %d --het_dim %d --num_vol %d --trainSize %d --outSize %d" \
                % (md_file, weigths_file, pad, sr, applyCTF, hetDim, numVol, trainSize, outSize)
 
         if self.ctfType.get() == 0:
             args += " --ctf_type apply"
         elif self.ctfType.get() == 1:
             args += " --ctf_type wiener"
```

### Comparing `scipion-em-flexutils-3.1.5/flexutils/protocols/xmipp/protocol_angular_align_homo_siren.py` & `scipion-em-flexutils-3.1.6/flexutils/protocols/xmipp/protocol_angular_align_homo_siren.py`

 * *Files identical despite different names*

### Comparing `scipion-em-flexutils-3.1.5/flexutils/protocols/xmipp/protocol_angular_align_zernike3deep.py` & `scipion-em-flexutils-3.1.6/flexutils/protocols/xmipp/protocol_angular_align_zernike3deep.py`

 * *Files identical despite different names*

### Comparing `scipion-em-flexutils-3.1.5/flexutils/protocols/xmipp/protocol_angular_alignment_zernike3d.py` & `scipion-em-flexutils-3.1.6/flexutils/protocols/xmipp/protocol_angular_alignment_zernike3d.py`

 * *Files identical despite different names*

### Comparing `scipion-em-flexutils-3.1.5/flexutils/protocols/xmipp/protocol_apply_field_nma.py` & `scipion-em-flexutils-3.1.6/flexutils/protocols/xmipp/protocol_apply_field_nma.py`

 * *Files identical despite different names*

### Comparing `scipion-em-flexutils-3.1.5/flexutils/protocols/xmipp/protocol_apply_field_zernike3d.py` & `scipion-em-flexutils-3.1.6/flexutils/protocols/xmipp/protocol_apply_field_zernike3d.py`

 * *Files identical despite different names*

### Comparing `scipion-em-flexutils-3.1.5/flexutils/protocols/xmipp/protocol_assign_heterogeneity_priors_zernike3d.py` & `scipion-em-flexutils-3.1.6/flexutils/protocols/xmipp/protocol_assign_heterogeneity_priors_zernike3d.py`

 * *Files identical despite different names*

### Comparing `scipion-em-flexutils-3.1.5/flexutils/protocols/xmipp/protocol_cluster_structures_zernike3d.py` & `scipion-em-flexutils-3.1.6/flexutils/protocols/xmipp/protocol_cluster_structures_zernike3d.py`

 * *Files identical despite different names*

### Comparing `scipion-em-flexutils-3.1.5/flexutils/protocols/xmipp/protocol_compute_priors_zernike3d.py` & `scipion-em-flexutils-3.1.6/flexutils/protocols/xmipp/protocol_compute_priors_zernike3d.py`

 * *Files identical despite different names*

### Comparing `scipion-em-flexutils-3.1.5/flexutils/protocols/xmipp/protocol_deform_map_zernike3d.py` & `scipion-em-flexutils-3.1.6/flexutils/protocols/xmipp/protocol_deform_map_zernike3d.py`

 * *Files identical despite different names*

### Comparing `scipion-em-flexutils-3.1.5/flexutils/protocols/xmipp/protocol_denoise_particles_het_siren.py` & `scipion-em-flexutils-3.1.6/flexutils/protocols/xmipp/protocol_denoise_particles_het_siren.py`

 * *Files identical despite different names*

### Comparing `scipion-em-flexutils-3.1.5/flexutils/protocols/xmipp/protocol_focus_zernike3d.py` & `scipion-em-flexutils-3.1.6/flexutils/protocols/xmipp/protocol_focus_zernike3d.py`

 * *Files identical despite different names*

### Comparing `scipion-em-flexutils-3.1.5/flexutils/protocols/xmipp/protocol_interactive_flex_consensus.py` & `scipion-em-flexutils-3.1.6/flexutils/protocols/xmipp/protocol_interactive_flex_consensus.py`

 * *Files identical despite different names*

### Comparing `scipion-em-flexutils-3.1.5/flexutils/protocols/xmipp/protocol_match_and_deform_map_zernike3d.py` & `scipion-em-flexutils-3.1.6/flexutils/protocols/xmipp/protocol_match_and_deform_map_zernike3d.py`

 * *Files identical despite different names*

### Comparing `scipion-em-flexutils-3.1.5/flexutils/protocols/xmipp/protocol_match_and_deform_structure_zernike3d.py` & `scipion-em-flexutils-3.1.6/flexutils/protocols/xmipp/protocol_match_and_deform_structure_zernike3d.py`

 * *Files identical despite different names*

### Comparing `scipion-em-flexutils-3.1.5/flexutils/protocols/xmipp/protocol_predict_deep_pose.py` & `scipion-em-flexutils-3.1.6/flexutils/protocols/xmipp/protocol_predict_deep_pose.py`

 * *Files identical despite different names*

### Comparing `scipion-em-flexutils-3.1.5/flexutils/protocols/xmipp/protocol_predict_het_siren.py` & `scipion-em-flexutils-3.1.6/flexutils/protocols/xmipp/protocol_predict_het_siren.py`

 * *Files identical despite different names*

### Comparing `scipion-em-flexutils-3.1.5/flexutils/protocols/xmipp/protocol_predict_homo_siren.py` & `scipion-em-flexutils-3.1.6/flexutils/protocols/xmipp/protocol_predict_homo_siren.py`

 * *Files identical despite different names*

### Comparing `scipion-em-flexutils-3.1.5/flexutils/protocols/xmipp/protocol_predict_zernike3deep.py` & `scipion-em-flexutils-3.1.6/flexutils/protocols/xmipp/protocol_predict_zernike3deep.py`

 * *Files identical despite different names*

### Comparing `scipion-em-flexutils-3.1.5/flexutils/protocols/xmipp/protocol_prepare_volumes_zernike3deep.py` & `scipion-em-flexutils-3.1.6/flexutils/protocols/xmipp/protocol_prepare_volumes_zernike3deep.py`

 * *Files identical despite different names*

### Comparing `scipion-em-flexutils-3.1.5/flexutils/protocols/xmipp/protocol_reassign_reference_zernike3d.py` & `scipion-em-flexutils-3.1.6/flexutils/protocols/xmipp/protocol_reassign_reference_zernike3d.py`

 * *Files identical despite different names*

### Comparing `scipion-em-flexutils-3.1.5/flexutils/protocols/xmipp/protocol_reconstruct_zart.py` & `scipion-em-flexutils-3.1.6/flexutils/protocols/xmipp/protocol_reconstruct_zart.py`

 * *Files identical despite different names*

### Comparing `scipion-em-flexutils-3.1.5/flexutils/protocols/xmipp/protocol_resize_zernike_data.py` & `scipion-em-flexutils-3.1.6/flexutils/protocols/xmipp/protocol_resize_zernike_data.py`

 * *Files identical despite different names*

### Comparing `scipion-em-flexutils-3.1.5/flexutils/protocols/xmipp/protocol_statistics_zernike3d.py` & `scipion-em-flexutils-3.1.6/flexutils/protocols/xmipp/protocol_statistics_zernike3d.py`

 * *Files identical despite different names*

### Comparing `scipion-em-flexutils-3.1.5/flexutils/protocols/xmipp/protocol_structure_landscape.py` & `scipion-em-flexutils-3.1.6/flexutils/protocols/xmipp/protocol_structure_landscape.py`

 * *Files identical despite different names*

### Comparing `scipion-em-flexutils-3.1.5/flexutils/protocols/xmipp/protocol_train_flex_consensus.py` & `scipion-em-flexutils-3.1.6/flexutils/protocols/xmipp/protocol_train_flex_consensus.py`

 * *Files identical despite different names*

### Comparing `scipion-em-flexutils-3.1.5/flexutils/protocols/xmipp/utils/__init__.py` & `scipion-em-flexutils-3.1.6/flexutils/protocols/xmipp/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-flexutils-3.1.5/flexutils/protocols/xmipp/utils/custom_pdb_parser.py` & `scipion-em-flexutils-3.1.6/flexutils/protocols/xmipp/utils/custom_pdb_parser.py`

 * *Files identical despite different names*

### Comparing `scipion-em-flexutils-3.1.5/flexutils/protocols/xmipp/utils/utils.py` & `scipion-em-flexutils-3.1.6/flexutils/protocols/xmipp/utils/utils.py`

 * *Files identical despite different names*

### Comparing `scipion-em-flexutils-3.1.5/flexutils/protocols.conf` & `scipion-em-flexutils-3.1.6/flexutils/protocols.conf`

 * *Files identical despite different names*

### Comparing `scipion-em-flexutils-3.1.5/flexutils/tests/__init__.py` & `scipion-em-flexutils-3.1.6/flexutils/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-flexutils-3.1.5/flexutils/utils.py` & `scipion-em-flexutils-3.1.6/flexutils/utils.py`

 * *Files identical despite different names*

### Comparing `scipion-em-flexutils-3.1.5/flexutils/viewers/__init__.py` & `scipion-em-flexutils-3.1.6/flexutils/viewers/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-flexutils-3.1.5/flexutils/viewers/clustering_viewers/viewer_optimal_clusters.py` & `scipion-em-flexutils-3.1.6/flexutils/viewers/clustering_viewers/viewer_optimal_clusters.py`

 * *Files identical despite different names*

### Comparing `scipion-em-flexutils-3.1.5/flexutils/viewers/consensus_viewers/viewer_interactive_hist.py` & `scipion-em-flexutils-3.1.6/flexutils/viewers/consensus_viewers/viewer_interactive_hist.py`

 * *Files identical despite different names*

### Comparing `scipion-em-flexutils-3.1.5/flexutils/viewers/imagej_viewers/viewer_ij.py` & `scipion-em-flexutils-3.1.6/flexutils/viewers/imagej_viewers/viewer_ij.py`

 * *Files identical despite different names*

### Comparing `scipion-em-flexutils-3.1.5/flexutils/viewers/map_model_viewers/viewer_show_maps.py` & `scipion-em-flexutils-3.1.6/flexutils/viewers/map_model_viewers/viewer_show_maps.py`

 * *Files identical despite different names*

### Comparing `scipion-em-flexutils-3.1.5/flexutils/viewers/tensorboard/__init__.py` & `scipion-em-flexutils-3.1.6/flexutils/viewers/tensorboard/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-flexutils-3.1.5/flexutils/viewers/tensorboard/setup_tensorboard.py` & `scipion-em-flexutils-3.1.6/flexutils/viewers/tensorboard/setup_tensorboard.py`

 * *Files identical despite different names*

### Comparing `scipion-em-flexutils-3.1.5/flexutils/viewers/tensorboard/viewer_tensorboard.py` & `scipion-em-flexutils-3.1.6/flexutils/viewers/tensorboard/viewer_tensorboard.py`

 * *Files identical despite different names*

### Comparing `scipion-em-flexutils-3.1.5/flexutils/viewers/viewer_show_structures.py` & `scipion-em-flexutils-3.1.6/flexutils/viewers/viewer_show_structures.py`

 * *Files identical despite different names*

### Comparing `scipion-em-flexutils-3.1.5/flexutils/viewers/viewers_data.py` & `scipion-em-flexutils-3.1.6/flexutils/viewers/viewers_data.py`

 * *Files identical despite different names*

### Comparing `scipion-em-flexutils-3.1.5/flexutils/viewers/xmipp/__init__.py` & `scipion-em-flexutils-3.1.6/flexutils/viewers/xmipp/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-flexutils-3.1.5/flexutils/viewers/xmipp/viewer_apply_field_nma.py` & `scipion-em-flexutils-3.1.6/flexutils/viewers/xmipp/viewer_apply_field_nma.py`

 * *Files identical despite different names*

### Comparing `scipion-em-flexutils-3.1.5/flexutils/viewers/xmipp/viewer_apply_field_zernike3d.py` & `scipion-em-flexutils-3.1.6/flexutils/viewers/xmipp/viewer_apply_field_zernike3d.py`

 * *Files identical despite different names*

### Comparing `scipion-em-flexutils-3.1.5/flexutils/viewers/xmipp/viewer_flex_consensus.py` & `scipion-em-flexutils-3.1.6/flexutils/viewers/xmipp/viewer_flex_consensus.py`

 * *Files identical despite different names*

### Comparing `scipion-em-flexutils-3.1.5/flexutils/viewers/xmipp/viewer_landscape.py` & `scipion-em-flexutils-3.1.6/flexutils/viewers/xmipp/viewer_landscape.py`

 * *Files identical despite different names*

### Comparing `scipion-em-flexutils-3.1.5/flexutils/viewers/xmipp/viewer_reduced_space.py` & `scipion-em-flexutils-3.1.6/flexutils/viewers/xmipp/viewer_reduced_space.py`

 * *Files 10% similar despite different names*

```diff
@@ -85,14 +85,18 @@
 
             # Generate files to call command line
             np.savetxt(file_interp, deformation)
 
             # Run slicer
             args = "--data %s --z_space %s --interp_val %s --onlyView" \
                    % (file_red_space, file_z_space, file_interp)
+            if hasattr(particles.getFlexInfo(), "umap_weights"):
+                args += " --reduce umap --umap_weights %s" % particles.getFlexInfo().getAttr("umap_weights")
+            else:
+                args += " --reduce pca"
             program = "viewer_interactive_3d.py"
             program = flexutils.Plugin.getProgram(program)
 
             command = buildRunCommand(program, args, 1)
             subprocess.Popen(command, shell=True)
 
         # Launch with Pathos
```

### Comparing `scipion-em-flexutils-3.1.5/flexutils/viewers/xmipp/viewer_structure_map_zernike3d.py` & `scipion-em-flexutils-3.1.6/flexutils/viewers/xmipp/viewer_structure_map_zernike3d.py`

 * *Files identical despite different names*

### Comparing `scipion-em-flexutils-3.1.5/scipion_em_flexutils.egg-info/PKG-INFO` & `scipion-em-flexutils-3.1.6/scipion_em_flexutils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: scipion-em-flexutils
-Version: 3.1.5
+Version: 3.1.6
 Summary: Tools for 3D visualization and manipulation of flexibility data
 Home-page: https://github.com/scipion-em/scipion-em-flexutils
 Author: David Herreros
 Author-email: dherreros@cnb.csic.es
 License: UNKNOWN
 Description: ==========================
         Scipion flexutils plugin
```

### Comparing `scipion-em-flexutils-3.1.5/scipion_em_flexutils.egg-info/SOURCES.txt` & `scipion-em-flexutils-3.1.6/scipion_em_flexutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scipion-em-flexutils-3.1.5/setup.py` & `scipion-em-flexutils-3.1.6/setup.py`

 * *Files identical despite different names*

