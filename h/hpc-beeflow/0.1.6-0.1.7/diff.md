# Comparing `tmp/hpc_beeflow-0.1.6.tar.gz` & `tmp/hpc-beeflow-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hpc_beeflow-0.1.6.tar", max compression
+gzip compressed data, was "hpc-beeflow-0.1.7.tar", max compression
```

## Comparing `hpc_beeflow-0.1.6.tar` & `hpc-beeflow-0.1.7.tar`

### file list

```diff
@@ -1,293 +1,303 @@
--rw-r--r--   0        0        0     1477 2023-04-25 21:47:28.980995 hpc_beeflow-0.1.6/LICENSE
--rw-r--r--   0        0        0     4903 2023-04-25 21:47:28.981096 hpc_beeflow-0.1.6/README.rst
--rw-r--r--   0        0        0      122 2023-04-25 21:47:28.981520 hpc_beeflow-0.1.6/beeflow/client/README.md
--rw-r--r--   0        0        0    20299 2023-12-08 20:10:43.772209 hpc_beeflow-0.1.6/beeflow/client/bee_client.py
--rw-r--r--   0        0        0    21981 2023-12-08 20:10:43.773237 hpc_beeflow-0.1.6/beeflow/client/core.py
--rw-r--r--   0        0        0     8036 2023-04-25 21:47:28.981805 hpc_beeflow-0.1.6/beeflow/cloud_launcher.py
--rw-r--r--   0        0        0      234 2023-04-25 21:47:28.981918 hpc_beeflow-0.1.6/beeflow/common/README.md
--rw-r--r--   0        0        0      459 2023-04-25 21:47:28.982000 hpc_beeflow-0.1.6/beeflow/common/api.py
--rw-r--r--   0        0        0    11473 2023-12-08 20:10:05.996523 hpc_beeflow-0.1.6/beeflow/common/build/README.md
--rw-r--r--   0        0        0     5734 2023-04-25 21:47:28.982334 hpc_beeflow-0.1.6/beeflow/common/build/build_driver.py
--rw-r--r--   0        0        0    18962 2023-05-05 17:47:06.278843 hpc_beeflow-0.1.6/beeflow/common/build/container_drivers.py
--rw-r--r--   0        0        0     3456 2023-04-25 21:47:28.982535 hpc_beeflow-0.1.6/beeflow/common/build_interfaces.py
--rw-r--r--   0        0        0      163 2023-12-08 20:10:43.773376 hpc_beeflow-0.1.6/beeflow/common/celery.py
--rw-r--r--   0        0        0      285 2023-04-25 21:47:28.982612 hpc_beeflow-0.1.6/beeflow/common/cli.py
--rw-r--r--   0        0        0     3023 2023-04-25 21:47:28.983190 hpc_beeflow-0.1.6/beeflow/common/cli_connection.py
--rw-r--r--   0        0        0     2542 2023-04-25 21:47:28.983324 hpc_beeflow-0.1.6/beeflow/common/cloud/README.md
--rw-r--r--   0        0        0      830 2023-04-25 21:47:28.983420 hpc_beeflow-0.1.6/beeflow/common/cloud/__init__.py
--rw-r--r--   0        0        0     1166 2023-04-25 21:47:28.983503 hpc_beeflow-0.1.6/beeflow/common/cloud/chameleoncloud.py
--rw-r--r--   0        0        0      175 2023-04-25 21:47:28.983588 hpc_beeflow-0.1.6/beeflow/common/cloud/cloud.py
--rw-r--r--   0        0        0       42 2023-04-25 21:47:28.983663 hpc_beeflow-0.1.6/beeflow/common/cloud/constants.py
--rw-r--r--   0        0        0     1599 2023-04-25 21:47:28.983758 hpc_beeflow-0.1.6/beeflow/common/cloud/google.py
--rw-r--r--   0        0        0     1093 2023-04-25 21:47:28.983846 hpc_beeflow-0.1.6/beeflow/common/cloud/openstack.py
--rw-r--r--   0        0        0      784 2023-04-25 21:47:28.983934 hpc_beeflow-0.1.6/beeflow/common/cloud/provider.py
--rw-r--r--   0        0        0    22424 2023-12-08 20:10:43.774157 hpc_beeflow-0.1.6/beeflow/common/config_driver.py
--rw-r--r--   0        0        0     5891 2023-04-25 21:47:28.984324 hpc_beeflow-0.1.6/beeflow/common/config_validator.py
--rw-r--r--   0        0        0     2420 2023-04-25 21:47:28.984426 hpc_beeflow-0.1.6/beeflow/common/connection.py
--rw-r--r--   0        0        0      947 2023-04-25 21:47:28.984512 hpc_beeflow-0.1.6/beeflow/common/container_path.py
--rw-r--r--   0        0        0     7091 2023-12-08 20:10:05.997206 hpc_beeflow-0.1.6/beeflow/common/crt/charliecloud_driver.py
--rw-r--r--   0        0        0     1487 2023-04-25 21:47:28.984782 hpc_beeflow-0.1.6/beeflow/common/crt/crt_driver.py
--rw-r--r--   0        0        0     1767 2023-04-25 21:47:28.984875 hpc_beeflow-0.1.6/beeflow/common/crt/singularity_driver.py
--rw-r--r--   0        0        0     1551 2023-04-25 21:47:28.985006 hpc_beeflow-0.1.6/beeflow/common/crt_interface.py
--rw-r--r--   0        0        0     2486 2023-12-08 20:10:05.997566 hpc_beeflow-0.1.6/beeflow/common/db/bdb.py
--rw-r--r--   0        0        0     1675 2023-04-25 21:47:28.985202 hpc_beeflow-0.1.6/beeflow/common/db/sched_db.py
--rw-r--r--   0        0        0     5075 2023-04-25 21:47:28.985280 hpc_beeflow-0.1.6/beeflow/common/db/tm_db.py
--rw-r--r--   0        0        0     8816 2023-12-08 20:10:43.774609 hpc_beeflow-0.1.6/beeflow/common/db/wfm_db.py
--rw-r--r--   0        0        0     2133 2023-04-25 21:47:28.985469 hpc_beeflow-0.1.6/beeflow/common/expr.py
--rw-r--r--   0        0        0     5924 2023-04-25 21:47:28.985612 hpc_beeflow-0.1.6/beeflow/common/gdb/DESIGN.md
--rw-r--r--   0        0        0     8239 2023-04-25 21:47:28.985717 hpc_beeflow-0.1.6/beeflow/common/gdb/gdb_driver.py
--rw-r--r--   0        0        0    23358 2023-12-08 20:10:05.998035 hpc_beeflow-0.1.6/beeflow/common/gdb/neo4j_cypher.py
--rw-r--r--   0        0        0    22756 2023-04-25 21:47:28.985994 hpc_beeflow-0.1.6/beeflow/common/gdb/neo4j_driver.py
--rw-r--r--   0        0        0     9736 2023-04-25 21:47:28.989071 hpc_beeflow-0.1.6/beeflow/common/gdb_interface.py
--rw-r--r--   0        0        0      642 2023-04-25 21:47:28.989144 hpc_beeflow-0.1.6/beeflow/common/log.py
--rw-r--r--   0        0        0       16 2023-04-25 21:47:28.989234 hpc_beeflow-0.1.6/beeflow/common/parser/.gitignore
--rw-r--r--   0        0        0     2614 2023-04-25 21:47:28.989307 hpc_beeflow-0.1.6/beeflow/common/parser/README.md
--rw-r--r--   0        0        0      102 2023-04-25 21:47:28.989397 hpc_beeflow-0.1.6/beeflow/common/parser/__init__.py
--rw-r--r--   0        0        0    14666 2023-12-08 20:10:05.998473 hpc_beeflow-0.1.6/beeflow/common/parser/parser.py
--rw-r--r--   0        0        0     2162 2023-12-08 20:10:43.775285 hpc_beeflow-0.1.6/beeflow/common/paths.py
--rw-r--r--   0        0        0      450 2023-12-08 20:10:43.775388 hpc_beeflow-0.1.6/beeflow/common/states.py
--rw-r--r--   0        0        0      493 2023-04-25 21:47:28.989613 hpc_beeflow-0.1.6/beeflow/common/tab_completion.py
--rw-r--r--   0        0        0     1643 2023-05-05 17:47:06.279186 hpc_beeflow-0.1.6/beeflow/common/validation.py
--rw-r--r--   0        0        0    11402 2023-12-08 20:10:05.999515 hpc_beeflow-0.1.6/beeflow/common/wf_data.py
--rw-r--r--   0        0        0    11430 2023-12-08 20:10:05.999893 hpc_beeflow-0.1.6/beeflow/common/wf_interface.py
--rw-r--r--   0        0        0     1522 2023-04-25 21:47:28.989906 hpc_beeflow-0.1.6/beeflow/common/wf_profiler.py
--rw-r--r--   0        0        0      493 2023-04-25 21:47:28.990038 hpc_beeflow-0.1.6/beeflow/common/worker/README.md
--rw-r--r--   0        0        0      597 2023-12-08 20:10:06.000678 hpc_beeflow-0.1.6/beeflow/common/worker/__init__.py
--rw-r--r--   0        0        0     5048 2023-12-08 20:10:06.000892 hpc_beeflow-0.1.6/beeflow/common/worker/flux_worker.py
--rw-r--r--   0        0        0     2570 2023-04-25 21:47:28.990261 hpc_beeflow-0.1.6/beeflow/common/worker/lsf_worker.py
--rw-r--r--   0        0        0     1731 2023-04-25 21:47:28.990365 hpc_beeflow-0.1.6/beeflow/common/worker/simple_worker.py
--rw-r--r--   0        0        0     9863 2023-12-08 20:10:43.776029 hpc_beeflow-0.1.6/beeflow/common/worker/slurm_worker.py
--rw-r--r--   0        0        0     2899 2023-05-05 17:47:06.279519 hpc_beeflow-0.1.6/beeflow/common/worker/worker.py
--rw-r--r--   0        0        0     1794 2023-04-25 21:47:28.990669 hpc_beeflow-0.1.6/beeflow/common/worker_interface.py
--rw-r--r--   0        0        0     4301 2023-04-25 21:47:28.990832 hpc_beeflow-0.1.6/beeflow/data/cloud_templates/dora.jinja
--rw-r--r--   0        0        0      866 2023-04-25 21:47:28.990917 hpc_beeflow-0.1.6/beeflow/data/cloud_templates/dora.yaml
--rw-r--r--   0        0        0      414 2023-04-25 21:47:28.991033 hpc_beeflow-0.1.6/beeflow/data/cwl/README.md
--rw-r--r--   0        0        0     1281 2023-04-25 21:47:28.991144 hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/README.md
--rw-r--r--   0        0        0      315 2023-04-25 21:47:28.991254 hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/blast/README.md
--rw-r--r--   0        0        0      418 2023-04-25 21:47:28.991479 hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/blast/blast.yml
--rw-r--r--   0        0        0      423 2023-04-25 21:47:28.991551 hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/blast/blast_output.cwl
--rw-r--r--   0        0        0      300 2023-04-25 21:47:28.991624 hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/blast/blast_output_err.cwl
--rw-r--r--   0        0        0      410 2023-04-25 21:47:28.991690 hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/blast/blast_split.cwl
--rw-r--r--   0        0        0     2009 2023-06-21 15:39:49.291706 hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/blast/blast_wf.cwl
--rw-r--r--   0        0        0      559 2023-04-25 21:47:28.991833 hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/blast/blast_worker001.cwl
--rw-r--r--   0        0        0      559 2023-04-25 21:47:28.991901 hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/blast/blast_worker002.cwl
--rwxr-xr-x   0        0        0   930997 2023-04-25 21:47:28.994579 hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/blast/input/small.fasta
--rw-r--r--   0        0        0       77 2023-12-08 20:10:43.776533 hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/cat-grep-fail/README.md
--rw-r--r--   0        0        0      258 2023-12-08 20:10:43.776920 hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/cat-grep-fail/cat.cwl
--rw-r--r--   0        0        0      272 2023-12-08 20:10:43.777135 hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/cat-grep-fail/grep0.cwl
--rw-r--r--   0        0        0      272 2023-12-08 20:10:43.777245 hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/cat-grep-fail/grep1.cwl
--rw-r--r--   0        0        0       76 2023-12-08 20:10:43.777342 hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/cat-grep-fail/input.yml
--rw-r--r--   0        0        0     3215 2023-12-08 20:10:43.777466 hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/cat-grep-fail/lorem.txt
--rw-r--r--   0        0        0      422 2023-12-08 20:10:43.777824 hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/cat-grep-fail/tar.cwl
--rw-r--r--   0        0        0      710 2023-12-08 20:10:43.778250 hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/cat-grep-fail/workflow.cwl
--rw-r--r--   0        0        0      350 2023-04-25 21:47:28.994706 hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/clamr-ci/README.md
--rw-r--r--   0        0        0     1968 2023-04-25 21:47:28.994777 hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/clamr-ci/clamr.cwl
--rw-r--r--   0        0        0      302 2023-04-25 21:47:28.994847 hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/clamr-ci/clamr_job.json
--rw-r--r--   0        0        0      429 2023-04-25 21:47:28.994926 hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/clamr-ci/clamr_job.yml
--rw-r--r--   0        0        0     2228 2023-04-25 21:47:28.995018 hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/clamr-ci/clamr_wf.cwl
--rw-r--r--   0        0        0      765 2023-04-25 21:47:28.995094 hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/clamr-ci/ffmpeg.cwl
--rw-r--r--   0        0        0      350 2023-04-25 21:47:28.999935 hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/clamr-wf/README.md
--rw-r--r--   0        0        0     1977 2023-04-25 21:47:29.000007 hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/clamr-wf/clamr.cwl
--rw-r--r--   0        0        0      302 2023-04-25 21:47:29.000067 hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/clamr-wf/clamr_job.json
--rw-r--r--   0        0        0      455 2023-04-25 21:47:29.000130 hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/clamr-wf/clamr_job.yml
--rw-r--r--   0        0        0     2145 2023-04-25 21:47:29.000192 hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/clamr-wf/clamr_wf.cwl
--rw-r--r--   0        0        0      815 2023-04-25 21:47:29.000252 hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/clamr-wf/ffmpeg.cwl
--rw-r--r--   0        0        0      411 2023-05-05 17:47:06.279682 hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/clamr-wf-checkpoint/Dockerfile.clamr-ffmpeg
--rw-r--r--   0        0        0      350 2023-04-25 21:47:28.995216 hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/clamr-wf-checkpoint/README.md
--rw-r--r--   0        0        0     2064 2023-05-05 17:47:06.279832 hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/clamr-wf-checkpoint/clamr.cwl
--rw-r--r--   0        0        0      339 2023-04-25 21:47:28.995402 hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/clamr-wf-checkpoint/clamr_job.json
--rw-r--r--   0        0        0      454 2023-04-25 21:47:28.995475 hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/clamr-wf-checkpoint/clamr_job.yml
--rw-r--r--   0        0        0      339 2023-04-25 21:47:28.995543 hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/clamr-wf-checkpoint/clamr_job_long.yml
--rw-r--r--   0        0        0     2524 2023-05-05 17:47:06.279976 hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/clamr-wf-checkpoint/clamr_wf.cwl
--rw-r--r--   0        0        0      765 2023-04-25 21:47:28.995695 hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/clamr-wf-checkpoint/ffmpeg.cwl
--rw-r--r--   0        0        0      383 2023-04-25 21:47:28.995807 hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/clamr-wf-chicoma/README.md
--rw-r--r--   0        0        0     1962 2023-04-25 21:47:28.995893 hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/clamr-wf-chicoma/clamr.cwl
--rw-r--r--   0        0        0      302 2023-04-25 21:47:28.995962 hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/clamr-wf-chicoma/clamr_job.json
--rw-r--r--   0        0        0      411 2023-04-25 21:47:28.996043 hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/clamr-wf-chicoma/clamr_job.yml
--rw-r--r--   0        0        0     2006 2023-04-25 21:47:28.996110 hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/clamr-wf-chicoma/clamr_wf.cwl
--rw-r--r--   0        0        0      753 2023-04-25 21:47:28.996179 hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/clamr-wf-chicoma/ffmpeg.cwl
--rw-r--r--   0        0        0      837 2023-04-25 21:47:28.996296 hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/README.md
--rw-r--r--   0        0        0      304 2023-04-25 21:47:28.996464 hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/lsf-charliecloud/README.md
--rw-r--r--   0        0        0     1234 2023-04-25 21:47:28.996562 hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/lsf-charliecloud/cf-summit.cwl
--rw-r--r--   0        0        0      145 2023-04-25 21:47:28.996681 hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/slurm-charliecloud/Dockerfile.clamr-lanl-x86_64
--rw-r--r--   0        0        0     3325 2023-04-25 21:47:28.996775 hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/slurm-charliecloud/README.md
--rw-r--r--   0        0        0     1127 2023-04-25 21:47:28.996851 hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/slurm-charliecloud/cf-darwin.cwl
--rw-r--r--   0        0        0     1135 2023-04-25 21:47:28.996921 hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/slurm-charliecloud/cf-no-owrite.cwl
--rw-r--r--   0        0        0     1137 2023-04-25 21:47:28.996990 hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/slurm-charliecloud/cf.cwl
--rw-r--r--   0        0        0     1176 2023-04-25 21:47:28.997063 hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/slurm-charliecloud/copyContainer_containerName.cwl
--rw-r--r--   0        0        0     1137 2023-04-25 21:47:28.997136 hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/slurm-charliecloud/dockerFile_containerName.cwl
--rw-r--r--   0        0        0     1133 2023-04-25 21:47:28.997217 hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/slurm-charliecloud/dockerPull.cwl
--rw-r--r--   0        0        0      182 2023-04-25 21:47:28.997348 hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/slurm-singularity/README.md
--rw-r--r--   0        0        0     1122 2023-04-25 21:47:28.997441 hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/slurm-singularity/cf-singularity.cwl
--rw-r--r--   0        0        0      303 2023-04-25 21:47:28.997562 hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/clamr-wf-singularity/README.md
--rw-r--r--   0        0        0     1975 2023-04-25 21:47:28.997639 hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/clamr-wf-singularity/clamr.cwl
--rw-r--r--   0        0        0      302 2023-04-25 21:47:28.997705 hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/clamr-wf-singularity/clamr_job.json
--rw-r--r--   0        0        0      418 2023-04-25 21:47:28.997783 hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/clamr-wf-singularity/clamr_job.yml
--rw-r--r--   0        0        0     2057 2023-04-25 21:47:28.997856 hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/clamr-wf-singularity/clamr_wf.cwl
--rw-r--r--   0        0        0      768 2023-04-25 21:47:28.997935 hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/clamr-wf-singularity/ffmpeg.cwl
--rw-r--r--   0        0        0      339 2023-04-25 21:47:28.998055 hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/clamr-wf-summit/README.md
--rw-r--r--   0        0        0     1962 2023-04-25 21:47:28.998134 hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/clamr-wf-summit/clamr.cwl
--rw-r--r--   0        0        0      302 2023-04-25 21:47:28.998270 hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/clamr-wf-summit/clamr_job.json
--rw-r--r--   0        0        0      418 2023-04-25 21:47:28.998350 hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/clamr-wf-summit/clamr_job.yml
--rw-r--r--   0        0        0     2103 2023-04-25 21:47:28.998435 hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/clamr-wf-summit/clamr_wf.cwl
--rw-r--r--   0        0        0      765 2023-04-25 21:47:28.998522 hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/clamr-wf-summit/ffmpeg.cwl
--rw-r--r--   0        0        0      350 2023-04-25 21:47:28.998645 hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/clamr-wf-use-container/README.md
--rw-r--r--   0        0        0     1981 2023-04-25 21:47:28.998789 hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/clamr-wf-use-container/clamr.cwl
--rw-r--r--   0        0        0      302 2023-04-25 21:47:28.999069 hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/clamr-wf-use-container/clamr_job.json
--rw-r--r--   0        0        0      430 2023-04-25 21:47:28.999155 hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/clamr-wf-use-container/clamr_job.yml
--rw-r--r--   0        0        0     1939 2023-04-25 21:47:28.999246 hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/clamr-wf-use-container/clamr_wf.cwl
--rw-r--r--   0        0        0      765 2023-04-25 21:47:28.999771 hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/clamr-wf-use-container/ffmpeg.cwl
--rw-r--r--   0        0        0      527 2023-04-25 21:47:29.000349 hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/comd-mpi/comd.cwl
--rw-r--r--   0        0        0      110 2023-04-25 21:47:29.000417 hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/comd-mpi/comd_job.yml
--rw-r--r--   0        0        0      555 2023-04-25 21:47:29.000482 hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/comd-mpi/comd_wf.cwl
--rw-r--r--   0        0        0      831 2023-04-25 21:47:29.000913 hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/lulesh-mpi/lulesh.cwl
--rw-r--r--   0        0        0       24 2023-04-25 21:47:29.001008 hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/lulesh-mpi/lulesh.yml
--rw-r--r--   0        0        0      264 2023-04-25 21:47:29.000577 hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/lulesh-mpi-multi-file/lulesh.cwl
--rw-r--r--   0        0        0       24 2023-04-25 21:47:29.000669 hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/lulesh-mpi-multi-file/lulesh_job.yml
--rw-r--r--   0        0        0      469 2023-04-25 21:47:29.000773 hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/lulesh-mpi-multi-file/lulesh_wf.cwl
--rw-r--r--   0        0        0     1282 2023-04-25 21:47:29.001147 hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/nwchem-mpi/README.md
--rw-r--r--   0        0        0      590 2023-04-25 21:47:29.001253 hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/nwchem-mpi/nwchem.cwl
--rw-r--r--   0        0        0      161 2023-04-25 21:47:29.001325 hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/nwchem-mpi/nwchem.yml
--rw-r--r--   0        0        0      199 2023-04-25 21:47:29.001386 hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/nwchem-mpi/nwchem_bin.cwl
--rw-r--r--   0        0        0      344 2023-12-08 20:10:06.005042 hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/pennant/graph.cwl
--rw-r--r--   0        0        0       43 2023-12-08 20:10:06.005318 hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/pennant/pennant.yml
--rw-r--r--   0        0        0      192 2023-12-08 20:10:06.005476 hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/pennant/pennant_1_node.cwl
--rw-r--r--   0        0        0      192 2023-12-08 20:10:06.005624 hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/pennant/pennant_2_node.cwl
--rw-r--r--   0        0        0      192 2023-12-08 20:10:06.005790 hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/pennant/pennant_4_node.cwl
--rw-r--r--   0        0        0     1217 2023-12-08 20:10:06.006671 hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/pennant/pennant_wf.cwl
--rw-r--r--   0        0        0     3881 2023-12-08 20:10:06.001642 hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/pennant-build/Dockerfile.pennant-flux-x86_64
--rw-r--r--   0        0        0      789 2023-12-08 20:10:06.002162 hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/pennant-build/Dockerfile.pennant-graph-x86_64
--rw-r--r--   0        0        0      407 2023-12-08 20:10:06.002802 hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/pennant-build/graph.cwl
--rw-r--r--   0        0        0     1294 2023-12-08 20:10:06.002984 hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/pennant-build/graph_pennant.py
--rw-r--r--   0        0        0      110 2023-12-08 20:10:06.003364 hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/pennant-build/graph_pennant.sh
--rw-r--r--   0        0        0       43 2023-12-08 20:10:06.003854 hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/pennant-build/pennant.yml
--rw-r--r--   0        0        0      192 2023-12-08 20:10:06.004022 hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/pennant-build/pennant_1_node.cwl
--rw-r--r--   0        0        0      192 2023-12-08 20:10:06.004148 hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/pennant-build/pennant_2_node.cwl
--rw-r--r--   0        0        0      192 2023-12-08 20:10:06.004309 hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/pennant-build/pennant_4_node.cwl
--rw-r--r--   0        0        0      192 2023-12-08 20:10:06.004448 hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/pennant-build/pennant_8_node.cwl
--rw-r--r--   0        0        0     1741 2023-12-08 20:10:06.004817 hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/pennant-build/pennant_wf.cwl
--rw-r--r--   0        0        0       71 2023-04-25 21:47:29.001443 hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/pytest.ini
--rw-r--r--   0        0        0      317 2023-04-25 21:47:29.001539 hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/simple-workflows/README.md
--rw-r--r--   0        0        0      986 2023-04-25 21:47:29.001615 hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/simple-workflows/cancel.cwl
--rw-r--r--   0        0        0      217 2023-04-25 21:47:29.001709 hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/simple-workflows/grep-wordcount/README.md
--rw-r--r--   0        0        0     1083 2023-04-25 21:47:29.001774 hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/simple-workflows/grep-wordcount/gc-nc.cwl
--rw-r--r--   0        0        0     1325 2023-04-25 21:47:29.001854 hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/simple-workflows/grep-wordcount/gc.cwl
--rw-r--r--   0        0        0     3776 2023-04-25 21:47:29.001951 hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/simple-workflows/grep-wordcount/lorem.txt
--rw-r--r--   0        0        0      426 2023-04-25 21:47:29.002093 hpc_beeflow-0.1.6/beeflow/data/cwl/cwl_validation/README.md
--rwxr-xr-x   0        0        0      398 2023-04-25 21:47:29.002238 hpc_beeflow-0.1.6/beeflow/data/cwl/cwl_validation/builder/dockerFile.cwl
--rwxr-xr-x   0        0        0      317 2023-04-25 21:47:29.002333 hpc_beeflow-0.1.6/beeflow/data/cwl/cwl_validation/builder/dockerPull.cwl
--rw-r--r--   0        0        0     1202 2023-04-25 21:47:29.002463 hpc_beeflow-0.1.6/beeflow/data/cwl/cwl_validation/grep-wordcount/gc.cwl
--rw-r--r--   0        0        0     3776 2023-04-25 21:47:29.002550 hpc_beeflow-0.1.6/beeflow/data/cwl/cwl_validation/grep-wordcount/lorem.txt
--rwxr-xr-x   0        0        0      169 2023-04-25 21:47:29.002620 hpc_beeflow-0.1.6/beeflow/data/cwl/cwl_validation/helloworld.cwl
--rw-r--r--   0        0        0       19 2023-04-25 21:47:29.002681 hpc_beeflow-0.1.6/beeflow/data/cwl/cwl_validation/helloworld_input.yaml
--rw-r--r--   0        0        0    59407 2023-04-25 21:47:29.003142 hpc_beeflow-0.1.6/beeflow/data/cwl/cwl_validation/ml-workflow/example-1/DAG_example-1.png
--rw-r--r--   0        0        0      833 2023-04-25 21:47:29.003262 hpc_beeflow-0.1.6/beeflow/data/cwl/cwl_validation/ml-workflow/example-1/README.md
--rw-r--r--   0        0        0      254 2023-04-25 21:47:29.003333 hpc_beeflow-0.1.6/beeflow/data/cwl/cwl_validation/ml-workflow/example-1/add.cwl
--rw-r--r--   0        0        0      351 2023-04-25 21:47:29.003405 hpc_beeflow-0.1.6/beeflow/data/cwl/cwl_validation/ml-workflow/example-1/add_multiply_example_workflow.cwl
--rw-r--r--   0        0        0      245 2023-04-25 21:47:29.003482 hpc_beeflow-0.1.6/beeflow/data/cwl/cwl_validation/ml-workflow/example-1/add_step1.py
--rw-r--r--   0        0        0      386 2023-04-25 21:47:29.003555 hpc_beeflow-0.1.6/beeflow/data/cwl/cwl_validation/ml-workflow/example-1/isolated test.cwl
--rw-r--r--   0        0        0       21 2023-04-25 21:47:29.003622 hpc_beeflow-0.1.6/beeflow/data/cwl/cwl_validation/ml-workflow/example-1/job.yaml
--rw-r--r--   0        0        0      304 2023-04-25 21:47:29.003687 hpc_beeflow-0.1.6/beeflow/data/cwl/cwl_validation/ml-workflow/example-1/multiply.cwl
--rw-r--r--   0        0        0      267 2023-04-25 21:47:29.003759 hpc_beeflow-0.1.6/beeflow/data/cwl/cwl_validation/ml-workflow/example-1/multiply_step2.py
--rw-r--r--   0        0        0      407 2023-04-25 21:47:29.003840 hpc_beeflow-0.1.6/beeflow/data/cwl/cwl_validation/ml-workflow/example-1/workflow_generater_python.py
--rw-r--r--   0        0        0     3496 2023-04-25 21:47:29.003994 hpc_beeflow-0.1.6/beeflow/data/cwl/cwl_validation/ml-workflow/machine_learning/README.md
--rw-r--r--   0        0        0      901 2023-04-25 21:47:29.004107 hpc_beeflow-0.1.6/beeflow/data/cwl/cwl_validation/ml-workflow/machine_learning/decision_tree.py
--rw-r--r--   0        0        0      443 2023-04-25 21:47:29.004204 hpc_beeflow-0.1.6/beeflow/data/cwl/cwl_validation/ml-workflow/machine_learning/decision_tree_output.txt
--rw-r--r--   0        0        0      234 2023-04-25 21:47:29.004308 hpc_beeflow-0.1.6/beeflow/data/cwl/cwl_validation/ml-workflow/machine_learning/decision_tree_tool.cwl
--rw-r--r--   0        0        0      178 2023-04-25 21:47:29.004411 hpc_beeflow-0.1.6/beeflow/data/cwl/cwl_validation/ml-workflow/machine_learning/expectedValue.txt
--rw-r--r--   0        0        0      157 2023-04-25 21:47:29.004497 hpc_beeflow-0.1.6/beeflow/data/cwl/cwl_validation/ml-workflow/machine_learning/hiring1.txt
--rw-r--r--   0        0        0      467 2023-04-25 21:47:29.004576 hpc_beeflow-0.1.6/beeflow/data/cwl/cwl_validation/ml-workflow/machine_learning/linear_regress_output.txt
--rw-r--r--   0        0        0     1203 2023-04-25 21:47:29.004690 hpc_beeflow-0.1.6/beeflow/data/cwl/cwl_validation/ml-workflow/machine_learning/linear_regression.py
--rw-r--r--   0        0        0      692 2023-04-25 21:47:29.004786 hpc_beeflow-0.1.6/beeflow/data/cwl/cwl_validation/ml-workflow/machine_learning/machinelearning_pipeline.cwl
--rw-r--r--   0        0        0    12405 2023-04-25 21:47:29.004908 hpc_beeflow-0.1.6/beeflow/data/cwl/cwl_validation/ml-workflow/machine_learning/out.PNG
--rw-r--r--   0        0        0     1517 2023-04-25 21:47:29.005030 hpc_beeflow-0.1.6/beeflow/data/cwl/cwl_validation/ml-workflow/machine_learning/predict_code.py
--rw-r--r--   0        0        0      336 2023-04-25 21:47:29.005110 hpc_beeflow-0.1.6/beeflow/data/cwl/cwl_validation/ml-workflow/machine_learning/predict_tool.cwl
--rw-r--r--   0        0        0     1054 2023-04-25 21:47:29.005209 hpc_beeflow-0.1.6/beeflow/data/cwl/cwl_validation/ml-workflow/machine_learning/read_dataset.py
--rw-r--r--   0        0        0      235 2023-04-25 21:47:29.005315 hpc_beeflow-0.1.6/beeflow/data/cwl/cwl_validation/ml-workflow/machine_learning/read_dataset_tool.cwl
--rw-r--r--   0        0        0      239 2023-04-25 21:47:29.005398 hpc_beeflow-0.1.6/beeflow/data/cwl/cwl_validation/ml-workflow/machine_learning/regress_tool.cwl
--rw-r--r--   0        0        0       80 2023-04-25 21:47:29.005519 hpc_beeflow-0.1.6/beeflow/data/dockerfiles/Dockerfile.builder_demo
--rw-r--r--   0        0        0      411 2023-04-25 21:47:29.005642 hpc_beeflow-0.1.6/beeflow/data/dockerfiles/Dockerfile.clamr-ffmpeg
--rw-r--r--   0        0        0      145 2023-04-25 21:47:29.005725 hpc_beeflow-0.1.6/beeflow/data/dockerfiles/Dockerfile.clamr-lanl-x86_64
--rw-r--r--   0        0        0      724 2023-04-25 21:47:29.005802 hpc_beeflow-0.1.6/beeflow/data/dockerfiles/Dockerfile.clamr-ppc64le
--rw-r--r--   0        0        0     3698 2023-12-08 20:10:06.006955 hpc_beeflow-0.1.6/beeflow/data/dockerfiles/Dockerfile.comd-flux-x86_64
--rw-r--r--   0        0        0     2303 2023-04-25 21:47:29.005907 hpc_beeflow-0.1.6/beeflow/data/dockerfiles/Dockerfile.comd-x86_64
--rw-r--r--   0        0        0      270 2023-04-25 21:47:29.005992 hpc_beeflow-0.1.6/beeflow/data/dockerfiles/Dockerfile.deb9ompi-x86_64
--rw-r--r--   0        0        0     2592 2023-04-25 21:47:29.006062 hpc_beeflow-0.1.6/beeflow/data/dockerfiles/Dockerfile.lulesh-x86_64
--rw-r--r--   0        0        0     1605 2023-04-25 21:47:29.006164 hpc_beeflow-0.1.6/beeflow/data/dockerfiles/Dockerfile.neo4j-ppc64le
--rw-r--r--   0        0        0     2489 2023-04-25 21:47:29.006269 hpc_beeflow-0.1.6/beeflow/data/dockerfiles/Dockerfile.nwchem-x86_64
--rw-r--r--   0        0        0     3881 2023-12-08 20:10:06.007207 hpc_beeflow-0.1.6/beeflow/data/dockerfiles/Dockerfile.pennant-flux-x86_64
--rw-r--r--   0        0        0     3446 2023-04-25 21:47:29.006374 hpc_beeflow-0.1.6/beeflow/data/dockerfiles/Dockerfile.vaspompi-x86_64
--rw-r--r--   0        0        0      614 2023-04-25 21:47:29.006482 hpc_beeflow-0.1.6/beeflow/data/dockerfiles/README.md
--rw-r--r--   0        0        0      331 2023-04-25 21:47:29.006618 hpc_beeflow-0.1.6/beeflow/data/dockerfiles/comd-pmix-support/Dockerfile.comd-x86_64-wpmix
--rw-r--r--   0        0        0      573 2023-04-25 21:47:29.006711 hpc_beeflow-0.1.6/beeflow/data/dockerfiles/comd-pmix-support/Dockerfile.debian
--rw-r--r--   0        0        0     3941 2023-04-25 21:47:29.006821 hpc_beeflow-0.1.6/beeflow/data/dockerfiles/comd-pmix-support/Dockerfile.openmpi-3.1.5
--rw-r--r--   0        0        0      509 2023-04-25 21:47:29.006927 hpc_beeflow-0.1.6/beeflow/data/dockerfiles/comd-pmix-support/README.md
--rw-r--r--   0        0        0      813 2023-04-25 21:47:29.007028 hpc_beeflow-0.1.6/beeflow/data/dockerfiles/comd-pmix-support/dont-init-ucx-on-intel-cray.patch
--rw-r--r--   0        0        0      789 2023-12-08 20:10:06.007513 hpc_beeflow-0.1.6/beeflow/data/dockerfiles/pennant-graph/Dockerfile.pennant-graph-x86_64
--rw-r--r--   0        0        0     1294 2023-12-08 20:10:06.007705 hpc_beeflow-0.1.6/beeflow/data/dockerfiles/pennant-graph/graph_pennant.py
--rw-r--r--   0        0        0      110 2023-12-08 20:10:06.007942 hpc_beeflow-0.1.6/beeflow/data/dockerfiles/pennant-graph/graph_pennant.sh
--rw-r--r--   0        0        0      640 2023-04-25 21:47:29.007462 hpc_beeflow-0.1.6/beeflow/enhanced_client/README.rst
--rw-r--r--   0        0        0        0 2023-04-25 21:47:29.007581 hpc_beeflow-0.1.6/beeflow/enhanced_client/data/.gitkeep
--rw-r--r--   0        0        0      386 2023-04-25 21:47:29.007687 hpc_beeflow-0.1.6/beeflow/enhanced_client/forge.config.js
--rw-r--r--   0        0        0     1682 2023-04-25 21:47:29.007800 hpc_beeflow-0.1.6/beeflow/enhanced_client/main.js
--rw-r--r--   0        0        0   231716 2023-12-08 20:10:43.779935 hpc_beeflow-0.1.6/beeflow/enhanced_client/package-lock.json
--rw-r--r--   0        0        0     1078 2023-12-08 20:10:43.780944 hpc_beeflow-0.1.6/beeflow/enhanced_client/package.json
--rw-r--r--   0        0        0     1219 2023-04-25 21:47:29.008916 hpc_beeflow-0.1.6/beeflow/enhanced_client/renderer/app.js
--rw-r--r--   0        0        0     5151 2023-04-25 21:47:29.009061 hpc_beeflow-0.1.6/beeflow/enhanced_client/renderer/client.js
--rw-r--r--   0        0        0      872 2023-04-25 21:47:29.009162 hpc_beeflow-0.1.6/beeflow/enhanced_client/renderer/config.js
--rw-r--r--   0        0        0     2013 2023-04-25 21:47:29.009273 hpc_beeflow-0.1.6/beeflow/enhanced_client/renderer/control.js
--rw-r--r--   0        0        0     3610 2023-04-25 21:47:29.009393 hpc_beeflow-0.1.6/beeflow/enhanced_client/renderer/database.js
--rw-r--r--   0        0        0    12140 2023-04-25 21:47:29.009519 hpc_beeflow-0.1.6/beeflow/enhanced_client/renderer/display.js
--rw-r--r--   0        0        0      455 2023-04-25 21:47:29.009613 hpc_beeflow-0.1.6/beeflow/enhanced_client/renderer/gdb.js
--rw-r--r--   0        0        0    33601 2023-04-25 21:47:29.009934 hpc_beeflow-0.1.6/beeflow/enhanced_client/renderer/img/logo.png
--rw-r--r--   0        0        0     2751 2023-04-25 21:47:29.010080 hpc_beeflow-0.1.6/beeflow/enhanced_client/renderer/main.html
--rw-r--r--   0        0        0   206620 2023-04-25 21:47:29.010757 hpc_beeflow-0.1.6/beeflow/enhanced_client/renderer/styles/bulma.min.css
--rw-r--r--   0        0        0      374 2023-04-25 21:47:29.010868 hpc_beeflow-0.1.6/beeflow/enhanced_client/renderer/styles/main.css
--rw-r--r--   0        0        0      498 2023-04-25 21:47:29.010960 hpc_beeflow-0.1.6/beeflow/enhanced_client/renderer/tunnel.js
--rw-r--r--   0        0        0      428 2023-04-25 21:47:29.011047 hpc_beeflow-0.1.6/beeflow/enhanced_client/renderer/viz.html
--rw-r--r--   0        0        0     1071 2023-04-25 21:47:29.011146 hpc_beeflow-0.1.6/beeflow/enhanced_client/renderer/viz.js
--rw-r--r--   0        0        0     7603 2023-04-25 21:47:29.011257 hpc_beeflow-0.1.6/beeflow/enhanced_client/renderer/workflows.js
--rw-r--r--   0        0        0     1708 2023-04-25 21:47:29.011551 hpc_beeflow-0.1.6/beeflow/scheduler/README.md
--rw-r--r--   0        0        0    10098 2023-04-25 21:47:29.011762 hpc_beeflow-0.1.6/beeflow/scheduler/algorithms.py
--rw-r--r--   0        0        0     9347 2023-04-25 21:47:29.011888 hpc_beeflow-0.1.6/beeflow/scheduler/resource_allocation.py
--rw-r--r--   0        0        0     3738 2023-12-08 20:10:06.008417 hpc_beeflow-0.1.6/beeflow/scheduler/scheduler.py
--rw-r--r--   0        0        0     2890 2023-04-25 21:47:29.012145 hpc_beeflow-0.1.6/beeflow/scheduler/scheduler.yaml
--rw-r--r--   0        0        0      708 2023-04-25 21:47:29.012263 hpc_beeflow-0.1.6/beeflow/scheduler/serializable.py
--rw-r--r--   0        0        0     2296 2023-04-25 21:47:29.012364 hpc_beeflow-0.1.6/beeflow/scheduler/task.py
--rwxr-xr-x   0        0        0    12833 2023-12-08 20:10:43.781478 hpc_beeflow-0.1.6/beeflow/task_manager.py
--rw-r--r--   0        0        0    34925 2023-04-25 21:47:29.012805 hpc_beeflow-0.1.6/beeflow/tests/42.tgz
--rw-r--r--   0        0        0      236 2023-04-25 21:47:29.012980 hpc_beeflow-0.1.6/beeflow/tests/README.md
--rw-r--r--   0        0        0     1139 2023-04-25 21:47:29.013070 hpc_beeflow-0.1.6/beeflow/tests/cf.cwl
--rw-r--r--   0        0        0     1093 2023-04-25 21:47:29.013282 hpc_beeflow-0.1.6/beeflow/tests/clamr-wf/clamr.cwl
--rw-r--r--   0        0        0      302 2023-04-25 21:47:29.013394 hpc_beeflow-0.1.6/beeflow/tests/clamr-wf/clamr_job.json
--rw-r--r--   0        0        0      424 2023-04-25 21:47:29.013478 hpc_beeflow-0.1.6/beeflow/tests/clamr-wf/clamr_job.yml
--rw-r--r--   0        0        0     1320 2023-04-25 21:47:29.013567 hpc_beeflow-0.1.6/beeflow/tests/clamr-wf/clamr_wf.cwl
--rw-r--r--   0        0        0      680 2023-04-25 21:47:29.013641 hpc_beeflow-0.1.6/beeflow/tests/clamr-wf/ffmpeg.cwl
--rw-r--r--   0        0        0      273 2023-04-25 21:47:29.013735 hpc_beeflow-0.1.6/beeflow/tests/clamr-wf/mv_script.cwl
--rwxr-xr-x   0        0        0      324 2023-04-25 21:47:29.013817 hpc_beeflow-0.1.6/beeflow/tests/clamr-wf/mv_script.sh
--rw-r--r--   0        0        0     2401 2023-04-25 21:47:29.013156 hpc_beeflow-0.1.6/beeflow/tests/clamr-wf.tgz
--rw-r--r--   0        0        0      774 2023-04-25 21:47:29.013918 hpc_beeflow-0.1.6/beeflow/tests/gdb.py
--rw-r--r--   0        0        0    12378 2023-04-25 21:47:29.014045 hpc_beeflow-0.1.6/beeflow/tests/mocks.py
--rw-r--r--   0        0        0      267 2023-04-25 21:47:29.014151 hpc_beeflow-0.1.6/beeflow/tests/test_cloud.py
--rw-r--r--   0        0        0     6006 2023-04-25 21:47:29.014267 hpc_beeflow-0.1.6/beeflow/tests/test_config_validator.py
--rw-r--r--   0        0        0      807 2023-04-25 21:47:29.014348 hpc_beeflow-0.1.6/beeflow/tests/test_container_path.py
--rw-r--r--   0        0        0      946 2023-04-25 21:47:29.014440 hpc_beeflow-0.1.6/beeflow/tests/test_db_sched.py
--rw-r--r--   0        0        0     4410 2023-04-25 21:47:29.014548 hpc_beeflow-0.1.6/beeflow/tests/test_db_tm.py
--rw-r--r--   0        0        0     9772 2023-12-08 20:10:06.009230 hpc_beeflow-0.1.6/beeflow/tests/test_parser.py
--rw-r--r--   0        0        0    15134 2023-04-25 21:47:29.014766 hpc_beeflow-0.1.6/beeflow/tests/test_scheduler.py
--rw-r--r--   0        0        0     2630 2023-04-25 21:47:29.014849 hpc_beeflow-0.1.6/beeflow/tests/test_scheduler_resource_allocation.py
--rw-r--r--   0        0        0     6557 2023-04-25 21:47:29.014958 hpc_beeflow-0.1.6/beeflow/tests/test_scheduler_rest.py
--rw-r--r--   0        0        0     4908 2023-12-08 20:10:43.782077 hpc_beeflow-0.1.6/beeflow/tests/test_slurm_worker.py
--rw-r--r--   0        0        0     3704 2023-04-25 21:47:29.015183 hpc_beeflow-0.1.6/beeflow/tests/test_tm.py
--rw-r--r--   0        0        0    33819 2023-12-08 20:10:06.010198 hpc_beeflow-0.1.6/beeflow/tests/test_wf_interface.py
--rw-r--r--   0        0        0    10108 2023-12-08 20:10:43.782756 hpc_beeflow-0.1.6/beeflow/tests/test_wf_manager.py
--rwxr-xr-x   0        0        0     7823 2023-12-08 20:10:43.783149 hpc_beeflow-0.1.6/beeflow/wf_manager/common/dep_manager.py
--rw-r--r--   0        0        0    10373 2023-12-08 20:10:43.783470 hpc_beeflow-0.1.6/beeflow/wf_manager/common/wf_db.py
--rw-r--r--   0        0        0     4059 2023-12-08 20:10:43.783946 hpc_beeflow-0.1.6/beeflow/wf_manager/resources/wf_actions.py
--rw-r--r--   0        0        0     8674 2023-12-08 20:10:43.784247 hpc_beeflow-0.1.6/beeflow/wf_manager/resources/wf_list.py
--rw-r--r--   0        0        0      560 2023-04-25 21:47:29.016239 hpc_beeflow-0.1.6/beeflow/wf_manager/resources/wf_metadata.py
--rw-r--r--   0        0        0     5794 2023-12-08 20:10:43.784707 hpc_beeflow-0.1.6/beeflow/wf_manager/resources/wf_update.py
--rw-r--r--   0        0        0     8816 2023-12-08 20:10:43.785026 hpc_beeflow-0.1.6/beeflow/wf_manager/resources/wf_utils.py
--rw-r--r--   0        0        0     1793 2023-12-08 20:10:43.785360 hpc_beeflow-0.1.6/beeflow/wf_manager/wf_manager.py
--rw-r--r--   0        0        0     2739 2023-12-08 20:10:43.788404 hpc_beeflow-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     7085 1970-01-01 00:00:00.000000 hpc_beeflow-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1477 2024-03-28 22:16:36.348299 hpc-beeflow-0.1.7/LICENSE
+-rw-r--r--   0        0        0     5235 2024-03-29 16:50:01.342051 hpc-beeflow-0.1.7/README.rst
+-rw-r--r--   0        0        0      122 2024-03-28 22:16:36.349367 hpc-beeflow-0.1.7/beeflow/client/README.md
+-rw-r--r--   0        0        0    22324 2024-03-29 16:50:01.343590 hpc-beeflow-0.1.7/beeflow/client/bee_client.py
+-rw-r--r--   0        0        0    23683 2024-03-29 16:50:01.344218 hpc-beeflow-0.1.7/beeflow/client/core.py
+-rw-r--r--   0        0        0     8036 2024-03-28 22:16:36.350389 hpc-beeflow-0.1.7/beeflow/cloud_launcher.py
+-rw-r--r--   0        0        0      234 2024-03-28 22:16:36.350628 hpc-beeflow-0.1.7/beeflow/common/README.md
+-rw-r--r--   0        0        0      459 2024-03-28 22:16:36.350800 hpc-beeflow-0.1.7/beeflow/common/api.py
+-rw-r--r--   0        0        0    11473 2024-03-28 22:16:36.351063 hpc-beeflow-0.1.7/beeflow/common/build/README.md
+-rw-r--r--   0        0        0     5116 2024-03-29 16:50:01.344806 hpc-beeflow-0.1.7/beeflow/common/build/build_driver.py
+-rw-r--r--   0        0        0    19130 2024-03-29 16:50:01.345249 hpc-beeflow-0.1.7/beeflow/common/build/container_drivers.py
+-rw-r--r--   0        0        0      733 2024-03-29 16:50:01.345495 hpc-beeflow-0.1.7/beeflow/common/build/utils.py
+-rw-r--r--   0        0        0     3534 2024-03-29 16:50:01.346124 hpc-beeflow-0.1.7/beeflow/common/build_interfaces.py
+-rw-r--r--   0        0        0      163 2024-03-28 22:16:36.352417 hpc-beeflow-0.1.7/beeflow/common/celery.py
+-rw-r--r--   0        0        0      285 2024-03-28 22:16:36.352577 hpc-beeflow-0.1.7/beeflow/common/cli.py
+-rw-r--r--   0        0        0     3023 2024-03-28 22:16:36.352758 hpc-beeflow-0.1.7/beeflow/common/cli_connection.py
+-rw-r--r--   0        0        0     2542 2024-03-28 22:16:36.353108 hpc-beeflow-0.1.7/beeflow/common/cloud/README.md
+-rw-r--r--   0        0        0      830 2024-03-28 22:16:36.353287 hpc-beeflow-0.1.7/beeflow/common/cloud/__init__.py
+-rw-r--r--   0        0        0     1166 2024-03-28 22:16:36.353541 hpc-beeflow-0.1.7/beeflow/common/cloud/chameleoncloud.py
+-rw-r--r--   0        0        0      175 2024-03-28 22:16:36.353879 hpc-beeflow-0.1.7/beeflow/common/cloud/cloud.py
+-rw-r--r--   0        0        0       42 2024-03-28 22:16:36.354153 hpc-beeflow-0.1.7/beeflow/common/cloud/constants.py
+-rw-r--r--   0        0        0     1599 2024-03-28 22:16:36.354427 hpc-beeflow-0.1.7/beeflow/common/cloud/google.py
+-rw-r--r--   0        0        0     1093 2024-03-28 22:16:36.354593 hpc-beeflow-0.1.7/beeflow/common/cloud/openstack.py
+-rw-r--r--   0        0        0      784 2024-03-28 22:16:36.354764 hpc-beeflow-0.1.7/beeflow/common/cloud/provider.py
+-rw-r--r--   0        0        0    22522 2024-03-29 16:50:01.346853 hpc-beeflow-0.1.7/beeflow/common/config_driver.py
+-rw-r--r--   0        0        0     5891 2024-03-28 22:16:36.355303 hpc-beeflow-0.1.7/beeflow/common/config_validator.py
+-rw-r--r--   0        0        0     2420 2024-03-28 22:16:36.355477 hpc-beeflow-0.1.7/beeflow/common/connection.py
+-rw-r--r--   0        0        0      947 2024-03-28 22:16:36.355625 hpc-beeflow-0.1.7/beeflow/common/container_path.py
+-rw-r--r--   0        0        0     7084 2024-03-29 16:50:01.347322 hpc-beeflow-0.1.7/beeflow/common/crt/charliecloud_driver.py
+-rw-r--r--   0        0        0     1487 2024-03-28 22:16:36.356338 hpc-beeflow-0.1.7/beeflow/common/crt/crt_driver.py
+-rw-r--r--   0        0        0     1760 2024-03-29 16:50:01.347773 hpc-beeflow-0.1.7/beeflow/common/crt/singularity_driver.py
+-rw-r--r--   0        0        0     1551 2024-03-28 22:16:36.356875 hpc-beeflow-0.1.7/beeflow/common/crt_interface.py
+-rw-r--r--   0        0        0     2486 2024-03-28 22:16:36.357355 hpc-beeflow-0.1.7/beeflow/common/db/bdb.py
+-rw-r--r--   0        0        0     1675 2024-03-28 22:16:36.357568 hpc-beeflow-0.1.7/beeflow/common/db/sched_db.py
+-rw-r--r--   0        0        0     5075 2024-03-28 22:16:36.357757 hpc-beeflow-0.1.7/beeflow/common/db/tm_db.py
+-rw-r--r--   0        0        0     8816 2024-03-28 22:16:36.358119 hpc-beeflow-0.1.7/beeflow/common/db/wfm_db.py
+-rw-r--r--   0        0        0     2133 2024-03-28 22:16:36.358379 hpc-beeflow-0.1.7/beeflow/common/expr.py
+-rw-r--r--   0        0        0     5924 2024-03-28 22:16:36.358925 hpc-beeflow-0.1.7/beeflow/common/gdb/DESIGN.md
+-rw-r--r--   0        0        0     8320 2024-03-29 16:50:01.348375 hpc-beeflow-0.1.7/beeflow/common/gdb/gdb_driver.py
+-rw-r--r--   0        0        0    23439 2024-03-29 16:50:01.348932 hpc-beeflow-0.1.7/beeflow/common/gdb/neo4j_cypher.py
+-rw-r--r--   0        0        0    22892 2024-03-29 16:50:01.349407 hpc-beeflow-0.1.7/beeflow/common/gdb/neo4j_driver.py
+-rw-r--r--   0        0        0     9736 2024-03-28 22:16:36.359945 hpc-beeflow-0.1.7/beeflow/common/gdb_interface.py
+-rw-r--r--   0        0        0     4222 2024-03-29 16:50:01.349743 hpc-beeflow-0.1.7/beeflow/common/integration/generated_workflows.py
+-rw-r--r--   0        0        0     8370 2024-03-29 16:50:01.349960 hpc-beeflow-0.1.7/beeflow/common/integration/utils.py
+-rw-r--r--   0        0        0    11162 2024-03-29 16:50:01.350145 hpc-beeflow-0.1.7/beeflow/common/integration_test.py
+-rw-r--r--   0        0        0      642 2024-03-28 22:16:36.360815 hpc-beeflow-0.1.7/beeflow/common/log.py
+-rw-r--r--   0        0        0       16 2024-03-28 22:16:36.361052 hpc-beeflow-0.1.7/beeflow/common/parser/.gitignore
+-rw-r--r--   0        0        0     2614 2024-03-28 22:16:36.361301 hpc-beeflow-0.1.7/beeflow/common/parser/README.md
+-rw-r--r--   0        0        0      102 2024-03-28 22:16:36.361545 hpc-beeflow-0.1.7/beeflow/common/parser/__init__.py
+-rw-r--r--   0        0        0    15464 2024-03-29 16:50:01.350621 hpc-beeflow-0.1.7/beeflow/common/parser/parser.py
+-rw-r--r--   0        0        0     2162 2024-03-28 22:16:36.362002 hpc-beeflow-0.1.7/beeflow/common/paths.py
+-rw-r--r--   0        0        0      450 2024-03-28 22:16:36.362142 hpc-beeflow-0.1.7/beeflow/common/states.py
+-rw-r--r--   0        0        0      493 2024-03-28 22:16:36.362369 hpc-beeflow-0.1.7/beeflow/common/tab_completion.py
+-rw-r--r--   0        0        0     1643 2024-03-28 22:16:36.362570 hpc-beeflow-0.1.7/beeflow/common/validation.py
+-rw-r--r--   0        0        0    12396 2024-03-29 16:50:01.351045 hpc-beeflow-0.1.7/beeflow/common/wf_data.py
+-rw-r--r--   0        0        0    11679 2024-03-29 16:50:01.351480 hpc-beeflow-0.1.7/beeflow/common/wf_interface.py
+-rw-r--r--   0        0        0     1522 2024-03-28 22:16:36.363159 hpc-beeflow-0.1.7/beeflow/common/wf_profiler.py
+-rw-r--r--   0        0        0      493 2024-03-28 22:16:36.363554 hpc-beeflow-0.1.7/beeflow/common/worker/README.md
+-rw-r--r--   0        0        0      597 2024-03-28 22:16:36.363810 hpc-beeflow-0.1.7/beeflow/common/worker/__init__.py
+-rw-r--r--   0        0        0     5048 2024-03-28 22:16:36.364014 hpc-beeflow-0.1.7/beeflow/common/worker/flux_worker.py
+-rw-r--r--   0        0        0     2570 2024-03-28 22:16:36.364334 hpc-beeflow-0.1.7/beeflow/common/worker/lsf_worker.py
+-rw-r--r--   0        0        0     1731 2024-03-28 22:16:36.364550 hpc-beeflow-0.1.7/beeflow/common/worker/simple_worker.py
+-rw-r--r--   0        0        0    10635 2024-03-29 16:50:01.352492 hpc-beeflow-0.1.7/beeflow/common/worker/slurm_worker.py
+-rw-r--r--   0        0        0     2899 2024-03-28 22:16:36.364935 hpc-beeflow-0.1.7/beeflow/common/worker/worker.py
+-rw-r--r--   0        0        0     1794 2024-03-28 22:16:36.365103 hpc-beeflow-0.1.7/beeflow/common/worker_interface.py
+-rw-r--r--   0        0        0     4301 2024-03-28 22:16:36.365494 hpc-beeflow-0.1.7/beeflow/data/cloud_templates/dora.jinja
+-rw-r--r--   0        0        0      866 2024-03-28 22:16:36.365754 hpc-beeflow-0.1.7/beeflow/data/cloud_templates/dora.yaml
+-rw-r--r--   0        0        0      414 2024-03-28 22:16:36.366199 hpc-beeflow-0.1.7/beeflow/data/cwl/README.md
+-rw-r--r--   0        0        0     1281 2024-03-28 22:16:36.366556 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/README.md
+-rw-r--r--   0        0        0      315 2024-03-28 22:16:36.366812 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/blast/README.md
+-rw-r--r--   0        0        0      418 2024-03-28 22:16:36.366971 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/blast/blast.yml
+-rw-r--r--   0        0        0      423 2024-03-28 22:16:36.367127 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/blast/blast_output.cwl
+-rw-r--r--   0        0        0      300 2024-03-28 22:16:36.367264 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/blast/blast_output_err.cwl
+-rw-r--r--   0        0        0      410 2024-03-28 22:16:36.367399 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/blast/blast_split.cwl
+-rw-r--r--   0        0        0     2009 2024-03-28 22:16:36.367628 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/blast/blast_wf.cwl
+-rw-r--r--   0        0        0      559 2024-03-28 22:16:36.367934 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/blast/blast_worker001.cwl
+-rw-r--r--   0        0        0      559 2024-03-28 22:16:36.368162 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/blast/blast_worker002.cwl
+-rwxr-xr-x   0        0        0   930997 2024-03-28 22:16:36.372172 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/blast/input/small.fasta
+-rw-r--r--   0        0        0       77 2024-03-28 22:16:36.372485 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/cat-grep-fail/README.md
+-rw-r--r--   0        0        0      258 2024-03-28 22:16:36.372649 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/cat-grep-fail/cat.cwl
+-rw-r--r--   0        0        0      272 2024-03-28 22:16:36.372795 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/cat-grep-fail/grep0.cwl
+-rw-r--r--   0        0        0      272 2024-03-28 22:16:36.372926 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/cat-grep-fail/grep1.cwl
+-rw-r--r--   0        0        0       76 2024-03-28 22:16:36.373063 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/cat-grep-fail/input.yml
+-rw-r--r--   0        0        0     3215 2024-03-28 22:16:36.373230 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/cat-grep-fail/lorem.txt
+-rw-r--r--   0        0        0      422 2024-03-28 22:16:36.373386 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/cat-grep-fail/tar.cwl
+-rw-r--r--   0        0        0      710 2024-03-28 22:16:36.373578 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/cat-grep-fail/workflow.cwl
+-rw-r--r--   0        0        0      350 2024-03-28 22:16:36.374050 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-ci/README.md
+-rw-r--r--   0        0        0     1968 2024-03-28 22:16:36.374314 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-ci/clamr.cwl
+-rw-r--r--   0        0        0      302 2024-03-28 22:16:36.374472 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-ci/clamr_job.json
+-rw-r--r--   0        0        0      429 2024-03-28 22:16:36.374724 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-ci/clamr_job.yml
+-rw-r--r--   0        0        0     2228 2024-03-28 22:16:36.375020 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-ci/clamr_wf.cwl
+-rw-r--r--   0        0        0      765 2024-03-28 22:16:36.375279 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-ci/ffmpeg.cwl
+-rw-r--r--   0        0        0      411 2024-03-29 16:50:01.383257 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-ffmpeg-build_script/Dockerfile.clamr-ffmpeg
+-rw-r--r--   0        0        0      347 2024-03-29 16:50:01.353020 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-ffmpeg-build_script/README.md
+-rw-r--r--   0        0        0     1446 2024-03-29 16:50:01.353180 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-ffmpeg-build_script/clamr.cwl
+-rw-r--r--   0        0        0      302 2024-03-29 16:50:01.353324 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-ffmpeg-build_script/clamr_job.json
+-rw-r--r--   0        0        0      405 2024-03-29 16:50:01.353481 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-ffmpeg-build_script/clamr_job.yml
+-rw-r--r--   0        0        0     2019 2024-03-29 16:50:01.353624 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-ffmpeg-build_script/clamr_wf.cwl
+-rw-r--r--   0        0        0      815 2024-03-29 16:50:01.353790 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-ffmpeg-build_script/ffmpeg.cwl
+-rw-r--r--   0        0        0       17 2024-03-29 16:50:01.353940 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-ffmpeg-build_script/post_run.sh
+-rw-r--r--   0        0        0       18 2024-03-29 16:50:01.354112 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-ffmpeg-build_script/pre_run.sh
+-rw-r--r--   0        0        0      350 2024-03-28 22:16:36.384975 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf/README.md
+-rw-r--r--   0        0        0     1977 2024-03-28 22:16:36.385149 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf/clamr.cwl
+-rw-r--r--   0        0        0      302 2024-03-28 22:16:36.385371 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf/clamr_job.json
+-rw-r--r--   0        0        0      455 2024-03-28 22:16:36.385604 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf/clamr_job.yml
+-rw-r--r--   0        0        0     2145 2024-03-28 22:16:36.385833 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf/clamr_wf.cwl
+-rw-r--r--   0        0        0      815 2024-03-28 22:16:36.386026 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf/ffmpeg.cwl
+-rw-r--r--   0        0        0      383 2024-03-28 22:16:36.377486 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf-chicoma/README.md
+-rw-r--r--   0        0        0     1962 2024-03-28 22:16:36.377745 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf-chicoma/clamr.cwl
+-rw-r--r--   0        0        0      302 2024-03-28 22:16:36.377970 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf-chicoma/clamr_job.json
+-rw-r--r--   0        0        0      411 2024-03-28 22:16:36.378197 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf-chicoma/clamr_job.yml
+-rw-r--r--   0        0        0     2006 2024-03-28 22:16:36.378352 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf-chicoma/clamr_wf.cwl
+-rw-r--r--   0        0        0      753 2024-03-28 22:16:36.378502 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf-chicoma/ffmpeg.cwl
+-rw-r--r--   0        0        0      837 2024-03-28 22:16:36.378731 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/README.md
+-rw-r--r--   0        0        0      304 2024-03-28 22:16:36.379016 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/lsf-charliecloud/README.md
+-rw-r--r--   0        0        0     1234 2024-03-28 22:16:36.379190 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/lsf-charliecloud/cf-summit.cwl
+-rw-r--r--   0        0        0      145 2024-03-28 22:16:36.379452 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/slurm-charliecloud/Dockerfile.clamr-lanl-x86_64
+-rw-r--r--   0        0        0     3325 2024-03-28 22:16:36.379703 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/slurm-charliecloud/README.md
+-rw-r--r--   0        0        0     1127 2024-03-28 22:16:36.379932 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/slurm-charliecloud/cf-darwin.cwl
+-rw-r--r--   0        0        0     1135 2024-03-28 22:16:36.380143 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/slurm-charliecloud/cf-no-owrite.cwl
+-rw-r--r--   0        0        0     1137 2024-03-28 22:16:36.380291 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/slurm-charliecloud/cf.cwl
+-rw-r--r--   0        0        0     1176 2024-03-28 22:16:36.380433 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/slurm-charliecloud/copyContainer_containerName.cwl
+-rw-r--r--   0        0        0     1137 2024-03-28 22:16:36.380602 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/slurm-charliecloud/dockerFile_containerName.cwl
+-rw-r--r--   0        0        0     1133 2024-03-28 22:16:36.380784 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/slurm-charliecloud/dockerPull.cwl
+-rw-r--r--   0        0        0      182 2024-03-28 22:16:36.381023 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/slurm-singularity/README.md
+-rw-r--r--   0        0        0     1122 2024-03-28 22:16:36.381197 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/slurm-singularity/cf-singularity.cwl
+-rw-r--r--   0        0        0      303 2024-03-28 22:16:36.381502 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf-singularity/README.md
+-rw-r--r--   0        0        0     1975 2024-03-28 22:16:36.381759 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf-singularity/clamr.cwl
+-rw-r--r--   0        0        0      302 2024-03-28 22:16:36.381982 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf-singularity/clamr_job.json
+-rw-r--r--   0        0        0      418 2024-03-28 22:16:36.382180 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf-singularity/clamr_job.yml
+-rw-r--r--   0        0        0     2057 2024-03-28 22:16:36.382381 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf-singularity/clamr_wf.cwl
+-rw-r--r--   0        0        0      768 2024-03-28 22:16:36.382528 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf-singularity/ffmpeg.cwl
+-rw-r--r--   0        0        0      339 2024-03-28 22:16:36.382785 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf-summit/README.md
+-rw-r--r--   0        0        0     1962 2024-03-28 22:16:36.382941 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf-summit/clamr.cwl
+-rw-r--r--   0        0        0      302 2024-03-28 22:16:36.383083 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf-summit/clamr_job.json
+-rw-r--r--   0        0        0      418 2024-03-28 22:16:36.383256 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf-summit/clamr_job.yml
+-rw-r--r--   0        0        0     2103 2024-03-28 22:16:36.383480 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf-summit/clamr_wf.cwl
+-rw-r--r--   0        0        0      765 2024-03-28 22:16:36.383728 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf-summit/ffmpeg.cwl
+-rw-r--r--   0        0        0      350 2024-03-28 22:16:36.384066 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf-use-container/README.md
+-rw-r--r--   0        0        0     1981 2024-03-28 22:16:36.384227 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf-use-container/clamr.cwl
+-rw-r--r--   0        0        0      302 2024-03-28 22:16:36.384363 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf-use-container/clamr_job.json
+-rw-r--r--   0        0        0      430 2024-03-28 22:16:36.384497 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf-use-container/clamr_job.yml
+-rw-r--r--   0        0        0     1939 2024-03-28 22:16:36.384630 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf-use-container/clamr_wf.cwl
+-rw-r--r--   0        0        0      765 2024-03-28 22:16:36.384760 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf-use-container/ffmpeg.cwl
+-rw-r--r--   0        0        0      527 2024-03-28 22:16:36.386265 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/comd-mpi/comd.cwl
+-rw-r--r--   0        0        0      110 2024-03-28 22:16:36.386428 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/comd-mpi/comd_job.yml
+-rw-r--r--   0        0        0      555 2024-03-28 22:16:36.386570 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/comd-mpi/comd_wf.cwl
+-rw-r--r--   0        0        0      831 2024-03-28 22:16:36.387677 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/lulesh-mpi/lulesh.cwl
+-rw-r--r--   0        0        0       24 2024-03-28 22:16:36.387837 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/lulesh-mpi/lulesh.yml
+-rw-r--r--   0        0        0      264 2024-03-28 22:16:36.386879 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/lulesh-mpi-multi-file/lulesh.cwl
+-rw-r--r--   0        0        0       24 2024-03-28 22:16:36.387091 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/lulesh-mpi-multi-file/lulesh_job.yml
+-rw-r--r--   0        0        0      469 2024-03-28 22:16:36.387331 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/lulesh-mpi-multi-file/lulesh_wf.cwl
+-rw-r--r--   0        0        0     1282 2024-03-28 22:16:36.388066 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/nwchem-mpi/README.md
+-rw-r--r--   0        0        0      590 2024-03-28 22:16:36.388225 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/nwchem-mpi/nwchem.cwl
+-rw-r--r--   0        0        0      161 2024-03-28 22:16:36.388407 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/nwchem-mpi/nwchem.yml
+-rw-r--r--   0        0        0      199 2024-03-28 22:16:36.388620 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/nwchem-mpi/nwchem_bin.cwl
+-rw-r--r--   0        0        0      344 2024-03-28 22:16:36.392197 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/pennant/graph.cwl
+-rw-r--r--   0        0        0       43 2024-03-28 22:16:36.392532 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/pennant/pennant.yml
+-rw-r--r--   0        0        0      192 2024-03-28 22:16:36.392781 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/pennant/pennant_1_node.cwl
+-rw-r--r--   0        0        0      192 2024-03-28 22:16:36.393036 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/pennant/pennant_2_node.cwl
+-rw-r--r--   0        0        0      192 2024-03-28 22:16:36.393273 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/pennant/pennant_4_node.cwl
+-rw-r--r--   0        0        0     1217 2024-03-28 22:16:36.393572 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/pennant/pennant_wf.cwl
+-rw-r--r--   0        0        0     3881 2024-03-28 22:16:36.388879 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/pennant-build/Dockerfile.pennant-flux-x86_64
+-rw-r--r--   0        0        0      789 2024-03-28 22:16:36.389106 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/pennant-build/Dockerfile.pennant-graph-x86_64
+-rw-r--r--   0        0        0      407 2024-03-28 22:16:36.389420 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/pennant-build/graph.cwl
+-rw-r--r--   0        0        0     1294 2024-03-28 22:16:36.389670 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/pennant-build/graph_pennant.py
+-rw-r--r--   0        0        0      110 2024-03-28 22:16:36.389905 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/pennant-build/graph_pennant.sh
+-rw-r--r--   0        0        0       43 2024-03-28 22:16:36.390208 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/pennant-build/pennant.yml
+-rw-r--r--   0        0        0      192 2024-03-28 22:16:36.390730 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/pennant-build/pennant_1_node.cwl
+-rw-r--r--   0        0        0      192 2024-03-28 22:16:36.390984 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/pennant-build/pennant_2_node.cwl
+-rw-r--r--   0        0        0      192 2024-03-28 22:16:36.391226 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/pennant-build/pennant_4_node.cwl
+-rw-r--r--   0        0        0      192 2024-03-28 22:16:36.391471 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/pennant-build/pennant_8_node.cwl
+-rw-r--r--   0        0        0     1741 2024-03-28 22:16:36.391720 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/pennant-build/pennant_wf.cwl
+-rw-r--r--   0        0        0       71 2024-03-28 22:16:36.393816 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/pytest.ini
+-rw-r--r--   0        0        0      317 2024-03-28 22:16:36.394254 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/simple-workflows/README.md
+-rw-r--r--   0        0        0      986 2024-03-28 22:16:36.394516 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/simple-workflows/cancel.cwl
+-rw-r--r--   0        0        0      217 2024-03-28 22:16:36.394918 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/simple-workflows/grep-wordcount/README.md
+-rw-r--r--   0        0        0     1083 2024-03-28 22:16:36.395183 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/simple-workflows/grep-wordcount/gc-nc.cwl
+-rw-r--r--   0        0        0     1325 2024-03-28 22:16:36.395445 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/simple-workflows/grep-wordcount/gc.cwl
+-rw-r--r--   0        0        0     3776 2024-03-28 22:16:36.395702 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/simple-workflows/grep-wordcount/lorem.txt
+-rw-r--r--   0        0        0      426 2024-03-28 22:16:36.396138 hpc-beeflow-0.1.7/beeflow/data/cwl/cwl_validation/README.md
+-rwxr-xr-x   0        0        0      398 2024-03-28 22:16:36.396514 hpc-beeflow-0.1.7/beeflow/data/cwl/cwl_validation/builder/dockerFile.cwl
+-rwxr-xr-x   0        0        0      317 2024-03-28 22:16:36.396740 hpc-beeflow-0.1.7/beeflow/data/cwl/cwl_validation/builder/dockerPull.cwl
+-rw-r--r--   0        0        0     1202 2024-03-28 22:16:36.397093 hpc-beeflow-0.1.7/beeflow/data/cwl/cwl_validation/grep-wordcount/gc.cwl
+-rw-r--r--   0        0        0     3776 2024-03-28 22:16:36.397288 hpc-beeflow-0.1.7/beeflow/data/cwl/cwl_validation/grep-wordcount/lorem.txt
+-rwxr-xr-x   0        0        0      169 2024-03-28 22:16:36.397530 hpc-beeflow-0.1.7/beeflow/data/cwl/cwl_validation/helloworld.cwl
+-rw-r--r--   0        0        0       19 2024-03-28 22:16:36.397778 hpc-beeflow-0.1.7/beeflow/data/cwl/cwl_validation/helloworld_input.yaml
+-rw-r--r--   0        0        0    59407 2024-03-28 22:16:36.398764 hpc-beeflow-0.1.7/beeflow/data/cwl/cwl_validation/ml-workflow/example-1/DAG_example-1.png
+-rw-r--r--   0        0        0      833 2024-03-28 22:16:36.399006 hpc-beeflow-0.1.7/beeflow/data/cwl/cwl_validation/ml-workflow/example-1/README.md
+-rw-r--r--   0        0        0      254 2024-03-28 22:16:36.399215 hpc-beeflow-0.1.7/beeflow/data/cwl/cwl_validation/ml-workflow/example-1/add.cwl
+-rw-r--r--   0        0        0      351 2024-03-28 22:16:36.399447 hpc-beeflow-0.1.7/beeflow/data/cwl/cwl_validation/ml-workflow/example-1/add_multiply_example_workflow.cwl
+-rw-r--r--   0        0        0      245 2024-03-28 22:16:36.399597 hpc-beeflow-0.1.7/beeflow/data/cwl/cwl_validation/ml-workflow/example-1/add_step1.py
+-rw-r--r--   0        0        0      386 2024-03-28 22:16:36.399737 hpc-beeflow-0.1.7/beeflow/data/cwl/cwl_validation/ml-workflow/example-1/isolated test.cwl
+-rw-r--r--   0        0        0       21 2024-03-28 22:16:36.399903 hpc-beeflow-0.1.7/beeflow/data/cwl/cwl_validation/ml-workflow/example-1/job.yaml
+-rw-r--r--   0        0        0      304 2024-03-28 22:16:36.400111 hpc-beeflow-0.1.7/beeflow/data/cwl/cwl_validation/ml-workflow/example-1/multiply.cwl
+-rw-r--r--   0        0        0      267 2024-03-28 22:16:36.400335 hpc-beeflow-0.1.7/beeflow/data/cwl/cwl_validation/ml-workflow/example-1/multiply_step2.py
+-rw-r--r--   0        0        0      407 2024-03-28 22:16:36.400569 hpc-beeflow-0.1.7/beeflow/data/cwl/cwl_validation/ml-workflow/example-1/workflow_generater_python.py
+-rw-r--r--   0        0        0     3496 2024-03-28 22:16:36.400990 hpc-beeflow-0.1.7/beeflow/data/cwl/cwl_validation/ml-workflow/machine_learning/README.md
+-rw-r--r--   0        0        0      901 2024-03-28 22:16:36.401373 hpc-beeflow-0.1.7/beeflow/data/cwl/cwl_validation/ml-workflow/machine_learning/decision_tree.py
+-rw-r--r--   0        0        0      443 2024-03-28 22:16:36.401536 hpc-beeflow-0.1.7/beeflow/data/cwl/cwl_validation/ml-workflow/machine_learning/decision_tree_output.txt
+-rw-r--r--   0        0        0      234 2024-03-28 22:16:36.401680 hpc-beeflow-0.1.7/beeflow/data/cwl/cwl_validation/ml-workflow/machine_learning/decision_tree_tool.cwl
+-rw-r--r--   0        0        0      178 2024-03-28 22:16:36.401859 hpc-beeflow-0.1.7/beeflow/data/cwl/cwl_validation/ml-workflow/machine_learning/expectedValue.txt
+-rw-r--r--   0        0        0      157 2024-03-28 22:16:36.402053 hpc-beeflow-0.1.7/beeflow/data/cwl/cwl_validation/ml-workflow/machine_learning/hiring1.txt
+-rw-r--r--   0        0        0      467 2024-03-28 22:16:36.402274 hpc-beeflow-0.1.7/beeflow/data/cwl/cwl_validation/ml-workflow/machine_learning/linear_regress_output.txt
+-rw-r--r--   0        0        0     1203 2024-03-28 22:16:36.402518 hpc-beeflow-0.1.7/beeflow/data/cwl/cwl_validation/ml-workflow/machine_learning/linear_regression.py
+-rw-r--r--   0        0        0      692 2024-03-28 22:16:36.402779 hpc-beeflow-0.1.7/beeflow/data/cwl/cwl_validation/ml-workflow/machine_learning/machinelearning_pipeline.cwl
+-rw-r--r--   0        0        0    12405 2024-03-28 22:16:36.403118 hpc-beeflow-0.1.7/beeflow/data/cwl/cwl_validation/ml-workflow/machine_learning/out.PNG
+-rw-r--r--   0        0        0     1517 2024-03-28 22:16:36.403293 hpc-beeflow-0.1.7/beeflow/data/cwl/cwl_validation/ml-workflow/machine_learning/predict_code.py
+-rw-r--r--   0        0        0      336 2024-03-28 22:16:36.403435 hpc-beeflow-0.1.7/beeflow/data/cwl/cwl_validation/ml-workflow/machine_learning/predict_tool.cwl
+-rw-r--r--   0        0        0     1054 2024-03-28 22:16:36.403665 hpc-beeflow-0.1.7/beeflow/data/cwl/cwl_validation/ml-workflow/machine_learning/read_dataset.py
+-rw-r--r--   0        0        0      235 2024-03-28 22:16:36.403835 hpc-beeflow-0.1.7/beeflow/data/cwl/cwl_validation/ml-workflow/machine_learning/read_dataset_tool.cwl
+-rw-r--r--   0        0        0      239 2024-03-28 22:16:36.404013 hpc-beeflow-0.1.7/beeflow/data/cwl/cwl_validation/ml-workflow/machine_learning/regress_tool.cwl
+-rw-r--r--   0        0        0       80 2024-03-28 22:16:36.404371 hpc-beeflow-0.1.7/beeflow/data/dockerfiles/Dockerfile.builder_demo
+-rw-r--r--   0        0        0      411 2024-03-28 22:16:36.404802 hpc-beeflow-0.1.7/beeflow/data/dockerfiles/Dockerfile.clamr-ffmpeg
+-rw-r--r--   0        0        0      145 2024-03-28 22:16:36.405084 hpc-beeflow-0.1.7/beeflow/data/dockerfiles/Dockerfile.clamr-lanl-x86_64
+-rw-r--r--   0        0        0      724 2024-03-28 22:16:36.405299 hpc-beeflow-0.1.7/beeflow/data/dockerfiles/Dockerfile.clamr-ppc64le
+-rw-r--r--   0        0        0     3698 2024-03-28 22:16:36.405538 hpc-beeflow-0.1.7/beeflow/data/dockerfiles/Dockerfile.comd-flux-x86_64
+-rw-r--r--   0        0        0     2303 2024-03-28 22:16:36.405728 hpc-beeflow-0.1.7/beeflow/data/dockerfiles/Dockerfile.comd-x86_64
+-rw-r--r--   0        0        0      270 2024-03-28 22:16:36.405908 hpc-beeflow-0.1.7/beeflow/data/dockerfiles/Dockerfile.deb9ompi-x86_64
+-rw-r--r--   0        0        0     2592 2024-03-28 22:16:36.406063 hpc-beeflow-0.1.7/beeflow/data/dockerfiles/Dockerfile.lulesh-x86_64
+-rw-r--r--   0        0        0     1605 2024-03-28 22:16:36.406255 hpc-beeflow-0.1.7/beeflow/data/dockerfiles/Dockerfile.neo4j-ppc64le
+-rw-r--r--   0        0        0     2489 2024-03-28 22:16:36.406541 hpc-beeflow-0.1.7/beeflow/data/dockerfiles/Dockerfile.nwchem-x86_64
+-rw-r--r--   0        0        0     3881 2024-03-28 22:16:36.406803 hpc-beeflow-0.1.7/beeflow/data/dockerfiles/Dockerfile.pennant-flux-x86_64
+-rw-r--r--   0        0        0     3446 2024-03-28 22:16:36.407037 hpc-beeflow-0.1.7/beeflow/data/dockerfiles/Dockerfile.vaspompi-x86_64
+-rw-r--r--   0        0        0      614 2024-03-28 22:16:36.407192 hpc-beeflow-0.1.7/beeflow/data/dockerfiles/README.md
+-rw-r--r--   0        0        0      331 2024-03-28 22:16:36.407464 hpc-beeflow-0.1.7/beeflow/data/dockerfiles/comd-pmix-support/Dockerfile.comd-x86_64-wpmix
+-rw-r--r--   0        0        0      573 2024-03-28 22:16:36.407617 hpc-beeflow-0.1.7/beeflow/data/dockerfiles/comd-pmix-support/Dockerfile.debian
+-rw-r--r--   0        0        0     3941 2024-03-28 22:16:36.407776 hpc-beeflow-0.1.7/beeflow/data/dockerfiles/comd-pmix-support/Dockerfile.openmpi-3.1.5
+-rw-r--r--   0        0        0      509 2024-03-28 22:16:36.407913 hpc-beeflow-0.1.7/beeflow/data/dockerfiles/comd-pmix-support/README.md
+-rw-r--r--   0        0        0      813 2024-03-28 22:16:36.408098 hpc-beeflow-0.1.7/beeflow/data/dockerfiles/comd-pmix-support/dont-init-ucx-on-intel-cray.patch
+-rw-r--r--   0        0        0      789 2024-03-28 22:16:36.408377 hpc-beeflow-0.1.7/beeflow/data/dockerfiles/pennant-graph/Dockerfile.pennant-graph-x86_64
+-rw-r--r--   0        0        0     1294 2024-03-28 22:16:36.408604 hpc-beeflow-0.1.7/beeflow/data/dockerfiles/pennant-graph/graph_pennant.py
+-rw-r--r--   0        0        0      110 2024-03-28 22:16:36.408820 hpc-beeflow-0.1.7/beeflow/data/dockerfiles/pennant-graph/graph_pennant.sh
+-rw-r--r--   0        0        0      640 2024-03-28 22:16:36.409201 hpc-beeflow-0.1.7/beeflow/enhanced_client/README.rst
+-rw-r--r--   0        0        0        0 2024-03-28 22:16:36.409471 hpc-beeflow-0.1.7/beeflow/enhanced_client/data/.gitkeep
+-rw-r--r--   0        0        0      386 2024-03-28 22:16:36.409640 hpc-beeflow-0.1.7/beeflow/enhanced_client/forge.config.js
+-rw-r--r--   0        0        0     1682 2024-03-28 22:16:36.409813 hpc-beeflow-0.1.7/beeflow/enhanced_client/main.js
+-rw-r--r--   0        0        0   231716 2024-03-29 16:50:01.355750 hpc-beeflow-0.1.7/beeflow/enhanced_client/package-lock.json
+-rw-r--r--   0        0        0     1078 2024-03-28 22:16:36.411301 hpc-beeflow-0.1.7/beeflow/enhanced_client/package.json
+-rw-r--r--   0        0        0     1219 2024-03-28 22:16:36.411639 hpc-beeflow-0.1.7/beeflow/enhanced_client/renderer/app.js
+-rw-r--r--   0        0        0     5151 2024-03-28 22:16:36.411951 hpc-beeflow-0.1.7/beeflow/enhanced_client/renderer/client.js
+-rw-r--r--   0        0        0      872 2024-03-28 22:16:36.412170 hpc-beeflow-0.1.7/beeflow/enhanced_client/renderer/config.js
+-rw-r--r--   0        0        0     2013 2024-03-28 22:16:36.412332 hpc-beeflow-0.1.7/beeflow/enhanced_client/renderer/control.js
+-rw-r--r--   0        0        0     3610 2024-03-28 22:16:36.412502 hpc-beeflow-0.1.7/beeflow/enhanced_client/renderer/database.js
+-rw-r--r--   0        0        0    12140 2024-03-28 22:16:36.412701 hpc-beeflow-0.1.7/beeflow/enhanced_client/renderer/display.js
+-rw-r--r--   0        0        0      455 2024-03-28 22:16:36.412897 hpc-beeflow-0.1.7/beeflow/enhanced_client/renderer/gdb.js
+-rw-r--r--   0        0        0    33601 2024-03-28 22:16:36.413313 hpc-beeflow-0.1.7/beeflow/enhanced_client/renderer/img/logo.png
+-rw-r--r--   0        0        0     2751 2024-03-28 22:16:36.413585 hpc-beeflow-0.1.7/beeflow/enhanced_client/renderer/main.html
+-rw-r--r--   0        0        0   206620 2024-03-28 22:16:36.414373 hpc-beeflow-0.1.7/beeflow/enhanced_client/renderer/styles/bulma.min.css
+-rw-r--r--   0        0        0      374 2024-03-28 22:16:36.414563 hpc-beeflow-0.1.7/beeflow/enhanced_client/renderer/styles/main.css
+-rw-r--r--   0        0        0      498 2024-03-28 22:16:36.414733 hpc-beeflow-0.1.7/beeflow/enhanced_client/renderer/tunnel.js
+-rw-r--r--   0        0        0      428 2024-03-28 22:16:36.414973 hpc-beeflow-0.1.7/beeflow/enhanced_client/renderer/viz.html
+-rw-r--r--   0        0        0     1071 2024-03-28 22:16:36.415256 hpc-beeflow-0.1.7/beeflow/enhanced_client/renderer/viz.js
+-rw-r--r--   0        0        0     7603 2024-03-28 22:16:36.415531 hpc-beeflow-0.1.7/beeflow/enhanced_client/renderer/workflows.js
+-rw-r--r--   0        0        0     1708 2024-03-28 22:16:36.415837 hpc-beeflow-0.1.7/beeflow/scheduler/README.md
+-rw-r--r--   0        0        0    10098 2024-03-28 22:16:36.416106 hpc-beeflow-0.1.7/beeflow/scheduler/algorithms.py
+-rw-r--r--   0        0        0     9347 2024-03-28 22:16:36.416370 hpc-beeflow-0.1.7/beeflow/scheduler/resource_allocation.py
+-rw-r--r--   0        0        0     3738 2024-03-28 22:16:36.416539 hpc-beeflow-0.1.7/beeflow/scheduler/scheduler.py
+-rw-r--r--   0        0        0     2890 2024-03-28 22:16:36.416765 hpc-beeflow-0.1.7/beeflow/scheduler/scheduler.yaml
+-rw-r--r--   0        0        0      708 2024-03-28 22:16:36.417035 hpc-beeflow-0.1.7/beeflow/scheduler/serializable.py
+-rw-r--r--   0        0        0     2296 2024-03-28 22:16:36.417255 hpc-beeflow-0.1.7/beeflow/scheduler/task.py
+-rw-r--r--   0        0        0     5500 2024-03-29 16:50:01.356040 hpc-beeflow-0.1.7/beeflow/task_manager/background.py
+-rw-r--r--   0        0        0     1239 2024-03-29 16:50:01.356206 hpc-beeflow-0.1.7/beeflow/task_manager/task_actions.py
+-rw-r--r--   0        0        0     1538 2024-03-29 16:50:01.356349 hpc-beeflow-0.1.7/beeflow/task_manager/task_manager.py
+-rw-r--r--   0        0        0      856 2024-03-29 16:50:01.356488 hpc-beeflow-0.1.7/beeflow/task_manager/task_submit.py
+-rw-r--r--   0        0        0     3602 2024-03-29 16:50:01.356645 hpc-beeflow-0.1.7/beeflow/task_manager/utils.py
+-rw-r--r--   0        0        0    34925 2024-03-28 22:16:36.418588 hpc-beeflow-0.1.7/beeflow/tests/42.tgz
+-rw-r--r--   0        0        0      236 2024-03-28 22:16:36.418758 hpc-beeflow-0.1.7/beeflow/tests/README.md
+-rw-r--r--   0        0        0     1139 2024-03-28 22:16:36.418913 hpc-beeflow-0.1.7/beeflow/tests/cf.cwl
+-rw-r--r--   0        0        0     1093 2024-03-28 22:16:36.419527 hpc-beeflow-0.1.7/beeflow/tests/clamr-wf/clamr.cwl
+-rw-r--r--   0        0        0      302 2024-03-28 22:16:36.419765 hpc-beeflow-0.1.7/beeflow/tests/clamr-wf/clamr_job.json
+-rw-r--r--   0        0        0      424 2024-03-28 22:16:36.419927 hpc-beeflow-0.1.7/beeflow/tests/clamr-wf/clamr_job.yml
+-rw-r--r--   0        0        0     1320 2024-03-28 22:16:36.420116 hpc-beeflow-0.1.7/beeflow/tests/clamr-wf/clamr_wf.cwl
+-rw-r--r--   0        0        0      680 2024-03-28 22:16:36.420363 hpc-beeflow-0.1.7/beeflow/tests/clamr-wf/ffmpeg.cwl
+-rw-r--r--   0        0        0      273 2024-03-28 22:16:36.420655 hpc-beeflow-0.1.7/beeflow/tests/clamr-wf/mv_script.cwl
+-rwxr-xr-x   0        0        0      324 2024-03-28 22:16:36.420825 hpc-beeflow-0.1.7/beeflow/tests/clamr-wf/mv_script.sh
+-rw-r--r--   0        0        0     2401 2024-03-28 22:16:36.419154 hpc-beeflow-0.1.7/beeflow/tests/clamr-wf.tgz
+-rw-r--r--   0        0        0      774 2024-03-28 22:16:36.420989 hpc-beeflow-0.1.7/beeflow/tests/gdb.py
+-rw-r--r--   0        0        0    12378 2024-03-28 22:16:36.421252 hpc-beeflow-0.1.7/beeflow/tests/mocks.py
+-rw-r--r--   0        0        0      267 2024-03-28 22:16:36.421532 hpc-beeflow-0.1.7/beeflow/tests/test_cloud.py
+-rw-r--r--   0        0        0     6006 2024-03-28 22:16:36.421841 hpc-beeflow-0.1.7/beeflow/tests/test_config_validator.py
+-rw-r--r--   0        0        0      807 2024-03-28 22:16:36.422052 hpc-beeflow-0.1.7/beeflow/tests/test_container_path.py
+-rw-r--r--   0        0        0      946 2024-03-28 22:16:36.422217 hpc-beeflow-0.1.7/beeflow/tests/test_db_sched.py
+-rw-r--r--   0        0        0     4410 2024-03-28 22:16:36.422409 hpc-beeflow-0.1.7/beeflow/tests/test_db_tm.py
+-rw-r--r--   0        0        0    16813 2024-03-29 16:50:01.357222 hpc-beeflow-0.1.7/beeflow/tests/test_parser.py
+-rw-r--r--   0        0        0    15134 2024-03-28 22:16:36.422830 hpc-beeflow-0.1.7/beeflow/tests/test_scheduler.py
+-rw-r--r--   0        0        0     2630 2024-03-28 22:16:36.423055 hpc-beeflow-0.1.7/beeflow/tests/test_scheduler_resource_allocation.py
+-rw-r--r--   0        0        0     6557 2024-03-28 22:16:36.423487 hpc-beeflow-0.1.7/beeflow/tests/test_scheduler_rest.py
+-rw-r--r--   0        0        0     4908 2024-03-28 22:16:36.423804 hpc-beeflow-0.1.7/beeflow/tests/test_slurm_worker.py
+-rw-r--r--   0        0        0     3796 2024-03-29 16:50:01.358063 hpc-beeflow-0.1.7/beeflow/tests/test_tm.py
+-rw-r--r--   0        0        0    33819 2024-03-28 22:16:36.424442 hpc-beeflow-0.1.7/beeflow/tests/test_wf_interface.py
+-rw-r--r--   0        0        0    11213 2024-03-29 16:50:01.358653 hpc-beeflow-0.1.7/beeflow/tests/test_wf_manager.py
+-rwxr-xr-x   0        0        0     7823 2024-03-28 22:16:36.425016 hpc-beeflow-0.1.7/beeflow/wf_manager/common/dep_manager.py
+-rw-r--r--   0        0        0    10373 2024-03-28 22:16:36.425189 hpc-beeflow-0.1.7/beeflow/wf_manager/common/wf_db.py
+-rw-r--r--   0        0        0     4722 2024-03-29 16:50:01.359171 hpc-beeflow-0.1.7/beeflow/wf_manager/resources/wf_actions.py
+-rw-r--r--   0        0        0     8674 2024-03-28 22:16:36.425643 hpc-beeflow-0.1.7/beeflow/wf_manager/resources/wf_list.py
+-rw-r--r--   0        0        0      560 2024-03-28 22:16:36.425839 hpc-beeflow-0.1.7/beeflow/wf_manager/resources/wf_metadata.py
+-rw-r--r--   0        0        0     6266 2024-03-29 16:50:01.359605 hpc-beeflow-0.1.7/beeflow/wf_manager/resources/wf_update.py
+-rw-r--r--   0        0        0     8816 2024-03-28 22:16:36.426616 hpc-beeflow-0.1.7/beeflow/wf_manager/resources/wf_utils.py
+-rw-r--r--   0        0        0     1793 2024-03-28 22:16:36.426816 hpc-beeflow-0.1.7/beeflow/wf_manager/wf_manager.py
+-rw-r--r--   0        0        0     2715 2024-03-29 16:50:01.369059 hpc-beeflow-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     9244 2024-04-01 17:14:02.170565 hpc-beeflow-0.1.7/setup.py
+-rw-r--r--   0        0        0     7288 2024-04-01 17:14:02.171060 hpc-beeflow-0.1.7/PKG-INFO
```

### Comparing `hpc_beeflow-0.1.6/LICENSE` & `hpc-beeflow-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/README.rst` & `hpc-beeflow-0.1.7/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 Contributors:
 ==========================
 
 * Steven Anaya - `Boogie3D <https://github.com/Boogie3D>`_
 * Paul Bryant - `paulbry <https://github.com/paulbry>`_
 * Rusty Davis - `rstyd <https://github.com/rstyd>`_
 * Jieyang Chen - `JieyangChen7 <https://github.com/JieyangChen7>`_
