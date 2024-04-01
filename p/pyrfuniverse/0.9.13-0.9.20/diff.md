# Comparing `tmp/pyrfuniverse-0.9.13.tar.gz` & `tmp/pyrfuniverse-0.9.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrfuniverse-0.9.13.tar", last modified: Wed Aug  2 02:39:41 2023, max compression
+gzip compressed data, was "pyrfuniverse-0.9.20.tar", last modified: Fri Aug 18 05:30:00 2023, max compression
```

## Comparing `pyrfuniverse-0.9.13.tar` & `pyrfuniverse-0.9.20.tar`

### file list

```diff
@@ -1,125 +1,128 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 02:39:41.268146 pyrfuniverse-0.9.13/
--rw-rw-rw-   0        0        0    11357 2022-08-10 05:19:33.000000 pyrfuniverse-0.9.13/LICENSE
--rw-rw-rw-   0        0        0      266 2023-08-02 02:39:41.268146 pyrfuniverse-0.9.13/PKG-INFO
--rw-rw-rw-   0        0        0     2758 2023-06-21 09:17:40.000000 pyrfuniverse-0.9.13/README.md
-drwxrwxrwx   0        0        0        0 2023-08-02 02:39:41.059138 pyrfuniverse-0.9.13/pyrfuniverse/
--rw-rw-rw-   0        0        0      759 2023-08-02 02:25:12.000000 pyrfuniverse-0.9.13/pyrfuniverse/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-02 02:39:41.141619 pyrfuniverse-0.9.13/pyrfuniverse/attributes/
--rw-rw-rw-   0        0        0     1472 2023-06-21 09:17:41.000000 pyrfuniverse-0.9.13/pyrfuniverse/attributes/__init__.py
--rw-rw-rw-   0        0        0     4555 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.13/pyrfuniverse/attributes/activelightsensor_attr.py
--rw-rw-rw-   0        0        0     9352 2023-07-12 10:53:12.000000 pyrfuniverse-0.9.13/pyrfuniverse/attributes/base_attr.py
--rw-rw-rw-   0        0        0     8438 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.13/pyrfuniverse/attributes/camera_attr.py
--rw-rw-rw-   0        0        0      384 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.13/pyrfuniverse/attributes/cloth_attr.py
--rw-rw-rw-   0        0        0      601 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.13/pyrfuniverse/attributes/collider_attr.py
--rw-rw-rw-   0        0        0    15137 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.13/pyrfuniverse/attributes/controller_attr.py
--rw-rw-rw-   0        0        0      622 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.13/pyrfuniverse/attributes/custom_attr.py
--rw-rw-rw-   0        0        0      678 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.13/pyrfuniverse/attributes/digit_attr.py
--rw-rw-rw-   0        0        0      871 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.13/pyrfuniverse/attributes/fallingcloth_attr.py
--rw-rw-rw-   0        0        0     1533 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.13/pyrfuniverse/attributes/gameobject_attr.py
--rw-rw-rw-   0        0        0     4038 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.13/pyrfuniverse/attributes/graspsim_attr.py
--rw-rw-rw-   0        0        0     4520 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.13/pyrfuniverse/attributes/humanbody_attr.py
--rw-rw-rw-   0        0        0     2643 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.13/pyrfuniverse/attributes/light_attr.py
--rw-rw-rw-   0        0        0     8924 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.13/pyrfuniverse/attributes/omplmanager_attr.py
--rw-rw-rw-   0        0        0     1331 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.13/pyrfuniverse/attributes/pointcloud_attr.py
--rw-rw-rw-   0        0        0     1737 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.13/pyrfuniverse/attributes/rigidbody_attr.py
--rw-rw-rw-   0        0        0      387 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.13/pyrfuniverse/attributes/softbody_attr.py
-drwxrwxrwx   0        0        0        0 2023-08-02 02:39:41.156498 pyrfuniverse-0.9.13/pyrfuniverse/envs/
--rw-rw-rw-   0        0        0    15241 2023-07-26 07:51:49.000000 pyrfuniverse-0.9.13/pyrfuniverse/envs/__init__.py
--rw-rw-rw-   0        0        0     4178 2022-07-08 02:22:23.000000 pyrfuniverse-0.9.13/pyrfuniverse/envs/balance_ball_env.py
--rw-rw-rw-   0        0        0    24832 2023-07-14 07:27:36.000000 pyrfuniverse-0.9.13/pyrfuniverse/envs/base_env.py
--rw-rw-rw-   0        0        0     4564 2022-07-08 02:22:23.000000 pyrfuniverse-0.9.13/pyrfuniverse/envs/bouncer_env.py
--rw-rw-rw-   0        0        0     3982 2023-02-10 17:44:39.000000 pyrfuniverse-0.9.13/pyrfuniverse/envs/franka_grasp_env.py
--rw-rw-rw-   0        0        0     3077 2022-07-08 02:22:23.000000 pyrfuniverse-0.9.13/pyrfuniverse/envs/franka_push_env.py
-drwxrwxrwx   0        0        0        0 2023-08-02 02:39:41.160015 pyrfuniverse-0.9.13/pyrfuniverse/envs/gripper_nail/
--rw-rw-rw-   0        0        0      736 2022-06-27 07:07:03.000000 pyrfuniverse-0.9.13/pyrfuniverse/envs/gripper_nail/__init__.py
--rw-rw-rw-   0        0        0     4209 2022-07-08 02:22:23.000000 pyrfuniverse-0.9.13/pyrfuniverse/envs/gripper_nail/nail_can_env.py
--rw-rw-rw-   0        0        0     5750 2022-07-08 02:22:23.000000 pyrfuniverse-0.9.13/pyrfuniverse/envs/gripper_nail/nail_card_env.py
--rw-rw-rw-   0        0        0     3917 2022-07-08 02:22:23.000000 pyrfuniverse-0.9.13/pyrfuniverse/envs/gripper_nail/robotiq85_insert_env.py
--rw-rw-rw-   0        0        0     4149 2022-07-08 02:22:23.000000 pyrfuniverse-0.9.13/pyrfuniverse/envs/gripper_nail/robotiq85_nail_book_env.py
--rw-rw-rw-   0        0        0     4220 2022-07-08 02:22:23.000000 pyrfuniverse-0.9.13/pyrfuniverse/envs/gripper_nail/robotiq85_nail_can_env.py
--rw-rw-rw-   0        0        0     5917 2022-07-08 02:22:23.000000 pyrfuniverse-0.9.13/pyrfuniverse/envs/gripper_nail/robotiq85_nail_card_env.py
--rw-rw-rw-   0        0        0     5696 2022-07-08 02:22:23.000000 pyrfuniverse-0.9.13/pyrfuniverse/envs/gripper_nail/robotiq85_nail_coin_env.py
--rw-rw-rw-   0        0        0      769 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.13/pyrfuniverse/envs/gym_goal_wrapper_env.py
--rw-rw-rw-   0        0        0      702 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.13/pyrfuniverse/envs/gym_wrapper_env.py
-drwxrwxrwx   0        0        0        0 2023-08-02 02:39:41.175061 pyrfuniverse-0.9.13/pyrfuniverse/envs/multi_agent/
--rw-rw-rw-   0        0        0      172 2022-06-27 07:07:03.000000 pyrfuniverse-0.9.13/pyrfuniverse/envs/multi_agent/__init__.py
--rw-rw-rw-   0        0        0     9111 2023-02-10 17:44:39.000000 pyrfuniverse-0.9.13/pyrfuniverse/envs/multi_agent/cleaner_env.py
--rw-rw-rw-   0        0        0    11818 2022-07-08 02:22:23.000000 pyrfuniverse-0.9.13/pyrfuniverse/envs/multi_agent/navigation_env.py
--rw-rw-rw-   0        0        0     6000 2022-07-08 02:22:23.000000 pyrfuniverse-0.9.13/pyrfuniverse/envs/multi_agent_navigation_env.py
-drwxrwxrwx   0        0        0        0 2023-08-02 02:39:41.177064 pyrfuniverse-0.9.13/pyrfuniverse/envs/multi_physics/
--rw-rw-rw-   0        0        0      871 2023-06-21 09:17:41.000000 pyrfuniverse-0.9.13/pyrfuniverse/envs/multi_physics/__init__.py
--rw-rw-rw-   0        0        0    13868 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.13/pyrfuniverse/envs/multi_physics/flexiv_cutting.py
--rw-rw-rw-   0        0        0     8156 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.13/pyrfuniverse/envs/multi_physics/kinova_gen2_catching_cloth_env.py
--rw-rw-rw-   0        0        0    10075 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.13/pyrfuniverse/envs/multi_physics/ur5_water_shooting.py
--rw-rw-rw-   0        0        0      513 2022-07-08 02:22:23.000000 pyrfuniverse-0.9.13/pyrfuniverse/envs/rfuniverse_robot_hub_env.py
-drwxrwxrwx   0        0        0        0 2023-08-02 02:39:41.184596 pyrfuniverse-0.9.13/pyrfuniverse/envs/robotics/
--rw-rw-rw-   0        0        0      675 2022-06-27 07:07:03.000000 pyrfuniverse-0.9.13/pyrfuniverse/envs/robotics/__init__.py
--rw-rw-rw-   0        0        0     7488 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.13/pyrfuniverse/envs/robotics/franka_cloth_env.py
--rw-rw-rw-   0        0        0     7679 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.13/pyrfuniverse/envs/robotics/franka_cloth_fold_env.py
--rw-rw-rw-   0        0        0     9654 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.13/pyrfuniverse/envs/robotics/franka_robotics_env.py
--rw-rw-rw-   0        0        0     8235 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.13/pyrfuniverse/envs/robotics/franka_softbody_env.py
--rw-rw-rw-   0        0        0      817 2022-12-15 05:37:19.000000 pyrfuniverse-0.9.13/pyrfuniverse/envs/robotics/pick_and_place_env.py
--rw-rw-rw-   0        0        0      754 2022-07-08 02:22:23.000000 pyrfuniverse-0.9.13/pyrfuniverse/envs/robotics/push_env.py
--rw-rw-rw-   0        0        0      864 2022-07-08 02:22:23.000000 pyrfuniverse-0.9.13/pyrfuniverse/envs/robotics/reach_env.py
--rw-rw-rw-   0        0        0     4463 2022-07-08 02:22:23.000000 pyrfuniverse-0.9.13/pyrfuniverse/envs/roller_env.py
-drwxrwxrwx   0        0        0        0 2023-08-02 02:39:41.185596 pyrfuniverse-0.9.13/pyrfuniverse/envs/tobor_robotics/
--rw-rw-rw-   0        0        0      121 2022-06-27 07:07:03.000000 pyrfuniverse-0.9.13/pyrfuniverse/envs/tobor_robotics/__init__.py
--rw-rw-rw-   0        0        0    10897 2022-07-08 02:22:23.000000 pyrfuniverse-0.9.13/pyrfuniverse/envs/tobor_robotics/tobor_push_pull_env.py
--rw-rw-rw-   0        0        0     8876 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.13/pyrfuniverse/envs/tobor_robotiq85_manipulation_env.py
--rw-rw-rw-   0        0        0     8205 2022-11-02 03:34:57.000000 pyrfuniverse-0.9.13/pyrfuniverse/envs/ur5_box_env.py
--rw-rw-rw-   0        0        0     8549 2022-11-02 03:34:57.000000 pyrfuniverse-0.9.13/pyrfuniverse/envs/ur5_drawer_env.py
-drwxrwxrwx   0        0        0        0 2023-08-02 02:39:41.200724 pyrfuniverse-0.9.13/pyrfuniverse/side_channel/
--rw-rw-rw-   0        0        0      144 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.13/pyrfuniverse/side_channel/__init__.py
--rw-rw-rw-   0        0        0     3244 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.13/pyrfuniverse/side_channel/incoming_message.py
--rw-rw-rw-   0        0        0     1536 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.13/pyrfuniverse/side_channel/outgoing_message.py
-drwxrwxrwx   0        0        0        0 2023-08-02 02:39:41.216340 pyrfuniverse-0.9.13/pyrfuniverse/utils/
--rw-rw-rw-   0        0        0        0 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.13/pyrfuniverse/utils/__init__.py
--rw-rw-rw-   0        0        0    13620 2023-02-10 17:44:39.000000 pyrfuniverse-0.9.13/pyrfuniverse/utils/active_depth_generate.py
--rw-rw-rw-   0        0        0     6006 2022-07-13 10:31:45.000000 pyrfuniverse-0.9.13/pyrfuniverse/utils/controller.py
--rw-rw-rw-   0        0        0    11746 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.13/pyrfuniverse/utils/depth_processor.py
--rw-rw-rw-   0        0        0     3314 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.13/pyrfuniverse/utils/interpolate_utils.py
--rw-rw-rw-   0        0        0     4304 2022-06-27 07:07:03.000000 pyrfuniverse-0.9.13/pyrfuniverse/utils/jaco_controller.py
--rw-rw-rw-   0        0        0     4908 2022-10-27 03:27:48.000000 pyrfuniverse-0.9.13/pyrfuniverse/utils/kinova_controller.py
--rw-rw-rw-   0        0        0      755 2022-06-27 07:07:03.000000 pyrfuniverse-0.9.13/pyrfuniverse/utils/os_utils.py
--rw-rw-rw-   0        0        0     9988 2023-08-01 12:00:28.000000 pyrfuniverse-0.9.13/pyrfuniverse/utils/rfuniverse_communicator.py
--rw-rw-rw-   0        0        0     3569 2023-06-21 09:17:41.000000 pyrfuniverse-0.9.13/pyrfuniverse/utils/rfuniverse_utility.py
--rw-rw-rw-   0        0        0     5690 2022-06-27 07:07:03.000000 pyrfuniverse-0.9.13/pyrfuniverse/utils/stretch_controller.py
--rw-rw-rw-   0        0        0     6776 2022-08-15 11:02:54.000000 pyrfuniverse-0.9.13/pyrfuniverse/utils/tobor_controller.py
--rw-rw-rw-   0        0        0     4783 2022-06-27 07:07:03.000000 pyrfuniverse-0.9.13/pyrfuniverse/utils/ur5_controller.py
-drwxrwxrwx   0        0        0        0 2023-08-02 02:39:41.073388 pyrfuniverse-0.9.13/pyrfuniverse.egg-info/
--rw-rw-rw-   0        0        0      266 2023-08-02 02:39:40.000000 pyrfuniverse-0.9.13/pyrfuniverse.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4080 2023-08-02 02:39:40.000000 pyrfuniverse-0.9.13/pyrfuniverse.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 02:39:40.000000 pyrfuniverse-0.9.13/pyrfuniverse.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-05-27 11:32:20.000000 pyrfuniverse-0.9.13/pyrfuniverse.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       36 2023-08-02 02:39:40.000000 pyrfuniverse-0.9.13/pyrfuniverse.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-08-02 02:39:40.000000 pyrfuniverse-0.9.13/pyrfuniverse.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-02 02:39:41.268146 pyrfuniverse-0.9.13/setup.cfg
--rw-rw-rw-   0        0        0      601 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.13/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-02 02:39:41.268146 pyrfuniverse-0.9.13/test/
--rw-rw-rw-   0        0        0     5924 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.13/test/test_active_depth.py
--rw-rw-rw-   0        0        0      995 2023-04-06 04:45:20.000000 pyrfuniverse-0.9.13/test/test_articulation_ik.py
--rw-rw-rw-   0        0        0      943 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.13/test/test_camera_image.py
--rw-rw-rw-   0        0        0     1939 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.13/test/test_custom_message.py
--rw-rw-rw-   0        0        0     1038 2023-04-06 04:49:14.000000 pyrfuniverse-0.9.13/test/test_debug.py
--rw-rw-rw-   0        0        0      439 2023-04-07 05:04:11.000000 pyrfuniverse-0.9.13/test/test_digit.py
--rw-rw-rw-   0        0        0      827 2023-04-06 04:45:20.000000 pyrfuniverse-0.9.13/test/test_grasp_pose.py
--rw-rw-rw-   0        0        0     2750 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.13/test/test_grasp_sim.py
--rw-rw-rw-   0        0        0      989 2023-04-10 09:39:27.000000 pyrfuniverse-0.9.13/test/test_heat_map.py
--rw-rw-rw-   0        0        0     1426 2023-04-06 04:45:20.000000 pyrfuniverse-0.9.13/test/test_humanbody_ik.py
--rw-rw-rw-   0        0        0     1093 2023-08-01 12:03:45.000000 pyrfuniverse-0.9.13/test/test_image_stream.py
--rw-rw-rw-   0        0        0     1984 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.13/test/test_label.py
--rw-rw-rw-   0        0        0      702 2023-04-06 04:45:20.000000 pyrfuniverse-0.9.13/test/test_light.py
--rw-rw-rw-   0        0        0      589 2023-06-13 10:33:21.000000 pyrfuniverse-0.9.13/test/test_load_mesh.py
--rw-rw-rw-   0        0        0     1008 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.13/test/test_load_urdf.py
--rw-rw-rw-   0        0        0      277 2023-07-10 14:17:21.000000 pyrfuniverse-0.9.13/test/test_load_urdf_akb.py
--rw-rw-rw-   0        0        0     1980 2023-07-13 08:59:36.000000 pyrfuniverse-0.9.13/test/test_object_data.py
--rw-rw-rw-   0        0        0     1646 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.13/test/test_ompl.py
--rw-rw-rw-   0        0        0     2149 2023-03-15 04:00:24.000000 pyrfuniverse-0.9.13/test/test_pick_and_place.py
--rw-rw-rw-   0        0        0     2174 2023-03-15 04:05:23.000000 pyrfuniverse-0.9.13/test/test_pick_and_place_flexiv.py
--rw-rw-rw-   0        0        0      441 2023-04-06 04:45:20.000000 pyrfuniverse-0.9.13/test/test_ply_render.py
--rw-rw-rw-   0        0        0     1658 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.13/test/test_point_cloud.py
--rw-rw-rw-   0        0        0     1830 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.13/test/test_point_cloud_with_intrinsic_matrix.py
--rw-rw-rw-   0        0        0      659 2023-04-13 02:37:33.000000 pyrfuniverse-0.9.13/test/test_save_gripper.py
--rw-rw-rw-   0        0        0      378 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.13/test/test_save_obj.py
--rw-rw-rw-   0        0        0     1024 2023-04-06 04:45:20.000000 pyrfuniverse-0.9.13/test/test_scene.py
--rw-rw-rw-   0        0        0      740 2023-04-07 07:58:17.000000 pyrfuniverse-0.9.13/test/test_tobor_move.py
+drwxrwxrwx   0        0        0        0 2023-08-18 05:30:00.657776 pyrfuniverse-0.9.20/
+-rw-rw-rw-   0        0        0    11357 2022-08-10 05:19:33.000000 pyrfuniverse-0.9.20/LICENSE
+-rw-rw-rw-   0        0        0      266 2023-08-18 05:30:00.657776 pyrfuniverse-0.9.20/PKG-INFO
+-rw-rw-rw-   0        0        0     2758 2023-06-21 09:17:40.000000 pyrfuniverse-0.9.20/README.md
+drwxrwxrwx   0        0        0        0 2023-08-18 05:30:00.587615 pyrfuniverse-0.9.20/pyrfuniverse/
+-rw-rw-rw-   0        0        0      865 2023-08-18 02:38:18.000000 pyrfuniverse-0.9.20/pyrfuniverse/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-18 05:30:00.601156 pyrfuniverse-0.9.20/pyrfuniverse/attributes/
+-rw-rw-rw-   0        0        0     1472 2023-06-21 09:17:41.000000 pyrfuniverse-0.9.20/pyrfuniverse/attributes/__init__.py
+-rw-rw-rw-   0        0        0     4555 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.20/pyrfuniverse/attributes/activelightsensor_attr.py
+-rw-rw-rw-   0        0        0     9144 2023-08-17 09:04:20.000000 pyrfuniverse-0.9.20/pyrfuniverse/attributes/base_attr.py
+-rw-rw-rw-   0        0        0     8438 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.20/pyrfuniverse/attributes/camera_attr.py
+-rw-rw-rw-   0        0        0      384 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.20/pyrfuniverse/attributes/cloth_attr.py
+-rw-rw-rw-   0        0        0     3110 2023-08-16 08:09:24.000000 pyrfuniverse-0.9.20/pyrfuniverse/attributes/collider_attr.py
+-rw-rw-rw-   0        0        0    15199 2023-08-16 08:09:24.000000 pyrfuniverse-0.9.20/pyrfuniverse/attributes/controller_attr.py
+-rw-rw-rw-   0        0        0      622 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.20/pyrfuniverse/attributes/custom_attr.py
+-rw-rw-rw-   0        0        0      678 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.20/pyrfuniverse/attributes/digit_attr.py
+-rw-rw-rw-   0        0        0      871 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.20/pyrfuniverse/attributes/fallingcloth_attr.py
+-rw-rw-rw-   0        0        0     1533 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.20/pyrfuniverse/attributes/gameobject_attr.py
+-rw-rw-rw-   0        0        0     4038 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.20/pyrfuniverse/attributes/graspsim_attr.py
+-rw-rw-rw-   0        0        0     4520 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.20/pyrfuniverse/attributes/humanbody_attr.py
+-rw-rw-rw-   0        0        0     2643 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.20/pyrfuniverse/attributes/light_attr.py
+-rw-rw-rw-   0        0        0     8924 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.20/pyrfuniverse/attributes/omplmanager_attr.py
+-rw-rw-rw-   0        0        0     1331 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.20/pyrfuniverse/attributes/pointcloud_attr.py
+-rw-rw-rw-   0        0        0     1737 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.20/pyrfuniverse/attributes/rigidbody_attr.py
+-rw-rw-rw-   0        0        0      387 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.20/pyrfuniverse/attributes/softbody_attr.py
+drwxrwxrwx   0        0        0        0 2023-08-18 05:30:00.609690 pyrfuniverse-0.9.20/pyrfuniverse/envs/
+-rw-rw-rw-   0        0        0    15241 2023-07-26 07:51:49.000000 pyrfuniverse-0.9.20/pyrfuniverse/envs/__init__.py
+-rw-rw-rw-   0        0        0     4178 2022-07-08 02:22:23.000000 pyrfuniverse-0.9.20/pyrfuniverse/envs/balance_ball_env.py
+-rw-rw-rw-   0        0        0    26897 2023-08-17 09:04:20.000000 pyrfuniverse-0.9.20/pyrfuniverse/envs/base_env.py
+-rw-rw-rw-   0        0        0     4564 2022-07-08 02:22:23.000000 pyrfuniverse-0.9.20/pyrfuniverse/envs/bouncer_env.py
+-rw-rw-rw-   0        0        0     3982 2023-02-10 17:44:39.000000 pyrfuniverse-0.9.20/pyrfuniverse/envs/franka_grasp_env.py
+-rw-rw-rw-   0        0        0     3077 2022-07-08 02:22:23.000000 pyrfuniverse-0.9.20/pyrfuniverse/envs/franka_push_env.py
+drwxrwxrwx   0        0        0        0 2023-08-18 05:30:00.613848 pyrfuniverse-0.9.20/pyrfuniverse/envs/gripper_nail/
+-rw-rw-rw-   0        0        0      736 2022-06-27 07:07:03.000000 pyrfuniverse-0.9.20/pyrfuniverse/envs/gripper_nail/__init__.py
+-rw-rw-rw-   0        0        0     4209 2022-07-08 02:22:23.000000 pyrfuniverse-0.9.20/pyrfuniverse/envs/gripper_nail/nail_can_env.py
+-rw-rw-rw-   0        0        0     5750 2022-07-08 02:22:23.000000 pyrfuniverse-0.9.20/pyrfuniverse/envs/gripper_nail/nail_card_env.py
+-rw-rw-rw-   0        0        0     3917 2022-07-08 02:22:23.000000 pyrfuniverse-0.9.20/pyrfuniverse/envs/gripper_nail/robotiq85_insert_env.py
+-rw-rw-rw-   0        0        0     4149 2022-07-08 02:22:23.000000 pyrfuniverse-0.9.20/pyrfuniverse/envs/gripper_nail/robotiq85_nail_book_env.py
+-rw-rw-rw-   0        0        0     4220 2022-07-08 02:22:23.000000 pyrfuniverse-0.9.20/pyrfuniverse/envs/gripper_nail/robotiq85_nail_can_env.py
+-rw-rw-rw-   0        0        0     5917 2022-07-08 02:22:23.000000 pyrfuniverse-0.9.20/pyrfuniverse/envs/gripper_nail/robotiq85_nail_card_env.py
+-rw-rw-rw-   0        0        0     5696 2022-07-08 02:22:23.000000 pyrfuniverse-0.9.20/pyrfuniverse/envs/gripper_nail/robotiq85_nail_coin_env.py
+-rw-rw-rw-   0        0        0      769 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.20/pyrfuniverse/envs/gym_goal_wrapper_env.py
+-rw-rw-rw-   0        0        0      702 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.20/pyrfuniverse/envs/gym_wrapper_env.py
+drwxrwxrwx   0        0        0        0 2023-08-18 05:30:00.614848 pyrfuniverse-0.9.20/pyrfuniverse/envs/multi_agent/
+-rw-rw-rw-   0        0        0      172 2022-06-27 07:07:03.000000 pyrfuniverse-0.9.20/pyrfuniverse/envs/multi_agent/__init__.py
+-rw-rw-rw-   0        0        0     9111 2023-02-10 17:44:39.000000 pyrfuniverse-0.9.20/pyrfuniverse/envs/multi_agent/cleaner_env.py
+-rw-rw-rw-   0        0        0    11818 2022-07-08 02:22:23.000000 pyrfuniverse-0.9.20/pyrfuniverse/envs/multi_agent/navigation_env.py
+-rw-rw-rw-   0        0        0     6000 2022-07-08 02:22:23.000000 pyrfuniverse-0.9.20/pyrfuniverse/envs/multi_agent_navigation_env.py
+drwxrwxrwx   0        0        0        0 2023-08-18 05:30:00.617865 pyrfuniverse-0.9.20/pyrfuniverse/envs/multi_physics/
+-rw-rw-rw-   0        0        0      871 2023-06-21 09:17:41.000000 pyrfuniverse-0.9.20/pyrfuniverse/envs/multi_physics/__init__.py
+-rw-rw-rw-   0        0        0    13868 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.20/pyrfuniverse/envs/multi_physics/flexiv_cutting.py
+-rw-rw-rw-   0        0        0     8156 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.20/pyrfuniverse/envs/multi_physics/kinova_gen2_catching_cloth_env.py
+-rw-rw-rw-   0        0        0    10075 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.20/pyrfuniverse/envs/multi_physics/ur5_water_shooting.py
+-rw-rw-rw-   0        0        0      513 2022-07-08 02:22:23.000000 pyrfuniverse-0.9.20/pyrfuniverse/envs/rfuniverse_robot_hub_env.py
+drwxrwxrwx   0        0        0        0 2023-08-18 05:30:00.621880 pyrfuniverse-0.9.20/pyrfuniverse/envs/robotics/
+-rw-rw-rw-   0        0        0      675 2022-06-27 07:07:03.000000 pyrfuniverse-0.9.20/pyrfuniverse/envs/robotics/__init__.py
+-rw-rw-rw-   0        0        0     7488 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.20/pyrfuniverse/envs/robotics/franka_cloth_env.py
+-rw-rw-rw-   0        0        0     7679 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.20/pyrfuniverse/envs/robotics/franka_cloth_fold_env.py
+-rw-rw-rw-   0        0        0     9654 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.20/pyrfuniverse/envs/robotics/franka_robotics_env.py
+-rw-rw-rw-   0        0        0     8235 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.20/pyrfuniverse/envs/robotics/franka_softbody_env.py
+-rw-rw-rw-   0        0        0      817 2022-12-15 05:37:19.000000 pyrfuniverse-0.9.20/pyrfuniverse/envs/robotics/pick_and_place_env.py
+-rw-rw-rw-   0        0        0      754 2022-07-08 02:22:23.000000 pyrfuniverse-0.9.20/pyrfuniverse/envs/robotics/push_env.py
+-rw-rw-rw-   0        0        0      864 2022-07-08 02:22:23.000000 pyrfuniverse-0.9.20/pyrfuniverse/envs/robotics/reach_env.py
+-rw-rw-rw-   0        0        0     4463 2022-07-08 02:22:23.000000 pyrfuniverse-0.9.20/pyrfuniverse/envs/roller_env.py
+drwxrwxrwx   0        0        0        0 2023-08-18 05:30:00.622880 pyrfuniverse-0.9.20/pyrfuniverse/envs/tobor_robotics/
+-rw-rw-rw-   0        0        0      121 2022-06-27 07:07:03.000000 pyrfuniverse-0.9.20/pyrfuniverse/envs/tobor_robotics/__init__.py
+-rw-rw-rw-   0        0        0    10897 2022-07-08 02:22:23.000000 pyrfuniverse-0.9.20/pyrfuniverse/envs/tobor_robotics/tobor_push_pull_env.py
+-rw-rw-rw-   0        0        0     8876 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.20/pyrfuniverse/envs/tobor_robotiq85_manipulation_env.py
+-rw-rw-rw-   0        0        0     8205 2022-11-02 03:34:57.000000 pyrfuniverse-0.9.20/pyrfuniverse/envs/ur5_box_env.py
+-rw-rw-rw-   0        0        0     8549 2022-11-02 03:34:57.000000 pyrfuniverse-0.9.20/pyrfuniverse/envs/ur5_drawer_env.py
+drwxrwxrwx   0        0        0        0 2023-08-18 05:30:00.624881 pyrfuniverse-0.9.20/pyrfuniverse/side_channel/
+-rw-rw-rw-   0        0        0      144 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.20/pyrfuniverse/side_channel/__init__.py
+-rw-rw-rw-   0        0        0     3244 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.20/pyrfuniverse/side_channel/incoming_message.py
+-rw-rw-rw-   0        0        0     1536 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.20/pyrfuniverse/side_channel/outgoing_message.py
+drwxrwxrwx   0        0        0        0 2023-08-18 05:30:00.634457 pyrfuniverse-0.9.20/pyrfuniverse/utils/
+-rw-rw-rw-   0        0        0        0 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.20/pyrfuniverse/utils/__init__.py
+-rw-rw-rw-   0        0        0    13620 2023-02-10 17:44:39.000000 pyrfuniverse-0.9.20/pyrfuniverse/utils/active_depth_generate.py
+-rw-rw-rw-   0        0        0     6006 2022-07-13 10:31:45.000000 pyrfuniverse-0.9.20/pyrfuniverse/utils/controller.py
+-rw-rw-rw-   0        0        0    11746 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.20/pyrfuniverse/utils/depth_processor.py
+-rw-rw-rw-   0        0        0     3314 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.20/pyrfuniverse/utils/interpolate_utils.py
+-rw-rw-rw-   0        0        0     4304 2022-06-27 07:07:03.000000 pyrfuniverse-0.9.20/pyrfuniverse/utils/jaco_controller.py
+-rw-rw-rw-   0        0        0     4908 2022-10-27 03:27:48.000000 pyrfuniverse-0.9.20/pyrfuniverse/utils/kinova_controller.py
+-rw-rw-rw-   0        0        0     1027 2023-08-16 08:09:23.000000 pyrfuniverse-0.9.20/pyrfuniverse/utils/locker.py
+-rw-rw-rw-   0        0        0      755 2022-06-27 07:07:03.000000 pyrfuniverse-0.9.20/pyrfuniverse/utils/os_utils.py
+-rw-rw-rw-   0        0        0    10753 2023-08-16 08:09:23.000000 pyrfuniverse-0.9.20/pyrfuniverse/utils/proc_wrapper.py
+-rw-rw-rw-   0        0        0     9993 2023-08-16 08:10:15.000000 pyrfuniverse-0.9.20/pyrfuniverse/utils/rfuniverse_communicator.py
+-rw-rw-rw-   0        0        0     3569 2023-06-21 09:17:41.000000 pyrfuniverse-0.9.20/pyrfuniverse/utils/rfuniverse_utility.py
+-rw-rw-rw-   0        0        0     5690 2022-06-27 07:07:03.000000 pyrfuniverse-0.9.20/pyrfuniverse/utils/stretch_controller.py
+-rw-rw-rw-   0        0        0     6776 2022-08-15 11:02:54.000000 pyrfuniverse-0.9.20/pyrfuniverse/utils/tobor_controller.py
+-rw-rw-rw-   0        0        0     4783 2022-06-27 07:07:03.000000 pyrfuniverse-0.9.20/pyrfuniverse/utils/ur5_controller.py
+drwxrwxrwx   0        0        0        0 2023-08-18 05:30:00.590990 pyrfuniverse-0.9.20/pyrfuniverse.egg-info/
+-rw-rw-rw-   0        0        0      266 2023-08-18 05:30:00.000000 pyrfuniverse-0.9.20/pyrfuniverse.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4172 2023-08-18 05:30:00.000000 pyrfuniverse-0.9.20/pyrfuniverse.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-18 05:30:00.000000 pyrfuniverse-0.9.20/pyrfuniverse.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-08-15 08:29:49.000000 pyrfuniverse-0.9.20/pyrfuniverse.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       36 2023-08-18 05:30:00.000000 pyrfuniverse-0.9.20/pyrfuniverse.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-08-18 05:30:00.000000 pyrfuniverse-0.9.20/pyrfuniverse.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-18 05:30:00.657776 pyrfuniverse-0.9.20/setup.cfg
+-rw-rw-rw-   0        0        0      601 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.20/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-18 05:30:00.656776 pyrfuniverse-0.9.20/test/
+-rw-rw-rw-   0        0        0     5924 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.20/test/test_active_depth.py
+-rw-rw-rw-   0        0        0      995 2023-04-06 04:45:20.000000 pyrfuniverse-0.9.20/test/test_articulation_ik.py
+-rw-rw-rw-   0        0        0      999 2023-08-17 09:04:55.000000 pyrfuniverse-0.9.20/test/test_camera_image.py
+-rw-rw-rw-   0        0        0     1939 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.20/test/test_custom_message.py
+-rw-rw-rw-   0        0        0     1038 2023-08-11 09:23:49.000000 pyrfuniverse-0.9.20/test/test_debug.py
+-rw-rw-rw-   0        0        0      439 2023-04-07 05:04:11.000000 pyrfuniverse-0.9.20/test/test_digit.py
+-rw-rw-rw-   0        0        0      827 2023-04-06 04:45:20.000000 pyrfuniverse-0.9.20/test/test_grasp_pose.py
+-rw-rw-rw-   0        0        0     2750 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.20/test/test_grasp_sim.py
+-rw-rw-rw-   0        0        0      989 2023-04-10 09:39:27.000000 pyrfuniverse-0.9.20/test/test_heat_map.py
+-rw-rw-rw-   0        0        0     1426 2023-04-06 04:45:20.000000 pyrfuniverse-0.9.20/test/test_humanbody_ik.py
+-rw-rw-rw-   0        0        0     1087 2023-08-16 08:09:10.000000 pyrfuniverse-0.9.20/test/test_image_stream.py
+-rw-rw-rw-   0        0        0     1984 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.20/test/test_label.py
+-rw-rw-rw-   0        0        0      702 2023-04-06 04:45:20.000000 pyrfuniverse-0.9.20/test/test_light.py
+-rw-rw-rw-   0        0        0      589 2023-06-13 10:33:21.000000 pyrfuniverse-0.9.20/test/test_load_mesh.py
+-rw-rw-rw-   0        0        0     1008 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.20/test/test_load_urdf.py
+-rw-rw-rw-   0        0        0      410 2023-08-18 02:22:24.000000 pyrfuniverse-0.9.20/test/test_load_urdf_akb.py
+-rw-rw-rw-   0        0        0     1980 2023-07-13 08:59:36.000000 pyrfuniverse-0.9.20/test/test_object_data.py
+-rw-rw-rw-   0        0        0     1646 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.20/test/test_ompl.py
+-rw-rw-rw-   0        0        0     2169 2023-08-18 03:01:55.000000 pyrfuniverse-0.9.20/test/test_pick_and_place.py
+-rw-rw-rw-   0        0        0     2171 2023-08-17 08:20:43.000000 pyrfuniverse-0.9.20/test/test_pick_and_place_flexiv.py
+-rw-rw-rw-   0        0        0      476 2023-08-18 03:02:53.000000 pyrfuniverse-0.9.20/test/test_ply_render.py
+-rw-rw-rw-   0        0        0     1658 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.20/test/test_point_cloud.py
+-rw-rw-rw-   0        0        0     1830 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.20/test/test_point_cloud_with_intrinsic_matrix.py
+-rw-rw-rw-   0        0        0      659 2023-04-13 02:37:33.000000 pyrfuniverse-0.9.20/test/test_save_gripper.py
+-rw-rw-rw-   0        0        0      378 2023-07-03 04:58:35.000000 pyrfuniverse-0.9.20/test/test_save_obj.py
+-rw-rw-rw-   0        0        0     1024 2023-04-06 04:45:20.000000 pyrfuniverse-0.9.20/test/test_scene.py
+-rw-rw-rw-   0        0        0      740 2023-04-07 07:58:17.000000 pyrfuniverse-0.9.20/test/test_tobor_move.py
+-rw-rw-rw-   0        0        0      279 2023-08-17 08:31:27.000000 pyrfuniverse-0.9.20/test/test_urdf_parameter.py
```

### Comparing `pyrfuniverse-0.9.13/LICENSE` & `pyrfuniverse-0.9.20/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.13/README.md` & `pyrfuniverse-0.9.20/README.md`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.13/pyrfuniverse/__init__.py` & `pyrfuniverse-0.9.20/pyrfuniverse/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 # Version of the library that will be used to upload to pypi
-__version__ = "0.9.13"
+__version__ = "0.9.20"
 
 import os.path
 import json
+from pyrfuniverse.utils.locker import Locker
 
 def read_config():
     if not os.path.exists(config_path):
+        print('creating config')
         config = {}
         config['assets_path'] = ''
         config['executable_file'] = ''
         with open(config_path, 'w', encoding='utf-8') as file:
             json.dump(config, file, indent=True)
     with open(config_path, 'r', encoding='utf-8') as file:
         return json.load(file)
 
 
 user_path = os.path.expanduser('~/.rfuniverse')
 if not os.path.exists(user_path):
     os.makedirs(user_path)
 config_path = os.path.join(user_path, 'config.json')
-config = read_config()
+with Locker('config'):
+    config = read_config()
 assets_path = config['assets_path']
-executable_file = config['executable_file']
+executable_file = config['executable_file']
```

