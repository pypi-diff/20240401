# Comparing `tmp/pye2-0.7.8.tar.gz` & `tmp/pye2-0.7.9.tar.gz`

## Comparing `pye2-0.7.8.tar` & `pye2-0.7.9.tar`

### file list

```diff
@@ -1,90 +1,90 @@
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 pye2-0.7.8/.gitattributes
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 pye2-0.7.8/TODOs.md
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 pye2-0.7.8/__init__.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 pye2-0.7.8/requirements.txt
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pye2-0.7.8/winrun.bat
--rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 pye2-0.7.8/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 pye2-0.7.8/PyE2/__init__.py
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 pye2-0.7.8/PyE2/_ver.py
--rw-r--r--   0        0        0     4173 2020-02-02 00:00:00.000000 pye2-0.7.8/PyE2/base_decentra_object.py
--rw-r--r--   0        0        0     9598 2020-02-02 00:00:00.000000 pye2-0.7.8/PyE2/plugins_manager_mixin.py
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 pye2-0.7.8/PyE2/base/__init__.py
--rw-r--r--   0        0        0    40906 2020-02-02 00:00:00.000000 pye2-0.7.8/PyE2/base/generic_session.py
--rw-r--r--   0        0        0     6610 2020-02-02 00:00:00.000000 pye2-0.7.8/PyE2/base/instance.py
--rw-r--r--   0        0        0    29508 2020-02-02 00:00:00.000000 pye2-0.7.8/PyE2/base/pipeline.py
--rw-r--r--   0        0        0    62467 2020-02-02 00:00:00.000000 pye2-0.7.8/PyE2/base/plugin_template.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 pye2-0.7.8/PyE2/base/payload/__init__.py
--rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 pye2-0.7.8/PyE2/base/payload/payload.py
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 pye2-0.7.8/PyE2/bc/__init__.py
--rw-r--r--   0        0        0    26813 2020-02-02 00:00:00.000000 pye2-0.7.8/PyE2/bc/base.py
--rw-r--r--   0        0        0     7553 2020-02-02 00:00:00.000000 pye2-0.7.8/PyE2/bc/ec.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 pye2-0.7.8/PyE2/code_cheker/__init__.py
--rw-r--r--   0        0        0    10347 2020-02-02 00:00:00.000000 pye2-0.7.8/PyE2/code_cheker/base.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 pye2-0.7.8/PyE2/comm/__init__.py
--rw-r--r--   0        0        0     8536 2020-02-02 00:00:00.000000 pye2-0.7.8/PyE2/comm/amqp_wrapper.py
--rw-r--r--   0        0        0    12378 2020-02-02 00:00:00.000000 pye2-0.7.8/PyE2/comm/mqtt_wrapper.py
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 pye2-0.7.8/PyE2/const/README.md
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 pye2-0.7.8/PyE2/const/__init__.py
--rw-r--r--   0        0        0     2401 2020-02-02 00:00:00.000000 pye2-0.7.8/PyE2/const/base.py
--rw-r--r--   0        0        0     2137 2020-02-02 00:00:00.000000 pye2-0.7.8/PyE2/const/comms.py
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 pye2-0.7.8/PyE2/const/environment.py
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 pye2-0.7.8/PyE2/const/formatter.py
--rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 pye2-0.7.8/PyE2/const/heartbeat.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 pye2-0.7.8/PyE2/const/misc.py
--rw-r--r--   0        0        0     5381 2020-02-02 00:00:00.000000 pye2-0.7.8/PyE2/const/payload.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 pye2-0.7.8/PyE2/default/__init__.py
--rw-r--r--   0        0        0     2572 2020-02-02 00:00:00.000000 pye2-0.7.8/PyE2/default/mqtt_session.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 pye2-0.7.8/PyE2/io_formatter/__init__.py
--rw-r--r--   0        0        0     3483 2020-02-02 00:00:00.000000 pye2-0.7.8/PyE2/io_formatter/io_formatter_manager.py
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 pye2-0.7.8/PyE2/io_formatter/base/__init__.py
--rw-r--r--   0        0        0     2337 2020-02-02 00:00:00.000000 pye2-0.7.8/PyE2/io_formatter/base/base_formatter.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 pye2-0.7.8/PyE2/io_formatter/default/__init__.py
--rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 pye2-0.7.8/PyE2/io_formatter/default/a_dummy.py
--rw-r--r--   0        0        0     3048 2020-02-02 00:00:00.000000 pye2-0.7.8/PyE2/io_formatter/default/aixp1.py
--rw-r--r--   0        0        0    10482 2020-02-02 00:00:00.000000 pye2-0.7.8/PyE2/io_formatter/default/cavi2.py
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 pye2-0.7.8/PyE2/io_formatter/default/default.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 pye2-0.7.8/PyE2/logging/__init__.py
--rw-r--r--   0        0        0    58743 2020-02-02 00:00:00.000000 pye2-0.7.8/PyE2/logging/base_logger.py
--rw-r--r--   0        0        0     2887 2020-02-02 00:00:00.000000 pye2-0.7.8/PyE2/logging/small_logger.py
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 pye2-0.7.8/PyE2/logging/logger_mixins/__init__.py
--rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 pye2-0.7.8/PyE2/logging/logger_mixins/class_instance_mixin.py
--rw-r--r--   0        0        0    13213 2020-02-02 00:00:00.000000 pye2-0.7.8/PyE2/logging/logger_mixins/computer_vision_mixin.py
--rw-r--r--   0        0        0    11305 2020-02-02 00:00:00.000000 pye2-0.7.8/PyE2/logging/logger_mixins/datetime_mixin.py
--rw-r--r--   0        0        0    13024 2020-02-02 00:00:00.000000 pye2-0.7.8/PyE2/logging/logger_mixins/download_mixin.py
--rw-r--r--   0        0        0     7420 2020-02-02 00:00:00.000000 pye2-0.7.8/PyE2/logging/logger_mixins/general_serialization_mixin.py
--rw-r--r--   0        0        0    14368 2020-02-02 00:00:00.000000 pye2-0.7.8/PyE2/logging/logger_mixins/json_serialization_mixin.py
--rw-r--r--   0        0        0     9146 2020-02-02 00:00:00.000000 pye2-0.7.8/PyE2/logging/logger_mixins/pickle_serialization_mixin.py
--rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 pye2-0.7.8/PyE2/logging/logger_mixins/process_mixin.py
--rw-r--r--   0        0        0     2277 2020-02-02 00:00:00.000000 pye2-0.7.8/PyE2/logging/logger_mixins/resource_size_mixin.py
--rw-r--r--   0        0        0    17133 2020-02-02 00:00:00.000000 pye2-0.7.8/PyE2/logging/logger_mixins/timers_mixin.py
--rw-r--r--   0        0        0     7677 2020-02-02 00:00:00.000000 pye2-0.7.8/PyE2/logging/logger_mixins/upload_mixin.py
--rw-r--r--   0        0        0    19342 2020-02-02 00:00:00.000000 pye2-0.7.8/PyE2/logging/logger_mixins/utils_mixin.py
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 pye2-0.7.8/PyE2/logging/tzlocal/__init__.py
--rw-r--r--   0        0        0     7268 2020-02-02 00:00:00.000000 pye2-0.7.8/PyE2/logging/tzlocal/unix.py
--rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 pye2-0.7.8/PyE2/logging/tzlocal/utils.py
--rw-r--r--   0        0        0     4462 2020-02-02 00:00:00.000000 pye2-0.7.8/PyE2/logging/tzlocal/win32.py
--rw-r--r--   0        0        0    34203 2020-02-02 00:00:00.000000 pye2-0.7.8/PyE2/logging/tzlocal/windows_tz.py
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 pye2-0.7.8/PyE2/tutorials/.example_env
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 pye2-0.7.8/PyE2/tutorials/1. hello_world.py
--rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 pye2-0.7.8/PyE2/tutorials/2. first_deploy.py
--rw-r--r--   0        0        0     2586 2020-02-02 00:00:00.000000 pye2-0.7.8/PyE2/tutorials/3. simple_real_time_custom_code.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 pye2-0.7.8/PyE2/utils/__init__.py
--rw-r--r--   0        0        0     5298 2020-02-02 00:00:00.000000 pye2-0.7.8/PyE2/utils/code.py
--rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 pye2-0.7.8/PyE2/utils/code_exec.py
--rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 pye2-0.7.8/PyE2/utils/comm_utils.py
--rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 pye2-0.7.8/PyE2/utils/dotenv.py
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 pye2-0.7.8/xperimental/.example_env
--rw-r--r--   0        0        0     2002 2020-02-02 00:00:00.000000 pye2-0.7.8/xperimental/attach_example.py
--rw-r--r--   0        0        0     1993 2020-02-02 00:00:00.000000 pye2-0.7.8/xperimental/ex1.py
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 pye2-0.7.8/xperimental/hello.py
--rw-r--r--   0        0        0     3187 2020-02-02 00:00:00.000000 pye2-0.7.8/xperimental/remote_exec.py
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 pye2-0.7.8/xperimental/save_images.py
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 pye2-0.7.8/xperimental/_archive/test.py
--rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 pye2-0.7.8/xperimental/decentralized/chain_dist_example.py
--rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 pye2-0.7.8/xperimental/decentralized/chain_dist_example_initiator.py
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 pye2-0.7.8/xperimental/decentralized/chain_dist_example_worker.py
--rw-r--r--   0        0        0     2467 2020-02-02 00:00:00.000000 pye2-0.7.8/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pye2-0.7.8/LICENSE
--rw-r--r--   0        0        0    11969 2020-02-02 00:00:00.000000 pye2-0.7.8/README.md
--rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 pye2-0.7.8/pyproject.toml
--rw-r--r--   0        0        0    12801 2020-02-02 00:00:00.000000 pye2-0.7.8/PKG-INFO
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 pye2-0.7.9/.gitattributes
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 pye2-0.7.9/TODOs.md
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 pye2-0.7.9/__init__.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 pye2-0.7.9/requirements.txt
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pye2-0.7.9/winrun.bat
+-rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 pye2-0.7.9/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/__init__.py
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/_ver.py
+-rw-r--r--   0        0        0     4173 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/base_decentra_object.py
+-rw-r--r--   0        0        0     8883 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/plugins_manager_mixin.py
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/base/__init__.py
+-rw-r--r--   0        0        0    40906 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/base/generic_session.py
+-rw-r--r--   0        0        0     6610 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/base/instance.py
+-rw-r--r--   0        0        0    29508 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/base/pipeline.py
+-rw-r--r--   0        0        0    62467 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/base/plugin_template.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/base/payload/__init__.py
+-rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/base/payload/payload.py
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/bc/__init__.py
+-rw-r--r--   0        0        0    26813 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/bc/base.py
+-rw-r--r--   0        0        0     7553 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/bc/ec.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/code_cheker/__init__.py
+-rw-r--r--   0        0        0     9608 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/code_cheker/base.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/comm/__init__.py
+-rw-r--r--   0        0        0     8536 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/comm/amqp_wrapper.py
+-rw-r--r--   0        0        0    12378 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/comm/mqtt_wrapper.py
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/const/README.md
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/const/__init__.py
+-rw-r--r--   0        0        0     2401 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/const/base.py
+-rw-r--r--   0        0        0     2137 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/const/comms.py
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/const/environment.py
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/const/formatter.py
+-rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/const/heartbeat.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/const/misc.py
+-rw-r--r--   0        0        0     5381 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/const/payload.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/default/__init__.py
+-rw-r--r--   0        0        0     2572 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/default/mqtt_session.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/io_formatter/__init__.py
+-rw-r--r--   0        0        0     3483 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/io_formatter/io_formatter_manager.py
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/io_formatter/base/__init__.py
+-rw-r--r--   0        0        0     2337 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/io_formatter/base/base_formatter.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/io_formatter/default/__init__.py
+-rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/io_formatter/default/a_dummy.py
+-rw-r--r--   0        0        0     3048 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/io_formatter/default/aixp1.py
+-rw-r--r--   0        0        0    10482 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/io_formatter/default/cavi2.py
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/io_formatter/default/default.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/logging/__init__.py
+-rw-r--r--   0        0        0    58743 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/logging/base_logger.py
+-rw-r--r--   0        0        0     2887 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/logging/small_logger.py
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/logging/logger_mixins/__init__.py
+-rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/logging/logger_mixins/class_instance_mixin.py
+-rw-r--r--   0        0        0    13213 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/logging/logger_mixins/computer_vision_mixin.py
+-rw-r--r--   0        0        0    11305 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/logging/logger_mixins/datetime_mixin.py
+-rw-r--r--   0        0        0    13024 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/logging/logger_mixins/download_mixin.py
+-rw-r--r--   0        0        0     7420 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/logging/logger_mixins/general_serialization_mixin.py
+-rw-r--r--   0        0        0    14368 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/logging/logger_mixins/json_serialization_mixin.py
+-rw-r--r--   0        0        0     9146 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/logging/logger_mixins/pickle_serialization_mixin.py
+-rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/logging/logger_mixins/process_mixin.py
+-rw-r--r--   0        0        0     2277 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/logging/logger_mixins/resource_size_mixin.py
+-rw-r--r--   0        0        0    17133 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/logging/logger_mixins/timers_mixin.py
+-rw-r--r--   0        0        0     7677 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/logging/logger_mixins/upload_mixin.py
+-rw-r--r--   0        0        0    19342 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/logging/logger_mixins/utils_mixin.py
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/logging/tzlocal/__init__.py
+-rw-r--r--   0        0        0     7268 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/logging/tzlocal/unix.py
+-rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/logging/tzlocal/utils.py
+-rw-r--r--   0        0        0     4462 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/logging/tzlocal/win32.py
+-rw-r--r--   0        0        0    34203 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/logging/tzlocal/windows_tz.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/tutorials/.example_env
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/tutorials/1. hello_world.py
+-rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/tutorials/2. first_deploy.py
+-rw-r--r--   0        0        0     2586 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/tutorials/3. simple_real_time_custom_code.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/utils/__init__.py
+-rw-r--r--   0        0        0     4559 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/utils/code.py
+-rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/utils/code_exec.py
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/utils/comm_utils.py
+-rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/utils/dotenv.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 pye2-0.7.9/xperimental/.example_env
+-rw-r--r--   0        0        0     2002 2020-02-02 00:00:00.000000 pye2-0.7.9/xperimental/attach_example.py
+-rw-r--r--   0        0        0     1993 2020-02-02 00:00:00.000000 pye2-0.7.9/xperimental/ex1.py
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 pye2-0.7.9/xperimental/hello.py
+-rw-r--r--   0        0        0     3187 2020-02-02 00:00:00.000000 pye2-0.7.9/xperimental/remote_exec.py
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 pye2-0.7.9/xperimental/save_images.py
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 pye2-0.7.9/xperimental/_archive/test.py
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 pye2-0.7.9/xperimental/decentralized/chain_dist_example.py
+-rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 pye2-0.7.9/xperimental/decentralized/chain_dist_example_initiator.py
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 pye2-0.7.9/xperimental/decentralized/chain_dist_example_worker.py
+-rw-r--r--   0        0        0     2467 2020-02-02 00:00:00.000000 pye2-0.7.9/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pye2-0.7.9/LICENSE
+-rw-r--r--   0        0        0    11969 2020-02-02 00:00:00.000000 pye2-0.7.9/README.md
+-rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 pye2-0.7.9/pyproject.toml
+-rw-r--r--   0        0        0    12801 2020-02-02 00:00:00.000000 pye2-0.7.9/PKG-INFO
```