+* Krishna Chilleri - `Krishna Chilleri <https://github.com/kchilleri>`_
 * Patricia Grubel - `pagrubel <https://github.com/pagrubel>`_
 * Qiang Guan - `guanxyz <https://github.com/guanxyz>`_
 * Ragini Gupta - `raginigupta6 <https://github.com/raginigupta6>`_
 * Andres Quan - `aquan9 <https://github.com/aquan9>`_
 * Quincy Wofford - `qwofford <https://github.com/qwofford>`_
 * Tim Randles - `trandles-lanl <https://github.com/trandles-lanl>`_
 * Jacob Tronge - `jtronge <https://github.com/jtronge>`_
@@ -81,13 +82,12 @@
 ==========================
 License can be found `here <https://github.com/lanl/BEE/blob/master/LICENSE>`_
 
 
 Publications
 ==========================
 
+- An HPC-Container Based Continuous Integration Tool for Detecting Scaling and Performance Issues in HPC Applications, IEEE Transactions on Services Computing, 2024, `DOI: 10.1109/TSC.2023.3337662 <https://doi.ieeecomputersociety.org/10.1109/TSC.2023.3337662>`_
 - BEE Orchestrator: Running Complex Scientific Workflows on Multiple Systems, HiPC, 2021, `DOI: 10.1109/HiPC53243.2021.00052 <https://doi.org/10.1109/HiPC53243.2021.00052>`_
 - "BeeSwarm: Enabling Parallel Scaling Performance Measurement in Continuous Integration for HPC Applications", ASE, 2021, `DOI: 10.1109/ASE51524.2021.9678805 <https://www.computer.org/csdl/proceedings-article/ase/2021/033700b136/1AjTjgnW2pa#:~:text=10.1109/ASE51524.2021.9678805>`_
 - "BeeFlow: A Workflow Management System for In Situ Processing across HPC and Cloud Systems", ICDCS, 2018, `DOI: 10.1109/ICDCS.2018.00103 <https://ieeexplore.ieee.org/abstract/document/8416366>`_
 - "Build and execution environment (BEE): an encapsulated environment enabling HPC applications running everywhere", IEEE BigData, 2018, `DOI: 10.1109/BigData.2018.8622572 <https://ieeexplore.ieee.org/document/8622572>`_