### Comparing `pyrfuniverse-0.9.13/pyrfuniverse/attributes/__init__.py` & `pyrfuniverse-0.9.20/pyrfuniverse/attributes/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.13/pyrfuniverse/attributes/activelightsensor_attr.py` & `pyrfuniverse-0.9.20/pyrfuniverse/attributes/activelightsensor_attr.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.13/pyrfuniverse/attributes/base_attr.py` & `pyrfuniverse-0.9.20/pyrfuniverse/attributes/base_attr.py`

 * *Files 3% similar despite different names*

```diff
@@ -151,22 +151,24 @@
             is_world: Bool, True for world coordinate, False for local coordinate.
         """
         assert len(rotation) == 3, 'rotation length must be 3'
         rotation = [float(i) for i in rotation]
 
         self._send_data('Rotate', rotation, is_world)
 
-    def LookAt(self, target: list, world_up: list):
+    def LookAt(self, target: list, world_up: list = None):
         """
         Rotates the transform so the forward vector points at target's current position.
 
         Args:
             target: A list of length 3, target to point towards.
             world_up: A list of length 3, vector specifying the upward direction.
         """
+        if world_up is None:
+            world_up = [0., 1., 0.]
         assert len(target) == 3, 'target length must be 3'
         target = [float(i) for i in target]
         assert len(world_up) == 3, 'world_up length must be 3'
         world_up = [float(i) for i in world_up]
 
         self._send_data('LookAt', target, world_up)
 
@@ -214,23 +216,14 @@
         """
         Destroy this object in Unity.
         """
         self._send_data('Destroy')
 
         self.env.attrs.pop(self.id)
 
-    def SetRFMoveColliderActive(self, active: bool):
-        """
-        Set the collider active or inactive in RFMove.
-
-        Args:
-            active: Bool, True for active and False for inactive.
-        """
-        self._send_data('SetRFMoveColliderActive', active)
-
     def GetLocalPointFromWorld(self, point: list):
         """
         Transform a point from local coordinate to world coordinate. After calling this method and stepping once, the result will be saved in self.data['result_local_point']
 
         Args:
             point: A list of length 3, representing the position of a point.
         """
```