### Comparing `pye2-0.7.8/.github/workflows/python-publish.yml` & `pye2-0.7.9/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `pye2-0.7.8/PyE2/base_decentra_object.py` & `pye2-0.7.9/PyE2/base_decentra_object.py`

 * *Files identical despite different names*

### Comparing `pye2-0.7.8/PyE2/plugins_manager_mixin.py` & `pye2-0.7.9/PyE2/plugins_manager_mixin.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-"""
-Copyright (C) 2017-2021 Andrei Damian, andrei.damian@me.com,  All rights reserved.
-
-This software and its associated documentation are the exclusive property of the creator. 
-Unauthorized use, copying, or distribution of this software, or any portion thereof, 
-is strictly prohibited.
-
-Parts of this software are licensed and used in software developed by Knowledge Investment Group SRL.
-Any software proprietary to Knowledge Investment Group SRL is covered by Romanian and  Foreign Patents, 
-patents in process, and are protected by trade secret or copyright law.
-
-Dissemination of this information or reproduction of this material is strictly forbidden unless prior 
-written permission from the author.
-
-"""
-
 import os
 import inspect
 import importlib
 import traceback
 
 from pkgutil import iter_modules
```

### Comparing `pye2-0.7.8/PyE2/base/generic_session.py` & `pye2-0.7.9/PyE2/base/generic_session.py`

 * *Files identical despite different names*

### Comparing `pye2-0.7.8/PyE2/base/instance.py` & `pye2-0.7.9/PyE2/base/instance.py`

 * *Files identical despite different names*

### Comparing `pye2-0.7.8/PyE2/base/pipeline.py` & `pye2-0.7.9/PyE2/base/pipeline.py`

 * *Files identical despite different names*

### Comparing `pye2-0.7.8/PyE2/base/plugin_template.py` & `pye2-0.7.9/PyE2/base/plugin_template.py`

 * *Files identical despite different names*

### Comparing `pye2-0.7.8/PyE2/base/payload/payload.py` & `pye2-0.7.9/PyE2/base/payload/payload.py`

 * *Files identical despite different names*

### Comparing `pye2-0.7.8/PyE2/bc/base.py` & `pye2-0.7.9/PyE2/bc/base.py`

 * *Files identical despite different names*

### Comparing `pye2-0.7.8/PyE2/bc/ec.py` & `pye2-0.7.9/PyE2/bc/ec.py`

 * *Files identical despite different names*

### Comparing `pye2-0.7.8/PyE2/code_cheker/base.py` & `pye2-0.7.9/PyE2/code_cheker/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-# -*- coding: utf-8 -*-
-"""
-Copyright (C) 2017-2021 Andrei Damian, andrei.damian@me.com,  All rights reserved.
-
-This software and its associated documentation are the exclusive property of the creator. 
-Unauthorized use, copying, or distribution of this software, or any portion thereof, 
-is strictly prohibited.
-
-Parts of this software are licensed and used in software developed by Knowledge Investment Group SRL.
-Any software proprietary to Knowledge Investment Group SRL is covered by Romanian and  Foreign Patents, 
-patents in process, and are protected by trade secret or copyright law.
-
-Dissemination of this information or reproduction of this material is strictly forbidden unless prior 
-written permission from the author.
-
-"""
-
 import zlib
 import sys
 import base64
 import traceback
 import re
 
 __VER__ = '0.6.1'
```

### Comparing `pye2-0.7.8/PyE2/comm/amqp_wrapper.py` & `pye2-0.7.9/PyE2/comm/amqp_wrapper.py`

 * *Files identical despite different names*

### Comparing `pye2-0.7.8/PyE2/comm/mqtt_wrapper.py` & `pye2-0.7.9/PyE2/comm/mqtt_wrapper.py`

 * *Files identical despite different names*

### Comparing `pye2-0.7.8/PyE2/const/base.py` & `pye2-0.7.9/PyE2/const/base.py`

 * *Files identical despite different names*

### Comparing `pye2-0.7.8/PyE2/const/comms.py` & `pye2-0.7.9/PyE2/const/comms.py`

 * *Files identical despite different names*

### Comparing `pye2-0.7.8/PyE2/const/heartbeat.py` & `pye2-0.7.9/PyE2/const/heartbeat.py`

 * *Files identical despite different names*

### Comparing `pye2-0.7.8/PyE2/const/payload.py` & `pye2-0.7.9/PyE2/const/payload.py`

 * *Files identical despite different names*

### Comparing `pye2-0.7.8/PyE2/default/mqtt_session.py` & `pye2-0.7.9/PyE2/default/mqtt_session.py`

 * *Files identical despite different names*

### Comparing `pye2-0.7.8/PyE2/io_formatter/io_formatter_manager.py` & `pye2-0.7.9/PyE2/io_formatter/io_formatter_manager.py`

 * *Files identical despite different names*

### Comparing `pye2-0.7.8/PyE2/io_formatter/base/base_formatter.py` & `pye2-0.7.9/PyE2/io_formatter/base/base_formatter.py`

 * *Files identical despite different names*

### Comparing `pye2-0.7.8/PyE2/io_formatter/default/a_dummy.py` & `pye2-0.7.9/PyE2/io_formatter/default/a_dummy.py`

 * *Files identical despite different names*

### Comparing `pye2-0.7.8/PyE2/io_formatter/default/aixp1.py` & `pye2-0.7.9/PyE2/io_formatter/default/aixp1.py`

 * *Files identical despite different names*

### Comparing `pye2-0.7.8/PyE2/io_formatter/default/cavi2.py` & `pye2-0.7.9/PyE2/io_formatter/default/cavi2.py`

 * *Files identical despite different names*

### Comparing `pye2-0.7.8/PyE2/logging/base_logger.py` & `pye2-0.7.9/PyE2/logging/base_logger.py`

 * *Files identical despite different names*

### Comparing `pye2-0.7.8/PyE2/logging/small_logger.py` & `pye2-0.7.9/PyE2/logging/small_logger.py`

 * *Files identical despite different names*

### Comparing `pye2-0.7.8/PyE2/logging/logger_mixins/__init__.py` & `pye2-0.7.9/PyE2/logging/logger_mixins/__init__.py`

 * *Files identical despite different names*

### Comparing `pye2-0.7.8/PyE2/logging/logger_mixins/class_instance_mixin.py` & `pye2-0.7.9/PyE2/logging/logger_mixins/class_instance_mixin.py`

 * *Files identical despite different names*

### Comparing `pye2-0.7.8/PyE2/logging/logger_mixins/computer_vision_mixin.py` & `pye2-0.7.9/PyE2/logging/logger_mixins/computer_vision_mixin.py`

 * *Files identical despite different names*

### Comparing `pye2-0.7.8/PyE2/logging/logger_mixins/datetime_mixin.py` & `pye2-0.7.9/PyE2/logging/logger_mixins/datetime_mixin.py`

 * *Files identical despite different names*

### Comparing `pye2-0.7.8/PyE2/logging/logger_mixins/download_mixin.py` & `pye2-0.7.9/PyE2/logging/logger_mixins/download_mixin.py`

 * *Files identical despite different names*

### Comparing `pye2-0.7.8/PyE2/logging/logger_mixins/general_serialization_mixin.py` & `pye2-0.7.9/PyE2/logging/logger_mixins/general_serialization_mixin.py`

 * *Files identical despite different names*

### Comparing `pye2-0.7.8/PyE2/logging/logger_mixins/json_serialization_mixin.py` & `pye2-0.7.9/PyE2/logging/logger_mixins/json_serialization_mixin.py`

 * *Files identical despite different names*

### Comparing `pye2-0.7.8/PyE2/logging/logger_mixins/pickle_serialization_mixin.py` & `pye2-0.7.9/PyE2/logging/logger_mixins/pickle_serialization_mixin.py`

 * *Files identical despite different names*

### Comparing `pye2-0.7.8/PyE2/logging/logger_mixins/process_mixin.py` & `pye2-0.7.9/PyE2/logging/logger_mixins/process_mixin.py`

 * *Files identical despite different names*

### Comparing `pye2-0.7.8/PyE2/logging/logger_mixins/resource_size_mixin.py` & `pye2-0.7.9/PyE2/logging/logger_mixins/resource_size_mixin.py`

 * *Files identical despite different names*

### Comparing `pye2-0.7.8/PyE2/logging/logger_mixins/timers_mixin.py` & `pye2-0.7.9/PyE2/logging/logger_mixins/timers_mixin.py`

 * *Files identical despite different names*

### Comparing `pye2-0.7.8/PyE2/logging/logger_mixins/upload_mixin.py` & `pye2-0.7.9/PyE2/logging/logger_mixins/upload_mixin.py`

 * *Files identical despite different names*

### Comparing `pye2-0.7.8/PyE2/logging/logger_mixins/utils_mixin.py` & `pye2-0.7.9/PyE2/logging/logger_mixins/utils_mixin.py`

 * *Files identical despite different names*

### Comparing `pye2-0.7.8/PyE2/logging/tzlocal/unix.py` & `pye2-0.7.9/PyE2/logging/tzlocal/unix.py`

 * *Files identical despite different names*

### Comparing `pye2-0.7.8/PyE2/logging/tzlocal/utils.py` & `pye2-0.7.9/PyE2/logging/tzlocal/utils.py`

 * *Files identical despite different names*

### Comparing `pye2-0.7.8/PyE2/logging/tzlocal/win32.py` & `pye2-0.7.9/PyE2/logging/tzlocal/win32.py`

 * *Files identical despite different names*

### Comparing `pye2-0.7.8/PyE2/logging/tzlocal/windows_tz.py` & `pye2-0.7.9/PyE2/logging/tzlocal/windows_tz.py`

 * *Files identical despite different names*

### Comparing `pye2-0.7.8/PyE2/tutorials/1. hello_world.py` & `pye2-0.7.9/PyE2/tutorials/1. hello_world.py`

 * *Files identical despite different names*

### Comparing `pye2-0.7.8/PyE2/tutorials/2. first_deploy.py` & `pye2-0.7.9/PyE2/tutorials/2. first_deploy.py`

 * *Files identical despite different names*

### Comparing `pye2-0.7.8/PyE2/tutorials/3. simple_real_time_custom_code.py` & `pye2-0.7.9/PyE2/tutorials/3. simple_real_time_custom_code.py`

 * *Files identical despite different names*

### Comparing `pye2-0.7.8/PyE2/utils/code_exec.py` & `pye2-0.7.9/PyE2/utils/code_exec.py`

 * *Files identical despite different names*

### Comparing `pye2-0.7.8/PyE2/utils/dotenv.py` & `pye2-0.7.9/PyE2/utils/dotenv.py`

 * *Files identical despite different names*

### Comparing `pye2-0.7.8/xperimental/attach_example.py` & `pye2-0.7.9/xperimental/attach_example.py`

 * *Files identical despite different names*

### Comparing `pye2-0.7.8/xperimental/ex1.py` & `pye2-0.7.9/xperimental/ex1.py`

 * *Files identical despite different names*

### Comparing `pye2-0.7.8/xperimental/remote_exec.py` & `pye2-0.7.9/xperimental/remote_exec.py`

 * *Files identical despite different names*

### Comparing `pye2-0.7.8/xperimental/save_images.py` & `pye2-0.7.9/xperimental/save_images.py`

 * *Files identical despite different names*

### Comparing `pye2-0.7.8/xperimental/decentralized/chain_dist_example.py` & `pye2-0.7.9/xperimental/decentralized/chain_dist_example.py`

 * *Files identical despite different names*

### Comparing `pye2-0.7.8/xperimental/decentralized/chain_dist_example_initiator.py` & `pye2-0.7.9/xperimental/decentralized/chain_dist_example_initiator.py`

 * *Files identical despite different names*

### Comparing `pye2-0.7.8/.gitignore` & `pye2-0.7.9/.gitignore`

 * *Files identical despite different names*

### Comparing `pye2-0.7.8/LICENSE` & `pye2-0.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pye2-0.7.8/README.md` & `pye2-0.7.9/README.md`

 * *Files identical despite different names*

### Comparing `pye2-0.7.8/pyproject.toml` & `pye2-0.7.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "PyE2"
-version = "0.7.8"
+version = "0.7.9"
 authors = [
   { name="Stefan Saraev", email="stefan.saraev@hyperfy.tech" },
   { name="Andrei Ionut Damian", email="andrei.damian@lummetry.ai" },
   { name="Cristan Bleotiu", email="cristan.bleotiu@hyperfy.tech" },
 ]
 description = "PyE2 is the Python SDK required for client app development in the AiXpand network"
 readme = "README.md"
```

### Comparing `pye2-0.7.8/PKG-INFO` & `pye2-0.7.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: PyE2
-Version: 0.7.8
+Version: 0.7.9
 Summary: PyE2 is the Python SDK required for client app development in the AiXpand network
 Project-URL: Homepage, https://github.com/AiXpand/PyE2
 Project-URL: Bug Tracker, https://github.com/AiXpand/PyE2/issues
 Author-email: Stefan Saraev <stefan.saraev@hyperfy.tech>, Andrei Ionut Damian <andrei.damian@lummetry.ai>, Cristan Bleotiu <cristan.bleotiu@hyperfy.tech>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