-
-
```

### Comparing `hpc_beeflow-0.1.6/beeflow/client/bee_client.py` & `hpc-beeflow-0.1.7/beeflow/client/bee_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 from beeflow.common import config_driver
 from beeflow.common.cli import NaturalOrderGroup
 from beeflow.common.connection import Connection
 from beeflow.common import paths
 from beeflow.common.parser import CwlParser
 from beeflow.common.wf_data import generate_workflow_id
 from beeflow.client import core
+from beeflow.wf_manager.resources import wf_utils
 
 # Length of a shortened workflow ID
 short_id_len = 6 #noqa: Not a constant
 
 # Maximum length of a workflow ID
 MAX_ID_LEN = 32
 
@@ -101,23 +102,33 @@
     return wf_id[:short_id_len]
 
 
 def _resource(tag=""):
     return _url() + str(tag)
 
 
+def get_wf_list():
+    """Get the list of all workflows."""
+    try:
+        conn = _wfm_conn()
+        resp = conn.get(_url(), timeout=60)
+    except requests.exceptions.ConnectionError:
+        error_exit('Could not reach WF Manager.')
+
+    if resp.status_code != requests.codes.okay:  # pylint: disable=no-member
+        error_exit('WF Manager did not return workflow list')
+
+    logging.info('List Jobs:  {resp.text}')
+    return jsonpickle.decode(resp.json()['workflow_list'])
+
+
 def check_short_id_collision():
     """Check short workflow IDs for colliions; increase short ID length if detected."""
     global short_id_len  #noqa: Not a constant