### Comparing `pyrfuniverse-0.9.13/pyrfuniverse/attributes/camera_attr.py` & `pyrfuniverse-0.9.20/pyrfuniverse/attributes/camera_attr.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.13/pyrfuniverse/attributes/collider_attr.py` & `pyrfuniverse-0.9.20/pyrfuniverse/attributes/digit_attr.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 import pyrfuniverse.attributes as attr
 
 
-class ColliderAttr(attr.GameObjectAttr):
+class DigitAttr(attr.BaseAttr):
     """
-    Collider class for objects who have collider in Unity.
+    Class for simulating DIGIT tactile sensor.
     """
     def parse_message(self, data: dict):
         """
         Parse messages. This function is called by internal function.
 
         Returns:
             Dict: A dict containing useful information of this class.
+
+            self.data['light']: Bytes of RGB light image in DIGIT.
+
+            self.data['depth']: Bytes of depth image in DIGIT.
         """
         super().parse_message(data)
 
-    def GenerateVHACDColider(self):
+    def GetData(self):
         """
-        Generate convex colliders using VHACD algorithm.
+        Get data from DIGIT in RFUniverse.
+
         """
-        self._send_data('GenerateVHACDColider')
+        self._send_data('GetData')
```

### Comparing `pyrfuniverse-0.9.13/pyrfuniverse/attributes/controller_attr.py` & `pyrfuniverse-0.9.20/pyrfuniverse/attributes/controller_attr.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,16 @@
         """
         Set the target joint position for each moveable joint and move with PD control continuously.
 
         Args:
             interval: Float, the time interval.
             time_joint_positions: A list of float list, representing the target joint positions at each time step.
         """
-        time_joint_positions = [float(i) for i in time_joint_positions]
+        for i in range(len(time_joint_positions)):
+            time_joint_positions[i] = [float(j) for j in time_joint_positions[i]]
         self._send_data('SetJointPositionContinue', interval, time_joint_positions)
 
     def SetJointVelocity(self, joint_velocitys: list):
         """
         Set the target joint velocity for each moveable joint.
 
         Args:
```

### Comparing `pyrfuniverse-0.9.13/pyrfuniverse/attributes/custom_attr.py` & `pyrfuniverse-0.9.20/pyrfuniverse/attributes/custom_attr.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.13/pyrfuniverse/attributes/fallingcloth_attr.py` & `pyrfuniverse-0.9.20/pyrfuniverse/attributes/fallingcloth_attr.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.13/pyrfuniverse/attributes/gameobject_attr.py` & `pyrfuniverse-0.9.20/pyrfuniverse/attributes/gameobject_attr.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.13/pyrfuniverse/attributes/graspsim_attr.py` & `pyrfuniverse-0.9.20/pyrfuniverse/attributes/graspsim_attr.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.13/pyrfuniverse/attributes/humanbody_attr.py` & `pyrfuniverse-0.9.20/pyrfuniverse/attributes/humanbody_attr.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.13/pyrfuniverse/attributes/light_attr.py` & `pyrfuniverse-0.9.20/pyrfuniverse/attributes/light_attr.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.13/pyrfuniverse/attributes/omplmanager_attr.py` & `pyrfuniverse-0.9.20/pyrfuniverse/attributes/omplmanager_attr.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.13/pyrfuniverse/attributes/pointcloud_attr.py` & `pyrfuniverse-0.9.20/pyrfuniverse/attributes/pointcloud_attr.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.13/pyrfuniverse/attributes/rigidbody_attr.py` & `pyrfuniverse-0.9.20/pyrfuniverse/attributes/rigidbody_attr.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.13/pyrfuniverse/envs/__init__.py` & `pyrfuniverse-0.9.20/pyrfuniverse/envs/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.13/pyrfuniverse/envs/balance_ball_env.py` & `pyrfuniverse-0.9.20/pyrfuniverse/envs/balance_ball_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.13/pyrfuniverse/envs/base_env.py` & `pyrfuniverse-0.9.20/pyrfuniverse/envs/base_env.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,68 +2,85 @@
 import subprocess
 from abc import ABC
 import socket
 import numpy as np
 import pyrfuniverse
 import pyrfuniverse.attributes as attr
 from pyrfuniverse.side_channel import IncomingMessage, OutgoingMessage
+from pyrfuniverse.utils.locker import Locker
 from pyrfuniverse.utils.rfuniverse_communicator import RFUniverseCommunicator
 import os
 
 
 class RFUniverseBaseEnv(ABC):
     """
     RFUniverse base environment class.
 
     Args:
         executable_file: Str, the absolute path of Unity executable file. None for last used executable file; "@editor" for using Unity Editor.
         scene_file: Str, the absolute path of Unity scene JSON file. All JSON files locate at `StraemingAssets/SceneData` by default.
         assets: List, the list of pre-load assets. All assets in the list will be pre-loaded in Unity when the environment is initialized, which will save time during instanciating.
         graphics: Bool, True for showing GUI and False for headless mode.
     """
-    metadata = {'render.modes': ['human', 'rgb_array']}
+
+    metadata = {"render.modes": ["human", "rgb_array"]}
 
     def __init__(
         self,
         executable_file: str = None,
         scene_file: str = None,
         assets: list = [],
         graphics: bool = True,
-        port: int = 5004
+        port: int = 5004,
+        proc_id=0,
+        log_level=1,
     ):
         # time step
         self.t = 0
         self.executable_file = executable_file
         self.scene_file = scene_file
         self.pre_load_assets = assets
         self.graphics = graphics
-
+        self.process = None
         self.attrs = {}
         self.data = {}
         self.listen_messages = {}
         self.listen_object = {}
         self.port = port
 
-        self.log_level = 1
-        self.log_map = {'Log': 3, 'Warning': 2, 'Error': 1, 'Exception': 1, 'Assert': 1}
+        self.log_level = log_level
+
+        self.log_map = {"Log": 3, "Warning": 2, "Error": 1, "Exception": 1, "Assert": 1}
 
         if self.executable_file is None:
             self.executable_file = pyrfuniverse.executable_file
 
-        if self.executable_file == '' or self.executable_file == '@editor':
-            print('Waiting for UnityEditor play...')
-            self.process = None
-        elif os.path.exists(self.executable_file):
-            self.port = self._get_port()
-            self.process = self._start_unity_env(self.executable_file, self.port)
-        else:
-            raise Exception('Executable file not exists')
-        self.communicator = RFUniverseCommunicator(port=self.port,
-                                                   receive_data_callback=self._receive_data)
-        self._send_debug_data('SetPythonVersion', pyrfuniverse.__version__)
+        PROC_TYPE = ""  # editor or release
+        if self.executable_file == "" or self.executable_file == "@editor":  # editor
+            assert proc_id == 0, "proc_id must be 0 when using editor"
+            print("Waiting for UnityEditor play...")
+            PROC_TYPE = "editor"
+            self.port = 5004
+        elif os.path.exists(self.executable_file):  # release
+            PROC_TYPE = "release"
+            self.port = 5005 + proc_id  # default release port
+        else:  # error
+            raise ValueError(f"Executable file {self.executable_file} not exists")
+
+        self.communicator = RFUniverseCommunicator(
+            port=self.port,
+            receive_data_callback=self._receive_data,
+            proc_type=PROC_TYPE,
+        )
+        self.port = self.communicator.port  # update port
+        if PROC_TYPE == "release":
+            with Locker('config'): # unity process will try to modify the config file
+                self.process = self._start_unity_env(self.executable_file, self.port)
+        self.communicator.online()
+        self._send_debug_data("SetPythonVersion", pyrfuniverse.__version__)
         if len(self.pre_load_assets) > 0:
             self.PreLoadAssetsAsync(assets, True)
         if self.scene_file is not None:
             self.LoadSceneAsync(self.scene_file, True)
 
     def _get_port(self) -> int:
         executable_port = 5005
@@ -77,69 +94,79 @@
                 executable_port += 1
                 continue
 
     def _start_unity_env(self, executable_file: str, port: int) -> subprocess.Popen:
         arg = [executable_file]
         if not self.graphics:
             arg.extend(["-nographics", "-batchmode"])
-        arg.append(f'-port:{port}')
-        return subprocess.Popen(arg)
+        if self.log_level == 0:
+            proc_out = subprocess.DEVNULL
+        else:
+            proc_out = None
+        arg.append(f"-port:{port}")
+        return subprocess.Popen(arg, stdout=proc_out, stderr=proc_out)
 
     def _receive_data(self, objs: list) -> None:
         msg = objs[0]
         objs = objs[1:]
-        if msg == 'Env':
+        if msg == "Env":
             self._parse_env_data(objs)
-        elif msg == 'Instance':
+        elif msg == "Instance":
             self._parse_instence_data(objs)
-        elif msg == 'Debug':
+        elif msg == "Debug":
             self._parse_debug_data(objs)
-        elif msg == 'Message':
+        elif msg == "Message":
             self._parse_message_data(objs)
-        elif msg == 'Object':
+        elif msg == "Object":
             self._parse_object_data(objs)
         return
 
     def _parse_env_data(self, objs: list) -> None:
         msg = objs[0]
         objs = objs[1:]
-        if msg == 'Close':
+        if msg == "Close":
             self.close()
-        elif msg == 'LoadDone':
-            self.data['load_done'] = True
-        elif msg == 'PendDone':
-            self.data['pend_done'] = True
-        elif msg == 'RFMoveColliders':
-            self.data['colliders'] = objs[0]
-        elif msg == 'CurrentCollisionPairs':
-            self.data['collision_pairs'] = objs[0]
+        elif msg == "LoadDone":
+            self.data["load_done"] = True
+        elif msg == "PendDone":
+            self.data["pend_done"] = True
+        elif msg == "RFMoveColliders":
+            self.data["colliders"] = objs[0]
+        elif msg == "CurrentCollisionPairs":
+            self.data["collision_pairs"] = objs[0]
         else:
-            print(f'unknown env data type: {msg}')
+            print(f"unknown env data type: {msg}")
 
     def _parse_instence_data(self, objs: list) -> None:
         this_object_id = objs[0]
         this_object_type = objs[1]
         this_object_data = objs[2]
 
-        attr_type = eval('attr.' + this_object_type)
+        attr_type = eval("attr." + this_object_type)
         if this_object_id not in self.attrs:
             self.attrs[this_object_id] = attr_type(self, this_object_id)
         elif type(self.attrs[this_object_id]) != attr_type:
-            self.attrs[this_object_id] = attr_type(self, this_object_id, self.attrs[this_object_id].data)
-
-        self.data[this_object_id] = self.attrs[this_object_id].parse_message(this_object_data)
+            self.attrs[this_object_id] = attr_type(
+                self, this_object_id, self.attrs[this_object_id].data
+            )
+
+        self.data[this_object_id] = self.attrs[this_object_id].parse_message(
+            this_object_data
+        )
 
     def _parse_debug_data(self, objs: list) -> None:
         msg = objs[0]
         objs = objs[1:]
-        if msg == 'Log':
+        if msg == "Log":
             if self.log_map[objs[0]] <= self.log_level:
-                print(f'Unity Env Log Type:{objs[0]}\nCondition:{objs[1]}\nStackTrace:{objs[2]}')
+                print(
+                    f"Unity Env Log Type:{objs[0]}\nCondition:{objs[1]}\nStackTrace:{objs[2]}"
+                )
         else:
-            print(f'unknown debug data type: {msg}')
+            print(f"unknown debug data type: {msg}")
         return
 
     def _parse_message_data(self, objs: list) -> None:
         msg = objs[0]
         objs = objs[1:]
         if msg in self.listen_messages:
             self.listen_messages[msg](IncomingMessage(objs[0]))
@@ -147,34 +174,34 @@
     def _parse_object_data(self, objs: list) -> None:
         head = objs[0]
         objs = objs[1:]
         if head in self.listen_object:
             self.listen_object[head](objs)
 
     def _send_env_data(self, *args) -> None:
-        self.communicator.send_object('Env', *args)
+        self.communicator.send_object("Env", *args)
 
     def _send_instance_data(self, *args) -> None:
-        self.communicator.send_object('Instance', *args)
+        self.communicator.send_object("Instance", *args)
 
     def _send_debug_data(self, *args) -> None:
-        self.communicator.send_object('Debug', *args)
+        self.communicator.send_object("Debug", *args)
 
     def _send_message_data(self, *args) -> None:
-        self.communicator.send_object('Message', *args)
+        self.communicator.send_object("Message", *args)
 
     def _send_object_data(self, *args) -> None:
-        self.communicator.send_object('Object', *args)
+        self.communicator.send_object("Object", *args)
 
     def _step(self):
         """
         Send the messages of called functions to Unity and simulate for a step, then accept the data from Unity.
         """
         if not self.communicator.connected:
-            raise Exception('Unity Env not connected')
+            raise Exception("Unity Env not connected")
         self.communicator.sync_step()
 
     def step(self, count: int = 1):
         """
         Send the messages of called functions to Unity and simulate for a step, then accept the data from Unity.
 
         Args:
@@ -200,73 +227,73 @@
 
         Args:
             id: Int, object id.
 
         Returns:
             pyrfuniverse.attributes.BaseAttr: An instance of attribute.
         """
-        assert id in self.attrs, 'this ID not exists'
+        assert id in self.attrs, "this ID not exists"
         return self.attrs[id]
 
-    #Env API
+    # Env API
     def PreLoadAssetsAsync(self, names: list, auto_wait: bool = False) -> None:
         """
         PreLoad the asset.
 
         Args:
             names: list, the name of assets.
             auto_wait: Bool, if True, this function will not return until the loading is done.
         """
-        self._send_env_data('PreLoadAssetsAsync', names)
+        self._send_env_data("PreLoadAssetsAsync", names)
 
         if auto_wait:
             self.WaitLoadDone()
 
     def LoadSceneAsync(self, file: str, auto_wait: bool = False) -> None:
         """
         Load the scene asynchronisely.
 
         Args:
             file: Str, the scene JSON file. If it's a relative path, it will load from `StraemingAssets`.
             auto_wait: Bool, if True, this function will not return until the loading is done.
         """
-        self._send_env_data('LoadSceneAsync', file)
+        self._send_env_data("LoadSceneAsync", file)
 
         if auto_wait:
             self.WaitLoadDone()
 
     def SwitchSceneAsync(self, name: str, auto_wait: bool = False) -> None:
         """
         Switch the scene asynchronisely.
 
         Args:
             name: Str, the scene name.
             auto_wait: Bool, if True, this function will not return until the loading is done.
         """
-        self._send_env_data('SwitchSceneAsync', name)
+        self._send_env_data("SwitchSceneAsync", name)
 
         if auto_wait:
             self.WaitLoadDone()
 
     def WaitLoadDone(self) -> None:
         """
         Wait for the loading is done.
         """
-        self.data['load_done'] = False
-        while not self.data['load_done']:
+        self.data["load_done"] = False
+        while not self.data["load_done"]:
             self._step()
 
     def Pend(self) -> None:
         """
         Pend the program until the `EndPend` button in `UnityPlayer` is clicked.
         """
-        self._send_env_data('Pend')
+        self._send_env_data("Pend")
 
-        self.data['pend_done'] = False
-        while not self.data['pend_done']:
+        self.data["pend_done"] = False
+        while not self.data["pend_done"]:
             self._step()
 
     def SendMessage(self, message: str, *args) -> None:
         """
         Send message to Unity.
 
         Args:
@@ -282,15 +309,15 @@
             elif type(i) == int:
                 msg.write_int32(i)
             elif type(i) == float or type(i) == np.float32 or type(i) == np.float64:
                 msg.write_float32(float(i))
             elif type(i) == list and type(i[0]) == float:
                 msg.write_float32_list(i)
             else:
-                print(f'dont support this data type:{type(i)}')
+                print(f"dont support this data type:{type(i)}")
         self._send_message_data(message, msg.buffer)
 
     def SendObject(self, head: str, *args) -> None:
         """
         Send object to Unity.
 
         Args:
@@ -334,20 +361,22 @@
         Remove object listener.
 
         Args:
             type: Str, the message head.
         """
         self.listen_object.pop(type)
 
-    def InstanceObject(self, name: str, id: int = None, attr_type: type = attr.BaseAttr):
+    def InstanceObject(
+        self, name: str, id: int = None, attr_type: type = attr.BaseAttr
+    ):
         """
         Instanciate an object.
 
         Built-in assets:
-    
+
         GameObjectAttr:
             Basic Objects:
                 "GameObject_Box",
                 "GameObject_Capsule",
                 "GameObject_Cylinder",
                 "GameObject_Sphere",
                 "GameObject_Quad",
@@ -375,15 +404,15 @@
 
         RigidbodyAttr:
             Basic Objects:
                 "Rigidbody_Box",
                 "GameObject_Capsule",
                 "Rigidbody_Cylinder",
                 "Rigidbody_Sphere",
-            YCB dataset: 
+            YCB dataset:
                 77 models in YCB dataset. See YCB Object and Model Set for detail: https://rse-lab.cs.washington.edu/projects/posecnn/
 
         ControllerAttr:
             gripper:
                 "allegro_hand_right",
                 "bhand",
                 "svh",
@@ -411,44 +440,45 @@
             name: Str, object name. Please check the above `built-in assets` list for names.
             id: Int, object id.
             attr_type: type(pyrfuniverse.attributes.BaseAttr), the attribute type.
 
         Returns:
             type(`attr_type`): The object attribute instance.
         """
-        assert id not in self.attrs, \
-            'this ID exists'
+        assert id not in self.attrs, "this ID exists"
 
         while id is None or id in self.attrs:
             id = random.randint(100000, 999999)
 
-        self._send_env_data('InstanceObject', name, id)
+        self._send_env_data("InstanceObject", name, id)
 
         self.attrs[id] = attr_type(self, id)
         return self.attrs[id]
 
-    def LoadURDF(self, path: str, id: int = None, native_ik: bool = False, axis: str = 'y') -> attr.ControllerAttr:
+    def LoadURDF(
+        self, path: str, id: int = None, native_ik: bool = False, axis: str = "y"
+    ) -> attr.ControllerAttr:
         """
         Load a model from URDF file.
 
         Args:
             path: Str, the URDF file path.
             id: Int, object id.
             native_ik: Bool, True for enabling native IK; False for using custom IK.When it is True, through the IKTargetDo*** interface, according to the end pose.When it is False, through the SetJoint*** interface, according to the joint movement.
             axis: Str, import axis, This can be 'z' or 'y', depending on the URDF file
 
         Returns:
             pyrfuniverse.attributes.ControllerAttr: The object attribute intance.
         """
-        assert id not in self.attrs, 'this ID exists'
+        assert id not in self.attrs, "this ID exists"
 
         while id is None or id in self.attrs:
             id = random.randint(100000, 999999)
 
-        self._send_env_data('LoadURDF', id, path, native_ik, axis)
+        self._send_env_data("LoadURDF", id, path, native_ik, axis)
 
         self.attrs[id] = attr.ControllerAttr(self, id)
         return self.attrs[id]
 
     def LoadMesh(self, path: str, id: int = None) -> attr.RigidbodyAttr:
         """
         Load a model from Mesh file.
@@ -456,260 +486,299 @@
         Args:
             path: Str, the Mesh file path.
             id: Int, object id.
 
         Returns:
             pyrfuniverse.attributes.RigidbodyAttr: The object attribute intance.
         """
-        assert id not in self.attrs, \
-            'this ID exists'
+        assert id not in self.attrs, "this ID exists"
 
         while id is None or id in self.attrs:
             id = random.randint(100000, 999999)
 
-        self._send_env_data('LoadMesh', id, path)
+        self._send_env_data("LoadMesh", id, path)
 
         self.attrs[id] = attr.RigidbodyAttr(self, id)
         return self.attrs[id]
 
     def IgnoreLayerCollision(self, layer1: int, layer2: int, ignore: bool) -> None:
         """
         Ignore or enable the collision between two layers.
 
         Args:
             layer1: Int, the layer number of the first layer.
             layer2: Int, the layer number of the second layer.
             ignore: Bool, True for ignoring collision between two layers; False for enabling collision between two layers.
         """
-        self._send_env_data('IgnoreLayerCollision', layer1, layer2, ignore)
+        self._send_env_data("IgnoreLayerCollision", layer1, layer2, ignore)
 
     def GetCurrentCollisionPairs(self) -> None:
         """
         Get the collision pairs of current collision. After calling this method and stepping once, the result will be saved in env.data['CurrentCollisionPairs']
         """
-        self._send_env_data('GetCurrentCollisionPairs')
+        self._send_env_data("GetCurrentCollisionPairs")
 
     def GetRFMoveColliders(self) -> None:
         """
         Get the RFMove colliders. After calling this method and stepping once, the result will be saved in env.data['RFMoveColliders']
         """
-        self._send_env_data('GetRFMoveColliders')
+        self._send_env_data("GetRFMoveColliders")
 
     def SetGravity(self, x: float, y: float, z: float) -> None:
         """
         Set the gravity of environment.
 
         Args:
             x: Float, gravity on global x-axis (right).
             y: Float, gravity on global y-axis (up).
             z: Float, gravity on global z-axis (forward).
         """
-        self._send_env_data('SetGravity', [float(x), float(y), float(z)])
+        self._send_env_data("SetGravity", [float(x), float(y), float(z)])
 
     def SetGroundActive(self, active: bool) -> None:
         """
         Set the ground active or inactive.
 
         Args:
             active: Bool, active or inactive the ground.
         """
-        self._send_env_data('GetRFMoveColliders', active)
+        self._send_env_data("GetRFMoveColliders", active)
 