-    conn = _wfm_conn()
-    resp = conn.get(_url(), timeout=60)
-    if resp.status_code != requests.codes.okay:  # pylint: disable=no-member
-        error_exit(f"Checking for ID collision failed: {resp.status_code}")
-
-    workflow_list = jsonpickle.decode(resp.json()['workflow_list'])
+    workflow_list = get_wf_list()
     if workflow_list:
         while short_id_len < MAX_ID_LEN:
             id_list = [_short_id(job[1]) for job in workflow_list]
             id_list_set = set(id_list)
             # Collision if set shorter than list
             if len(id_list_set) < len(id_list):
                 short_id_len += 1
@@ -128,26 +139,15 @@
     else:
         print("There are currently no jobs.")
 
 
 def match_short_id(wf_id):
     """Match user-provided short workflow ID to full workflow IDs."""
     matched_ids = []
-
-    try:
-        conn = _wfm_conn()
-        resp = conn.get(_url(), timeout=60)
-    except requests.exceptions.ConnectionError:
-        error_exit('Could not reach WF Manager.')
-
-    if resp.status_code != requests.codes.okay:  # pylint: disable=no-member
-        error_exit(f'Could not match ID: {wf_id}. Code {resp.status_code}')
-        # raise ApiError("GET /jobs".format(resp.status_code))
-
-    workflow_list = jsonpickle.decode(resp.json()['workflow_list'])
+    workflow_list = get_wf_list()
     if workflow_list:
         for job in workflow_list:
             if job[1].startswith(wf_id):
                 matched_ids.append(job[1])
         if len(matched_ids) > 1:
             logging.info(f"user-provided workflow ID {wf_id} matched multiple stored workflow IDs")
             error_exit("provided workflow ID ambiguous")
@@ -158,19 +158,33 @@
                        "workflows")
         else:
             logging.info(f"user-provided workflow ID {wf_id} matched stored"
                          "workflow ID {matched_ids[0]}")
             long_wf_id = matched_ids[0]
             return long_wf_id
     else:
-        print("There are currently no workflows.")
+        sys.exit("There are currently no workflows.")
 
     return None
 
 
+def get_wf_status(wf_id):
+    """Get workflow status."""
+    try:
+        conn = _wfm_conn()
+        resp = conn.get(_resource(wf_id), timeout=60)
+    except requests.exceptions.ConnectionError:
+        error_exit('Could not reach WF Manager.')
+
+    if resp.status_code != requests.codes.okay:  # pylint: disable=no-member
+        error_exit('Could not successfully query workflow manager')
+
+    return resp.json()['wf_status']
+
+
 app = typer.Typer(no_args_is_help=True, add_completion=False, cls=NaturalOrderGroup)
 app.add_typer(core.app, name='core')
 app.add_typer(config_driver.app, name='config')
 
 
 @app.command()
 def submit(wf_name: str = typer.Argument(..., help='the workflow name'),  # pylint:disable=R0915
@@ -277,14 +291,27 @@
                 f"{_short_id(wf_id)}.", fg=typer.colors.GREEN)
     logging.info('Sumit workflow:  {resp.text}')
 
     # Cleanup code
     if tarball_path:
         os.remove(tarball_path)
 
+    # Store provided arguments in text file for future reference
+    wf_dir = wf_utils.get_workflow_dir(wf_id)
+    sub_wf_dir = wf_dir + "/submit_command_args.txt"
+
+    f_name = open(sub_wf_dir, "w", encoding="utf-8")
+    f_name.write(f"wf_name: {wf_name}\n")
+    f_name.write(f"wf_path: {wf_path}\n")
+    f_name.write(f"main_cwl: {main_cwl}\n")
+    f_name.write(f"yaml: {yaml}\n")
+    f_name.write(f"workdir: {workdir}\n")
+    f_name.write(f"wf_id: {wf_id}")
+    f_name.close()
+
     return wf_id
 
 
 @app.command()
 def start(wf_id: str = typer.Argument(..., callback=match_short_id)):
     """Start a workflow with a workflow ID."""
     long_wf_id = wf_id
@@ -336,14 +363,44 @@
         error_exit("Package failed")
     else:
         print(f"Package {tarball} created successfully")
 
     return package_path
 
 