-    def SetGroundPhysicMaterial(self, bounciness: float, dynamic_friction: float, static_friction: float, friction_combine: int, bounce_combine: int) -> None:
+    def SetGroundPhysicMaterial(
+        self,
+        bounciness: float,
+        dynamic_friction: float,
+        static_friction: float,
+        friction_combine: int,
+        bounce_combine: int,
+    ) -> None:
         """
         Set the physics material of ground in environment.
 
         Args:
             bounciness: Float, the bounciness.
             dynamic_friction: Float, the dynamic friction coefficient (0-1).
             static_friction: Float, the static friction coefficient (0-1).
             friction_combine: Int, how friction of two colliding objects is combined. 0 for Average, 1 for Minimum, 2 for Maximum and 3 for Multiply. See https://docs.unity3d.com/Manual/class-PhysicMaterial.html for more details.
             bounce_combine: Int, how bounciness of two colliding objects is combined. The value representation is the same with `friction_combine`.
         """
-        self._send_env_data('SetGroundPhysicMaterial', float(bounciness), float(dynamic_friction), float(static_friction), friction_combine, bounce_combine)
+        self._send_env_data(
+            "SetGroundPhysicMaterial",
+            float(bounciness),
+            float(dynamic_friction),
+            float(static_friction),
+            friction_combine,
+            bounce_combine,
+        )
 
     def SetTimeStep(self, delta_time: float) -> None:
         """
         Set the time for a step in Unity.
 
         Args:
             delta_time: Float, the time for a step in Unity.
         """
-        self._send_env_data('SetTimeStep', float(delta_time))
+        self._send_env_data("SetTimeStep", float(delta_time))
 
     def SetTimeScale(self, time_scale: float) -> None:
         """
         Set the time scale in Unity.
 
         Args:
             time_scale: Float, the time scale in Unity.
         """
-        self._send_env_data('SetTimeScale', float(time_scale))
+        self._send_env_data("SetTimeScale", float(time_scale))
 
     def SetResolution(self, resolution_x: int, resolution_y: int) -> None:
         """
         Set the resolution of windowed GUI.
 
         Args:
             resolution_x: Int, window width.
             resolution_y: Int, window height.
         """
-        self._send_env_data('SetResolution', resolution_x, resolution_y)
+        self._send_env_data("SetResolution", resolution_x, resolution_y)
 
     def ExportOBJ(self, items_id: list, save_path: str) -> None:
         """
         Export the specified object list to OBJ file. For native bundle models, the `Read/Write` must be checked in Unity Editor.
 
         Args:
             items_id: List, the object ids.
             save_path: Str, the path to save the OBJ files.
         """
-        self._send_env_data('ExportOBJ', items_id, save_path)
+        self._send_env_data("ExportOBJ", items_id, save_path)
 
     def SetShadowDistance(self, distance: float) -> None:
         """
         Set the shadow distance for rendering in environment.
 
         Args:
             distance: Float, the shadow distance measured in meter.
         """
-        self._send_env_data('SetShadowDistance', float(distance))
+        self._send_env_data("SetShadowDistance", float(distance))
 
     def SaveScene(self, file: str) -> None:
         """
         Save current scene.
 
         Args:
             file: Str, the file path to save current scene. Default saving to `StreamingAssets` folder.
         """
-        self._send_env_data('SaveScene', file)
+        self._send_env_data("SaveScene", file)
 
     def ClearScene(self) -> None:
         """
         Clear current scene.
         """
-        self._send_env_data('ClearScene')
+        self._send_env_data("ClearScene")
 
     def AlignCamera(self, camera_id: int) -> None:
         """
         Align current GUI view to a given camera.
 
         Args:
             camera_id: Int, camera id.
         """
-        self._send_env_data('AlignCamera', camera_id)
+        self._send_env_data("AlignCamera", camera_id)
 
     def SetViewTransform(self, position: list = None, rotation: list = None) -> None:
         """
         Set the GUI view.
 
         Args:
             position: A list of length 3, representing the position of GUI view.
             rotation: A list of length 3, representing the rotation of GUI view.
         """
         if position is not None:
-            assert type(position) == list and len(position) == 3, \
-                'Argument position must be a 3-d list.'
+            assert (
+                type(position) == list and len(position) == 3
+            ), "Argument position must be a 3-d list."
             position = [float(i) for i in position]
         if rotation is not None:
-            assert type(rotation) == list and len(rotation) == 3, \
-                'Argument rotation must be a 3-d list.'
+            assert (
+                type(rotation) == list and len(rotation) == 3
+            ), "Argument rotation must be a 3-d list."
             rotation = [float(i) for i in rotation]
 
-        self._send_env_data('SetViewTransform', position, rotation)
+        self._send_env_data("SetViewTransform", position, rotation)
+
+    def ViewLookAt(self, target: list, world_up: list = None) -> None:
+        """
+        Rotates the transform so the forward vector points at target's current position.
+
+        Args:
+            target: A list of length 3, target to point towards.
+            world_up: A list of length 3, vector specifying the upward direction.
+        """
+        if world_up is None:
+            world_up = [0., 1., 0.]
+        assert len(target) == 3, 'target length must be 3'
+        target = [float(i) for i in target]
+        assert len(world_up) == 3, 'world_up length must be 3'
+        world_up = [float(i) for i in world_up]
+
+        self._send_env_data('ViewLookAt', target, world_up)
 
     def SetViewBackGround(self, color: list = None) -> None:
         """
         Set the GUI view.
 
         Args:
             color: A list of length 3, background color of GUI view. None : default skybox.
         """
         if color is not None:
-            assert type(color) == list and len(color) == 3, 'color length must be 3'
+            assert type(color) == list and len(color) == 3, "color length must be 3"
             color = [float(i) for i in color]
 
-        self._send_env_data('SetViewBackGround', color)
-
+        self._send_env_data("SetViewBackGround", color)
 
-    #Dubug API
+    # Dubug API
     def DebugGraspPoint(self, enabled: bool = True) -> None:
         """
         Show or hide end effector of robot arm for debug.
 
         Args:
             enabled: Bool, True for showing and False for hiding.
         """
-        self._send_debug_data('DebugGraspPoint', enabled)
+        self._send_debug_data("DebugGraspPoint", enabled)
 
     def DebugObjectPose(self, enabled: bool = True) -> None:
         """
         Show or hide object base point for debug.
 
         Args:
             enabled: Bool, True for showing and False for hiding.
         """
-        self._send_debug_data('DebugObjectPose', enabled)
+        self._send_debug_data("DebugObjectPose", enabled)
 
     def DebugCollisionPair(self, enabled: bool = True) -> None:
         """
         Show or hide collision pairs for debug.
 
         Args:
             enabled: Bool, True for showing and False for hiding.
         """
-        self._send_debug_data('DebugCollisionPair', enabled)
-    
+        self._send_debug_data("DebugCollisionPair", enabled)
+
     def DebugColliderBound(self, enabled: bool = True) -> None:
         """
         Show or hide collider bounding box for debug.
 
         Args:
             enabled: Bool, True for showing and False for hiding.
         """
-        self._send_debug_data('DebugColliderBound', enabled)
+        self._send_debug_data("DebugColliderBound", enabled)
 
     def DebugObjectID(self, enabled: bool = True) -> None:
         """
         Show or hide object id for debug.
 
         Args:
             enabled: Bool, True for showing and False for hiding.
         """
-        self._send_debug_data('DebugObjectID', enabled)
+        self._send_debug_data("DebugObjectID", enabled)
 
     def Debug3DBBox(self, enabled: bool = True) -> None:
         """
         Show or hide 3d bounding box of objects for debug.
 
         Args:
             enabled: Bool, True for showing and False for hiding.
         """
-        self._send_debug_data('Debug3DBBox', enabled)
+        self._send_debug_data("Debug3DBBox", enabled)
 
     def Debug2DBBox(self, enabled: bool = True) -> None:
         """
         Show or hide 2d bounding box of objects for debug.
 
         Args:
             enabled: Bool, True for showing and False for hiding.
         """
-        self._send_debug_data('Debug2DBBox', enabled)
+        self._send_debug_data("Debug2DBBox", enabled)
 
     def DebugJointLink(self, enabled: bool = True) -> None:
         """
         Show or hide joint information of articulation for debug.
 
         Args:
             enabled: Bool, True for showing and False for hiding.
         """
-        self._send_debug_data('DebugJointLink', enabled)
+        self._send_debug_data("DebugJointLink", enabled)
 
     def SendLog(self, log: str) -> None:
         """
         Send log messange and show it on Unity GUI window.
 
         Args:
             log: Str, log message.
         """
-        self._send_debug_data('SendLog', log)
+        self._send_debug_data("SendLog", log)
+
+    def ShowArticulationParameter(self, controller_id: int) -> None:
+        """
+        Show Articulation Parameter on Unity GUI window.
 
+        Args:
+            controller_id: int, controller_attr id.
+        """
+        self._send_debug_data("ShowArticulationParameter", int(controller_id))
```

### Comparing `pyrfuniverse-0.9.13/pyrfuniverse/envs/bouncer_env.py` & `pyrfuniverse-0.9.20/pyrfuniverse/envs/bouncer_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.13/pyrfuniverse/envs/franka_grasp_env.py` & `pyrfuniverse-0.9.20/pyrfuniverse/envs/franka_grasp_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.13/pyrfuniverse/envs/franka_push_env.py` & `pyrfuniverse-0.9.20/pyrfuniverse/envs/franka_push_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.13/pyrfuniverse/envs/gripper_nail/__init__.py` & `pyrfuniverse-0.9.20/pyrfuniverse/envs/gripper_nail/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.13/pyrfuniverse/envs/gripper_nail/nail_can_env.py` & `pyrfuniverse-0.9.20/pyrfuniverse/envs/gripper_nail/nail_can_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.13/pyrfuniverse/envs/gripper_nail/nail_card_env.py` & `pyrfuniverse-0.9.20/pyrfuniverse/envs/gripper_nail/nail_card_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.13/pyrfuniverse/envs/gripper_nail/robotiq85_insert_env.py` & `pyrfuniverse-0.9.20/pyrfuniverse/envs/gripper_nail/robotiq85_insert_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.13/pyrfuniverse/envs/gripper_nail/robotiq85_nail_book_env.py` & `pyrfuniverse-0.9.20/pyrfuniverse/envs/gripper_nail/robotiq85_nail_book_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.13/pyrfuniverse/envs/gripper_nail/robotiq85_nail_can_env.py` & `pyrfuniverse-0.9.20/pyrfuniverse/envs/gripper_nail/robotiq85_nail_can_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.13/pyrfuniverse/envs/gripper_nail/robotiq85_nail_card_env.py` & `pyrfuniverse-0.9.20/pyrfuniverse/envs/gripper_nail/robotiq85_nail_card_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.13/pyrfuniverse/envs/gripper_nail/robotiq85_nail_coin_env.py` & `pyrfuniverse-0.9.20/pyrfuniverse/envs/gripper_nail/robotiq85_nail_coin_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.13/pyrfuniverse/envs/gym_goal_wrapper_env.py` & `pyrfuniverse-0.9.20/pyrfuniverse/envs/gym_goal_wrapper_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.13/pyrfuniverse/envs/gym_wrapper_env.py` & `pyrfuniverse-0.9.20/pyrfuniverse/envs/gym_wrapper_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.13/pyrfuniverse/envs/multi_agent/cleaner_env.py` & `pyrfuniverse-0.9.20/pyrfuniverse/envs/multi_agent/cleaner_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.13/pyrfuniverse/envs/multi_agent/navigation_env.py` & `pyrfuniverse-0.9.20/pyrfuniverse/envs/multi_agent/navigation_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.13/pyrfuniverse/envs/multi_agent_navigation_env.py` & `pyrfuniverse-0.9.20/pyrfuniverse/envs/multi_agent_navigation_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.13/pyrfuniverse/envs/multi_physics/__init__.py` & `pyrfuniverse-0.9.20/pyrfuniverse/envs/multi_physics/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.13/pyrfuniverse/envs/multi_physics/flexiv_cutting.py` & `pyrfuniverse-0.9.20/pyrfuniverse/envs/multi_physics/flexiv_cutting.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.13/pyrfuniverse/envs/multi_physics/kinova_gen2_catching_cloth_env.py` & `pyrfuniverse-0.9.20/pyrfuniverse/envs/multi_physics/kinova_gen2_catching_cloth_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.13/pyrfuniverse/envs/multi_physics/ur5_water_shooting.py` & `pyrfuniverse-0.9.20/pyrfuniverse/envs/multi_physics/ur5_water_shooting.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.13/pyrfuniverse/envs/rfuniverse_robot_hub_env.py` & `pyrfuniverse-0.9.20/pyrfuniverse/envs/rfuniverse_robot_hub_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.13/pyrfuniverse/envs/robotics/__init__.py` & `pyrfuniverse-0.9.20/pyrfuniverse/envs/robotics/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.13/pyrfuniverse/envs/robotics/franka_cloth_env.py` & `pyrfuniverse-0.9.20/pyrfuniverse/envs/robotics/franka_cloth_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.13/pyrfuniverse/envs/robotics/franka_cloth_fold_env.py` & `pyrfuniverse-0.9.20/pyrfuniverse/envs/robotics/franka_cloth_fold_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.13/pyrfuniverse/envs/robotics/franka_robotics_env.py` & `pyrfuniverse-0.9.20/pyrfuniverse/envs/robotics/franka_robotics_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.13/pyrfuniverse/envs/robotics/franka_softbody_env.py` & `pyrfuniverse-0.9.20/pyrfuniverse/envs/robotics/franka_softbody_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.13/pyrfuniverse/envs/robotics/pick_and_place_env.py` & `pyrfuniverse-0.9.20/pyrfuniverse/envs/robotics/pick_and_place_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.13/pyrfuniverse/envs/robotics/push_env.py` & `pyrfuniverse-0.9.20/pyrfuniverse/envs/robotics/push_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.13/pyrfuniverse/envs/robotics/reach_env.py` & `pyrfuniverse-0.9.20/pyrfuniverse/envs/robotics/reach_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.13/pyrfuniverse/envs/roller_env.py` & `pyrfuniverse-0.9.20/pyrfuniverse/envs/roller_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.13/pyrfuniverse/envs/tobor_robotics/tobor_push_pull_env.py` & `pyrfuniverse-0.9.20/pyrfuniverse/envs/tobor_robotics/tobor_push_pull_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.13/pyrfuniverse/envs/tobor_robotiq85_manipulation_env.py` & `pyrfuniverse-0.9.20/pyrfuniverse/envs/tobor_robotiq85_manipulation_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.13/pyrfuniverse/envs/ur5_box_env.py` & `pyrfuniverse-0.9.20/pyrfuniverse/envs/ur5_box_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.13/pyrfuniverse/envs/ur5_drawer_env.py` & `pyrfuniverse-0.9.20/pyrfuniverse/envs/ur5_drawer_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.13/pyrfuniverse/side_channel/incoming_message.py` & `pyrfuniverse-0.9.20/pyrfuniverse/side_channel/incoming_message.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.13/pyrfuniverse/side_channel/outgoing_message.py` & `pyrfuniverse-0.9.20/pyrfuniverse/side_channel/outgoing_message.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.13/pyrfuniverse/utils/active_depth_generate.py` & `pyrfuniverse-0.9.20/pyrfuniverse/utils/active_depth_generate.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.13/pyrfuniverse/utils/controller.py` & `pyrfuniverse-0.9.20/pyrfuniverse/utils/controller.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.13/pyrfuniverse/utils/depth_processor.py` & `pyrfuniverse-0.9.20/pyrfuniverse/utils/depth_processor.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.13/pyrfuniverse/utils/interpolate_utils.py` & `pyrfuniverse-0.9.20/pyrfuniverse/utils/interpolate_utils.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.13/pyrfuniverse/utils/jaco_controller.py` & `pyrfuniverse-0.9.20/pyrfuniverse/utils/jaco_controller.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.13/pyrfuniverse/utils/kinova_controller.py` & `pyrfuniverse-0.9.20/pyrfuniverse/utils/kinova_controller.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.13/pyrfuniverse/utils/os_utils.py` & `pyrfuniverse-0.9.20/pyrfuniverse/utils/os_utils.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.13/pyrfuniverse/utils/rfuniverse_communicator.py` & `pyrfuniverse-0.9.20/pyrfuniverse/utils/rfuniverse_communicator.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,57 @@
 import math