+@app.command()
+def remove(wf_id: str = typer.Argument(..., callback=match_short_id)):
+    """Remove cancelled, paused, or archived workflow with a workflow ID."""
+    long_wf_id = wf_id
+
+    wf_status = get_wf_status(wf_id)
+    print(f"Workflow Status is {wf_status}")
+    if wf_status in ('Cancelled', 'Archived', 'Paused'):
+        verify = f"All stored information for workflow {_short_id(wf_id)} will be removed."
+        verify += "\nContinue to remove? yes(y)/no(n): """
+        response = input(verify)
+        if response in ("n", "no"):
+            sys.exit("Workflow not removed.")
+        elif response in ("y", "yes"):
+            try:
+                conn = _wfm_conn()
+                resp = conn.delete(_resource(long_wf_id), json={'option': 'remove'}, timeout=60)
+            except requests.exceptions.ConnectionError:
+                error_exit('Could not reach WF Manager.')
+            if resp.status_code != requests.codes.accepted:  # pylint: disable=no-member
+                error_exit('WF Manager could not remove workflow.')
+            typer.secho("Workflow removed!", fg=typer.colors.GREEN)
+            logging.info(f'Remove workflow: {resp.text}')
+    else:
+        print(f"{_short_id(wf_id)} may still be running.")
+        print("The workflow must be cancelled before attempting removal.")
+
+    sys.exit()
+
+
 def unpackage(package_path, dest_path):
     """Unpackage a workflow tarball for parsing."""
     package_str = str(package_path)
     package_path = package_path.resolve()
 
     if not package_str.endswith('.tgz'):
         # No cleanup, maybe we should rm dest_path?
@@ -359,25 +416,15 @@
         print(f"Package {package_str} unpackaged successfully")
     return pathlib.Path(dest_path / wf_dir)
 
 
 @app.command('list')
 def list_workflows():
     """List all workflows."""
-    try:
-        conn = _wfm_conn()
-        resp = conn.get(_url(), timeout=60)
-    except requests.exceptions.ConnectionError:
-        error_exit('Could not reach WF Manager.')
-
-    if resp.status_code != requests.codes.okay:  # pylint: disable=no-member
-        error_exit('WF Manager did not return workflow list')
-
-    logging.info('List Jobs:  {resp.text}')
-    workflow_list = jsonpickle.decode(resp.json()['workflow_list'])
+    workflow_list = get_wf_list()
     if workflow_list:
         typer.secho("Name\tID\tStatus", fg=typer.colors.GREEN)
 
         for name, wf_id, status in workflow_list:
             typer.echo(f"{name}\t{_short_id(wf_id)}\t{status}")
     else:
         typer.echo("There are currently no workflows.")
@@ -397,19 +444,17 @@
         error_exit('Could not reach WF Manager.')
 
     if resp.status_code != requests.codes.okay:  # pylint: disable=no-member
         error_exit('Could not successfully query workflow manager')
 
     tasks_status = resp.json()['tasks_status']
     wf_status = resp.json()['wf_status']
-    if tasks_status == 'Unavailable':
-        typer.echo(wf_status)
-    else:
-        typer.echo(wf_status)
-        typer.echo(tasks_status)
+    typer.echo(wf_status)
+    for _task_id, task_name, task_state in tasks_status:
+        typer.echo(f'{task_name}--{task_state}')
 
     logging.info('Query workflow:  {resp.text}')
     return wf_status, tasks_status
 
 
 @app.command()
 def metadata(wf_id: str = typer.Argument(..., callback=match_short_id)):
@@ -459,25 +504,32 @@
     if resp.status_code != requests.codes.okay:  # pylint: disable=no-member
         error_exit('WF Manager could not resume workflow.')
     logging.info('Resume workflow:  {resp.text}')
 
 
 @app.command()
 def cancel(wf_id: str = typer.Argument(..., callback=match_short_id)):
-    """Cancel a workflow."""
+    """Cancel a paused or running workflow."""
     long_wf_id = wf_id
-    try:
-        conn = _wfm_conn()
-        resp = conn.delete(_resource(long_wf_id), timeout=60)
-    except requests.exceptions.ConnectionError:
-        error_exit('Could not reach WF Manager.')
-    if resp.status_code != requests.codes.accepted:  # pylint: disable=no-member
-        error_exit('WF Manager could not cancel workflow.')
-    typer.secho("Workflow cancelled!", fg=typer.colors.GREEN)
-    logging.info(f'Cancel workflow: {resp.text}')
+    wf_status = get_wf_status(wf_id)
+    if wf_status in ('Running', 'Paused'):
+        try:
+            conn = _wfm_conn()
+            resp = conn.delete(_resource(long_wf_id), json={'option': 'cancel'}, timeout=60)
+
+        except requests.exceptions.ConnectionError:
+            error_exit('Could not reach WF Manager.')
+        if resp.status_code != requests.codes.accepted:  # pylint: disable=no-member
+            error_exit('WF Manager could not cancel workflow.')
+        typer.secho("Workflow cancelled!", fg=typer.colors.GREEN)
+        logging.info(f'Cancel workflow: {resp.text}')
+    elif wf_status == "Intializing":
+        print(f"Workflow is {wf_status}, try cancel later.")
+    else:
+        print(f"Workflow is {wf_status} cannot cancel.")
 
 
 @app.command()
 def copy(wf_id: str = typer.Argument(..., callback=match_short_id)):
     """Copy an archived workflow."""
     long_wf_id = wf_id
     try:
```

### Comparing `hpc_beeflow-0.1.6/beeflow/client/core.py` & `hpc-beeflow-0.1.7/beeflow/client/core.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,24 +10,32 @@
 """
 import os
 import signal
 import subprocess
 import socket
 import sys
 import shutil
+import datetime
 import time
 
 import daemon
 import typer
 
+from beeflow.client import bee_client
 from beeflow.common.config_driver import BeeConfig as bc
 from beeflow.common import cli_connection
 from beeflow.common import paths
 from beeflow.wf_manager.resources import wf_utils
 
+from beeflow.common.db import wfm_db
+from beeflow.common.db.bdb import connect_db
+from beeflow.wf_manager.common import dep_manager
+
+db_path = wf_utils.get_db_path()
+
 
 class ComponentManager:
     """Component manager class."""
 
     def __init__(self):
         """Construct the component manager."""
         self.components = {}
@@ -167,16 +175,16 @@
     if need_slurmrestd():
         tm_deps.append('slurmrestd')
 
     @mgr.component('task_manager', tm_deps)
     def start_task_manager():
         """Start the TM."""
         fp = open_log('task_manager')
-        return launch_with_gunicorn('beeflow.task_manager:flask_app', paths.tm_socket(),
-                                    stdout=fp, stderr=fp)
+        return launch_with_gunicorn('beeflow.task_manager.task_manager:create_app()',
+                                    paths.tm_socket(), stdout=fp, stderr=fp)
 
     @mgr.component('scheduler', ())
     def start_scheduler():
         """Start the scheduler."""
         fp = open_log('scheduler')
         # Using a function here because of the funny way that the scheduler's written
         return launch_with_gunicorn('beeflow.scheduler.scheduler:create_app()',
@@ -224,14 +232,15 @@
         ]
         log = open_log('redis')
         # Ran into a strange "Failed to configure LOCALE for invalid locale name."
         # from Redis, so setting LANG=C. This could have consequences for UTF-8
         # strings.
         env = dict(os.environ)
         env['LANG'] = 'C'
+        env['LC_ALL'] = 'C'
         return subprocess.Popen(cmd, env=env, stdout=log, stderr=log)
 
     # Workflow manager and task manager need to be opened with PIPE for their stdout/stderr
     if need_slurmrestd():
         @mgr.component('slurmrestd')
         def start_slurm_restd():
             """Start BEESlurmRestD. Returns a Popen process object."""
@@ -398,15 +407,15 @@
                 pass
         else:
             # It's already running, so print an error and exit
             warn(f'Beeflow appears to be running. Check the beeflow log: "{beeflow_log}"')
             sys.exit(1)
     print('Starting beeflow...')
     if not foreground:
-        print(f'Check "{beeflow_log}" or run `beeflow core status` for more information.')
+        print('Run `beeflow core status` for more information.')
     # Create the log path if it doesn't exist yet
     path = paths.log_path()
     os.makedirs(path, exist_ok=True)
     base_components = ['wf_manager', 'task_manager', 'scheduler']
     if foreground:
         try:
             Beeflow(mgr, base_components).loop()
@@ -427,99 +436,142 @@
         sys.exit(1)
     print('beeflow components:')
     for comp, stat in resp['components'].items():
         print(f'{comp} ... {stat}')
 
 
 @app.command()
-def stop():
+def stop(query='yes'):
     """Stop the current running beeflow daemon."""
-    stop_msg = ("\n** Please ensure all workflows are complete before stopping beeflow. **"
-                + "\n** Check the status of workflows by running 'beeflow list'.    **"
-                + "\nAre you sure you want to kill beeflow components? [y/n] ")
-    ans = input(stop_msg)
+    if query == 'yes':
+        ans = input("""
+              ** Please ensure all workflows are complete before stopping beeflow. **
+              ** Check the status of workflows by running 'beeflow list'.    **
+
+              Are you sure you want to kill beeflow components? [y/n] """)
+    else:
+        ans = 'y'
     if ans.lower() != 'y':
         return
     resp = cli_connection.send(paths.beeflow_socket(), {'type': 'quit'})
     if resp is None:
         beeflow_log = paths.log_fname('beeflow')
         warn('Error: beeflow is not running on this system. It could be '
              'running on a different front end.\n'
              f'       Check the beeflow log: "{beeflow_log}".')
         sys.exit(1)
     # As long as it returned something, we should be good
     beeflow_log = paths.log_fname('beeflow')
-    print(f'Beeflow has stopped. Check the log at "{beeflow_log}".')
+    if query == "no":
+        print(f'Beeflow has stopped. Check the log at "{beeflow_log}".')
+
+
+def kill_active_workflows(active_states, workflow_list):
+    """Kill workflows with active states."""
+    db = connect_db(wfm_db, db_path)
+    success = True
+    for name, wf_id, state in workflow_list:
+        if state in active_states:
+            pid = db.workflows.get_gdb_pid(wf_id)
+            if pid > 0:
+                dep_manager.kill_gdb(pid)
+            else:
+                # Failure most likely caused by an Initializing workflow.
+                print(f"No process for {name}, {wf_id}, {state}.")
+                success = False
+    return success
+
+
+def archive_dir(dir_to_archive):
+    """Archive directories for archive flag in reset."""
+    archive_dirs = ['logs', 'container_archive', 'archives', 'workflows']
+    date_str = f"{datetime.datetime.now().strftime('%Y-%m-%d_%H%M%S')}"
+    backup_dir = f"{dir_to_archive}.{date_str}"
+    for a_dir in archive_dirs:
+        try:
+            shutil.copytree(f"{dir_to_archive}/{a_dir}",
+                            f"{backup_dir}/{a_dir}")
+        except FileNotFoundError:
+            pass
+    print("Archive flag enabled.",
+          "Existing logs, containers, and workflows backed up in:\n"
+          f"{backup_dir}")
+
+
+def handle_rm_error(err, dir_to_check, wf_list):
+    """Handle IO error caused by either initializing workflows or nfs files."""
+    # Check if only nfs mounts are causing the problem and ignore
+    dir_list = os.listdir(dir_to_check)
+    nfs_list = [x for x in dir_list if x.startswith('.nfs')]
+    if dir_list and (dir_list != nfs_list):
+        print(f"Unable to remove {dir_to_check} \n {err.strerror}")
+        # Often initializing workflows cause a problem
+        if any('Initializing' in sublist for sublist in wf_list):
+            warn('Initializing workflows may have prevented removal.\n')
+            print(f"Try removing {dir_to_check} manually, to complete reset.")
 
 
 @app.command()
 def reset(archive: bool = typer.Option(False, '--archive', '-a',
                                        help='Archive bee_workdir  before removal')):
-    """Delete the bee_workdir directory."""
-    # Check to see if the user is absolutely sure. Warning Message.
+    """Stop all components and delete the bee_workdir directory."""
+    # Check workflow states; warn if there are active states.
+    workflow_list = bee_client.get_wf_list()
+    active_states = {'Running', 'Paused', 'Initializing', 'Waiting'}
+    caution = ""
+    if {item for row in workflow_list for item in row}.intersection(active_states):
+        caution = """
+        **************************************************************
+          Caution: There are active workflows! They will be removed!
+          Try 'beeflow list' to view them.
+        **************************************************************
+        """
     absolutely_sure = ""
+    dir_to_delete = os.path.expanduser(wf_utils.get_bee_workdir())
+    warn(f"\n    A reset will remove this directory: {dir_to_delete}\n")
+    if archive:
+        print("    Archive flag is set: logs, workflows and containers will be backed up.")
+    print("""
+    A reset will:
+        Shutdown beeflow and all BEE components.
+        Delete the bee_workdir directory which results in:
+            Removing the archive of all workflows.
+            Removing the archive of workflow containers
+                (unless container_archive is configured elsewhere).
+            Reset all databases associated with the beeflow app.
+            Removing all beeflow logs.
+    Beeflow configuration files from bee_cfg will not be deleted.
+    """)
+    warn(f"{caution}\nAre you sure you want to reset?")
     while absolutely_sure != "y" or absolutely_sure != "n":
-        # Get the user's bee_workdir directory
-        directory_to_delete = os.path.expanduser(wf_utils.get_bee_workdir())
-        print(f"A reset will remove this directory: {directory_to_delete}")
-
-        absolutely_sure = input(
-            """
-Are you sure you want to reset?
-
-Please ensure all workflows are complete before running a reset
-Check the status of workflows by running 'beeflow list'
-
-A reset will shutdown beeflow and its components.
-
-A reset will delete the bee_workdir directory which results in:
-Removing the archive of workflows executed.
-Removing the archive of workflow containers.
-Reset all databases associated with the beeflow app.
-Removing all beeflow logs.
-
-Beeflow configuration files from bee_cfg will remain.
-
-Respond with yes(y)/no(n):  """)
+        absolutely_sure = input("Respond with yes(y)/no(n): ")
         if absolutely_sure in ("n", "no"):
             # Exit out if the user didn't really mean to do a reset
             sys.exit()
-        if absolutely_sure in ("y", "yes"):
+        elif absolutely_sure in ("y", "yes"):
+            # First stop all active workflow processes
+            workflow_list = bee_client.get_wf_list()
+            kill_active_workflows(active_states, workflow_list)
             # Stop all of the beeflow processes
-            resp = cli_connection.send(paths.beeflow_socket(), {'type': 'quit'})
-            if resp is not None:
-                print("Beeflow has been shutdown.")
-                print("Waiting for components to cleanly stop.")
-                # This wait is essential. It takes a minute to shut down.
-                time.sleep(5)
-
-            if os.path.exists(directory_to_delete):
-                # Save the bee_workdir directory if the archive option was set
-                if archive:
-                    if os.path.exists(directory_to_delete + "/logs"):
-                        shutil.copytree(directory_to_delete + "/logs",
-                                        directory_to_delete + ".backup/logs")
-                    if os.path.exists(directory_to_delete + "/container_archive"):
-                        shutil.copytree(directory_to_delete + "/container_archive",
-                                        directory_to_delete + ".backup/container_archive")
-                    if os.path.exists(directory_to_delete + "/archives"):
-                        shutil.copytree(directory_to_delete + "/archives",
-                                        directory_to_delete + ".backup/archives")
-                    if os.path.exists(directory_to_delete + "/workflows"):
-                        shutil.copytree(directory_to_delete + "/workflows",
-                                        directory_to_delete + ".backup/workflows")
-                    print("Archive flag enabled,")
-                    print("Existing logs, containers, and workflows backed up in:")
-                    print(f"{directory_to_delete}.backup")
-                shutil.rmtree(directory_to_delete)
-                print(f"{directory_to_delete} has been removed.")
-                sys.exit()
+            stop("quiet")
+            print("Beeflow is shutting down.")
+            print("Waiting for components to cleanly stop.")
+            # This wait is essential. It takes a minute to shut down.
+            time.sleep(5)
+
+            # Save the bee_workdir directory if the archive option was set
+            if archive:
+                archive_dir(dir_to_delete)
+            try:
+                shutil.rmtree(dir_to_delete)
+            except OSError as err:
+                handle_rm_error(err, dir_to_delete, workflow_list)
             else:
-                print(f"{directory_to_delete} does not exist. Exiting.")
-                sys.exit()
+                print(f"{dir_to_delete} has been removed.")
+            sys.exit()
         print("Please respond with either the letter (y) or (n).")
 
 
 @app.command()
 def restart(foreground: bool = typer.Option(False, '--foreground', '-F',
             help='run in the foreground')):
     """Attempt to stop and restart the beeflow daemon."""
```

### Comparing `hpc_beeflow-0.1.6/beeflow/cloud_launcher.py` & `hpc-beeflow-0.1.7/beeflow/cloud_launcher.py`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/common/build/README.md` & `hpc-beeflow-0.1.7/beeflow/common/build/README.md`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/common/build/build_driver.py` & `hpc-beeflow-0.1.7/beeflow/common/build/build_driver.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,10 @@
 """Abstract base class for the handling build systems."""
 
 from abc import ABC, abstractmethod
-import jsonpickle
-
-
-def arg2task(task_arg):
-    """Convert JSON encoded task to Task object.
-
-    The build driver will expect a Task object, and the build
-    interface starts with a JSON representation of the Task object.
-    """
-    return jsonpickle.decode(task_arg)
-
-
-def task2arg(task):
-    """Convert Task object to JSON encoded string.
-
-    The build interface needs to pass Task data on the command line,
-    because each compute node needs to understand the Task description.
-    JSON format is a convenient way to describe the Task object at the
-    command line.
-    """
-    return jsonpickle.encode(task)
 
 
 class BuildDriver(ABC):
     """Driver interface between WFM and a generic build system.
 
     A driver object must implement an __init__ method that
     requests a Runtime Environment (RTE), and a method to
```

### Comparing `hpc_beeflow-0.1.6/beeflow/common/build/container_drivers.py` & `hpc-beeflow-0.1.7/beeflow/common/build/container_drivers.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 import os
 import shutil
 import subprocess
 import tempfile
 from beeflow.common.config_driver import BeeConfig as bc
 from beeflow.common import log as bee_logging
+from beeflow.common.build.utils import ContainerBuildError
 from beeflow.common.build.build_driver import BuildDriver
 from beeflow.common.crt.charliecloud_driver import CharliecloudDriver as crt_driver
 
 
 log = bee_logging.setup(__name__)
 
 
@@ -121,16 +122,15 @@
 
         # Use task specified image if image parameter empty
         if not addr:
             addr = task_addr
 
         # If Requirement is set but not specified, and param empty, do nothing and error.
         if self.task.requirements == {} and not addr:
-            log.error("dockerPull set but no image path specified.")
-            return 1
+            raise ContainerBuildError("dockerPull set but no image path specified.")
         # If no image specified and no image required, nothing to do.
         if not task_addr and not addr:
             log.info('No image specified and no image required, nothing to do.')
             return 0
 
         # Determine name for successful build target
         ch_build_addr = addr.replace('/', '%')
@@ -166,37 +166,36 @@
         download a Docker image using docker load.
         """
         # Need to know if dockerLoad is specified in order to determine fail/success
         req_dockerload = self.get_docker_req('dockerLoad')
         log.warning('Charliecloud does not have the concept of a layered image tarball.')
         log.warning('Did you mean to use dockerImport?')
         if req_dockerload:
-            log.warning('dockerLoad specified as requirement.')
-            return 1
+            raise ContainerBuildError('dockerLoad is not supported')
         return 0
 
     def process_docker_file(self, task_dockerfile=None, force=False):
         """Get and process the CWL compliant dockerFile dockerRequirement.
 
         CWL spec 09-23-2020: Supply the contents of a Dockerfile
         which will be built using docker build. We have discussed implementing CWL
         change to expect a file handle instead of file contents, and use the file
         handle expectation here.
         """
         # beeflow:containerName is always processed before dockerFile, so safe to assume it exists
         # otherwise, raise an error.
         if self.container_name is None:
-            log.error("dockerFile may not be specified without beeflow:containerName")
-            return 1
+            raise ContainerBuildError(
+                "dockerFile may not be specified without beeflow:containerName"
+            )
 
         # Need dockerfile in order to build, else fail
         task_dockerfile = self.get_docker_req('dockerFile')
         if not task_dockerfile:
-            log.error("dockerFile not specified as task attribute or parameter.")
-            return 1
+            raise ContainerBuildError("dockerFile not specified as task attribute or parameter.")
 
         # Create context directory to use as Dockerfile context, use container name so user
         # can prep the directory with COPY sources as needed.
         context_dir = os.path.expanduser('~')
         log.info(f'Context directory will be {context_dir}')
 
         # Determine name for successful build target
@@ -277,15 +276,15 @@
 
         # Set imageid
         self.docker_image_id = task_image_id
 
         # If task and parameter still doesn't specify ImageId, consider this an error.
         if not self.docker_image_id:
             return 0
-        return 1
+        raise ContainerBuildError('dockerImageId is required but not found')
 
     def process_docker_output_directory(self, param_output_directory=None):
         """Get and process the CWL compliant dockerOutputDirectory dockerRequirement.
 
         CWL spec 09-23-2020: Set the designated output directory
         to a specific location inside the Docker container. The
         param_output_directory may be used to override DockerRequirement
@@ -304,16 +303,17 @@
         If you have a container tarball, and all you need to do is stage it,
         that is, all you need to do is copy it to a location that BEE knows,
         use this to put the container into the build archive.
         """
         # Need container_path to know how dockerfile should be named, else fail
         task_container_path = self.get_docker_req('beeflow:copyContainer')
         if not task_container_path:
-            log.error("beeflow:copyContainer: You must specify the path to an existing container.")
-            return 1
+            raise ContainerBuildError(
+                "beeflow:copyContainer: You must specify the path to an existing container."
+            )
 
         if self.container_name:
             copy_target = '/'.join([self.container_archive, self.container_name + '.tar.gz'])
         else:
             copy_target = '/'.join([self.container_archive,
                                     crt_driver.get_ccname(task_container_path) + '.tar.gz'])
         log.info(f'Build will copy a container to {copy_target}')
@@ -341,16 +341,17 @@
 
         The CWL spec currently uses dockerImageId to refer to the name of a container
         but this is explicitly not how Docker defines it. We need a way to name
         containers in a human readable format.
         """
         task_container_name = self.get_docker_req('beeflow:containerName')
         if not task_container_name and self.docker_image_id is None:
-            log.error("beeflow:containerName: You must specify the containerName or dockerImageId")
-            return 1
+            raise ContainerBuildError(
+                "beeflow:containerName: You must specify the containerName or dockerImageId"
+            )
         self.container_name = task_container_name
         log.info(f'Setting container_name to: {self.container_name}')
         return 0
 
 
 class SingularityBuildDriver(ContainerBuildDriver):
     """Driver interface between WFM and a container build system.
```

### Comparing `hpc_beeflow-0.1.6/beeflow/common/build_interfaces.py` & `hpc-beeflow-0.1.7/beeflow/common/build_interfaces.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # from beeflow.common.build.container_drivers import CharliecloudBuildDriver,
 #                                                    SingularityBuildDriver
 import sys
 from subprocess import CalledProcessError
 from beeflow.common.build.container_drivers import CharliecloudBuildDriver
 from beeflow.common.config_driver import BeeConfig as bc
 from beeflow.common import log as bee_logging
-from beeflow.common.build.build_driver import arg2task
+from beeflow.common.build.utils import arg2task, ContainerBuildError
 
 
 log = bee_logging.setup(__name__)
 
 
 def build_main(task):
     """Process build instructions - main code."""
@@ -43,17 +43,19 @@
         try:
             return_obj = op_dict["build_op"]()
             # Return objects will be successful subprocess or return code.
             try:
                 return_code = return_obj.returncode
             except AttributeError:
                 return_code = int(return_obj)
-        except CalledProcessError:
+        except CalledProcessError as error:
             return_code = 1
-            log.warning(f'There was a problem executing {op_dict["op_name"]}!')
+            raise ContainerBuildError(
+                f'There was a problem executing {op_dict["op_name"]}!'
+            ) from error
         # Case 1: Not the last operation spec'd, but is a terminal operation.
         if op_dict["op_terminal"] and return_code == 0:
             op_values = [None, None, None, True]
             op_dict = dict(zip(op_keys, op_values))
             continue
         # Case 2: Go to next, or last operation spec'd.
         try:
```

### Comparing `hpc_beeflow-0.1.6/beeflow/common/cli_connection.py` & `hpc-beeflow-0.1.7/beeflow/common/cli_connection.py`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/common/cloud/README.md` & `hpc-beeflow-0.1.7/beeflow/common/cloud/README.md`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/common/cloud/__init__.py` & `hpc-beeflow-0.1.7/beeflow/common/cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/common/cloud/chameleoncloud.py` & `hpc-beeflow-0.1.7/beeflow/common/cloud/chameleoncloud.py`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/common/cloud/google.py` & `hpc-beeflow-0.1.7/beeflow/common/cloud/google.py`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/common/cloud/openstack.py` & `hpc-beeflow-0.1.7/beeflow/common/cloud/openstack.py`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/common/cloud/provider.py` & `hpc-beeflow-0.1.7/beeflow/common/cloud/provider.py`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/common/config_driver.py` & `hpc-beeflow-0.1.7/beeflow/common/config_driver.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,18 @@
 elif _SYSTEM == 'Windows':
     CONF_DIR = os.path.expandvars(r'%APPDATA%\beeflow')
     SYSCONFIG_FILE = None
     USERCONFIG_FILE = os.path.expandvars(r'%APPDATA%\beeflow\bee.conf')
 else:
     raise RuntimeError(f'System "{_SYSTEM}" is not supported')
 
+BEE_CONFIG = os.getenv('BEE_CONFIG')
+if BEE_CONFIG is not None:
+    USERCONFIG_FILE = BEE_CONFIG
+
 
 class BeeConfig:
     r"""Class to manage and store all BEE configuration.
 
     All configuration values can be retrieved by using the get(section, key)
     class method. If those particular values are not in the config file, then
     defaults will be set, or a validation error raised, based on the validation code