+import os
 import struct
 import socket
 import threading
 from sys import platform
 
 import numpy as np
+import time
+from pyrfuniverse.utils.locker import Locker
 
 
 class RFUniverseCommunicator(threading.Thread):
-    def __init__(self, port: int = 5004, is_async: bool = False, receive_data_callback=None):
+    def __init__(
+        self,
+        port: int = 5004,
+        is_async: bool = False,
+        receive_data_callback=None,
+        proc_type="editor",
+    ):
         threading.Thread.__init__(self)
         self.is_async = is_async
         # self.sync_send_bytes_queue = []
         self.read_offset = 0
         self.on_receive_data = receive_data_callback
-        self.port = port
         self.server = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         self.server.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
-        self.server.bind(('localhost', self.port))
-        print(f'Waiting for connections on port: {self.port}...')
+        self.port = port
+        if proc_type == "editor":
+            self.server.bind(("localhost", self.port))
+        elif proc_type == "release":
+            with Locker('port'):
+                while self.port < 65536:
+                    try:
+                        self.server.bind(("localhost", self.port))
+                        print(f"discover port {self.port}")
+                        return
+                    except OSError:
+                        self.port += 256
+                raise OSError("No available port")
+        else:
+            raise ValueError(f"Unknown proc_type: {proc_type}")
+
+    def online(self):
+        print(f"Waiting for connections on port: {self.port}...")
         self.server.listen(1)
         self.client, self.addr = self.server.accept()
-        print(f'Connected successfully')
+        print(f"Connected successfully")
         self.connected = True
         self.client.settimeout(None)
-        # self.buffer_size = 1024 * 10
-        # self.client.setsockopt(socket.SOL_SOCKET, socket.SO_SNDBUF, self.buffer_size)
-        # self.client.setsockopt(socket.SOL_SOCKET, socket.SO_RCVBUF, self.buffer_size)
         self.client.setsockopt(socket.IPPROTO_TCP, socket.TCP_NODELAY, 1)
         if self.is_async:
             self.start()
         else:
             self.receive_step()
 
     def close(self):
@@ -46,217 +67,211 @@
                 self.on_receive_data(objs)
 
     def sync_step(self):
         if self.is_async:
             return
         self.send_object("StepStart")
         # for item in self.sync_send_bytes_queue:
-            # self.send_bytes(item)
+        # self.send_bytes(item)
         # self.sync_send_bytes_queue.clear()
         self.receive_step()
 
     def receive_step(self):
         # sync_receive_objects_queue = []
         while True:
             if not self.connected:
                 return
             data = self.receive_bytes()
             if data is not None and len(data) > 0:
                 objs = self.receive_object(data)
                 if len(objs) > 0 and objs[0] == "StepEnd":
-
                     break
                 self.on_receive_data(objs)
-        #     sync_receive_objects_queue.append(objs)
-        # if self.on_receive_data is not None:
-        #     for item in sync_receive_objects_queue:
-        #         self.on_receive_data(item)
-        # sync_receive_objects_queue.clear()
 
     def receive_bytes(self):
         data = self.client.recv(4)
-        length = int.from_bytes(data, byteorder='little', signed=False)
+        length = int.from_bytes(data, byteorder="little", signed=False)
         if length == 0:
             return None
         buffer = bytearray()
         while len(buffer) < length:
             buffer.extend(self.client.recv(length - len(buffer)))
         return buffer
 
     def send_bytes(self, data: bytes):
         if not self.connected:
             return
-        length = len(data).to_bytes(4, byteorder='little', signed=False)
+        length = len(data).to_bytes(4, byteorder="little", signed=False)
         self.client.send(length)
         self.client.send(data)
 
-        # offset = 0
-        # while offset < len(data):
-        #     offset_max = offset + self.buffer_size
-        #     if offset_max > len(data):
-        #         offset_max = len(data)
-        #     self.client.send(data[offset: offset_max])
-        #     offset = offset_max
-        # # self.client.send(data)
-        # if platform == 'linux':
-        #     self.client.setsockopt(socket.IPPROTO_TCP, socket.TCP_QUICKACK, 1)
+        if platform == 'linux':
+            self.client.setsockopt(socket.IPPROTO_TCP, socket.TCP_QUICKACK, 1)
 
     def receive_object(self, data: bytes) -> list:
         self.read_offset = 0
         count = self.read_int(data)
         objs = []
         for i in range(count):
             objs.append(self.read_object(data))
         return objs
 
     def read_object(self, datas: bytes) -> object:
         data_type = self.read_string(datas)
-        if data_type == 'int':
+        if data_type == "int":
             return self.read_int(datas)
-        elif data_type == 'float':
+        elif data_type == "float":
             return self.read_float(datas)
-        elif data_type == 'string':
+        elif data_type == "string":
             return self.read_string(datas)
-        elif data_type == 'bool':
+        elif data_type == "bool":
             return self.read_bool(datas)
-        elif data_type == 'bytes':
+        elif data_type == "bytes":
             return self.read_bytes(datas)
-        elif data_type == 'vector3':
+        elif data_type == "vector3":
             return self.read_object(datas)
-        elif data_type == 'quaternion':
+        elif data_type == "quaternion":
             return self.read_object(datas)
-        elif data_type == 'matrix':
+        elif data_type == "matrix":
             return self.read_object(datas)
-        elif data_type == 'rect':
+        elif data_type == "rect":
             return [self.read_float(datas) for _ in range(4)]
-        elif data_type == 'array':
+        elif data_type == "array":
             rank = self.read_int(datas)
             shape = []
             for _ in range(rank):
                 shape.append(self.read_int(datas))
             result = np.ndarray(shape, dtype=np.float32)
             result = result.reshape(-1)
             for i in range(len(result)):
                 result[i] = self.read_float(datas)
             return result.reshape(shape)
-        elif data_type == 'list':
+        elif data_type == "list":
             count = self.read_int(datas)
             result = []
             for _ in range(count):
                 result.append(self.read_object(datas))
             return result
-        elif data_type == 'dict':
+        elif data_type == "dict":
             count = self.read_int(datas)
             result = {}
             for _ in range(count):
                 key = self.read_object(datas)
                 value = self.read_object(datas)
                 result[key] = value
             return result
-        elif data_type == 'tuple':
+        elif data_type == "tuple":
             count = self.read_int(datas)
             result = []
             for _ in range(count):
                 result.append(self.read_object(datas))
             return tuple(result)
-        elif data_type == 'null' or data_type == 'none':
+        elif data_type == "null" or data_type == "none":
             return None
         else:
-            print(f'dont support this type: {data_type}')
+            print(f"dont support this type: {data_type}")
             return None
 
     def read_string(self, datas: bytes) -> str:
         count = self.read_int(datas)
         self.read_offset += count
-        return datas[self.read_offset - count:self.read_offset].decode('utf-8')
+        return datas[self.read_offset - count : self.read_offset].decode("utf-8")
 
     def read_int(self, datas: bytes) -> int:
         self.read_offset += 4
-        return int.from_bytes(datas[self.read_offset - 4:self.read_offset], byteorder='little')
+        return int.from_bytes(
+            datas[self.read_offset - 4 : self.read_offset], byteorder="little"
+        )
 
     def read_float(self, datas: bytes) -> float:
         self.read_offset += 4
-        return struct.unpack('f', datas[self.read_offset - 4:self.read_offset])[0]
+        return struct.unpack("f", datas[self.read_offset - 4 : self.read_offset])[0]
 
     def read_bool(self, datas: bytes) -> bool:
         self.read_offset += 1
-        return bool(int.from_bytes(datas[self.read_offset - 1:self.read_offset], byteorder='little'))
+        return bool(
+            int.from_bytes(
+                datas[self.read_offset - 1 : self.read_offset], byteorder="little"
+            )
+        )
 
     def read_bytes(self, datas: bytes) -> bytes:
         count = self.read_int(datas)
         self.read_offset += count
-        return datas[self.read_offset - count:self.read_offset]
+        return datas[self.read_offset - count : self.read_offset]
 
     def send_object(self, *args):
         datas = bytearray()
         self.write_int(datas, len(args))
         for obj in args:
             self.write_object(datas, obj)
 
         # if self.is_async:
         self.send_bytes(bytes(datas))
         # else:
-            # self.sync_send_bytes_queue.append(bytes(datas))
+        # self.sync_send_bytes_queue.append(bytes(datas))
 
     def write_object(self, datas: bytearray, obj):
         if obj is None:
-            self.write_string(datas, 'none')
+            self.write_string(datas, "none")
         elif type(obj) == int or type(obj) == np.int32 or type(obj) == np.int64:
-            self.write_string(datas, 'int')
+            self.write_string(datas, "int")
             self.write_int(datas, obj)
         elif type(obj) == float or type(obj) == np.float32 or type(obj) == np.float64:
-            self.write_string(datas, 'float')
+            self.write_string(datas, "float")
             self.write_float(datas, obj)
         elif type(obj) == bool:
-            self.write_string(datas, 'bool')
+            self.write_string(datas, "bool")
             self.write_bool(datas, obj)
         elif type(obj) == str:
-            self.write_string(datas, 'string')
+            self.write_string(datas, "string")
             self.write_string(datas, obj)
         elif type(obj) == bytes or type(obj) == bytearray:
-            self.write_string(datas, 'bytes')
+            self.write_string(datas, "bytes")
             self.write_bytes(datas, bytes(obj))
         elif type(obj) == list:
-            self.write_string(datas, 'list')
+            self.write_string(datas, "list")
             self.write_int(datas, len(obj))
             for item in obj:
                 self.write_object(datas, item)
         elif type(obj) == dict:
-            self.write_string(datas, 'dict')
+            self.write_string(datas, "dict")
             self.write_int(datas, len(obj))
             for item in obj:
                 self.write_object(datas, item)
                 self.write_object(datas, obj[item])
         elif type(obj) == np.ndarray:
-            self.write_string(datas, 'array')
+            self.write_string(datas, "array")
             self.write_int(datas, len(obj.shape))
             for i in range(len(obj.shape)):
                 self.write_int(datas, obj.shape[i])
             obj = obj.reshape(-1)
             for i in range(len(obj)):
                 self.write_float(datas, float(obj[i]))
         elif type(obj) == tuple:
-            self.write_string(datas, 'tuple')
+            self.write_string(datas, "tuple")
             self.write_int(datas, len(obj))
             for i in range(len(obj)):
                 self.write_object(datas, obj[i])
         else:
-            print(f'dont support this type: {type(obj)}')
-            self.write_string(datas, 'null')
+            print(f"dont support this type: {type(obj)}")
+            self.write_string(datas, "null")
 
     def write_string(self, datas: bytearray, s: str):
-        s_byte = s.encode('utf-8')
+        s_byte = s.encode("utf-8")
         self.write_int(datas, len(s_byte))
         datas.extend(s_byte)
 
     def write_int(self, datas: bytearray, i: int):
-        datas.extend(i.to_bytes(4, byteorder='little'))
+        datas.extend(i.to_bytes(4, byteorder="little"))
 
     def write_float(self, datas: bytearray, f: float):
-        datas.extend(struct.pack('f', f))
+        datas.extend(struct.pack("f", f))
 
     def write_bool(self, datas: bytearray, b: bool):
-        datas.extend(int(b).to_bytes(1, byteorder='little'))
+        datas.extend(int(b).to_bytes(1, byteorder="little"))
 
     def write_bytes(self, datas: bytearray, b: bytes):
         self.write_int(datas, len(b))
         datas.extend(b)
+
+
```

### Comparing `pyrfuniverse-0.9.13/pyrfuniverse/utils/rfuniverse_utility.py` & `pyrfuniverse-0.9.20/pyrfuniverse/utils/rfuniverse_utility.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.13/pyrfuniverse/utils/stretch_controller.py` & `pyrfuniverse-0.9.20/pyrfuniverse/utils/stretch_controller.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.13/pyrfuniverse/utils/tobor_controller.py` & `pyrfuniverse-0.9.20/pyrfuniverse/utils/tobor_controller.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.13/pyrfuniverse/utils/ur5_controller.py` & `pyrfuniverse-0.9.20/pyrfuniverse/utils/ur5_controller.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.13/pyrfuniverse.egg-info/SOURCES.txt` & `pyrfuniverse-0.9.20/pyrfuniverse.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -71,15 +71,17 @@
 pyrfuniverse/utils/__init__.py
 pyrfuniverse/utils/active_depth_generate.py
 pyrfuniverse/utils/controller.py
 pyrfuniverse/utils/depth_processor.py
 pyrfuniverse/utils/interpolate_utils.py
 pyrfuniverse/utils/jaco_controller.py
 pyrfuniverse/utils/kinova_controller.py
+pyrfuniverse/utils/locker.py
 pyrfuniverse/utils/os_utils.py
+pyrfuniverse/utils/proc_wrapper.py
 pyrfuniverse/utils/rfuniverse_communicator.py
 pyrfuniverse/utils/rfuniverse_utility.py
 pyrfuniverse/utils/stretch_controller.py
 pyrfuniverse/utils/tobor_controller.py
 pyrfuniverse/utils/ur5_controller.py
 test/test_active_depth.py
 test/test_articulation_ik.py
@@ -103,8 +105,9 @@
 test/test_pick_and_place_flexiv.py
 test/test_ply_render.py
 test/test_point_cloud.py
 test/test_point_cloud_with_intrinsic_matrix.py
 test/test_save_gripper.py
 test/test_save_obj.py
 test/test_scene.py
-test/test_tobor_move.py
+test/test_tobor_move.py
+test/test_urdf_parameter.py
```

### Comparing `pyrfuniverse-0.9.13/setup.py` & `pyrfuniverse-0.9.20/setup.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.13/test/test_active_depth.py` & `pyrfuniverse-0.9.20/test/test_active_depth.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.13/test/test_articulation_ik.py` & `pyrfuniverse-0.9.20/test/test_articulation_ik.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.13/test/test_camera_image.py` & `pyrfuniverse-0.9.20/test/test_camera_image.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,17 @@
 
 env = RFUniverseBaseEnv(assets=['Camera', 'GameObject_Box'])
 
 camera = env.InstanceObject(name='Camera', id=123456, attr_type=attr.CameraAttr)
 box = env.InstanceObject(name='GameObject_Box', attr_type=attr.GameObjectAttr)
 box.SetTransform(position=[0, 0.05, 0.5], scale=[0.1, 0.1, 0.1])
 box.SetColor([1, 0, 0, 1])
+env.step()
 camera.SetTransform(position=[0, 0.25, 0], rotation=[30, 0, 0])
+camera.LookAt(target=box.data['position'])
 camera.GetDepth(width=512, height=512, zero_dis=1, one_dis=5)
 camera.GetDepthEXR(width=512, height=512)
 camera.GetRGB(width=512, height=512)
 env.step()
 print(camera.data['depth'])
 print(camera.data['depth_exr'])
 print(camera.data['rgb'])
```

### Comparing `pyrfuniverse-0.9.13/test/test_custom_message.py` & `pyrfuniverse-0.9.20/test/test_custom_message.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.13/test/test_debug.py` & `pyrfuniverse-0.9.20/test/test_debug.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.13/test/test_grasp_pose.py` & `pyrfuniverse-0.9.20/test/test_grasp_pose.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.13/test/test_grasp_sim.py` & `pyrfuniverse-0.9.20/test/test_grasp_sim.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.13/test/test_heat_map.py` & `pyrfuniverse-0.9.20/test/test_heat_map.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.13/test/test_humanbody_ik.py` & `pyrfuniverse-0.9.20/test/test_humanbody_ik.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.13/test/test_image_stream.py` & `pyrfuniverse-0.9.20/test/test_image_stream.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,25 @@
 import threading
 from pyrfuniverse.envs.base_env import RFUniverseBaseEnv
 import pyrfuniverse.attributes as attr
 import cv2
 import numpy as np
 
 img = None
-
-
 class ImageThread(threading.Thread):
     def __init__(self):
         threading.Thread.__init__(self)
 
     def run(self):
         while True:
             global img
             if img is not None:
                 cv2.imshow('image', img)
                 cv2.waitKey(10)
 
-
 env = RFUniverseBaseEnv(assets=['Camera', 'GameObject_Box'])
 
 camera = env.InstanceObject(name='Camera', id=123456, attr_type=attr.CameraAttr)
 camera.SetTransform(position=[0, 0.25, 0], rotation=[30, 0, 0])
 box = env.InstanceObject(name='GameObject_Box', attr_type=attr.GameObjectAttr)
 box.SetTransform(position=[0, 0.05, 0.5], scale=[0.1, 0.1, 0.1])
 box.SetColor([1, 0, 0, 1])
```

### Comparing `pyrfuniverse-0.9.13/test/test_label.py` & `pyrfuniverse-0.9.20/test/test_label.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.13/test/test_light.py` & `pyrfuniverse-0.9.20/test/test_light.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.13/test/test_load_mesh.py` & `pyrfuniverse-0.9.20/test/test_load_mesh.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.13/test/test_load_urdf.py` & `pyrfuniverse-0.9.20/test/test_load_urdf.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.13/test/test_object_data.py` & `pyrfuniverse-0.9.20/test/test_object_data.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.13/test/test_ompl.py` & `pyrfuniverse-0.9.20/test/test_ompl.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.13/test/test_pick_and_place.py` & `pyrfuniverse-0.9.20/test/test_pick_and_place.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import random
 from pyrfuniverse.envs.base_env import RFUniverseBaseEnv
 import pyrfuniverse.attributes as attr
 
-env = RFUniverseBaseEnv()
+env = RFUniverseBaseEnv(assets=['franka_panda'])
 
 robot = env.InstanceObject(name='franka_panda', id=123456, attr_type=attr.ControllerAttr)
 robot.SetIKTargetOffset(position=[0, 0.105, 0])
-env.step(200)
+env.step()
 gripper = env.GetAttr(1234560)
 gripper.GripperOpen()
-robot.IKTargetDoMove(position=[0, 0.7, 0.5], duration=0, speed_based=False)
+robot.IKTargetDoMove(position=[0, 0.5, 0.5], duration=0, speed_based=False)
 robot.IKTargetDoRotate(rotation=[0, 45, 180], duration=0, speed_based=False)
 env.step()
 robot.WaitDo()
 
 while 1:
     box1 = env.InstanceObject(name='Rigidbody_Box', id=111111, attr_type=attr.RigidbodyAttr)
     box1.SetTransform(position=[random.uniform(-0.5, -0.3), 0.03, random.uniform(0.3, 0.5)], scale=[0.06, 0.06, 0.06])
@@ -42,13 +42,13 @@
     env.step()
     robot.WaitDo()
     gripper.GripperOpen()
     env.step(50)
     robot.IKTargetDoMove(position=[0, 0.5, 0], duration=2, speed_based=False, relative=True)
     env.step()
     robot.WaitDo()
-    robot.IKTargetDoMove(position=[0, 0.7, 0.5], duration=2, speed_based=False)
+    robot.IKTargetDoMove(position=[0, 0.5, 0.5], duration=2, speed_based=False)
     env.step()
     robot.WaitDo()
     box1.Destroy()
     box2.Destroy()
     env.step()
```

### Comparing `pyrfuniverse-0.9.13/test/test_pick_and_place_flexiv.py` & `pyrfuniverse-0.9.20/test/test_pick_and_place_flexiv.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 from pyrfuniverse.envs.base_env import RFUniverseBaseEnv
 import pyrfuniverse.attributes as attr
 
 env = RFUniverseBaseEnv(assets=['flexivArm_ag95'])
 
 robot = env.InstanceObject(name='flexivArm_ag95', id=123456, attr_type=attr.ControllerAttr)
 robot.SetIKTargetOffset(position=[0, 0.25, 0])
-env.step(200)
+env.step()
 gripper = env.GetAttr(1234560)
 gripper.GripperOpen()
-robot.IKTargetDoMove(position=[0, 0.7, 0.5], duration=0, speed_based=False)
+robot.IKTargetDoMove(position=[0, 0.5, 0.5], duration=0, speed_based=False)
 robot.IKTargetDoRotate(rotation=[0, 0, 180], duration=0, speed_based=False)
 env.step()
 robot.WaitDo()
 
 while 1:
     box1 = env.InstanceObject(name='Rigidbody_Box', id=111111, attr_type=attr.RigidbodyAttr)
     box1.SetTransform(position=[random.uniform(-0.5, -0.3), 0.03, random.uniform(0.3, 0.5)], scale=[0.06, 0.06, 0.06])
@@ -42,13 +42,13 @@
     env.step()
     robot.WaitDo()
     gripper.GripperOpen()
     env.step(50)
     robot.IKTargetDoMove(position=[0, 0.5, 0], duration=2, speed_based=False, relative=True)
     env.step()
     robot.WaitDo()
-    robot.IKTargetDoMove(position=[0, 0.7, 0.5], duration=2, speed_based=False)
+    robot.IKTargetDoMove(position=[0, 0.5, 0.5], duration=2, speed_based=False)
     env.step()
     robot.WaitDo()
     box1.Destroy()
     box2.Destroy()
     env.step()
```

### Comparing `pyrfuniverse-0.9.13/test/test_point_cloud.py` & `pyrfuniverse-0.9.20/test/test_point_cloud.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.13/test/test_point_cloud_with_intrinsic_matrix.py` & `pyrfuniverse-0.9.20/test/test_point_cloud_with_intrinsic_matrix.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.13/test/test_save_gripper.py` & `pyrfuniverse-0.9.20/test/test_save_gripper.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.13/test/test_scene.py` & `pyrfuniverse-0.9.20/test/test_scene.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.9.13/test/test_tobor_move.py` & `pyrfuniverse-0.9.20/test/test_tobor_move.py`

 * *Files identical despite different names*