```

### Comparing `hpc_beeflow-0.1.6/beeflow/common/config_validator.py` & `hpc-beeflow-0.1.7/beeflow/common/config_validator.py`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/common/connection.py` & `hpc-beeflow-0.1.7/beeflow/common/connection.py`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/common/container_path.py` & `hpc-beeflow-0.1.7/beeflow/common/container_path.py`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/common/crt/charliecloud_driver.py` & `hpc-beeflow-0.1.7/beeflow/common/crt/charliecloud_driver.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 """
 
 import os
 import yaml
 from beeflow.common.crt.crt_driver import (ContainerRuntimeDriver, ContainerRuntimeResult,
                                            Command, CommandType)
 from beeflow.common.config_driver import BeeConfig as bc
-from beeflow.common.build.build_driver import task2arg
+from beeflow.common.build.utils import task2arg
 from beeflow.common.container_path import convert_path
 from beeflow.common import log as bee_logging
 
 
 log = bee_logging.setup(__name__)
```

### Comparing `hpc_beeflow-0.1.6/beeflow/common/crt/crt_driver.py` & `hpc-beeflow-0.1.7/beeflow/common/crt/crt_driver.py`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/common/crt/singularity_driver.py` & `hpc-beeflow-0.1.7/beeflow/common/crt/singularity_driver.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Singularity driver as the container runtime system for tasks.
 
 Creates text for tasks using Singularity.
 """
 
 from beeflow.common.crt.crt_driver import (ContainerRuntimeDriver, ContainerRuntimeResult, Command)
-from beeflow.common.build.build_driver import task2arg
+from beeflow.common.build.utils import task2arg
 
 
 class SingularityDriver(ContainerRuntimeDriver):
     """The ContainerRuntimeDriver for Singularity as container runtime system.
 
     Creates the text for the task for using Singularity to test abstract class.
     """
```

### Comparing `hpc_beeflow-0.1.6/beeflow/common/crt_interface.py` & `hpc-beeflow-0.1.7/beeflow/common/crt_interface.py`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/common/db/bdb.py` & `hpc-beeflow-0.1.7/beeflow/common/db/bdb.py`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/common/db/sched_db.py` & `hpc-beeflow-0.1.7/beeflow/common/db/sched_db.py`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/common/db/tm_db.py` & `hpc-beeflow-0.1.7/beeflow/common/db/tm_db.py`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/common/db/wfm_db.py` & `hpc-beeflow-0.1.7/beeflow/common/db/wfm_db.py`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/common/expr.py` & `hpc-beeflow-0.1.7/beeflow/common/expr.py`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/common/gdb/DESIGN.md` & `hpc-beeflow-0.1.7/beeflow/common/gdb/DESIGN.md`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/common/gdb/gdb_driver.py` & `hpc-beeflow-0.1.7/beeflow/common/gdb/gdb_driver.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 """Abstract base class for the handling of workflow DAGs."""
 
 from abc import ABC, abstractmethod
+from beeflow.common import log as bee_logging
+
+log = bee_logging.setup(__name__)
 
 
 class GraphDatabaseDriver(ABC):
     """Driver interface for a generic graph database.
 
     The driver must implement a __init__ method that creates/connects to
     the graph database and returns some kind of 'connection' interface object.
```

### Comparing `hpc_beeflow-0.1.6/beeflow/common/gdb/neo4j_cypher.py` & `hpc-beeflow-0.1.7/beeflow/common/gdb/neo4j_cypher.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 """Neo4j/Cypher transaction functions used by the Neo4jDriver class."""
 
 from re import fullmatch
+from beeflow.common import log as bee_logging
+
+log = bee_logging.setup(__name__)
 
 
 def create_workflow_node(tx, workflow):
     """Create a Workflow node in the Neo4j database.
 
     The workflow node is the entry point to the workflow.
     :param workflow: the workflow description
```

### Comparing `hpc_beeflow-0.1.6/beeflow/common/gdb/neo4j_driver.py` & `hpc-beeflow-0.1.7/beeflow/common/gdb/neo4j_driver.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,14 +8,17 @@
 from neo4j import GraphDatabase as Neo4jDatabase
 from neobolt.exceptions import ServiceUnavailable
 
 from beeflow.common.gdb.gdb_driver import GraphDatabaseDriver
 from beeflow.common.gdb import neo4j_cypher as tx
 from beeflow.common.wf_data import (Workflow, Task, Requirement, Hint,
                                     InputParameter, OutputParameter, StepInput, StepOutput)
+from beeflow.common import log as bee_logging
+
+log = bee_logging.setup(__name__)
 
 # Default Neo4j authentication
 # We may want to instead get these from a config at some point
 DEFAULT_HOSTNAME = "localhost"
 DEFAULT_BOLT_PORT = "7687"
 DEFAULT_USER = "neo4j"
 DEFAULT_PASSWORD = "password"
@@ -47,14 +50,15 @@
         password = kwargs.get("db_pass", DEFAULT_PASSWORD)
         uri = f"bolt://{db_hostname}:{bolt_port}"
 
         try:
             # Connect to the Neo4j database using the Neo4j proprietary driver
             self._driver = Neo4jDatabase.driver(uri, auth=(user, password))
         except ServiceUnavailable as sue:
+            log.error("Neo4j database is unavailable")
             raise Neo4JNotRunning("Neo4j database is unavailable") from sue
 
     def initialize_workflow(self, workflow):
         """Begin construction of a workflow stored in Neo4j.
 
         Creates the Workflow, Requirement, and Hint nodes in the Neo4j database.
```

### Comparing `hpc_beeflow-0.1.6/beeflow/common/gdb_interface.py` & `hpc-beeflow-0.1.7/beeflow/common/gdb_interface.py`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/common/log.py` & `hpc-beeflow-0.1.7/beeflow/common/log.py`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/common/parser/README.md` & `hpc-beeflow-0.1.7/beeflow/common/parser/README.md`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/common/parser/parser.py` & `hpc-beeflow-0.1.7/beeflow/common/parser/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,14 @@
                                     OutputParameter,
                                     StepInput,
                                     StepOutput,
                                     Hint,
                                     Requirement,
                                     generate_workflow_id)
 
-
 # Map CWL types to Python types
 type_map = {
     "string": str,
     "int": int,
     "long": int,
     "float": float,
     "double": float,
@@ -137,14 +136,19 @@
         if isinstance(step.run, str):
             step_run = f"{os.path.dirname(step.id)}/{step.run}"
             step_cwl = cwl_parser.load_document(step_run)
             step_id = os.path.basename(step_cwl.id).split(".")[0]
         else:
             step_cwl = step.run
             step_id = _shortname(step.id)
+            # step_input.id needs to have its step.id prefix stripped
+            for step_input in step_cwl.inputs:
+                step_shortname = _shortname(step_input.id)
+                step_input.id = step_input.id.replace(step_shortname,
+                                                      step_shortname.split("/")[-1])
 
         if step_cwl.class_ != "CommandLineTool":
             raise CwlParseError(f"Step {step.id} class must be CommandLineTool")
 
         step_name = os.path.basename(step_id).split(".")[0]
         step_command = step_cwl.baseCommand
         step_inputs = self.parse_step_inputs(step.in_, step_cwl.inputs)
@@ -298,18 +302,28 @@
         :rtype: list of Hint or list of Requirement or None
         """
         reqs = []
         if not requirements:
             return reqs
         if as_hints:
             for req in requirements:
-                items = {k: str(v) for k, v in req.items() if k != "class"}
+                items = {}
+                for k, v in req.items():
+                    if k != 'class':
+                        if isinstance(v, (int, float)):
+                            items[k] = v
+                        else:
+                            items[k] = str(v)
                 # Load in the dockerfile at parse time
                 if 'dockerFile' in items:
                     self._read_requirement_file('dockerFile', items)
+                if 'pre_script' in items and items['enabled']:
+                    self._read_requirement_file('pre_script', items)
+                if 'post_script' in items and items['enabled']:
+                    self._read_requirement_file('post_script', items)
                 if 'beeflow:bindMounts' in items:
                     self._read_requirement_file('beeflow:bindMounts', items)
                 reqs.append(Hint(req['class'], items))
         else:
             for req in requirements:
                 reqs.append(Requirement(req.class_, {k: str(v) for k, v in vars(req).items()
                                                      if k not in ("extension_fields",
```

### Comparing `hpc_beeflow-0.1.6/beeflow/common/paths.py` & `hpc-beeflow-0.1.7/beeflow/common/paths.py`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/common/validation.py` & `hpc-beeflow-0.1.7/beeflow/common/validation.py`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/common/wf_data.py` & `hpc-beeflow-0.1.7/beeflow/common/wf_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -193,14 +193,44 @@
                 # Try to get Hints
                 requirement = hints[req_type][req_param]
             except (KeyError, TypeError):
                 # Task Hints are not mandatory. No docker_req_param specified in task hints.
                 requirement = default
         return requirement
 
+    def get_full_requirement(self, req_type):
+        """Get the full requirement (or hint) for this task, if it has one.
+
+        :param req_type: the type of requirement (e.g. 'DockerRequirement')
+        :type req_type: str
+
+        This prefers requirements over hints. Returns None if no hint or
+        requirement found.
+        """
+        result = None
+        hints = dict(self.hints)
+        try:
+            # Try to get Hints
+            hint = hints[req_type]
+        except (KeyError, TypeError):
+            # Task Hints are not mandatory. No task hint specified.
+            hint = None
+        try:
+            # Try to get Requirements
+            req = self.requirements[req_type]
+        except (KeyError, TypeError):
+            # Task Requirements are not mandatory. No task requirement specified.
+            req = None
+        # Prefer requirements over hints
+        if req:
+            result = req
+        elif hint:
+            result = hint
+        return result
+
     def __eq__(self, other):
         """Test the equality of two tasks.
 
         Task ID and dependencies do not factor into equality testing.
         :param other: the task with which to test equality
         :type other: Task
         :rtype: bool
```

### Comparing `hpc_beeflow-0.1.6/beeflow/common/wf_interface.py` & `hpc-beeflow-0.1.7/beeflow/common/wf_interface.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 """High-level BEE workflow management interface.
 
 Delegates its work to a GraphDatabaseInterface instance.
 """
 
 import re
+from beeflow.common import log as bee_logging
+
+log = bee_logging.setup(__name__)
 
 
 class WorkflowInterface:
     """Interface for manipulating workflows."""
 
     def __init__(self, gdb_interface):
         """Initialize the Workflow interface.
@@ -29,14 +32,15 @@
     def initialize_workflow(self, workflow):
         """Begin construction of a BEE workflow.
 
         :param workflow: the workflow object
         :type workflow: Workflow
         """
         if self.workflow_loaded():
+            log.error("attempt to re-initialize existing workflow")
             raise RuntimeError("attempt to re-initialize existing workflow")
         if workflow.requirements is None:
             workflow.requirements = []
         if workflow.hints is None:
             workflow.hints = []
 
         self._workflow_id = workflow.id
@@ -90,26 +94,28 @@
 
         The task must have a beeflow:CheckpointRequirement hint. If there are no
         remaining retry attemps (num_tries = 0) then the graph database is
         unmodified and this method returns None.
 
         :param task: the task to restart
         :type task: Task
+        :param checkpoint_file: the task checkpoint file
         :rtype: Task or None
         """
         for hint in task.hints:
             if hint.class_ == "beeflow:CheckpointRequirement":
                 if hint.params["num_tries"] > 0:
                     hint.params["num_tries"] -= 1
                     hint.params["bee_checkpoint_file__"] = checkpoint_file
                     break
-                state = self.get_task_state(task)
-                self.set_task_state(task, f"FAILED RESTART: {state}")
+                self.set_task_state(task, "FAILED")
+                self.set_workflow_state("FAILED")
                 return None
         else:
+            log.error("invalid task for checkpoint restart")
             raise ValueError("invalid task for checkpoint restart")
 
         new_task = task.copy(new_id=True)
         # Pattern match on task name
         # Append (1) if not in name already
         # Increment number on each restart
         match = re.match(r".+\(([0-9]+)\)$", new_task.name)
```

### Comparing `hpc_beeflow-0.1.6/beeflow/common/wf_profiler.py` & `hpc-beeflow-0.1.7/beeflow/common/wf_profiler.py`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/common/worker/__init__.py` & `hpc-beeflow-0.1.7/beeflow/common/worker/__init__.py`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/common/worker/flux_worker.py` & `hpc-beeflow-0.1.7/beeflow/common/worker/flux_worker.py`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/common/worker/lsf_worker.py` & `hpc-beeflow-0.1.7/beeflow/common/worker/lsf_worker.py`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/common/worker/simple_worker.py` & `hpc-beeflow-0.1.7/beeflow/common/worker/simple_worker.py`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/common/worker/slurm_worker.py` & `hpc-beeflow-0.1.7/beeflow/common/worker/slurm_worker.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Slurm worker for work load management.
 
 Builds command for submitting batch job.
 """
 
+import io
 import subprocess
 import json
 import urllib
 import getpass
 import requests_unixsocket
 import requests
 
@@ -49,14 +50,22 @@
         time_limit = validation.time_limit(time_limit)
         account = task.get_requirement('beeflow:SchedulerRequirement', 'account',
                                        default=self.default_account)
         partition = task.get_requirement('beeflow:SchedulerRequirement',
                                          'partition',
                                          default=self.default_partition)
 
+        scripts_enabled = task.get_requirement('beeflow:ScriptRequirement', 'enabled',
+                                               default=False)
+        if scripts_enabled:
+            # We use StringIO here to properly break the script up into lines with readlines
+            pre_script = io.StringIO(task.get_requirement('beeflow:ScriptRequirement',
+                                     'pre_script')).readlines()
+            post_script = io.StringIO(task.get_requirement('beeflow:ScriptRequirement',
+                                      'post_script')).readlines()
         # sbatch header
         script = [
             '#!/bin/bash',
             f'#SBATCH --job-name={task.name}-{task.id}',
             f'#SBATCH --output={task_save_path}/{task.name}-{task.id}.out',
             f'#SBATCH --error={task_save_path}/{task.name}-{task.id}.err',
             f'#SBATCH -N {nodes}',
@@ -79,26 +88,34 @@
             cmd_args = ' '.join(script_cmd.args)
             if script_cmd.type == 'one-per-node':
                 script.append(f'srun -N {nodes} -n {nodes} {cmd_args}')
             else:
                 script_lines.append(f'srun {cmd_args}')
 
         # Pre commands
+        if scripts_enabled:
+            for cmd in pre_script:
+                script.append(cmd)
+
         for cmd in crt_res.pre_commands:
             srun(script, cmd)
 
         # Main command
         srun_args = ' '.join(main_command_srun_args)
-        print(crt_res.main_command)
         args = ' '.join(crt_res.main_command.args)
         script.append(f'srun --mpi={mpi_version} {srun_args} {args}')
 
+        # Post commands
         for cmd in crt_res.post_commands:
             srun(script, cmd)
 
+        if scripts_enabled:
+            for cmd in post_script:
+                script.append(cmd)
+
         return '\n'.join(script)
 
     def write_script(self, task):
         """Build task script; returns filename of script."""
         task_text = self.build_text(task)
 
         task_script = f'{self.task_save_path(task)}/{task.name}-{task.id}.sh'
```

### Comparing `hpc_beeflow-0.1.6/beeflow/common/worker/worker.py` & `hpc-beeflow-0.1.7/beeflow/common/worker/worker.py`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/common/worker_interface.py` & `hpc-beeflow-0.1.7/beeflow/common/worker_interface.py`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/data/cloud_templates/dora.jinja` & `hpc-beeflow-0.1.7/beeflow/data/cloud_templates/dora.jinja`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/data/cloud_templates/dora.yaml` & `hpc-beeflow-0.1.7/beeflow/data/cloud_templates/dora.yaml`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/README.md` & `hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/README.md`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/blast/blast_wf.cwl` & `hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/blast/blast_wf.cwl`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/blast/blast_worker001.cwl` & `hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/blast/blast_worker001.cwl`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/blast/blast_worker002.cwl` & `hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/blast/blast_worker002.cwl`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/blast/input/small.fasta` & `hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/blast/input/small.fasta`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/cat-grep-fail/lorem.txt` & `hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/cat-grep-fail/lorem.txt`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/cat-grep-fail/workflow.cwl` & `hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/cat-grep-fail/workflow.cwl`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/clamr-ci/clamr.cwl` & `hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-ci/clamr.cwl`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/clamr-ci/clamr_wf.cwl` & `hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-ci/clamr_wf.cwl`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/clamr-ci/ffmpeg.cwl` & `hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-ci/ffmpeg.cwl`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/clamr-wf/clamr.cwl` & `hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf/clamr.cwl`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/clamr-wf/clamr_wf.cwl` & `hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf/clamr_wf.cwl`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/clamr-wf/ffmpeg.cwl` & `hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-ffmpeg-build_script/ffmpeg.cwl`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/clamr-wf-checkpoint/clamr.cwl` & `hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-ffmpeg-build_script/clamr.cwl`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # -*- mode: YAML; -*-
 
 class: CommandLineTool
 cwlVersion: v1.0
 
 baseCommand: /CLAMR/clamr_cpuonly
 # This is the stdout field which makes all stdout be captured in this file
-# stderr is not currently implemented but it is also a thing
 stdout: clamr_stdout.txt
 # Arguments to the command
 inputs:
   amr_type:
     # ? means the argument is optional
     # All of the ? here are legacy from the original CWL
     type: string?
@@ -58,30 +57,16 @@
     type: string?
     inputBinding:
       prefix: -e
   
 outputs:
   # Captures stdout. Name is arbitrary.
   clamr_stdout:
-    # type is syntactic sugar to just grab the output file defined above
-    # stdout:
-    #     type: File
-    #     outputBinding: 
-    #       glob: clamr_stdout.txt
-    #     stdout is easy shorthand
     type: stdout
   outdir:
-    # directory is just another type. Scan the files for a directory with the name specified in glob
-    # If you add a wildcard, it'd do expansion
     type: Directory
     outputBinding:
-      # Glob can be either a constant string or have a wildcard 
-      # TODO verify CWLs glob support
       glob: graphics_output/graph%05d.png
-  checkpoint_dir:
-    type: Directory
-    outputBinding:
-      glob: checkpoint_output/backup%05d.crx
   time_log:
     type: File
     outputBinding:
       glob: total_execution_time.log
```

### Comparing `hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/clamr-wf-checkpoint/clamr_wf.cwl` & `hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf-singularity/clamr_wf.cwl`

 * *Files 17% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 # takes ID:Type syntax
   grid_resolution: int
   max_levels: int
   time_steps: int
   steps_between_outputs: int
   steps_between_graphics: int
   graphics_type: string
-  checkpoint_disk_interval: int
 ##### FFMPEG inputs #####
   input_format: string
   frame_rate: int
   frame_size: string
   pixel_format: string
   output_filename: string
 
@@ -46,29 +45,22 @@
     in:
       grid_res: grid_resolution
       max_levels: max_levels
       time_steps: time_steps
       output_steps: steps_between_outputs
       graphic_steps: steps_between_graphics
       graphics_type: graphics_type
-      checkpoint_disk_interval: checkpoint_disk_interval
-    out: [clamr_stdout, outdir, checkpoint_dir, time_log]
+    out: [clamr_stdout, outdir, time_log]
     hints:
-        beeflow:CheckpointRequirement:
-            enabled: true
-            file_path: checkpoint_output
-            container_path: checkpoint_output
-            file_regex: backup[0-9]*.crx 
-            restart_parameters: -R
-            num_tries: 3
-        beeflow:SchedulerRequirement:
-            timeLimit: 00:00:10
         DockerRequirement:
-            dockerFile: "Dockerfile.clamr-ffmpeg"
-            beeflow:containerName: "clamr-ffmpeg"
+            # TODO Sort this out
+            #dockerImport: clamr_img.tar.gz
+            #beeflow:copyContainer: clamr
+            beeflow:copyContainer: "/usr/projects/beedev/clamr/clamr-toss.simg"
+
   ffmpeg:
     run: ffmpeg.cwl
     in:
       input_format: input_format
       # input syntax is name: <step>/dependent_object
       ffmpeg_input: clamr/outdir
       frame_rate: frame_rate
@@ -77,11 +69,7 @@
       # Setting output file with file_name
       # output_filename set in wf inputs
       output_file: output_filename
     # Multiple outputs can be in array
     out: [movie]
     requirements:
         InlineJavascriptRequirement: {}
-    hints:
-        DockerRequirement:
-            dockerFile: "Dockerfile.clamr-ffmpeg"
-            beeflow:containerName: "clamr-ffmpeg"
```

### Comparing `hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/clamr-wf-checkpoint/ffmpeg.cwl` & `hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf-summit/ffmpeg.cwl`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/clamr-wf-chicoma/clamr.cwl` & `hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf-chicoma/clamr.cwl`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/clamr-wf-chicoma/clamr_wf.cwl` & `hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf-chicoma/clamr_wf.cwl`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/clamr-wf-chicoma/ffmpeg.cwl` & `hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf-chicoma/ffmpeg.cwl`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/README.md` & `hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/README.md`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/lsf-charliecloud/cf-summit.cwl` & `hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/lsf-charliecloud/cf-summit.cwl`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/slurm-charliecloud/README.md` & `hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/slurm-charliecloud/README.md`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/slurm-charliecloud/cf-darwin.cwl` & `hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/slurm-charliecloud/cf-darwin.cwl`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/slurm-charliecloud/cf-no-owrite.cwl` & `hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/slurm-charliecloud/cf-no-owrite.cwl`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/slurm-charliecloud/cf.cwl` & `hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/slurm-charliecloud/cf.cwl`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/slurm-charliecloud/copyContainer_containerName.cwl` & `hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/slurm-charliecloud/copyContainer_containerName.cwl`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/slurm-charliecloud/dockerFile_containerName.cwl` & `hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/slurm-charliecloud/dockerFile_containerName.cwl`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/slurm-charliecloud/dockerPull.cwl` & `hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/slurm-charliecloud/dockerPull.cwl`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/slurm-singularity/cf-singularity.cwl` & `hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/slurm-singularity/cf-singularity.cwl`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/clamr-wf-singularity/clamr.cwl` & `hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf-singularity/clamr.cwl`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/clamr-wf-singularity/clamr_wf.cwl` & `hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf-summit/clamr_wf.cwl`

 * *Files 10% similar despite different names*

```diff
@@ -51,25 +51,25 @@
       graphics_type: graphics_type
     out: [clamr_stdout, outdir, time_log]
     hints:
         DockerRequirement:
             # TODO Sort this out
             #dockerImport: clamr_img.tar.gz
             #beeflow:copyContainer: clamr
-            beeflow:copyContainer: "/usr/projects/beedev/clamr/clamr-toss.simg"
+            beeflow:copyContainer: "/ccs/proj/csc420/BEE/clamr-ppc64le.tar.gz"
 
   ffmpeg:
     run: ffmpeg.cwl
     in:
-      input_format: input_format
-      # input syntax is name: <step>/dependent_object
+      input_format: input_format # input syntax is name: <step>/dependent_object
       ffmpeg_input: clamr/outdir
       frame_rate: frame_rate
       frame_size: frame_size
       pixel_format: pixel_format
       # Setting output file with file_name
       # output_filename set in wf inputs
       output_file: output_filename
     # Multiple outputs can be in array
     out: [movie]
-    requirements:
-        InlineJavascriptRequirement: {}
+    hints:
+      DockerRequirement:
+        beeflow:copyContainer: "/ccs/proj/csc420/BEE/clamr-ppc64le.tar.gz"
```

### Comparing `hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/clamr-wf-singularity/ffmpeg.cwl` & `hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf-singularity/ffmpeg.cwl`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/clamr-wf-summit/clamr.cwl` & `hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf-summit/clamr.cwl`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/clamr-wf-summit/clamr_wf.cwl` & `hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf-use-container/clamr_wf.cwl`

 * *Files 5% similar despite different names*

```diff
@@ -48,28 +48,25 @@
       time_steps: time_steps
       output_steps: steps_between_outputs
       graphic_steps: steps_between_graphics
       graphics_type: graphics_type
     out: [clamr_stdout, outdir, time_log]
     hints:
         DockerRequirement:
-            # TODO Sort this out
-            #dockerImport: clamr_img.tar.gz
-            #beeflow:copyContainer: clamr
-            beeflow:copyContainer: "/ccs/proj/csc420/BEE/clamr-ppc64le.tar.gz"
+            beeflow:useContainer: "/usr/projects/beedev/clamr/clamr-toss.tar.gz"
 
   ffmpeg:
     run: ffmpeg.cwl
     in:
-      input_format: input_format # input syntax is name: <step>/dependent_object
+      input_format: input_format
+      # input syntax is name: <step>/dependent_object
       ffmpeg_input: clamr/outdir
       frame_rate: frame_rate
       frame_size: frame_size
       pixel_format: pixel_format
       # Setting output file with file_name
       # output_filename set in wf inputs
       output_file: output_filename
     # Multiple outputs can be in array
     out: [movie]
-    hints:
-      DockerRequirement:
-        beeflow:copyContainer: "/ccs/proj/csc420/BEE/clamr-ppc64le.tar.gz"
+    requirements:
+        InlineJavascriptRequirement: {}
```

### Comparing `hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/clamr-wf-summit/ffmpeg.cwl` & `hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf-use-container/ffmpeg.cwl`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/clamr-wf-use-container/clamr.cwl` & `hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf-use-container/clamr.cwl`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/clamr-wf-use-container/clamr_wf.cwl` & `hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-ffmpeg-build_script/clamr_wf.cwl`

 * *Files 20% similar despite different names*

```diff
@@ -21,52 +21,58 @@
   frame_rate: int
   frame_size: string
   pixel_format: string
   output_filename: string
 
 outputs:
 # Outputs for all the steps
-# Check where we copy these probably at CWD
-# Files need to exist at end of workflow, but we aren't currently checking
-# We have function to get workflow_outputs
-# TODO add step to workflow_manager to confirm that each of these outputs exist
   clamr_stdout:
     type: File
     outputSource: clamr/clamr_stdout
   clamr_time_log:
     type: File
     outputSource: clamr/time_log
   clamr_movie:
     type: File
     outputSource: ffmpeg/movie
+  ffmpeg_stderr:
+    type: File
+    outputSource: ffmpeg/ffmpeg_stderr
 
 steps:
   clamr:
     run: clamr.cwl
     in:
       grid_res: grid_resolution
       max_levels: max_levels
       time_steps: time_steps
       output_steps: steps_between_outputs
       graphic_steps: steps_between_graphics
       graphics_type: graphics_type
     out: [clamr_stdout, outdir, time_log]
     hints:
+        beeflow:ScriptRequirement:
+            enabled: true
+            pre_script: "pre_run.sh"
+            post_script: "post_run.sh"
         DockerRequirement:
-            beeflow:useContainer: "/usr/projects/beedev/clamr/clamr-toss.tar.gz"
+            dockerFile: "Dockerfile.clamr-ffmpeg"
+            beeflow:containerName: "clamr-ffmpeg"
 
   ffmpeg:
     run: ffmpeg.cwl
     in:
       input_format: input_format
       # input syntax is name: <step>/dependent_object
       ffmpeg_input: clamr/outdir
       frame_rate: frame_rate
       frame_size: frame_size
       pixel_format: pixel_format
       # Setting output file with file_name
       # output_filename set in wf inputs
       output_file: output_filename
     # Multiple outputs can be in array
-    out: [movie]
-    requirements:
-        InlineJavascriptRequirement: {}
+    out: [movie, ffmpeg_stderr]
+    hints:
+        DockerRequirement:
+            dockerFile: "Dockerfile.clamr-ffmpeg"
+            beeflow:containerName: "clamr-ffmpeg"
```

### Comparing `hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/clamr-wf-use-container/ffmpeg.cwl` & `hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf/ffmpeg.cwl`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 # -*- mode: YAML; -*-
 
 class: CommandLineTool
 cwlVersion: v1.0
 
 baseCommand: ffmpeg -y
+
+stderr: ffmpeg_stderr.txt
+
 inputs:
   input_format:
     type: string?
     inputBinding:
       prefix: -f
       position: 1
   ffmpeg_input:
     type: Directory
     inputBinding:
       prefix: -i
       position: 2
-      valueFrom: $(self.path + "/graph%05d.png")
+      valueFrom: $("/graph%05d.png")
   frame_rate:
     type: int?
     inputBinding:
       prefix: -r
       position: 3
   frame_size:
     type: string?
@@ -38,7 +41,9 @@
 
 outputs:
   movie:
     type: File
     outputBinding:
       glob: $(inputs.output_file)
       # glob: CLAMR_movie.mp4
+  ffmpeg_stderr:
+    type: stderr
```

### Comparing `hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/comd-mpi/comd.cwl` & `hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/comd-mpi/comd.cwl`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/comd-mpi/comd_wf.cwl` & `hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/comd-mpi/comd_wf.cwl`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/lulesh-mpi/lulesh.cwl` & `hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/lulesh-mpi/lulesh.cwl`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/nwchem-mpi/README.md` & `hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/nwchem-mpi/README.md`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/nwchem-mpi/nwchem.cwl` & `hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/nwchem-mpi/nwchem.cwl`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/pennant/pennant_wf.cwl` & `hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/pennant/pennant_wf.cwl`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/pennant-build/Dockerfile.pennant-flux-x86_64` & `hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/pennant-build/Dockerfile.pennant-flux-x86_64`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/pennant-build/Dockerfile.pennant-graph-x86_64` & `hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/pennant-build/Dockerfile.pennant-graph-x86_64`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/pennant-build/graph_pennant.py` & `hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/pennant-build/graph_pennant.py`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/pennant-build/pennant_wf.cwl` & `hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/pennant-build/pennant_wf.cwl`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/simple-workflows/cancel.cwl` & `hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/simple-workflows/cancel.cwl`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/simple-workflows/grep-wordcount/gc-nc.cwl` & `hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/simple-workflows/grep-wordcount/gc-nc.cwl`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/simple-workflows/grep-wordcount/gc.cwl` & `hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/simple-workflows/grep-wordcount/gc.cwl`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/data/cwl/bee_workflows/simple-workflows/grep-wordcount/lorem.txt` & `hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/simple-workflows/grep-wordcount/lorem.txt`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/data/cwl/cwl_validation/grep-wordcount/gc.cwl` & `hpc-beeflow-0.1.7/beeflow/data/cwl/cwl_validation/grep-wordcount/gc.cwl`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/data/cwl/cwl_validation/grep-wordcount/lorem.txt` & `hpc-beeflow-0.1.7/beeflow/data/cwl/cwl_validation/grep-wordcount/lorem.txt`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/data/cwl/cwl_validation/ml-workflow/example-1/DAG_example-1.png` & `hpc-beeflow-0.1.7/beeflow/data/cwl/cwl_validation/ml-workflow/example-1/DAG_example-1.png`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/data/cwl/cwl_validation/ml-workflow/example-1/README.md` & `hpc-beeflow-0.1.7/beeflow/data/cwl/cwl_validation/ml-workflow/example-1/README.md`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/data/cwl/cwl_validation/ml-workflow/machine_learning/README.md` & `hpc-beeflow-0.1.7/beeflow/data/cwl/cwl_validation/ml-workflow/machine_learning/README.md`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/data/cwl/cwl_validation/ml-workflow/machine_learning/decision_tree.py` & `hpc-beeflow-0.1.7/beeflow/data/cwl/cwl_validation/ml-workflow/machine_learning/decision_tree.py`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/data/cwl/cwl_validation/ml-workflow/machine_learning/linear_regression.py` & `hpc-beeflow-0.1.7/beeflow/data/cwl/cwl_validation/ml-workflow/machine_learning/linear_regression.py`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/data/cwl/cwl_validation/ml-workflow/machine_learning/machinelearning_pipeline.cwl` & `hpc-beeflow-0.1.7/beeflow/data/cwl/cwl_validation/ml-workflow/machine_learning/machinelearning_pipeline.cwl`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/data/cwl/cwl_validation/ml-workflow/machine_learning/out.PNG` & `hpc-beeflow-0.1.7/beeflow/data/cwl/cwl_validation/ml-workflow/machine_learning/out.PNG`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/data/cwl/cwl_validation/ml-workflow/machine_learning/predict_code.py` & `hpc-beeflow-0.1.7/beeflow/data/cwl/cwl_validation/ml-workflow/machine_learning/predict_code.py`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/data/cwl/cwl_validation/ml-workflow/machine_learning/read_dataset.py` & `hpc-beeflow-0.1.7/beeflow/data/cwl/cwl_validation/ml-workflow/machine_learning/read_dataset.py`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/data/dockerfiles/Dockerfile.clamr-ppc64le` & `hpc-beeflow-0.1.7/beeflow/data/dockerfiles/Dockerfile.clamr-ppc64le`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/data/dockerfiles/Dockerfile.comd-flux-x86_64` & `hpc-beeflow-0.1.7/beeflow/data/dockerfiles/Dockerfile.comd-flux-x86_64`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/data/dockerfiles/Dockerfile.comd-x86_64` & `hpc-beeflow-0.1.7/beeflow/data/dockerfiles/Dockerfile.comd-x86_64`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/data/dockerfiles/Dockerfile.lulesh-x86_64` & `hpc-beeflow-0.1.7/beeflow/data/dockerfiles/Dockerfile.lulesh-x86_64`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/data/dockerfiles/Dockerfile.neo4j-ppc64le` & `hpc-beeflow-0.1.7/beeflow/data/dockerfiles/Dockerfile.neo4j-ppc64le`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/data/dockerfiles/Dockerfile.nwchem-x86_64` & `hpc-beeflow-0.1.7/beeflow/data/dockerfiles/Dockerfile.nwchem-x86_64`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/data/dockerfiles/Dockerfile.pennant-flux-x86_64` & `hpc-beeflow-0.1.7/beeflow/data/dockerfiles/Dockerfile.pennant-flux-x86_64`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/data/dockerfiles/Dockerfile.vaspompi-x86_64` & `hpc-beeflow-0.1.7/beeflow/data/dockerfiles/Dockerfile.vaspompi-x86_64`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/data/dockerfiles/README.md` & `hpc-beeflow-0.1.7/beeflow/data/dockerfiles/README.md`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/data/dockerfiles/comd-pmix-support/Dockerfile.debian` & `hpc-beeflow-0.1.7/beeflow/data/dockerfiles/comd-pmix-support/Dockerfile.debian`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/data/dockerfiles/comd-pmix-support/Dockerfile.openmpi-3.1.5` & `hpc-beeflow-0.1.7/beeflow/data/dockerfiles/comd-pmix-support/Dockerfile.openmpi-3.1.5`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/data/dockerfiles/comd-pmix-support/dont-init-ucx-on-intel-cray.patch` & `hpc-beeflow-0.1.7/beeflow/data/dockerfiles/comd-pmix-support/dont-init-ucx-on-intel-cray.patch`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/data/dockerfiles/pennant-graph/Dockerfile.pennant-graph-x86_64` & `hpc-beeflow-0.1.7/beeflow/data/dockerfiles/pennant-graph/Dockerfile.pennant-graph-x86_64`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/data/dockerfiles/pennant-graph/graph_pennant.py` & `hpc-beeflow-0.1.7/beeflow/data/dockerfiles/pennant-graph/graph_pennant.py`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/enhanced_client/README.rst` & `hpc-beeflow-0.1.7/beeflow/enhanced_client/README.rst`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/enhanced_client/main.js` & `hpc-beeflow-0.1.7/beeflow/enhanced_client/main.js`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/enhanced_client/package-lock.json` & `hpc-beeflow-0.1.7/beeflow/enhanced_client/package-lock.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999765037593985%*

 * *Differences: {"'packages'": "{'node_modules/follow-redirects': {'version': '1.15.5', 'resolved': "*

 * *               "'https://registry.npmjs.org/follow-redirects/-/follow-redirects-1.15.5.tgz', "*

 * *               "'integrity': "*

 * *               "'sha512-vSFWUON1B+yAw1VN4xMfxgn5fTUiaOzAJCKBwIIgT/+7CuGy9+r+5gITvP62j3RmaD5Ph65UaERdOSRGUzZtgw=='}}"}*

```diff
@@ -3190,22 +3190,22 @@
             },
             "funding": [
                 {
                     "type": "individual",
                     "url": "https://github.com/sponsors/RubenVerborgh"
                 }
             ],
-            "integrity": "sha512-VQLG33o04KaQ8uYi2tVNbdrWp1QWxNNea+nmIB4EVM28v0hmP17z7aG1+wAkNzVq4KeXTq3221ye5qTJP91JwA==",
+            "integrity": "sha512-vSFWUON1B+yAw1VN4xMfxgn5fTUiaOzAJCKBwIIgT/+7CuGy9+r+5gITvP62j3RmaD5Ph65UaERdOSRGUzZtgw==",
             "peerDependenciesMeta": {
                 "debug": {
                     "optional": true
                 }
             },
-            "resolved": "https://registry.npmjs.org/follow-redirects/-/follow-redirects-1.15.2.tgz",
-            "version": "1.15.2"
+            "resolved": "https://registry.npmjs.org/follow-redirects/-/follow-redirects-1.15.5.tgz",
+            "version": "1.15.5"
         },
         "node_modules/form-data": {
             "dependencies": {
                 "asynckit": "^0.4.0",
                 "combined-stream": "^1.0.8",
                 "mime-types": "^2.1.12"
             },
```

### Comparing `hpc_beeflow-0.1.6/beeflow/enhanced_client/package.json` & `hpc-beeflow-0.1.7/beeflow/enhanced_client/package.json`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/enhanced_client/renderer/app.js` & `hpc-beeflow-0.1.7/beeflow/enhanced_client/renderer/app.js`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/enhanced_client/renderer/client.js` & `hpc-beeflow-0.1.7/beeflow/enhanced_client/renderer/client.js`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/enhanced_client/renderer/config.js` & `hpc-beeflow-0.1.7/beeflow/enhanced_client/renderer/config.js`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/enhanced_client/renderer/control.js` & `hpc-beeflow-0.1.7/beeflow/enhanced_client/renderer/control.js`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/enhanced_client/renderer/database.js` & `hpc-beeflow-0.1.7/beeflow/enhanced_client/renderer/database.js`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/enhanced_client/renderer/display.js` & `hpc-beeflow-0.1.7/beeflow/enhanced_client/renderer/display.js`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/enhanced_client/renderer/img/logo.png` & `hpc-beeflow-0.1.7/beeflow/enhanced_client/renderer/img/logo.png`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/enhanced_client/renderer/main.html` & `hpc-beeflow-0.1.7/beeflow/enhanced_client/renderer/main.html`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/enhanced_client/renderer/styles/bulma.min.css` & `hpc-beeflow-0.1.7/beeflow/enhanced_client/renderer/styles/bulma.min.css`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/enhanced_client/renderer/viz.js` & `hpc-beeflow-0.1.7/beeflow/enhanced_client/renderer/viz.js`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/enhanced_client/renderer/workflows.js` & `hpc-beeflow-0.1.7/beeflow/enhanced_client/renderer/workflows.js`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/scheduler/README.md` & `hpc-beeflow-0.1.7/beeflow/scheduler/README.md`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/scheduler/algorithms.py` & `hpc-beeflow-0.1.7/beeflow/scheduler/algorithms.py`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/scheduler/resource_allocation.py` & `hpc-beeflow-0.1.7/beeflow/scheduler/resource_allocation.py`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/scheduler/scheduler.py` & `hpc-beeflow-0.1.7/beeflow/scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/scheduler/scheduler.yaml` & `hpc-beeflow-0.1.7/beeflow/scheduler/scheduler.yaml`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/scheduler/serializable.py` & `hpc-beeflow-0.1.7/beeflow/scheduler/serializable.py`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/scheduler/task.py` & `hpc-beeflow-0.1.7/beeflow/scheduler/task.py`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/tests/42.tgz` & `hpc-beeflow-0.1.7/beeflow/tests/42.tgz`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/tests/cf.cwl` & `hpc-beeflow-0.1.7/beeflow/tests/cf.cwl`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/tests/clamr-wf/clamr.cwl` & `hpc-beeflow-0.1.7/beeflow/tests/clamr-wf/clamr.cwl`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/tests/clamr-wf/clamr_wf.cwl` & `hpc-beeflow-0.1.7/beeflow/tests/clamr-wf/clamr_wf.cwl`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/tests/clamr-wf/ffmpeg.cwl` & `hpc-beeflow-0.1.7/beeflow/tests/clamr-wf/ffmpeg.cwl`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/tests/clamr-wf.tgz` & `hpc-beeflow-0.1.7/beeflow/tests/clamr-wf.tgz`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/tests/gdb.py` & `hpc-beeflow-0.1.7/beeflow/tests/gdb.py`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/tests/mocks.py` & `hpc-beeflow-0.1.7/beeflow/tests/mocks.py`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/tests/test_config_validator.py` & `hpc-beeflow-0.1.7/beeflow/tests/test_config_validator.py`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/tests/test_container_path.py` & `hpc-beeflow-0.1.7/beeflow/tests/test_container_path.py`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/tests/test_db_sched.py` & `hpc-beeflow-0.1.7/beeflow/tests/test_db_sched.py`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/tests/test_db_tm.py` & `hpc-beeflow-0.1.7/beeflow/tests/test_db_tm.py`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/tests/test_parser.py` & `hpc-beeflow-0.1.7/beeflow/tests/test_parser.py`

 * *Files 21% similar despite different names*

```diff
@@ -25,22 +25,35 @@
         cls.parser = CwlParser()
 
     def test_parse_workflow_yaml(self):
         """Test parsing of workflow with a YAML input job file."""
         cwl_wf_file = find("examples/clamr-ffmpeg-build/clamr_wf.cwl")
         cwl_job_yaml = find("examples/clamr-ffmpeg-build/clamr_job.yml")
         workflow_id = generate_workflow_id()
-
         workflow, tasks = self.parser.parse_workflow(workflow_id, cwl_wf_file, cwl_job_yaml)
 
         self.assertEqual(workflow, WORKFLOW_GOLD)
         self.assertListEqual(tasks, TASKS_GOLD)
         for task in tasks:
             self.assertEqual(task.workflow_id, workflow_id)
 
+    def test_parse_workflow_script(self):
+        """Test parsing of workflow with a YAML input job file."""
+        cwl_wf_file = find("beeflow/data/cwl/bee_workflows/clamr-ffmpeg-build_script/clamr_wf.cwl") #noqa
+        cwl_job_yaml = find("beeflow/data/cwl/bee_workflows/clamr-ffmpeg-build_script/clamr_job.yml") #noqa
+
+        workflow_id = generate_workflow_id()
+
+        workflow, tasks = self.parser.parse_workflow(workflow_id, cwl_wf_file, cwl_job_yaml)
+
+        self.assertEqual(workflow, WORKFLOW_GOLD)
+        self.assertListEqual(tasks, TASKS_GOLD_SCRIPT)
+        for task in tasks:
+            self.assertEqual(task.workflow_id, workflow_id)
+
     def test_parse_workflow_json(self):
         """Test parsing of workflow with a JSON input job file."""
         cwl_wf_file = find("examples/clamr-ffmpeg-build/clamr_wf.cwl")
         cwl_job_json = find("examples/clamr-ffmpeg-build/clamr_job.json")
         workflow_id = generate_workflow_id()
 
         workflow, tasks = self.parser.parse_workflow(workflow_id, cwl_wf_file, cwl_job_json)
@@ -60,14 +73,39 @@
 
         self.assertEqual(workflow, WORKFLOW_NOJOB_GOLD)
         self.assertListEqual(tasks, TASKS_NOJOB_GOLD)
         for task in tasks:
             self.assertEqual(task.workflow_id, workflow_id)
 
 
+WORKFLOW_GOLD_SCRIPT = Workflow(
+    name='clamr_wf',
+    hints=[],
+    requirements=[],
+    inputs={InputParameter(id='input_format', type='string', value='image2'),
+            InputParameter(id='time_steps', type='int', value=5000),
+            InputParameter(id='output_filename', type='string', value='./CLAMR_movie.mp4'),
+            InputParameter(id='frame_size', type='string', value='800x800'),
+            InputParameter(id='frame_rate', type='int', value=12),
+            InputParameter(id='max_levels', type='int', value=3),
+            InputParameter(id='graphics_type', type='string', value='png'),
+            InputParameter(id='steps_between_outputs', type='int', value=10),
+            InputParameter(id='pixel_format', type='string', value='yuv420p'),
+            InputParameter(id='grid_resolution', type='int', value=32),
+            InputParameter(id='steps_between_graphics', type='int', value=25)},
+    outputs={OutputParameter(id='clamr_stdout', type='File', value=None,
+                             source='clamr/clamr_stdout'),
+             OutputParameter(id='clamr_movie', type='File', value=None, source='ffmpeg/movie'),
+             OutputParameter(id='ffmpeg_stderr', type='File', value=None,
+                             source='ffmpeg/ffmpeg_stderr'),
+             OutputParameter(id='clamr_time_log', type='File', value=None,
+                             source='clamr/time_log')},
+    workflow_id=generate_workflow_id())
+
+
 WORKFLOW_GOLD = Workflow(
     name='clamr_wf',
     hints=[],
     requirements=[],
     inputs={InputParameter(id='input_format', type='string', value='image2'),
             InputParameter(id='time_steps', type='int', value=5000),
             InputParameter(id='output_filename', type='string', value='CLAMR_movie.mp4'),
@@ -84,14 +122,72 @@
              OutputParameter(id='clamr_movie', type='File', value=None, source='ffmpeg/movie'),
              OutputParameter(id='ffmpeg_stderr', type='File', value=None,
                              source='ffmpeg/ffmpeg_stderr'),
              OutputParameter(id='clamr_time_log', type='File', value=None,
                              source='clamr/time_log')},
     workflow_id=generate_workflow_id())
 
+TASKS_GOLD_SCRIPT = [
+    Task(
+        name='clamr',
+        base_command='/CLAMR/clamr_cpuonly',
+        hints=[Hint(class_='DockerRequirement', params={'dockerFile': '# Dockerfile.clamr-ffmpeg\n# Developed on Chicoma @lanl\n# Patricia Grubel <pagrubel@lanl.gov>\n\nFROM debian:11\n\n\nRUN apt-get update && \\\n    apt-get install -y wget gnupg git cmake ffmpeg g++ make openmpi-bin libopenmpi-dev libpng-dev libpng16-16 libpng-tools imagemagick libmagickwand-6.q16-6 libmagickwand-6.q16-dev\n\nRUN git clone https://github.com/lanl/CLAMR.git\nRUN cd CLAMR && cmake . && make clamr_cpuonly\n', 'beeflow:containerName': 'clamr-ffmpeg'}), #noqa
+               Hint(class_='beeflow:ScriptRequirement', params={'enabled': True, 'pre_script': 'echo "Before run"\n', 'post_script': 'echo "After run"\n'})], #noqa
+        requirements=[],
+        inputs=[StepInput(id='graphic_steps', type='int', value=None, default=None,
+                          source='steps_between_graphics', prefix='-g', position=None,
+                          value_from=None),
+                StepInput(id='graphics_type', type='string', value=None, default=None,
+                          source='graphics_type', prefix='-G', position=None, value_from=None),
+                StepInput(id='grid_res', type='int', value=None, default=None,
+                          source='grid_resolution', prefix='-n', position=None, value_from=None),
+                StepInput(id='max_levels', type='int', value=None, default=None,
+                          source='max_levels', prefix='-l', position=None, value_from=None),
+                StepInput(id='output_steps', type='int', value=None, default=None,
+                          source='steps_between_outputs', prefix='-i', position=None,
+                          value_from=None),
+                StepInput(id='time_steps', type='int', value=None, default=None,
+                          source='time_steps', prefix='-t', position=None, value_from=None)],
+        outputs=[StepOutput(id='clamr/clamr_stdout', type='stdout', value=None,
+                            glob='clamr_stdout.txt'),
+                 StepOutput(id='clamr/outdir', type='Directory', value=None,
+                            glob='graphics_output/graph%05d.png'),
+                 StepOutput(id='clamr/time_log', type='File', value=None,
+                            glob='total_execution_time.log')],
+        stdout='clamr_stdout.txt',
+        stderr=None,
+        workflow_id=WORKFLOW_GOLD.id
+    ),
+    Task(
+        name='ffmpeg',
+        base_command='ffmpeg -y',
+        hints=[Hint(class_='DockerRequirement', params={'dockerFile': '# Dockerfile.clamr-ffmpeg\n# Developed on Chicoma @lanl\n# Patricia Grubel <pagrubel@lanl.gov>\n\nFROM debian:11\n\n\nRUN apt-get update && \\\n    apt-get install -y wget gnupg git cmake ffmpeg g++ make openmpi-bin libopenmpi-dev libpng-dev libpng16-16 libpng-tools imagemagick libmagickwand-6.q16-6 libmagickwand-6.q16-dev\n\nRUN git clone https://github.com/lanl/CLAMR.git\nRUN cd CLAMR && cmake . && make clamr_cpuonly\n', 'beeflow:containerName': 'clamr-ffmpeg'})], # noqa
+        requirements=[],
+        inputs=[StepInput(id='ffmpeg_input', type='Directory', value=None, default=None,
+                          source='clamr/outdir', prefix='-i', position=2,
+                          value_from='$("/graph%05d.png")'),
+                StepInput(id='frame_rate', type='int', value=None, default=None,
+                          source='frame_rate', prefix='-r', position=3, value_from=None),
+                StepInput(id='frame_size', type='string', value=None, default=None,
+                          source='frame_size', prefix='-s', position=4, value_from=None),
+                StepInput(id='input_format', type='string', value=None, default=None,
+                          source='input_format', prefix='-f', position=1, value_from=None),
+                StepInput(id='output_file', type='string', value=None, default=None,
+                          source='output_filename', prefix=None, position=6, value_from=None),
+                StepInput(id='pixel_format', type='string', value=None, default=None,
+                          source='pixel_format', prefix='-pix_fmt', position=5, value_from=None)],
+        outputs=[StepOutput(id='ffmpeg/movie', type='File', value=None,
+                            glob='$(inputs.output_file)'),
+                 StepOutput(id='ffmpeg/ffmpeg_stderr', type='stderr', value=None,
+                            glob='ffmpeg_stderr.txt')],
+        stdout=None,
+        stderr='ffmpeg_stderr.txt',
+        workflow_id=WORKFLOW_GOLD.id)
+]
+
 
 TASKS_GOLD = [
     Task(
         name='clamr',
         base_command='/CLAMR/clamr_cpuonly',
         hints=[Hint(class_='DockerRequirement', params={'dockerFile': '# Dockerfile.clamr-ffmpeg\n# Developed on Chicoma @lanl\n# Patricia Grubel <pagrubel@lanl.gov>\n\nFROM debian:11\n\n\nRUN apt-get update && \\\n    apt-get install -y wget gnupg git cmake ffmpeg g++ make openmpi-bin libopenmpi-dev libpng-dev libpng16-16 libpng-tools imagemagick libmagickwand-6.q16-6 libmagickwand-6.q16-dev\n\nRUN git clone https://github.com/lanl/CLAMR.git\nRUN cd CLAMR && cmake . && make clamr_cpuonly\n', 'beeflow:containerName': 'clamr-ffmpeg'})], # noqa
         requirements=[],
@@ -160,26 +256,28 @@
 TASKS_NOJOB_GOLD = [
     Task(
         name='clamr',
         base_command='/clamr/CLAMR-master/clamr_cpuonly -n 32 -l 3 -t 5000 -i 10 -g 25 -G png',
         hints=[Hint(class_='DockerRequirement',
                     params={'dockerImageId': '/usr/projects/beedev/clamr/clamr-toss.tar.gz'})],
         requirements=[],
-        inputs=[],
+        inputs=[StepInput(id='infile', type='File', value=None, default='lorem.txt',
+                          source='infile', prefix=None, position=1, value_from=None)],
         outputs=[StepOutput(id='clamr/outfile', type='stdout', value=None,
                             glob='graphics_output')],
         stdout='graphics_output',
         stderr=None,
         workflow_id=WORKFLOW_NOJOB_GOLD.id),
     Task(
         name='ffmpeg',
         base_command='ffmpeg -f image2 -i $HOME/graphics_output/graph%05d.png -r 12 -s 800x800 -pix_fmt yuv420p $HOME/CLAMR_movie.mp4', # noqa
         hints=[],
         requirements=[],
-        inputs=[],
+        inputs=[StepInput(id='infile', type='File', value=None, default='graphics_output',
+                          source='clamr/outfile', prefix=None, position=1, value_from=None)],
         outputs=[StepOutput(id='ffmpeg/outfile', type='stdout', value=None,
                             glob='CLAMR_movie.mp4')],
         stdout='CLAMR_movie.mp4',
         stderr=None,
         workflow_id=WORKFLOW_NOJOB_GOLD.id)
 ]
```

### Comparing `hpc_beeflow-0.1.6/beeflow/tests/test_scheduler.py` & `hpc-beeflow-0.1.7/beeflow/tests/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/tests/test_scheduler_resource_allocation.py` & `hpc-beeflow-0.1.7/beeflow/tests/test_scheduler_resource_allocation.py`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/tests/test_scheduler_rest.py` & `hpc-beeflow-0.1.7/beeflow/tests/test_scheduler_rest.py`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/tests/test_slurm_worker.py` & `hpc-beeflow-0.1.7/beeflow/tests/test_slurm_worker.py`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/tests/test_tm.py` & `hpc-beeflow-0.1.7/beeflow/tests/test_tm.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 import pytest
 import jsonpickle
 from mocks import mock_put
 from mocks import MockWorkerCompletion, MockWorkerSubmission
 
 from beeflow.common.db.bdb import connect_db
 from beeflow.common.db import tm_db
-import beeflow.task_manager as tm
+import beeflow.task_manager.task_manager as tm
 from beeflow.common.wf_data import Task
 import beeflow
 
 
 @pytest.fixture
 def flask_client():
     """Client lets us run flask queries."""
-    app = tm.flask_app
+    app = tm.create_app()
     client = app.test_client()
     yield client
 
 
 def generate_tasks(n):
     """Generate n tasks for testing."""
     return [
@@ -41,30 +41,30 @@
     yield db
     os.remove(fname)
 
 
 @pytest.mark.usefixtures('flask_client', 'mocker')
 def test_submit_task(flask_client, mocker, temp_db):  # noqa
     """Create a workflow and get the ID back."""
-    mocker.patch('beeflow.task_manager.worker',
-                 new_callable=MockWorkerSubmission)
-    mocker.patch('beeflow.task_manager.db_path', temp_db.db_file)
+    mocker.patch('beeflow.task_manager.utils.worker_interface',
+                 MockWorkerSubmission)
+    mocker.patch('beeflow.task_manager.utils.db_path', lambda: temp_db.db_file)
     # Generate a task
     tasks = generate_tasks(1)
     tasks_json = jsonpickle.encode(tasks)
 
     response = flask_client.post('/bee_tm/v1/task/submit/',
                                  json={'tasks': tasks_json})
 
-    mocker.patch('beeflow.task_manager.worker',
-                 new_callable=MockWorkerSubmission)
+    mocker.patch('beeflow.task_manager.utils.worker_interface',
+                 MockWorkerSubmission)
 
     # Patch the connection object for WFM communication
     mocker.patch('beeflow.common.connection.Connection.put', mock_put)
-    beeflow.task_manager.process_queues()
+    beeflow.task_manager.background.process_queues()
 
     msg = response.get_json()['msg']
     status = response.status_code
     job_queue = list(temp_db.job_queue)
 
     # We should only have a single job on the queue
     assert len(job_queue) == 1
@@ -77,38 +77,38 @@
     assert msg == 'Tasks Added!'
 
 
 @pytest.mark.usefixtures('flask_client', 'mocker')
 def test_completed_task(flask_client, mocker, temp_db): # noqa
     """Tests how the task manager processes a completed task."""
     # 42 is the sample task ID
-    mocker.patch('beeflow.task_manager.worker',
-                 new_callable=MockWorkerCompletion)
+    mocker.patch('beeflow.task_manager.utils.worker_interface',
+                 MockWorkerCompletion)
     # Patch the connection object for WFM communication
     mocker.patch('beeflow.common.connection.Connection.put', mock_put)
-    mocker.patch('beeflow.task_manager.db_path', temp_db.db_file)
+    mocker.patch('beeflow.task_manager.utils.db_path', lambda: temp_db.db_file)
 
     # This should notice the job is complete and empty the job_queue
-    beeflow.task_manager.process_queues()
+    beeflow.task_manager.background.process_queues()
     job_queue = list(temp_db.job_queue)
     assert len(job_queue) == 0
 
 
 @pytest.mark.usefixtures('flask_client', 'mocker')
 def test_remove_task(flask_client, mocker, temp_db):  # noqa
     """Test cancelling a workflow and removing tasks."""
     task1, task2, task3 = generate_tasks(3)
     # Add a few tasks
     temp_db.job_queue.push(task=task1, job_id=1, job_state='RUNNING')
     temp_db.job_queue.push(task=task2, job_id=2, job_state='PENDING')
     temp_db.job_queue.push(task=task3, job_id=3, job_state='PENDING')
 
-    mocker.patch('beeflow.task_manager.worker',
-                 new_callable=MockWorkerCompletion)
-    mocker.patch('beeflow.task_manager.db_path', temp_db.db_file)
+    mocker.patch('beeflow.task_manager.utils.worker_interface',
+                 MockWorkerCompletion)
+    mocker.patch('beeflow.task_manager.utils.db_path', lambda: temp_db.db_file)
 
     response = flask_client.delete('/bee_tm/v1/task/')
 
     msg = response.get_json()['msg']
     status = response.status_code
     assert status == 200
     assert msg.count('CANCELLED') == 3
```

### Comparing `hpc_beeflow-0.1.6/beeflow/tests/test_wf_interface.py` & `hpc-beeflow-0.1.7/beeflow/tests/test_wf_interface.py`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/tests/test_wf_manager.py` & `hpc-beeflow-0.1.7/beeflow/tests/test_wf_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -186,15 +186,16 @@
     https_port = 3455
 
     temp_db.workflows.init_workflow(WF_ID, wf_name, 'dir', bolt_port, http_port, https_port)
     temp_db.workflows.add_task(123, WF_ID, 'task', "WAITING")
     temp_db.workflows.add_task(124, WF_ID, 'task', "RUNNING")
 
     resp = client().get(f'/bee_wfm/v1/jobs/{WF_ID}')
-    assert 'RUNNING' in resp.json['tasks_status']
+    tasks_status = resp.json['tasks_status']
+    assert tasks_status[0][2] == 'RUNNING' or tasks_status[1][2] == 'RUNNING'
 
 
 def test_cancel_workflow(client, mocker, setup_teardown_workflow, temp_db):
     """Test cancelling a workflow."""
     mocker.patch('beeflow.wf_manager.resources.wf_utils.get_workflow_interface',
                  return_value=MockWFI())
     mocker.patch('beeflow.wf_manager.resources.wf_utils.get_db_path', temp_db.db_file)
@@ -206,20 +207,43 @@
     gdb_pid = 12345
 
     temp_db.workflows.init_workflow(WF_ID, wf_name, wf_status, 'dir', bolt_port, gdb_pid)
     temp_db.workflows.add_task(123, WF_ID, 'task', "WAITING")
     temp_db.workflows.add_task(124, WF_ID, 'task', "RUNNING")
     mocker.patch('beeflow.wf_manager.resources.wf_actions.dep_manager.kill_gdb', return_value=None)
 
-    request = {'wf_id': WF_ID}
+    request = {'wf_id': WF_ID, 'option': 'cancel'}
     resp = client().delete(f'/bee_wfm/v1/jobs/{WF_ID}', json=request)
     assert resp.json['status'] == 'Cancelled'
     assert resp.status_code == 202
 
 
+def test_remove_workflow(client, mocker, setup_teardown_workflow, temp_db):
+    """Test removing a workflow."""
+    mocker.patch('beeflow.wf_manager.resources.wf_utils.get_workflow_interface',
+                 return_value=MockWFI())
+    mocker.patch('beeflow.wf_manager.resources.wf_utils.get_db_path', temp_db.db_file)
+    mocker.patch('beeflow.wf_manager.resources.wf_actions.db_path', temp_db.db_file)
+
+    wf_name = 'wf'
+    wf_status = 'Archived'
+    bolt_port = 3030
+    gdb_pid = 12345
+
+    temp_db.workflows.init_workflow(WF_ID, wf_name, wf_status, 'dir', bolt_port, gdb_pid)
+    temp_db.workflows.add_task(123, WF_ID, 'task', "WAITING")
+    temp_db.workflows.add_task(124, WF_ID, 'task', "RUNNING")
+    mocker.patch('beeflow.wf_manager.resources.wf_actions.dep_manager.kill_gdb', return_value=None)
+
+    request = {'wf_id': WF_ID, 'option': 'remove'}
+    resp = client().delete(f'/bee_wfm/v1/jobs/{WF_ID}', json=request)
+    assert resp.json['status'] == 'Removed'
+    assert resp.status_code == 202
+
+
 def test_pause_workflow(client, mocker, setup_teardown_workflow, temp_db):
     """Test pausing a workflow."""
     mocker.patch('beeflow.wf_manager.resources.wf_utils.get_workflow_interface',
                  return_value=MockWFI())
     mocker.patch('beeflow.tests.mocks.MockWFI.get_workflow_state',
                  return_value='RUNNING')
     mocker.patch('beeflow.wf_manager.resources.wf_utils.get_db_path', temp_db.db_file)
```

### Comparing `hpc_beeflow-0.1.6/beeflow/wf_manager/common/dep_manager.py` & `hpc-beeflow-0.1.7/beeflow/wf_manager/common/dep_manager.py`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/wf_manager/common/wf_db.py` & `hpc-beeflow-0.1.7/beeflow/wf_manager/common/wf_db.py`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/wf_manager/resources/wf_actions.py` & `hpc-beeflow-0.1.7/beeflow/wf_manager/resources/wf_actions.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 """This module contains the workflow action endpoints."""
+import shutil
+import os
 
 from flask import make_response, jsonify
 from flask_restful import Resource, reqparse
 from beeflow.common import log as bee_logging
 from beeflow.wf_manager.resources import wf_utils
 
 from beeflow.common.db import wfm_db
@@ -36,42 +38,52 @@
         """Check the database for the current status of all tasks."""
         db = connect_db(wfm_db, db_path)
         tasks = db.workflows.get_tasks(wf_id)
         tasks_status = []
         if not tasks:
             log.info(f"Bad query for wf {wf_id}.")
             wf_status = 'No workflow with that ID is currently loaded'
-            tasks_status.append('Unavailable')
             resp = make_response(jsonify(tasks_status=tasks_status,
                                  wf_status=wf_status, status='not found'), 404)
 
         for task in tasks:
-            tasks_status.append(f"{task.name}--{task.state}")
-        tasks_status = '\n'.join(tasks_status)
+            tasks_status.append((task.id, task.name, task.state))
         wf_status = db.workflows.get_workflow_state(wf_id)
 
         resp = make_response(jsonify(tasks_status=tasks_status,
                              wf_status=wf_status, status='ok'), 200)
         return resp
 
-    @staticmethod
-    def delete(wf_id):
-        """Cancel the workflow. Lets current tasks finish running."""
+    def delete(self, wf_id):
+        """Cancel or delete the workflow. For cancel, current tasks finish running."""
+        self.reqparse.add_argument('option', type=str, location='json')
+        option = self.reqparse.parse_args()['option']
         db = connect_db(wfm_db, db_path)
-        wfi = wf_utils.get_workflow_interface(wf_id)
-        # Remove all tasks currently in the database
-        if wfi.workflow_loaded():
-            wfi.finalize_workflow()
-        wf_utils.update_wf_status(wf_id, 'Cancelled')
-        db.workflows.update_workflow_state(wf_id, 'Cancelled')
-        log.info("Workflow cancelled")
-        log.info("Shutting down gdb")
-        pid = db.workflows.get_gdb_pid(wf_id)
-        dep_manager.kill_gdb(pid)
-        resp = make_response(jsonify(status='Cancelled'), 202)
+        if option == "cancel":
+            wfi = wf_utils.get_workflow_interface(wf_id)
+            # Remove all tasks currently in the database
+            if wfi.workflow_loaded():
+                wfi.finalize_workflow()
+            wf_utils.update_wf_status(wf_id, 'Cancelled')
+            db.workflows.update_workflow_state(wf_id, 'Cancelled')
+            log.info("Workflow cancelled")
+            log.info("Shutting down gdb")
+            pid = db.workflows.get_gdb_pid(wf_id)
+            dep_manager.kill_gdb(pid)
+            resp = make_response(jsonify(status='Cancelled'), 202)
+        elif option == "remove":
+            log.info(f"Removing workflow {wf_id}.")
+            db.workflows.delete_workflow(wf_id)
+            resp = make_response(jsonify(status='Removed'), 202)
+            bee_workdir = wf_utils.get_bee_workdir()
+            workflow_dir = f"{bee_workdir}/workflows/{wf_id}"
+            shutil.rmtree(workflow_dir, ignore_errors=True)
+            archive_path = f"{bee_workdir}/archives/{wf_id}.tgz"
+            if os.path.exists(archive_path):
+                os.remove(archive_path)
         return resp
 
     def patch(self, wf_id):
         """Pause or resume workflow."""
         db = connect_db(wfm_db, db_path)
         self.reqparse.add_argument('option', type=str, location='json')
         option = self.reqparse.parse_args()['option']
```

### Comparing `hpc_beeflow-0.1.6/beeflow/wf_manager/resources/wf_list.py` & `hpc-beeflow-0.1.7/beeflow/wf_manager/resources/wf_list.py`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/wf_manager/resources/wf_metadata.py` & `hpc-beeflow-0.1.7/beeflow/wf_manager/resources/wf_metadata.py`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/wf_manager/resources/wf_update.py` & `hpc-beeflow-0.1.7/beeflow/wf_manager/resources/wf_update.py`

 * *Files 6% similar despite different names*

```diff
@@ -92,19 +92,22 @@
             with open(task_output_path, 'w', encoding='utf8') as fp:
                 json.dump(json.loads(data['output']), fp, indent=4)
 
         if 'task_info' in data and data['task_info'] is not None:
             task_info = jsonpickle.decode(data['task_info'])
             checkpoint_file = task_info['checkpoint_file']
             new_task = wfi.restart_task(task, checkpoint_file)
-            db.workflows.add_task(new_task.id, wf_id, new_task.name, "WAITING")
             if new_task is None:
                 log.info('No more restarts')
-                wf_state = wfi.get_task_state(task)
+                wf_state = wfi.get_workflow_state()
+                wfi.set_workflow_state('Failed')
+                wf_utils.update_wf_status(wf_id, 'Failed')
+                db.workflows.update_workflow_state(wf_id, 'Failed')
                 return make_response(jsonify(status=f'Task {task_id} set to {job_state}'))
+            db.workflows.add_task(new_task.id, wf_id, new_task.name, "WAITING")
             # Submit the restart task
             tasks = [new_task]
             wf_utils.schedule_submit_tasks(wf_id, tasks)
             return make_response(jsonify(status='Task {task_id} restarted'))
 
         if job_state in ('COMPLETED', 'FAILED'):
             for output in task.outputs:
@@ -127,13 +130,19 @@
                 log.info("Workflow failed")
                 log.info("Shutting down GDB")
                 wf_id = wfi.workflow_id
                 archive_workflow(db, wf_id)
                 pid = db.workflows.get_gdb_pid(wf_id)
                 dep_manager.kill_gdb(pid)
 
+        if job_state == 'BUILD_FAIL':
+            log.error(f'Workflow failed due to failed container build for task {task.name}')
+            wfi.set_workflow_state('Failed')
+            wf_utils.update_wf_status(wf_id, 'Failed')
+            db.workflows.update_workflow_state(wf_id, 'Failed')
+
         resp = make_response(jsonify(status=(f'Task {task_id} belonging to WF {wf_id} set to'
                                              f'{job_state}')), 200)
         return resp
 # Ignoring C901,R0915: "'WFUPdate.put' is too complex" - this requires a refactor
 #                      (or maybe the LOC limit is too low)
 # pylama:ignore=C901,R0915
```

### Comparing `hpc_beeflow-0.1.6/beeflow/wf_manager/resources/wf_utils.py` & `hpc-beeflow-0.1.7/beeflow/wf_manager/resources/wf_utils.py`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/beeflow/wf_manager/wf_manager.py` & `hpc-beeflow-0.1.7/beeflow/wf_manager/wf_manager.py`

 * *Files identical despite different names*

### Comparing `hpc_beeflow-0.1.6/pyproject.toml` & `hpc-beeflow-0.1.7/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hpc-beeflow"
-version = "0.1.6"
+version = "0.1.7"
 description = "A software package for containerizing HPC applications and managing job workflows"
 
 
 authors = [
     "BEE-LANL Dev Team <bee-dev@lanl.gov>"
 ]
 
@@ -43,20 +43,20 @@
 ]
 
 [tool.poetry.scripts]
 beeflow = 'beeflow.client.bee_client:main'
 beecloud = 'beeflow.cloud_launcher:main'
 
 [tool.poetry.dependencies]
-# Python version (>=3.8.3, <3.11)
-python = ">=3.8.3,<=3.11"
+
+# Python version (>=3.8.3, <=3.12.2)
+python = ">=3.8.3,<=3.12.2"
 
 # Package dependencies
 Flask = { version = "^2.0" }
-Jinja2 = { version = "<3.1" }
 neo4j = { version = "^1.7.4" }
 PyYAML = { version = "^6.0.1" }
 flask_restful = "0.3.9"
 cwl-utils = "^0.16"
 APScheduler = "^3.6.3"
 jsonpickle = "^2.2.0"
 # Fix for urllib3 2.0 breaking change (similar error to this https://github.com/docker/docker-py/issues/3113)
```

### Comparing `hpc_beeflow-0.1.6/PKG-INFO` & `hpc-beeflow-0.1.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,51 +1,48 @@
 Metadata-Version: 2.1
 Name: hpc-beeflow
-Version: 0.1.6
+Version: 0.1.7
 Summary: A software package for containerizing HPC applications and managing job workflows
 Home-page: https://github.com/lanl/BEE
 Keywords: bee,hpc,workflow,cluster,computing
 Author: BEE-LANL Dev Team
 Author-email: bee-dev@lanl.gov
-Requires-Python: >=3.8.3,<=3.11
+Requires-Python: >=3.8.3,<=3.12.2
 Classifier: Environment :: Console
 Classifier: Environment :: OpenStack
 Classifier: Environment :: Other Environment
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: Other/Proprietary License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: System :: Clustering
 Classifier: Topic :: System :: Distributed Computing
 Classifier: Topic :: System :: Logging
 Classifier: Topic :: System :: Monitoring
-Provides-Extra: cloud-extras
+Provides-Extra: cloud_extras
 Requires-Dist: APScheduler (>=3.6.3,<4.0.0)
 Requires-Dist: Flask (>=2.0,<3.0)
-Requires-Dist: Jinja2 (<3.1)
 Requires-Dist: PyYAML (>=6.0.1,<7.0.0)
 Requires-Dist: celery[redis,sqlalchemy] (>=5.3.4,<6.0.0)
 Requires-Dist: cffi (>=1.15.1,<2.0.0)
 Requires-Dist: cwl-utils (>=0.16,<0.17)
 Requires-Dist: flask_restful (==0.3.9)
-Requires-Dist: google-api-python-client (>=2.66.0,<3.0.0) ; extra == "cloud-extras"
+Requires-Dist: google-api-python-client (>=2.66.0,<3.0.0); extra == "cloud_extras"
 Requires-Dist: gunicorn (>=20.1.0,<21.0.0)
 Requires-Dist: jsonpickle (>=2.2.0,<3.0.0)
 Requires-Dist: neo4j (>=1.7.4,<2.0.0)
 Requires-Dist: python-daemon (>=2.3.1,<3.0.0)
-Requires-Dist: python-heatclient (>=3.1.0,<4.0.0) ; extra == "cloud-extras"
-Requires-Dist: python-openstackclient (>=6.0.0,<7.0.0) ; extra == "cloud-extras"
+Requires-Dist: python-heatclient (>=3.1.0,<4.0.0); extra == "cloud_extras"
+Requires-Dist: python-openstackclient (>=6.0.0,<7.0.0); extra == "cloud_extras"
 Requires-Dist: requests (<2.29.0)
 Requires-Dist: requests-unixsocket (>=0.3.0,<0.4.0)
 Requires-Dist: typer (>=0.5.0,<0.6.0)
 Project-URL: Repository, https://github.com/lanl/BEE
 Description-Content-Type: text/x-rst
 
 BEE: Build and Execution Environment
@@ -88,14 +85,15 @@
 Contributors:
 ==========================
 
 * Steven Anaya - `Boogie3D <https://github.com/Boogie3D>`_
 * Paul Bryant - `paulbry <https://github.com/paulbry>`_
 * Rusty Davis - `rstyd <https://github.com/rstyd>`_
 * Jieyang Chen - `JieyangChen7 <https://github.com/JieyangChen7>`_
+* Krishna Chilleri - `Krishna Chilleri <https://github.com/kchilleri>`_
 * Patricia Grubel - `pagrubel <https://github.com/pagrubel>`_
 * Qiang Guan - `guanxyz <https://github.com/guanxyz>`_
 * Ragini Gupta - `raginigupta6 <https://github.com/raginigupta6>`_
 * Andres Quan - `aquan9 <https://github.com/aquan9>`_
 * Quincy Wofford - `qwofford <https://github.com/qwofford>`_
 * Tim Randles - `trandles-lanl <https://github.com/trandles-lanl>`_
 * Jacob Tronge - `jtronge <https://github.com/jtronge>`_
@@ -131,14 +129,13 @@
 ==========================
 License can be found `here <https://github.com/lanl/BEE/blob/master/LICENSE>`_
 
 
 Publications
 ==========================
 
+- An HPC-Container Based Continuous Integration Tool for Detecting Scaling and Performance Issues in HPC Applications, IEEE Transactions on Services Computing, 2024, `DOI: 10.1109/TSC.2023.3337662 <https://doi.ieeecomputersociety.org/10.1109/TSC.2023.3337662>`_
 - BEE Orchestrator: Running Complex Scientific Workflows on Multiple Systems, HiPC, 2021, `DOI: 10.1109/HiPC53243.2021.00052 <https://doi.org/10.1109/HiPC53243.2021.00052>`_
 - "BeeSwarm: Enabling Parallel Scaling Performance Measurement in Continuous Integration for HPC Applications", ASE, 2021, `DOI: 10.1109/ASE51524.2021.9678805 <https://www.computer.org/csdl/proceedings-article/ase/2021/033700b136/1AjTjgnW2pa#:~:text=10.1109/ASE51524.2021.9678805>`_
 - "BeeFlow: A Workflow Management System for In Situ Processing across HPC and Cloud Systems", ICDCS, 2018, `DOI: 10.1109/ICDCS.2018.00103 <https://ieeexplore.ieee.org/abstract/document/8416366>`_
 - "Build and execution environment (BEE): an encapsulated environment enabling HPC applications running everywhere", IEEE BigData, 2018, `DOI: 10.1109/BigData.2018.8622572 <https://ieeexplore.ieee.org/document/8622572>`_
 
-
-
```

