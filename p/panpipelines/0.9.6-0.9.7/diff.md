# Comparing `tmp/panpipelines-0.9.6.tar.gz` & `tmp/panpipelines-0.9.7.tar.gz`

## Comparing `panpipelines-0.9.6.tar` & `panpipelines-0.9.7.tar`

### file list

```diff
@@ -1,175 +1,179 @@
--rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 panpipelines-0.9.6/.github/workflows/python-package.yml
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 panpipelines-0.9.6/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     5401 2020-02-02 00:00:00.000000 panpipelines-0.9.6/PAN250_Deployment/README.md
--rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 panpipelines-0.9.6/PAN250_Deployment/run_pan250.sh
--rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 panpipelines-0.9.6/PAN250_Deployment/atlas/Arterial/README.md
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 panpipelines-0.9.6/PAN250_Deployment/atlas/Arterial/res-02_atlas-Arterial_dseg.tsv
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 panpipelines-0.9.6/PAN250_Deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-Arterial_dseg.json
--rw-r--r--   0        0        0    37861 2020-02-02 00:00:00.000000 panpipelines-0.9.6/PAN250_Deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-Arterial_dseg.nii.gz
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 panpipelines-0.9.6/PAN250_Deployment/atlas/XTRACT/README.md
--rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 panpipelines-0.9.6/PAN250_Deployment/atlas/XTRACT/res-02_atlas-XTRACT_dseg.txt
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 panpipelines-0.9.6/PAN250_Deployment/atlas/XTRACT/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-XTRACT_dseg.json
--rw-r--r--   0        0        0    42696 2020-02-02 00:00:00.000000 panpipelines-0.9.6/PAN250_Deployment/atlas/XTRACT/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-XTRACT_dseg.nii.gz
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 panpipelines-0.9.6/PAN250_Deployment/batch_scripts/group_template.pbs
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 panpipelines-0.9.6/PAN250_Deployment/batch_scripts/participant_template.pbs
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 panpipelines-0.9.6/PAN250_Deployment/batch_scripts/headers/slurm_cpu.pbs
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 panpipelines-0.9.6/PAN250_Deployment/batch_scripts/headers/slurm_cpu_highpri.pbs
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 panpipelines-0.9.6/PAN250_Deployment/batch_scripts/headers/slurm_cpu_highpri_long.pbs
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 panpipelines-0.9.6/PAN250_Deployment/batch_scripts/headers/slurm_cpu_highpri_medium.pbs
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 panpipelines-0.9.6/PAN250_Deployment/batch_scripts/headers/slurm_cpu_highpri_small.pbs
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 panpipelines-0.9.6/PAN250_Deployment/batch_scripts/headers/slurm_cpu_highpri_tiny.pbs
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 panpipelines-0.9.6/PAN250_Deployment/batch_scripts/headers/slurm_cpu_highpri_verylong.pbs
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 panpipelines-0.9.6/PAN250_Deployment/batch_scripts/headers/slurm_cpu_small.pbs
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 panpipelines-0.9.6/PAN250_Deployment/batch_scripts/headers/slurm_cpu_tiny.pbs
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 panpipelines-0.9.6/PAN250_Deployment/batch_scripts/headers/slurm_gpu.pbs
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 panpipelines-0.9.6/PAN250_Deployment/config/license.txt
--rw-r--r--   0        0        0    10449 2020-02-02 00:00:00.000000 panpipelines-0.9.6/PAN250_Deployment/config/pan250.config
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 panpipelines-0.9.6/PAN250_Deployment/config/pan250_eddyparams.json
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 panpipelines-0.9.6/PAN250_Deployment/config/credentials/credentials.json
--rw-r--r--   0        0        0    10047 2020-02-02 00:00:00.000000 panpipelines-0.9.6/deployment/README.md
--rwxr-xr-x   0        0        0     1471 2020-02-02 00:00:00.000000 panpipelines-0.9.6/deployment/run_pan_slurm.sh
--rw-r--r--   0        0        0     2740 2020-02-02 00:00:00.000000 panpipelines-0.9.6/deployment/atlas/AAL3/AAL3v1_1mm_index.txt
--rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 panpipelines-0.9.6/deployment/atlas/AAL3/README.md
--rw-r--r--   0        0        0     3254 2020-02-02 00:00:00.000000 panpipelines-0.9.6/deployment/atlas/AAL3/res-01_atlas-AAL3_dseg.tsv
--rw-r--r--   0        0        0     3254 2020-02-02 00:00:00.000000 panpipelines-0.9.6/deployment/atlas/AAL3/res-02_atlas-AAL3_dseg.tsv
--rw-r--r--   0        0        0   119500 2020-02-02 00:00:00.000000 panpipelines-0.9.6/deployment/atlas/AAL3/MNI152NLin6Asym/AAL3v1_1mm_MNI152NLin6Asym.nii.gz
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 panpipelines-0.9.6/deployment/atlas/AAL3/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-AAL3_dseg.json
--rw-r--r--   0        0        0   119500 2020-02-02 00:00:00.000000 panpipelines-0.9.6/deployment/atlas/AAL3/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-AAL3_dseg.nii.gz
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 panpipelines-0.9.6/deployment/atlas/AAL3/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-AAL3_dseg.json
--rw-r--r--   0        0        0    38695 2020-02-02 00:00:00.000000 panpipelines-0.9.6/deployment/atlas/AAL3/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-AAL3_dseg.nii.gz
--rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 panpipelines-0.9.6/deployment/atlas/AAL3/MNI152NLin6Asym/Development/convert.sh
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 panpipelines-0.9.6/deployment/atlas/AAL3/MNI152NLin6Asym/Development/eye.mat
--rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 panpipelines-0.9.6/deployment/atlas/AAL3/MNI152NLin6Asym/Development/getTemplate.py
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 panpipelines-0.9.6/deployment/atlas/Arterial/ArterialAtlasLabels.txt
--rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 panpipelines-0.9.6/deployment/atlas/Arterial/README.md
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 panpipelines-0.9.6/deployment/atlas/Arterial/res-01_atlas-Arterial_dseg.tsv
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 panpipelines-0.9.6/deployment/atlas/Arterial/res-02_atlas-Arterial_dseg.tsv
--rw-r--r--   0        0        0   182712 2020-02-02 00:00:00.000000 panpipelines-0.9.6/deployment/atlas/Arterial/MNI152NLin6Asym/ArterialAtlas_int.nii.gz
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 panpipelines-0.9.6/deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-Arterial_dseg.json
--rw-r--r--   0        0        0   182309 2020-02-02 00:00:00.000000 panpipelines-0.9.6/deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-Arterial_dseg.nii.gz
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 panpipelines-0.9.6/deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-Arterial_dseg.json
--rw-r--r--   0        0        0    37861 2020-02-02 00:00:00.000000 panpipelines-0.9.6/deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-Arterial_dseg.nii.gz
--rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 panpipelines-0.9.6/deployment/atlas/HARVCORT/HarvardOxford-Cortical_index.txt
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 panpipelines-0.9.6/deployment/atlas/HARVCORT/README.md
--rwxr-xr-x   0        0        0   138203 2020-02-02 00:00:00.000000 panpipelines-0.9.6/deployment/atlas/HARVCORT/MNI152NLinAsym/HarvardOxford-cort-maxprob-thr25-1mm.nii.gz
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 panpipelines-0.9.6/deployment/atlas/HARVSUBCORT/HarvardOxford-Subcortical_index.txt
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 panpipelines-0.9.6/deployment/atlas/HARVSUBCORT/README.md
--rwxr-xr-x   0        0        0   166519 2020-02-02 00:00:00.000000 panpipelines-0.9.6/deployment/atlas/HARVSUBCORT/MNI152NLinAsym/HarvardOxford-sub-maxprob-thr25-1mm.nii.gz
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 panpipelines-0.9.6/deployment/atlas/HCPMMP1_FREESURFER/README.md
--rwxr-xr-x   0        0        0    14105 2020-02-02 00:00:00.000000 panpipelines-0.9.6/deployment/atlas/HCPMMP1_FREESURFER/hcpmmp1_ordered.txt
--rwxr-xr-x   0        0        0    12646 2020-02-02 00:00:00.000000 panpipelines-0.9.6/deployment/atlas/HCPMMP1_FREESURFER/hcpmmp1_original.txt
--rw-r--r--   0        0        0  1316983 2020-02-02 00:00:00.000000 panpipelines-0.9.6/deployment/atlas/HCPMMP1_FREESURFER/lh.HCP-MMP1.annot
--rw-r--r--   0        0        0  1316984 2020-02-02 00:00:00.000000 panpipelines-0.9.6/deployment/atlas/HCPMMP1_FREESURFER/rh.HCP-MMP1.annot
--rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 panpipelines-0.9.6/deployment/atlas/JHU/JHU-labels_index.txt
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 panpipelines-0.9.6/deployment/atlas/JHU/JHU-tracts_index.txt
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 panpipelines-0.9.6/deployment/atlas/JHU/README.md
--rwxr-xr-x   0        0        0    47474 2020-02-02 00:00:00.000000 panpipelines-0.9.6/deployment/atlas/JHU/MNI152NLinAsym/JHU-ICBM-labels-1mm.nii.gz
--rwxr-xr-x   0        0        0    47922 2020-02-02 00:00:00.000000 panpipelines-0.9.6/deployment/atlas/JHU/MNI152NLinAsym/JHU-ICBM-tracts-maxprob-thr25-1mm.nii.gz
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 panpipelines-0.9.6/deployment/atlas/XTRACT/README.md
--rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 panpipelines-0.9.6/deployment/atlas/XTRACT/XTRACT_index.txt
--rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 panpipelines-0.9.6/deployment/atlas/XTRACT/res-01_atlas-XTRACT_dseg.txt
--rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 panpipelines-0.9.6/deployment/atlas/XTRACT/res-02_atlas-XTRACT_dseg.txt
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 panpipelines-0.9.6/deployment/atlas/XTRACT/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-XTRACT_dseg.json
--rw-r--r--   0        0        0   191828 2020-02-02 00:00:00.000000 panpipelines-0.9.6/deployment/atlas/XTRACT/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-XTRACT_dseg.nii.gz
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 panpipelines-0.9.6/deployment/atlas/XTRACT/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-XTRACT_dseg.json
--rw-r--r--   0        0        0    42696 2020-02-02 00:00:00.000000 panpipelines-0.9.6/deployment/atlas/XTRACT/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-XTRACT_dseg.nii.gz
--rw-r--r--   0        0        0   196623 2020-02-02 00:00:00.000000 panpipelines-0.9.6/deployment/atlas/XTRACT/MNI152NLin6Asym/xtract-tract-atlases-maxprob5-1mm.nii.gz
--rwxr-xr-x   0        0        0    89181 2020-02-02 00:00:00.000000 panpipelines-0.9.6/deployment/atlas/freesurfer_atlas/FreeSurferColorLUT.txt
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 panpipelines-0.9.6/deployment/atlas/freesurfer_atlas/README.md
--rwxr-xr-x   0        0        0    10131 2020-02-02 00:00:00.000000 panpipelines-0.9.6/deployment/atlas/freesurfer_atlas/fs_a2009s.txt
--rw-r--r--   0        0        0     6193 2020-02-02 00:00:00.000000 panpipelines-0.9.6/deployment/atlas/freesurfer_atlas/fs_default.txt
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 panpipelines-0.9.6/deployment/atlas/hcpmmp1_subfields_atlas/README.md
--rwxr-xr-x   0        0        0    14879 2020-02-02 00:00:00.000000 panpipelines-0.9.6/deployment/atlas/hcpmmp1_subfields_atlas/hcpmmp1_subfields_ordered.txt
--rwxr-xr-x   0        0        0    13454 2020-02-02 00:00:00.000000 panpipelines-0.9.6/deployment/atlas/hcpmmp1_subfields_atlas/hcpmmp1_subfields_original.txt
--rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 panpipelines-0.9.6/deployment/batch_scripts/group_template.pbs
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 panpipelines-0.9.6/deployment/batch_scripts/participant_template.pbs
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 panpipelines-0.9.6/deployment/batch_scripts/headers/slurm_cpu.pbs
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 panpipelines-0.9.6/deployment/batch_scripts/headers/slurm_cpu_fmriprep.pbs
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 panpipelines-0.9.6/deployment/batch_scripts/headers/slurm_cpu_highpri.pbs
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 panpipelines-0.9.6/deployment/batch_scripts/headers/slurm_cpu_highpri_fmriprep.pbs
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 panpipelines-0.9.6/deployment/batch_scripts/headers/slurm_gpu.pbs
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 panpipelines-0.9.6/deployment/batch_scripts/headers/slurm_gpu_highpri.pbs
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 panpipelines-0.9.6/deployment/batch_scripts/headers/slurm_gpu_windfall.pbs
--rwxr-xr-x   0        0        0      384 2020-02-02 00:00:00.000000 panpipelines-0.9.6/deployment/config/eddy_params.json
--rwxr-xr-x   0        0        0      379 2020-02-02 00:00:00.000000 panpipelines-0.9.6/deployment/config/eddy_params_cpu.json
--rwxr-xr-x   0        0        0      124 2020-02-02 00:00:00.000000 panpipelines-0.9.6/deployment/config/freebash.sh
--rwxr-xr-x   0        0        0       66 2020-02-02 00:00:00.000000 panpipelines-0.9.6/deployment/config/license.txt
--rw-r--r--   0        0        0    23977 2020-02-02 00:00:00.000000 panpipelines-0.9.6/deployment/config/panpipeconfig_expanded_slurm.config
--rw-r--r--   0        0        0    28701 2020-02-02 00:00:00.000000 panpipelines-0.9.6/deployment/config/panpipeconfig_slurm.config
--rwxr-xr-x   0        0        0       59 2020-02-02 00:00:00.000000 panpipelines-0.9.6/deployment/config/credentials/credentials.json
--rwxr-xr-x   0        0        0      215 2020-02-02 00:00:00.000000 panpipelines-0.9.6/example/run_pan_example.sh
--rw-r--r--   0        0        0     3641 2020-02-02 00:00:00.000000 panpipelines-0.9.6/example/config/panpipeconfig_example.config
--rwxr-xr-x   0        0        0       59 2020-02-02 00:00:00.000000 panpipelines-0.9.6/example/config/credentials/credentials_example.json
--rw-r--r--   0        0        0     5085 2020-02-02 00:00:00.000000 panpipelines-0.9.6/src/panpipelines/Factory.py
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 panpipelines-0.9.6/src/panpipelines/__init__.py
--rw-r--r--   0        0        0     4878 2020-02-02 00:00:00.000000 panpipelines-0.9.6/src/panpipelines/group_subjects.py
--rwxr-xr-x   0        0        0    18168 2020-02-02 00:00:00.000000 panpipelines-0.9.6/src/panpipelines/pan_processing.py
--rw-r--r--   0        0        0     8417 2020-02-02 00:00:00.000000 panpipelines-0.9.6/src/panpipelines/single_subject.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 panpipelines-0.9.6/src/panpipelines/version.py
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 panpipelines-0.9.6/src/panpipelines/nodes/__init__.py
--rw-r--r--   0        0        0    14132 2020-02-02 00:00:00.000000 panpipelines-0.9.6/src/panpipelines/nodes/antstransform.py
--rw-r--r--   0        0        0     6406 2020-02-02 00:00:00.000000 panpipelines-0.9.6/src/panpipelines/nodes/aslprep.py
--rw-r--r--   0        0        0     5264 2020-02-02 00:00:00.000000 panpipelines-0.9.6/src/panpipelines/nodes/atlascreate.py
--rw-r--r--   0        0        0    21152 2020-02-02 00:00:00.000000 panpipelines-0.9.6/src/panpipelines/nodes/basil.py
--rw-r--r--   0        0        0     7549 2020-02-02 00:00:00.000000 panpipelines-0.9.6/src/panpipelines/nodes/collate_csv_group.py
--rw-r--r--   0        0        0     6288 2020-02-02 00:00:00.000000 panpipelines-0.9.6/src/panpipelines/nodes/collate_csv_single.py
--rw-r--r--   0        0        0     4563 2020-02-02 00:00:00.000000 panpipelines-0.9.6/src/panpipelines/nodes/dummy.py
--rw-r--r--   0        0        0    10177 2020-02-02 00:00:00.000000 panpipelines-0.9.6/src/panpipelines/nodes/fmriprep.py
--rw-r--r--   0        0        0    10720 2020-02-02 00:00:00.000000 panpipelines-0.9.6/src/panpipelines/nodes/freesurfer.py
--rw-r--r--   0        0        0     3495 2020-02-02 00:00:00.000000 panpipelines-0.9.6/src/panpipelines/nodes/fslanat.py
--rw-r--r--   0        0        0     7191 2020-02-02 00:00:00.000000 panpipelines-0.9.6/src/panpipelines/nodes/glm_randomize_group.py
--rw-r--r--   0        0        0     7622 2020-02-02 00:00:00.000000 panpipelines-0.9.6/src/panpipelines/nodes/lst.py
--rw-r--r--   0        0        0     6175 2020-02-02 00:00:00.000000 panpipelines-0.9.6/src/panpipelines/nodes/noddi.py
--rw-r--r--   0        0        0     8370 2020-02-02 00:00:00.000000 panpipelines-0.9.6/src/panpipelines/nodes/parse_textdata.py
--rw-r--r--   0        0        0     7399 2020-02-02 00:00:00.000000 panpipelines-0.9.6/src/panpipelines/nodes/qsiprep.py
--rw-r--r--   0        0        0    14947 2020-02-02 00:00:00.000000 panpipelines-0.9.6/src/panpipelines/nodes/roi_extract.py
--rw-r--r--   0        0        0     5324 2020-02-02 00:00:00.000000 panpipelines-0.9.6/src/panpipelines/nodes/roi_mean_group.py
--rw-r--r--   0        0        0    11130 2020-02-02 00:00:00.000000 panpipelines-0.9.6/src/panpipelines/nodes/roi_mean_single.py
--rw-r--r--   0        0        0    10201 2020-02-02 00:00:00.000000 panpipelines-0.9.6/src/panpipelines/nodes/tensor.py
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 panpipelines-0.9.6/src/panpipelines/pipelines/__init__.py
--rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 panpipelines-0.9.6/src/panpipelines/pipelines/aslprep_panpipeline.py
--rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 panpipelines-0.9.6/src/panpipelines/pipelines/basil_panpipeline.py
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 panpipelines-0.9.6/src/panpipelines/pipelines/collatecsv_panpipeline.py
--rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 panpipelines-0.9.6/src/panpipelines/pipelines/collatecsvgroup_panpipeline.py
--rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 panpipelines-0.9.6/src/panpipelines/pipelines/dummy_panpipeline.py
--rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 panpipelines-0.9.6/src/panpipelines/pipelines/fmriprep_panpipeline.py
--rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 panpipelines-0.9.6/src/panpipelines/pipelines/freesurfer_panpipeline.py
--rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 panpipelines-0.9.6/src/panpipelines/pipelines/lst_panpipeline.py
--rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 panpipelines-0.9.6/src/panpipelines/pipelines/noddi_panpipeline.py
--rw-r--r--   0        0        0     3297 2020-02-02 00:00:00.000000 panpipelines-0.9.6/src/panpipelines/pipelines/panpipeline.py
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 panpipelines-0.9.6/src/panpipelines/pipelines/qsiprep_panpipeline.py
--rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 panpipelines-0.9.6/src/panpipelines/pipelines/roiextract_panpipeline.py
--rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 panpipelines-0.9.6/src/panpipelines/pipelines/tensor_panpipeline.py
--rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 panpipelines-0.9.6/src/panpipelines/pipelines/textmeasures_panpipeline.py
--rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 panpipelines-0.9.6/src/panpipelines/pipelines/volmeasures_panpipeline.py
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 panpipelines-0.9.6/src/panpipelines/scripts/__init__.py
--rw-r--r--   0        0        0     7141 2020-02-02 00:00:00.000000 panpipelines-0.9.6/src/panpipelines/scripts/aslprep_panscript.py
--rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 panpipelines-0.9.6/src/panpipelines/scripts/fmriprep_panscript.py
--rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 panpipelines-0.9.6/src/panpipelines/scripts/pancontainer_panscript.py
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 panpipelines-0.9.6/src/panpipelines/scripts/panscript.py
--rw-r--r--   0        0        0     2173 2020-02-02 00:00:00.000000 panpipelines-0.9.6/src/panpipelines/scripts/sdcflows_fieldmap.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 panpipelines-0.9.6/src/panpipelines/utils/__init__.py
--rw-r--r--   0        0        0    31963 2020-02-02 00:00:00.000000 panpipelines-0.9.6/src/panpipelines/utils/transformer.py
--rw-r--r--   0        0        0    71325 2020-02-02 00:00:00.000000 panpipelines-0.9.6/src/panpipelines/utils/util_functions.py
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 panpipelines-0.9.6/src/panpipelines/workflows/__init__.py
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 panpipelines-0.9.6/src/panpipelines/workflows/aslprep_workflow.py
--rw-r--r--   0        0        0     4783 2020-02-02 00:00:00.000000 panpipelines-0.9.6/src/panpipelines/workflows/basil_workflow.py
--rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 panpipelines-0.9.6/src/panpipelines/workflows/collatecsv_workflow.py
--rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 panpipelines-0.9.6/src/panpipelines/workflows/collatecsvgroup_workflow.py
--rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 panpipelines-0.9.6/src/panpipelines/workflows/dummy_workflow.py
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 panpipelines-0.9.6/src/panpipelines/workflows/fmriprep_workflow.py
--rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 panpipelines-0.9.6/src/panpipelines/workflows/freesurfer_workflow.py
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 panpipelines-0.9.6/src/panpipelines/workflows/lst_workflow.py
--rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 panpipelines-0.9.6/src/panpipelines/workflows/noddi_workflow.py
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 panpipelines-0.9.6/src/panpipelines/workflows/qsiprep_workflow.py
--rw-r--r--   0        0        0     4897 2020-02-02 00:00:00.000000 panpipelines-0.9.6/src/panpipelines/workflows/roiextract_workflow.py
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 panpipelines-0.9.6/src/panpipelines/workflows/tensor_workflow.py
--rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 panpipelines-0.9.6/src/panpipelines/workflows/textmeasures_workflow.py
--rw-r--r--   0        0        0     4946 2020-02-02 00:00:00.000000 panpipelines-0.9.6/src/panpipelines/workflows/volmeasures_workflow.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panpipelines-0.9.6/tests/__init__.py
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 panpipelines-0.9.6/tests/test_PANFactory.py
--rw-r--r--   0        0        0     3152 2020-02-02 00:00:00.000000 panpipelines-0.9.6/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 panpipelines-0.9.6/LICENSE
--rw-r--r--   0        0        0    12997 2020-02-02 00:00:00.000000 panpipelines-0.9.6/README.md
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 panpipelines-0.9.6/pyproject.toml
--rw-r--r--   0        0        0    15157 2020-02-02 00:00:00.000000 panpipelines-0.9.6/PKG-INFO
+-rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 panpipelines-0.9.7/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 panpipelines-0.9.7/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     5401 2020-02-02 00:00:00.000000 panpipelines-0.9.7/PAN250_Deployment/README.md
+-rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 panpipelines-0.9.7/PAN250_Deployment/run_pan250.sh
+-rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 panpipelines-0.9.7/PAN250_Deployment/atlas/Arterial/README.md
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 panpipelines-0.9.7/PAN250_Deployment/atlas/Arterial/res-02_atlas-Arterial_dseg.tsv
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 panpipelines-0.9.7/PAN250_Deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-Arterial_dseg.json
+-rw-r--r--   0        0        0    37861 2020-02-02 00:00:00.000000 panpipelines-0.9.7/PAN250_Deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-Arterial_dseg.nii.gz
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 panpipelines-0.9.7/PAN250_Deployment/atlas/XTRACT/README.md
+-rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 panpipelines-0.9.7/PAN250_Deployment/atlas/XTRACT/res-02_atlas-XTRACT_dseg.txt
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 panpipelines-0.9.7/PAN250_Deployment/atlas/XTRACT/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-XTRACT_dseg.json
+-rw-r--r--   0        0        0    42696 2020-02-02 00:00:00.000000 panpipelines-0.9.7/PAN250_Deployment/atlas/XTRACT/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-XTRACT_dseg.nii.gz
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 panpipelines-0.9.7/PAN250_Deployment/batch_scripts/group_template.pbs
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 panpipelines-0.9.7/PAN250_Deployment/batch_scripts/participant_template.pbs
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 panpipelines-0.9.7/PAN250_Deployment/batch_scripts/headers/slurm_cpu.pbs
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 panpipelines-0.9.7/PAN250_Deployment/batch_scripts/headers/slurm_cpu_highpri.pbs
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 panpipelines-0.9.7/PAN250_Deployment/batch_scripts/headers/slurm_cpu_highpri_long.pbs
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 panpipelines-0.9.7/PAN250_Deployment/batch_scripts/headers/slurm_cpu_highpri_medium.pbs
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 panpipelines-0.9.7/PAN250_Deployment/batch_scripts/headers/slurm_cpu_highpri_small.pbs
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 panpipelines-0.9.7/PAN250_Deployment/batch_scripts/headers/slurm_cpu_highpri_tiny.pbs
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 panpipelines-0.9.7/PAN250_Deployment/batch_scripts/headers/slurm_cpu_highpri_verylong.pbs
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 panpipelines-0.9.7/PAN250_Deployment/batch_scripts/headers/slurm_cpu_small.pbs
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 panpipelines-0.9.7/PAN250_Deployment/batch_scripts/headers/slurm_cpu_tiny.pbs
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 panpipelines-0.9.7/PAN250_Deployment/batch_scripts/headers/slurm_gpu.pbs
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 panpipelines-0.9.7/PAN250_Deployment/config/license.txt
+-rw-r--r--   0        0        0    10449 2020-02-02 00:00:00.000000 panpipelines-0.9.7/PAN250_Deployment/config/pan250.config
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 panpipelines-0.9.7/PAN250_Deployment/config/pan250_eddyparams.json
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 panpipelines-0.9.7/PAN250_Deployment/config/credentials/credentials.json
+-rw-r--r--   0        0        0    10047 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/README.md
+-rwxr-xr-x   0        0        0     1471 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/run_pan_slurm.sh
+-rw-r--r--   0        0        0     2740 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/atlas/AAL3/AAL3v1_1mm_index.txt
+-rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/atlas/AAL3/README.md
+-rw-r--r--   0        0        0     3254 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/atlas/AAL3/res-01_atlas-AAL3_dseg.tsv
+-rw-r--r--   0        0        0     3254 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/atlas/AAL3/res-02_atlas-AAL3_dseg.tsv
+-rw-r--r--   0        0        0   119500 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/atlas/AAL3/MNI152NLin6Asym/AAL3v1_1mm_MNI152NLin6Asym.nii.gz
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/atlas/AAL3/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-AAL3_dseg.json
+-rw-r--r--   0        0        0   119500 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/atlas/AAL3/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-AAL3_dseg.nii.gz
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/atlas/AAL3/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-AAL3_dseg.json
+-rw-r--r--   0        0        0    38695 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/atlas/AAL3/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-AAL3_dseg.nii.gz
+-rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/atlas/AAL3/MNI152NLin6Asym/Development/convert.sh
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/atlas/AAL3/MNI152NLin6Asym/Development/eye.mat
+-rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/atlas/AAL3/MNI152NLin6Asym/Development/getTemplate.py
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/atlas/Arterial/ArterialAtlasLabels.txt
+-rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/atlas/Arterial/README.md
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/atlas/Arterial/res-01_atlas-Arterial_dseg.tsv
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/atlas/Arterial/res-02_atlas-Arterial_dseg.tsv
+-rw-r--r--   0        0        0   182712 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/atlas/Arterial/MNI152NLin6Asym/ArterialAtlas_int.nii.gz
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-Arterial_dseg.json
+-rw-r--r--   0        0        0   182309 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-Arterial_dseg.nii.gz
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-Arterial_dseg.json
+-rw-r--r--   0        0        0    37861 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-Arterial_dseg.nii.gz
+-rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/atlas/HARVCORT/HarvardOxford-Cortical_index.txt
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/atlas/HARVCORT/README.md
+-rwxr-xr-x   0        0        0   138203 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/atlas/HARVCORT/MNI152NLinAsym/HarvardOxford-cort-maxprob-thr25-1mm.nii.gz
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/atlas/HARVSUBCORT/HarvardOxford-Subcortical_index.txt
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/atlas/HARVSUBCORT/README.md
+-rwxr-xr-x   0        0        0   166519 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/atlas/HARVSUBCORT/MNI152NLinAsym/HarvardOxford-sub-maxprob-thr25-1mm.nii.gz
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/atlas/HCPMMP1_FREESURFER/README.md
+-rwxr-xr-x   0        0        0    14105 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/atlas/HCPMMP1_FREESURFER/hcpmmp1_ordered.txt
+-rwxr-xr-x   0        0        0    12646 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/atlas/HCPMMP1_FREESURFER/hcpmmp1_original.txt
+-rw-r--r--   0        0        0  1316983 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/atlas/HCPMMP1_FREESURFER/lh.HCP-MMP1.annot
+-rw-r--r--   0        0        0  1316984 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/atlas/HCPMMP1_FREESURFER/rh.HCP-MMP1.annot
+-rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/atlas/JHU/JHU-labels_index.txt
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/atlas/JHU/JHU-tracts_index.txt
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/atlas/JHU/README.md
+-rwxr-xr-x   0        0        0    47474 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/atlas/JHU/MNI152NLinAsym/JHU-ICBM-labels-1mm.nii.gz
+-rwxr-xr-x   0        0        0    47922 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/atlas/JHU/MNI152NLinAsym/JHU-ICBM-tracts-maxprob-thr25-1mm.nii.gz
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/atlas/XTRACT/README.md
+-rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/atlas/XTRACT/XTRACT_index.txt
+-rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/atlas/XTRACT/res-01_atlas-XTRACT_dseg.txt
+-rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/atlas/XTRACT/res-02_atlas-XTRACT_dseg.txt
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/atlas/XTRACT/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-XTRACT_dseg.json
+-rw-r--r--   0        0        0   191828 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/atlas/XTRACT/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-XTRACT_dseg.nii.gz
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/atlas/XTRACT/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-XTRACT_dseg.json
+-rw-r--r--   0        0        0    42696 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/atlas/XTRACT/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-XTRACT_dseg.nii.gz
+-rw-r--r--   0        0        0   196623 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/atlas/XTRACT/MNI152NLin6Asym/xtract-tract-atlases-maxprob5-1mm.nii.gz
+-rwxr-xr-x   0        0        0    89181 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/atlas/freesurfer_atlas/FreeSurferColorLUT.txt
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/atlas/freesurfer_atlas/README.md
+-rwxr-xr-x   0        0        0    10131 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/atlas/freesurfer_atlas/fs_a2009s.txt
+-rw-r--r--   0        0        0     6193 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/atlas/freesurfer_atlas/fs_default.txt
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/atlas/hcpmmp1_subfields_atlas/README.md
+-rwxr-xr-x   0        0        0    14879 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/atlas/hcpmmp1_subfields_atlas/hcpmmp1_subfields_ordered.txt
+-rwxr-xr-x   0        0        0    13454 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/atlas/hcpmmp1_subfields_atlas/hcpmmp1_subfields_original.txt
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/batch_scripts/group_template.pbs
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/batch_scripts/participant_template.pbs
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/batch_scripts/headers/slurm_cpu.pbs
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/batch_scripts/headers/slurm_cpu_fmriprep.pbs
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/batch_scripts/headers/slurm_cpu_highpri.pbs
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/batch_scripts/headers/slurm_cpu_highpri_fmriprep.pbs
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/batch_scripts/headers/slurm_gpu.pbs
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/batch_scripts/headers/slurm_gpu_highpri.pbs
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/batch_scripts/headers/slurm_gpu_windfall.pbs
+-rwxr-xr-x   0        0        0      384 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/config/eddy_params.json
+-rwxr-xr-x   0        0        0      379 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/config/eddy_params_cpu.json
+-rwxr-xr-x   0        0        0      124 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/config/freebash.sh
+-rwxr-xr-x   0        0        0       66 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/config/license.txt
+-rw-r--r--   0        0        0    23977 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/config/panpipeconfig_expanded_slurm.config
+-rw-r--r--   0        0        0    28701 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/config/panpipeconfig_slurm.config
+-rwxr-xr-x   0        0        0       59 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/config/credentials/credentials.json
+-rwxr-xr-x   0        0        0      215 2020-02-02 00:00:00.000000 panpipelines-0.9.7/example/run_pan_example.sh
+-rw-r--r--   0        0        0     3641 2020-02-02 00:00:00.000000 panpipelines-0.9.7/example/config/panpipeconfig_example.config
+-rwxr-xr-x   0        0        0       59 2020-02-02 00:00:00.000000 panpipelines-0.9.7/example/config/credentials/credentials_example.json
+-rw-r--r--   0        0        0     5085 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/Factory.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/__init__.py
+-rw-r--r--   0        0        0     4878 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/group_subjects.py
+-rwxr-xr-x   0        0        0    18168 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/pan_processing.py
+-rw-r--r--   0        0        0     8417 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/single_subject.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/version.py
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/nodes/__init__.py
+-rw-r--r--   0        0        0    14132 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/nodes/antstransform.py
+-rw-r--r--   0        0        0     6406 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/nodes/aslprep.py
+-rw-r--r--   0        0        0     5264 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/nodes/atlascreate.py
+-rw-r--r--   0        0        0    21152 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/nodes/basil.py
+-rw-r--r--   0        0        0     7549 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/nodes/collate_csv_group.py
+-rw-r--r--   0        0        0     6288 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/nodes/collate_csv_single.py
+-rw-r--r--   0        0        0     4563 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/nodes/dummy.py
+-rw-r--r--   0        0        0    10177 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/nodes/fmriprep.py
+-rw-r--r--   0        0        0    10720 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/nodes/freesurfer.py
+-rw-r--r--   0        0        0     3495 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/nodes/fslanat.py
+-rw-r--r--   0        0        0     7191 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/nodes/glm_randomize_group.py
+-rw-r--r--   0        0        0     7622 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/nodes/lst.py
+-rw-r--r--   0        0        0     6175 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/nodes/noddi.py
+-rw-r--r--   0        0        0     8370 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/nodes/parse_textdata.py
+-rw-r--r--   0        0        0    14261 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/nodes/preproc.py
+-rw-r--r--   0        0        0     7399 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/nodes/qsiprep.py
+-rw-r--r--   0        0        0    16463 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/nodes/roi_extract.py
+-rw-r--r--   0        0        0     5324 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/nodes/roi_mean_group.py
+-rw-r--r--   0        0        0    11130 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/nodes/roi_mean_single.py
+-rw-r--r--   0        0        0    10201 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/nodes/tensor.py
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/pipelines/__init__.py
+-rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/pipelines/aslprep_panpipeline.py
+-rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/pipelines/basil_panpipeline.py
+-rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/pipelines/collatecsv_panpipeline.py
+-rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/pipelines/collatecsvgroup_panpipeline.py
+-rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/pipelines/dummy_panpipeline.py
+-rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/pipelines/fmriprep_panpipeline.py
+-rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/pipelines/freesurfer_panpipeline.py
+-rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/pipelines/lst_panpipeline.py
+-rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/pipelines/noddi_panpipeline.py
+-rw-r--r--   0        0        0     3297 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/pipelines/panpipeline.py
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/pipelines/preproc_panpipeline.py
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/pipelines/qsiprep_panpipeline.py
+-rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/pipelines/roiextract_panpipeline.py
+-rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/pipelines/tensor_panpipeline.py
+-rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/pipelines/textmeasures_panpipeline.py
+-rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/pipelines/volmeasures_panpipeline.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/scripts/__init__.py
+-rw-r--r--   0        0        0     7141 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/scripts/aslprep_panscript.py
+-rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/scripts/fmriprep_panscript.py
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/scripts/mne_make_surfaces.py
+-rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/scripts/pancontainer_panscript.py
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/scripts/panscript.py
+-rw-r--r--   0        0        0     2173 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/scripts/sdcflows_fieldmap.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/utils/__init__.py
+-rw-r--r--   0        0        0    31963 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/utils/transformer.py
+-rw-r--r--   0        0        0    71325 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/utils/util_functions.py
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/workflows/__init__.py
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/workflows/aslprep_workflow.py
+-rw-r--r--   0        0        0     4783 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/workflows/basil_workflow.py
+-rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/workflows/collatecsv_workflow.py
+-rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/workflows/collatecsvgroup_workflow.py
+-rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/workflows/dummy_workflow.py
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/workflows/fmriprep_workflow.py
+-rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/workflows/freesurfer_workflow.py
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/workflows/lst_workflow.py
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/workflows/noddi_workflow.py
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/workflows/preproc_workflow.py
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/workflows/qsiprep_workflow.py
+-rw-r--r--   0        0        0     7525 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/workflows/roiextract_workflow.py
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/workflows/tensor_workflow.py
+-rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/workflows/textmeasures_workflow.py
+-rw-r--r--   0        0        0     4946 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/workflows/volmeasures_workflow.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panpipelines-0.9.7/tests/__init__.py
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 panpipelines-0.9.7/tests/test_PANFactory.py
+-rw-r--r--   0        0        0     3152 2020-02-02 00:00:00.000000 panpipelines-0.9.7/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 panpipelines-0.9.7/LICENSE
+-rw-r--r--   0        0        0    12997 2020-02-02 00:00:00.000000 panpipelines-0.9.7/README.md
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 panpipelines-0.9.7/pyproject.toml
+-rw-r--r--   0        0        0    15188 2020-02-02 00:00:00.000000 panpipelines-0.9.7/PKG-INFO
```

### Comparing `panpipelines-0.9.6/.github/workflows/python-package.yml` & `panpipelines-0.9.7/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/.github/workflows/python-publish.yml` & `panpipelines-0.9.7/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/PAN250_Deployment/README.md` & `panpipelines-0.9.7/PAN250_Deployment/README.md`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/PAN250_Deployment/run_pan250.sh` & `panpipelines-0.9.7/PAN250_Deployment/run_pan250.sh`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/PAN250_Deployment/atlas/Arterial/README.md` & `panpipelines-0.9.7/PAN250_Deployment/atlas/Arterial/README.md`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/PAN250_Deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-Arterial_dseg.json` & `panpipelines-0.9.7/PAN250_Deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-Arterial_dseg.json`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/PAN250_Deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-Arterial_dseg.nii.gz` & `panpipelines-0.9.7/PAN250_Deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-Arterial_dseg.nii.gz`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/PAN250_Deployment/atlas/XTRACT/README.md` & `panpipelines-0.9.7/PAN250_Deployment/atlas/XTRACT/README.md`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/PAN250_Deployment/atlas/XTRACT/res-02_atlas-XTRACT_dseg.txt` & `panpipelines-0.9.7/PAN250_Deployment/atlas/XTRACT/res-02_atlas-XTRACT_dseg.txt`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/PAN250_Deployment/atlas/XTRACT/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-XTRACT_dseg.json` & `panpipelines-0.9.7/PAN250_Deployment/atlas/XTRACT/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-XTRACT_dseg.json`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/PAN250_Deployment/atlas/XTRACT/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-XTRACT_dseg.nii.gz` & `panpipelines-0.9.7/PAN250_Deployment/atlas/XTRACT/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-XTRACT_dseg.nii.gz`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/PAN250_Deployment/batch_scripts/group_template.pbs` & `panpipelines-0.9.7/PAN250_Deployment/batch_scripts/group_template.pbs`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/PAN250_Deployment/batch_scripts/participant_template.pbs` & `panpipelines-0.9.7/PAN250_Deployment/batch_scripts/participant_template.pbs`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/PAN250_Deployment/config/pan250.config` & `panpipelines-0.9.7/PAN250_Deployment/config/pan250.config`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/deployment/README.md` & `panpipelines-0.9.7/deployment/README.md`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/deployment/run_pan_slurm.sh` & `panpipelines-0.9.7/deployment/run_pan_slurm.sh`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/deployment/atlas/AAL3/AAL3v1_1mm_index.txt` & `panpipelines-0.9.7/deployment/atlas/AAL3/AAL3v1_1mm_index.txt`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/deployment/atlas/AAL3/README.md` & `panpipelines-0.9.7/deployment/atlas/AAL3/README.md`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/deployment/atlas/AAL3/res-01_atlas-AAL3_dseg.tsv` & `panpipelines-0.9.7/deployment/atlas/AAL3/res-01_atlas-AAL3_dseg.tsv`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/deployment/atlas/AAL3/res-02_atlas-AAL3_dseg.tsv` & `panpipelines-0.9.7/deployment/atlas/AAL3/res-02_atlas-AAL3_dseg.tsv`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/deployment/atlas/AAL3/MNI152NLin6Asym/AAL3v1_1mm_MNI152NLin6Asym.nii.gz` & `panpipelines-0.9.7/deployment/atlas/AAL3/MNI152NLin6Asym/AAL3v1_1mm_MNI152NLin6Asym.nii.gz`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/deployment/atlas/AAL3/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-AAL3_dseg.json` & `panpipelines-0.9.7/deployment/atlas/AAL3/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-AAL3_dseg.json`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/deployment/atlas/AAL3/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-AAL3_dseg.nii.gz` & `panpipelines-0.9.7/deployment/atlas/AAL3/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-AAL3_dseg.nii.gz`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/deployment/atlas/AAL3/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-AAL3_dseg.json` & `panpipelines-0.9.7/deployment/atlas/AAL3/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-AAL3_dseg.json`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/deployment/atlas/AAL3/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-AAL3_dseg.nii.gz` & `panpipelines-0.9.7/deployment/atlas/AAL3/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-AAL3_dseg.nii.gz`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/deployment/atlas/AAL3/MNI152NLin6Asym/Development/convert.sh` & `panpipelines-0.9.7/deployment/atlas/AAL3/MNI152NLin6Asym/Development/convert.sh`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/deployment/atlas/AAL3/MNI152NLin6Asym/Development/getTemplate.py` & `panpipelines-0.9.7/deployment/atlas/AAL3/MNI152NLin6Asym/Development/getTemplate.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/deployment/atlas/Arterial/README.md` & `panpipelines-0.9.7/deployment/atlas/Arterial/README.md`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/deployment/atlas/Arterial/MNI152NLin6Asym/ArterialAtlas_int.nii.gz` & `panpipelines-0.9.7/deployment/atlas/Arterial/MNI152NLin6Asym/ArterialAtlas_int.nii.gz`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-Arterial_dseg.json` & `panpipelines-0.9.7/deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-Arterial_dseg.json`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-Arterial_dseg.nii.gz` & `panpipelines-0.9.7/deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-Arterial_dseg.nii.gz`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-Arterial_dseg.json` & `panpipelines-0.9.7/deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-Arterial_dseg.json`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-Arterial_dseg.nii.gz` & `panpipelines-0.9.7/deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-Arterial_dseg.nii.gz`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/deployment/atlas/HARVCORT/HarvardOxford-Cortical_index.txt` & `panpipelines-0.9.7/deployment/atlas/HARVCORT/HarvardOxford-Cortical_index.txt`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/deployment/atlas/HARVCORT/MNI152NLinAsym/HarvardOxford-cort-maxprob-thr25-1mm.nii.gz` & `panpipelines-0.9.7/deployment/atlas/HARVCORT/MNI152NLinAsym/HarvardOxford-cort-maxprob-thr25-1mm.nii.gz`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/deployment/atlas/HARVSUBCORT/MNI152NLinAsym/HarvardOxford-sub-maxprob-thr25-1mm.nii.gz` & `panpipelines-0.9.7/deployment/atlas/HARVSUBCORT/MNI152NLinAsym/HarvardOxford-sub-maxprob-thr25-1mm.nii.gz`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/deployment/atlas/HCPMMP1_FREESURFER/README.md` & `panpipelines-0.9.7/deployment/atlas/HCPMMP1_FREESURFER/README.md`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/deployment/atlas/HCPMMP1_FREESURFER/hcpmmp1_ordered.txt` & `panpipelines-0.9.7/deployment/atlas/HCPMMP1_FREESURFER/hcpmmp1_ordered.txt`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/deployment/atlas/HCPMMP1_FREESURFER/hcpmmp1_original.txt` & `panpipelines-0.9.7/deployment/atlas/HCPMMP1_FREESURFER/hcpmmp1_original.txt`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/deployment/atlas/HCPMMP1_FREESURFER/lh.HCP-MMP1.annot` & `panpipelines-0.9.7/deployment/atlas/HCPMMP1_FREESURFER/lh.HCP-MMP1.annot`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/deployment/atlas/HCPMMP1_FREESURFER/rh.HCP-MMP1.annot` & `panpipelines-0.9.7/deployment/atlas/HCPMMP1_FREESURFER/rh.HCP-MMP1.annot`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/deployment/atlas/JHU/JHU-labels_index.txt` & `panpipelines-0.9.7/deployment/atlas/JHU/JHU-labels_index.txt`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/deployment/atlas/JHU/JHU-tracts_index.txt` & `panpipelines-0.9.7/deployment/atlas/JHU/JHU-tracts_index.txt`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/deployment/atlas/JHU/MNI152NLinAsym/JHU-ICBM-labels-1mm.nii.gz` & `panpipelines-0.9.7/deployment/atlas/JHU/MNI152NLinAsym/JHU-ICBM-labels-1mm.nii.gz`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/deployment/atlas/JHU/MNI152NLinAsym/JHU-ICBM-tracts-maxprob-thr25-1mm.nii.gz` & `panpipelines-0.9.7/deployment/atlas/JHU/MNI152NLinAsym/JHU-ICBM-tracts-maxprob-thr25-1mm.nii.gz`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/deployment/atlas/XTRACT/README.md` & `panpipelines-0.9.7/deployment/atlas/XTRACT/README.md`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/deployment/atlas/XTRACT/XTRACT_index.txt` & `panpipelines-0.9.7/deployment/atlas/XTRACT/XTRACT_index.txt`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/deployment/atlas/XTRACT/res-01_atlas-XTRACT_dseg.txt` & `panpipelines-0.9.7/deployment/atlas/XTRACT/res-01_atlas-XTRACT_dseg.txt`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/deployment/atlas/XTRACT/res-02_atlas-XTRACT_dseg.txt` & `panpipelines-0.9.7/deployment/atlas/XTRACT/res-02_atlas-XTRACT_dseg.txt`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/deployment/atlas/XTRACT/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-XTRACT_dseg.json` & `panpipelines-0.9.7/deployment/atlas/XTRACT/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-XTRACT_dseg.json`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/deployment/atlas/XTRACT/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-XTRACT_dseg.nii.gz` & `panpipelines-0.9.7/deployment/atlas/XTRACT/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-XTRACT_dseg.nii.gz`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/deployment/atlas/XTRACT/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-XTRACT_dseg.json` & `panpipelines-0.9.7/deployment/atlas/XTRACT/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-XTRACT_dseg.json`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/deployment/atlas/XTRACT/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-XTRACT_dseg.nii.gz` & `panpipelines-0.9.7/deployment/atlas/XTRACT/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-XTRACT_dseg.nii.gz`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/deployment/atlas/XTRACT/MNI152NLin6Asym/xtract-tract-atlases-maxprob5-1mm.nii.gz` & `panpipelines-0.9.7/deployment/atlas/XTRACT/MNI152NLin6Asym/xtract-tract-atlases-maxprob5-1mm.nii.gz`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/deployment/atlas/freesurfer_atlas/FreeSurferColorLUT.txt` & `panpipelines-0.9.7/deployment/atlas/freesurfer_atlas/FreeSurferColorLUT.txt`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/deployment/atlas/freesurfer_atlas/fs_a2009s.txt` & `panpipelines-0.9.7/deployment/atlas/freesurfer_atlas/fs_a2009s.txt`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/deployment/atlas/freesurfer_atlas/fs_default.txt` & `panpipelines-0.9.7/deployment/atlas/freesurfer_atlas/fs_default.txt`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/deployment/atlas/hcpmmp1_subfields_atlas/hcpmmp1_subfields_ordered.txt` & `panpipelines-0.9.7/deployment/atlas/hcpmmp1_subfields_atlas/hcpmmp1_subfields_ordered.txt`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/deployment/atlas/hcpmmp1_subfields_atlas/hcpmmp1_subfields_original.txt` & `panpipelines-0.9.7/deployment/atlas/hcpmmp1_subfields_atlas/hcpmmp1_subfields_original.txt`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/deployment/batch_scripts/group_template.pbs` & `panpipelines-0.9.7/deployment/batch_scripts/group_template.pbs`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/deployment/batch_scripts/participant_template.pbs` & `panpipelines-0.9.7/deployment/batch_scripts/participant_template.pbs`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/deployment/config/panpipeconfig_expanded_slurm.config` & `panpipelines-0.9.7/deployment/config/panpipeconfig_expanded_slurm.config`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/deployment/config/panpipeconfig_slurm.config` & `panpipelines-0.9.7/deployment/config/panpipeconfig_slurm.config`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/example/config/panpipeconfig_example.config` & `panpipelines-0.9.7/example/config/panpipeconfig_example.config`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/src/panpipelines/Factory.py` & `panpipelines-0.9.7/src/panpipelines/Factory.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/src/panpipelines/group_subjects.py` & `panpipelines-0.9.7/src/panpipelines/group_subjects.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/src/panpipelines/pan_processing.py` & `panpipelines-0.9.7/src/panpipelines/pan_processing.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/src/panpipelines/single_subject.py` & `panpipelines-0.9.7/src/panpipelines/single_subject.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/src/panpipelines/nodes/antstransform.py` & `panpipelines-0.9.7/src/panpipelines/nodes/antstransform.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/src/panpipelines/nodes/aslprep.py` & `panpipelines-0.9.7/src/panpipelines/nodes/aslprep.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/src/panpipelines/nodes/atlascreate.py` & `panpipelines-0.9.7/src/panpipelines/nodes/atlascreate.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/src/panpipelines/nodes/basil.py` & `panpipelines-0.9.7/src/panpipelines/nodes/basil.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/src/panpipelines/nodes/collate_csv_group.py` & `panpipelines-0.9.7/src/panpipelines/nodes/collate_csv_group.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/src/panpipelines/nodes/collate_csv_single.py` & `panpipelines-0.9.7/src/panpipelines/nodes/collate_csv_single.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/src/panpipelines/nodes/dummy.py` & `panpipelines-0.9.7/src/panpipelines/nodes/dummy.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/src/panpipelines/nodes/fmriprep.py` & `panpipelines-0.9.7/src/panpipelines/nodes/fmriprep.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/src/panpipelines/nodes/freesurfer.py` & `panpipelines-0.9.7/src/panpipelines/nodes/freesurfer.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/src/panpipelines/nodes/fslanat.py` & `panpipelines-0.9.7/src/panpipelines/nodes/fslanat.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/src/panpipelines/nodes/glm_randomize_group.py` & `panpipelines-0.9.7/src/panpipelines/nodes/glm_randomize_group.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/src/panpipelines/nodes/lst.py` & `panpipelines-0.9.7/src/panpipelines/nodes/lst.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/src/panpipelines/nodes/noddi.py` & `panpipelines-0.9.7/src/panpipelines/nodes/noddi.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/src/panpipelines/nodes/parse_textdata.py` & `panpipelines-0.9.7/src/panpipelines/nodes/parse_textdata.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/src/panpipelines/nodes/qsiprep.py` & `panpipelines-0.9.7/src/panpipelines/nodes/qsiprep.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/src/panpipelines/nodes/roi_extract.py` & `panpipelines-0.9.7/src/panpipelines/nodes/roi_extract.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,22 +14,31 @@
 from nipype import logging as nlogging
 from nilearn.maskers import NiftiLabelsMasker
 from nilearn.maskers import NiftiMapsMasker
 from nilearn import image
 
 IFLOGGER=nlogging.getLogger('nipype.interface')
 
-def roi_extract_proc(labels_dict,input_file,atlas_file,atlas_index):
+def roi_extract_proc(labels_dict,input_file,atlas_file,atlas_index, lesion_file):
 
     metadata_comments=""
     cwd=os.getcwd()
     labels_dict = updateParams(labels_dict,"CWD",cwd)
     output_dir=cwd
     participant_label = getParams(labels_dict,'PARTICIPANT_LABEL')
     session_label = getParams(labels_dict,'PARTICIPANT_SESSION')
+
+    lesion_inverse_img = None
+    if lesion_file and not lesion_file == ".": 
+        lesion_img = nib.load(lesion_file)
+        lesion_data = lesion_img.get_fdata()
+        inverse_data = np.zeros(lesion_data.shape)
+        inverse_data[lesion_data < 1] = 1 
+        lesion_inverse_img=nib.Nifti1Image(inverse_data, lesion_img.affine)
+
     
     if not session_label:
         roi_output_dir = os.path.join(cwd,f"sub-{participant_label}_roi_output_dir")
     else:
         roi_output_dir = os.path.join(cwd,f"sub-{participant_label}_ses-{session_label}_roi_output_dir")
 
     if not os.path.isdir(roi_output_dir):
@@ -51,14 +60,23 @@
             os.makedirs(mgzdir)
 
         fs_command_base, fscontainer = getContainer(labels_dict,nodename="convMGZ2NII",SPECIFIC="FREESURFER_CONTAINER",LOGGER=IFLOGGER)
         input_file_nii = newfile(mgzdir,input_file,extension=".nii.gz")
         convMGZ2NII(input_file, input_file_nii, fs_command_base)
         input_file = input_file_nii
 
+    if Path(lesion_file).suffix == ".mgz":
+        mgzdir = os.path.join(cwd,'mgz_nii')
+        if not os.path.isdir(mgzdir):
+            os.makedirs(mgzdir)
+
+        fs_command_base, fscontainer = getContainer(labels_dict,nodename="convMGZ2NII",SPECIFIC="FREESURFER_CONTAINER",LOGGER=IFLOGGER)
+        lesion_file_nii = newfile(mgzdir,lesion_file,extension=".nii.gz")
+        convMGZ2NII(lesion_file, lesion_file_nii, fs_command_base)
+        lesion_file = lesion_file_nii
 
     atlas_type="3D"
     atlas_img  = nib.load(atlas_file)
     atlas_dim = 1
     atlas_shape = atlas_img.header.get_data_shape()
     if len(atlas_shape) > 3:
         if atlas_shape[3]> 1:
@@ -105,25 +123,41 @@
     measure_data = measure_img.get_fdata()
     measure_shape = measure_img.header.get_data_shape()
     if len(measure_shape) > 3:
         if measure_shape[3] > 1:
             measure_type = "4D"
 
     if atlas_type == "4D":
-        NiftiMasker = NiftiMapsMasker(
-            atlas_img,
-            Labels = labels_name_list,
-            standardize=False
-        )
+        if lesion_inverse_img:
+            NiftiMasker = NiftiMapsMasker(
+                atlas_img,
+                mask_img = lesion_inverse_img,
+                Labels = labels_name_list,
+                standardize=False
+            )
+        else:
+            NiftiMasker = NiftiMapsMasker(
+                atlas_img,
+                Labels = labels_name_list,
+                standardize=False
+            )
     else:
-        NiftiMasker = NiftiLabelsMasker(
-            atlas_img,
-            Labels = labels_name_list,
-            standardize=False
-        )
+        if lesion_inverse_img:
+            NiftiMasker = NiftiLabelsMasker(
+                atlas_img,
+                mask_img = lesion_inverse_img,
+                Labels = labels_name_list,
+                standardize=False
+            )
+        else:
+            NiftiMasker = NiftiLabelsMasker(
+                atlas_img,
+                Labels = labels_name_list,
+                standardize=False
+            )
 
     NiftiMasker.fit(input_file)
     signals = NiftiMasker.transform(input_file)
     num_rows = signals.shape[0]
 
     # check that rois exist:
     missing_rois = []
@@ -307,14 +341,15 @@
 
 
 class roi_extractInputSpec(BaseInterfaceInputSpec):
     labels_dict = traits.Dict({},mandatory=False,desc='labels', usedefault=True)
     input_file = File(desc="input file")
     atlas_file = File(desc='atlas file')
     atlas_index = File(desc='atlas index file')
+    lesion_file = File(desc='lesion file')
 
 class roi_extractOutputSpec(TraitedSpec):
     roi_csv = File(desc='CSV file of results')
     roi_output_dir = traits.String(desc='roi output dir')
     output_dir = traits.String(desc='output dir')
     out_files = traits.List(desc='list of files')
     
@@ -326,33 +361,35 @@
 
         # Call our python code here:
         outputs = roi_extract_proc(
             self.inputs.labels_dict,
             self.inputs.input_file,
             self.inputs.atlas_file,
             self.inputs.atlas_index,
+            self.inputs.lesion_file,
         )
 
         setattr(self, "_results", outputs)
         # And we are done
         return runtime
 
     def _list_outputs(self):
         return self._results
 
 
-def create(labels_dict,name="roi_extract_node",input_file="",atlas_file="",atlas_index="", LOGGER=IFLOGGER):
+def create(labels_dict,name="roi_extract_node",input_file="",atlas_file="",atlas_index="", lesion_file="", LOGGER=IFLOGGER):
     # Create Node
     pan_node = Node(roi_extract_pan(), name=name)
 
     if LOGGER:
         LOGGER.info(f"Created Node {pan_node!r}")
         
     # Specify node inputs
     pan_node.inputs.labels_dict = labels_dict
     pan_node.inputs.input_file = input_file
     pan_node.inputs.atlas_file =  atlas_file
     pan_node.inputs.atlas_index =  atlas_index
+    pan_node.inputs.lesion_file =  lesion_file
 
     return pan_node
```

### Comparing `panpipelines-0.9.6/src/panpipelines/nodes/roi_mean_group.py` & `panpipelines-0.9.7/src/panpipelines/nodes/roi_mean_group.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/src/panpipelines/nodes/roi_mean_single.py` & `panpipelines-0.9.7/src/panpipelines/nodes/roi_mean_single.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/src/panpipelines/nodes/tensor.py` & `panpipelines-0.9.7/src/panpipelines/nodes/tensor.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/src/panpipelines/pipelines/aslprep_panpipeline.py` & `panpipelines-0.9.7/src/panpipelines/pipelines/aslprep_panpipeline.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/src/panpipelines/pipelines/basil_panpipeline.py` & `panpipelines-0.9.7/src/panpipelines/pipelines/basil_panpipeline.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/src/panpipelines/pipelines/collatecsv_panpipeline.py` & `panpipelines-0.9.7/src/panpipelines/pipelines/collatecsv_panpipeline.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/src/panpipelines/pipelines/collatecsvgroup_panpipeline.py` & `panpipelines-0.9.7/src/panpipelines/pipelines/collatecsvgroup_panpipeline.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/src/panpipelines/pipelines/dummy_panpipeline.py` & `panpipelines-0.9.7/src/panpipelines/pipelines/dummy_panpipeline.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/src/panpipelines/pipelines/fmriprep_panpipeline.py` & `panpipelines-0.9.7/src/panpipelines/pipelines/fmriprep_panpipeline.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/src/panpipelines/pipelines/freesurfer_panpipeline.py` & `panpipelines-0.9.7/src/panpipelines/pipelines/freesurfer_panpipeline.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/src/panpipelines/pipelines/lst_panpipeline.py` & `panpipelines-0.9.7/src/panpipelines/pipelines/lst_panpipeline.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/src/panpipelines/pipelines/noddi_panpipeline.py` & `panpipelines-0.9.7/src/panpipelines/pipelines/noddi_panpipeline.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/src/panpipelines/pipelines/panpipeline.py` & `panpipelines-0.9.7/src/panpipelines/pipelines/panpipeline.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/src/panpipelines/pipelines/qsiprep_panpipeline.py` & `panpipelines-0.9.7/src/panpipelines/pipelines/qsiprep_panpipeline.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/src/panpipelines/pipelines/roiextract_panpipeline.py` & `panpipelines-0.9.7/src/panpipelines/pipelines/roiextract_panpipeline.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/src/panpipelines/pipelines/tensor_panpipeline.py` & `panpipelines-0.9.7/src/panpipelines/pipelines/tensor_panpipeline.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/src/panpipelines/pipelines/textmeasures_panpipeline.py` & `panpipelines-0.9.7/src/panpipelines/pipelines/textmeasures_panpipeline.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/src/panpipelines/pipelines/volmeasures_panpipeline.py` & `panpipelines-0.9.7/src/panpipelines/pipelines/volmeasures_panpipeline.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/src/panpipelines/scripts/aslprep_panscript.py` & `panpipelines-0.9.7/src/panpipelines/scripts/aslprep_panscript.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/src/panpipelines/scripts/fmriprep_panscript.py` & `panpipelines-0.9.7/src/panpipelines/scripts/fmriprep_panscript.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/src/panpipelines/scripts/pancontainer_panscript.py` & `panpipelines-0.9.7/src/panpipelines/scripts/pancontainer_panscript.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/src/panpipelines/scripts/panscript.py` & `panpipelines-0.9.7/src/panpipelines/scripts/panscript.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/src/panpipelines/scripts/sdcflows_fieldmap.py` & `panpipelines-0.9.7/src/panpipelines/scripts/sdcflows_fieldmap.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/src/panpipelines/utils/transformer.py` & `panpipelines-0.9.7/src/panpipelines/utils/transformer.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/src/panpipelines/utils/util_functions.py` & `panpipelines-0.9.7/src/panpipelines/utils/util_functions.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/src/panpipelines/workflows/aslprep_workflow.py` & `panpipelines-0.9.7/src/panpipelines/workflows/aslprep_workflow.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/src/panpipelines/workflows/basil_workflow.py` & `panpipelines-0.9.7/src/panpipelines/workflows/basil_workflow.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/src/panpipelines/workflows/collatecsv_workflow.py` & `panpipelines-0.9.7/src/panpipelines/workflows/collatecsv_workflow.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/src/panpipelines/workflows/collatecsvgroup_workflow.py` & `panpipelines-0.9.7/src/panpipelines/workflows/collatecsvgroup_workflow.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/src/panpipelines/workflows/dummy_workflow.py` & `panpipelines-0.9.7/src/panpipelines/workflows/dummy_workflow.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/src/panpipelines/workflows/fmriprep_workflow.py` & `panpipelines-0.9.7/src/panpipelines/workflows/fmriprep_workflow.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/src/panpipelines/workflows/freesurfer_workflow.py` & `panpipelines-0.9.7/src/panpipelines/workflows/freesurfer_workflow.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/src/panpipelines/workflows/lst_workflow.py` & `panpipelines-0.9.7/src/panpipelines/workflows/lst_workflow.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/src/panpipelines/workflows/noddi_workflow.py` & `panpipelines-0.9.7/src/panpipelines/workflows/noddi_workflow.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/src/panpipelines/workflows/qsiprep_workflow.py` & `panpipelines-0.9.7/src/panpipelines/workflows/qsiprep_workflow.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/src/panpipelines/workflows/roiextract_workflow.py` & `panpipelines-0.9.7/src/panpipelines/workflows/volmeasures_workflow.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from nipype import Workflow, MapNode, Node
 
 import panpipelines.nodes.antstransform as antstransform
 import panpipelines.nodes.atlascreate as atlascreate
-import panpipelines.nodes.roi_extract as roiextract
+import panpipelines.nodes.roi_mean_single as roimean
 from panpipelines.utils.util_functions import *
 from panpipelines.utils.transformer import *
 import glob
 
 def create(name, wf_base_dir,labels_dict,createGraph=True,execution={},LOGGER=None):
     # Create workflow
     pan_workflow = Workflow(name=name, base_dir=wf_base_dir)
@@ -35,15 +35,15 @@
                     newatlas_list.extend(glob.glob(evaluated_newatlas_template))
         else:
             newatlas_list.extend(glob.glob(newatlas_templates))
             
         labels_dict = updateParams(labels_dict,"COST_FUNCTION","NearestNeighbor")
         atlascreate_node = atlascreate.create(labels_dict,name=f"atlascreate_{atlas_name}_node",roi_list=newatlas_list,roilabels_list=newatlas_index,LOGGER=LOGGER)
 
-    roimean_node = roiextract.create(labels_dict,name="subject_metrics",LOGGER=LOGGER)
+    roimean_node = roimean.create(labels_dict,name="subject_metrics",LOGGER=LOGGER)
     roimean_map_node = MapNode(roimean_node.interface,name="subject_metrics_map",iterfield=['input_file'])
 
     if atlascreate_node:
         pan_workflow.connect(atlascreate_node,'atlas_index',roimean_map_node,'atlas_index')
     else:
         roimean_map_node.inputs.atlas_index = atlas_index
 
@@ -77,14 +77,15 @@
         
     measures_list.sort()
 
     # should we transform measures?
     measures_transform_mat=getParams(labels_dict,"MEASURES_TRANSFORM_MAT")
     measures_transform_ref=getParams(labels_dict,"MEASURES_TRANSFORM_REF")
     if measures_transform_mat is not None:
+        # go back to default cost function lancsoz
         labels_dict = removeParam(labels_dict,"COST_FUNCTION")
         labels_dict = removeParam(labels_dict,"OUTPUT_TYPE")
         measures_transform_node = antstransform.create(labels_dict,name="measure_transform",trans_mat=measures_transform_mat,ref_file=measures_transform_ref,LOGGER=LOGGER)
         measures_transform_map_node = MapNode(measures_transform_node.interface,name="measure_transform_map",iterfield=['input_file'])
         measures_transform_map_node.inputs.input_file = measures_list
         pan_workflow.connect(measures_transform_map_node,'out_file',roimean_map_node,'input_file')
```

### Comparing `panpipelines-0.9.6/src/panpipelines/workflows/tensor_workflow.py` & `panpipelines-0.9.7/src/panpipelines/workflows/tensor_workflow.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/src/panpipelines/workflows/textmeasures_workflow.py` & `panpipelines-0.9.7/src/panpipelines/workflows/textmeasures_workflow.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/src/panpipelines/workflows/volmeasures_workflow.py` & `panpipelines-0.9.7/src/panpipelines/workflows/roiextract_workflow.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,49 +1,96 @@
 from nipype import Workflow, MapNode, Node
 
 import panpipelines.nodes.antstransform as antstransform
 import panpipelines.nodes.atlascreate as atlascreate
-import panpipelines.nodes.roi_mean_single as roimean
+import panpipelines.nodes.roi_extract as roiextract
 from panpipelines.utils.util_functions import *
 from panpipelines.utils.transformer import *
 import glob
 
 def create(name, wf_base_dir,labels_dict,createGraph=True,execution={},LOGGER=None):
     # Create workflow
     pan_workflow = Workflow(name=name, base_dir=wf_base_dir)
 
     if LOGGER:
         LOGGER.info(f"Created Workflow {name} with base directory {wf_base_dir}")
 
     if len(execution.keys()) > 0:
         pan_workflow.config = process_dict(pan_workflow.config,execution)
 
+    # do we have  a lesion to exclude?
+    lesioncreate_node = None
+    lesion_templates = getParams(labels_dict,"LESION_TEMPLATE")
+    if lesion_templates:
+        lesion_list=[]
+        lesion_name = getParams(labels_dict,"LESION_NAME")
+        if not lesion_name:
+            lesion_name="lesion"
+        lesion_index = getParams(labels_dict,"LESION_INDEX")
+        if isinstance(lesion_templates,list):
+            for lesion_template in lesion_templates:
+                evaluated_lesion_template = substitute_labels(lesion_template,labels_dict)
+                if "*" not in evaluated_lesion_template:
+                    lesion_list.append(evaluated_lesion_template)
+                else:
+                    lesion_list.extend(glob.glob(evaluated_lesion_template))
+        else:
+            lesion_list.extend(glob.glob(lesion_templates))
+
+        # if lesion template is invalid then continue, otherwise print message and continue without
+        # using lesion segmenntation
+        LESION_TEMPLATE_EXISTS=True
+        for lesion in lesion_list:
+            if not os.path.exists(lesion):
+                LESION_TEMPLATE_EXISTS = False
+
+        if lesion_list and LESION_TEMPLATE_EXISTS:    
+            # store and restore parameters used by both lesion and newatlas
+            newatlas_transform_mat = getParams(labels_dict,"NEWATLAS_TRANSFORM_MAT")
+            newatlas_transform_ref = getParams(labels_dict,"NEWATLAS_TRANSFORM_REF")
+            lesion_transform_mat = getParams(labels_dict,"LESION_TRANSFORM_MAT")
+            lesion_transform_ref = getParams(labels_dict,"LESION_TRANSFORM_REF")
+
+            labels_dict = updateParams(labels_dict,"NEWATLAS_TRANSFORM_MAT",lesion_transform_mat)
+            labels_dict = updateParams(labels_dict,"NEWATLAS_TRANSFORM_REF",lesion_transform_ref)
+
+            labels_dict = updateParams(labels_dict,"COST_FUNCTION","NearestNeighbor")
+            lesioncreate_node = atlascreate.create(labels_dict,name=f"lesioncreate_{lesion_name}_node",roi_list=lesion_list,roilabels_list=lesion_index,LOGGER=LOGGER)
+
+            labels_dict = updateParams(labels_dict,"NEWATLAS_TRANSFORM_MAT",newatlas_transform_mat)
+            labels_dict = updateParams(labels_dict,"NEWATLAS_TRANSFORM_REF",newatlas_transform_ref)
+        else:
+            if LOGGER:
+                LOGGER.info(f"Lesion Template defined but valid template file not found. Ignoring Lesion Template.")
+
     # do we need to create a custom atlas?
     atlas_index = getParams(labels_dict,"ATLAS_INDEX")
     atlas_file = getParams(labels_dict,"ATLAS_FILE")
     atlas_name = getParams(labels_dict,"ATLAS_NAME")
     atlascreate_node=None
     if not atlas_file:
         newatlas_list=[]
         newatlas_templates = getParams(labels_dict,"NEWATLAS_TEMPLATE")
         newatlas_index = getParams(labels_dict,"NEWATLAS_INDEX")
+        if not atlas_name:
+            atlas_name = getParams(labels_dict,"NEWATLAS_NAME")
         if isinstance(newatlas_templates,list):
             for newatlas_template in newatlas_templates:
                 evaluated_newatlas_template = substitute_labels(newatlas_template,labels_dict)
                 if "*" not in evaluated_newatlas_template:
                     newatlas_list.append(evaluated_newatlas_template)
                 else:
                     newatlas_list.extend(glob.glob(evaluated_newatlas_template))
         else:
             newatlas_list.extend(glob.glob(newatlas_templates))
             
         labels_dict = updateParams(labels_dict,"COST_FUNCTION","NearestNeighbor")
         atlascreate_node = atlascreate.create(labels_dict,name=f"atlascreate_{atlas_name}_node",roi_list=newatlas_list,roilabels_list=newatlas_index,LOGGER=LOGGER)
 
-    roimean_node = roimean.create(labels_dict,name="subject_metrics",LOGGER=LOGGER)
+    roimean_node = roiextract.create(labels_dict,name="subject_metrics",LOGGER=LOGGER)
     roimean_map_node = MapNode(roimean_node.interface,name="subject_metrics_map",iterfield=['input_file'])
 
     if atlascreate_node:
         pan_workflow.connect(atlascreate_node,'atlas_index',roimean_map_node,'atlas_index')
     else:
         roimean_map_node.inputs.atlas_index = atlas_index
 
@@ -77,24 +124,27 @@
         
     measures_list.sort()
 
     # should we transform measures?
     measures_transform_mat=getParams(labels_dict,"MEASURES_TRANSFORM_MAT")
     measures_transform_ref=getParams(labels_dict,"MEASURES_TRANSFORM_REF")
     if measures_transform_mat is not None:
-        # go back to default cost function lancsoz
         labels_dict = removeParam(labels_dict,"COST_FUNCTION")
         labels_dict = removeParam(labels_dict,"OUTPUT_TYPE")
         measures_transform_node = antstransform.create(labels_dict,name="measure_transform",trans_mat=measures_transform_mat,ref_file=measures_transform_ref,LOGGER=LOGGER)
         measures_transform_map_node = MapNode(measures_transform_node.interface,name="measure_transform_map",iterfield=['input_file'])
         measures_transform_map_node.inputs.input_file = measures_list
         pan_workflow.connect(measures_transform_map_node,'out_file',roimean_map_node,'input_file')
             
     else:
         roimean_map_node.inputs.input_file = measures_list
 
 
+    if lesioncreate_node:
+        pan_workflow.connect(lesioncreate_node,'atlas_file',roimean_map_node,'lesion_file')
+
+
     if createGraph:
          pan_workflow.write_graph(graph2use='flat')
 
 
     return pan_workflow
```

### Comparing `panpipelines-0.9.6/.gitignore` & `panpipelines-0.9.7/.gitignore`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/LICENSE` & `panpipelines-0.9.7/LICENSE`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/README.md` & `panpipelines-0.9.7/README.md`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.6/pyproject.toml` & `panpipelines-0.9.7/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -31,13 +31,14 @@
   "pandas==2.1.4",
   "xnat==0.5.3",
   "pydicom==2.4.4",
   "templateflow==23.1.0",
   "nitransforms==23.0.1",
   "pybids==0.16.4",
   "scipy==1.11.4",
-  "sdcflows==2.8.0"
+  "sdcflows==2.8.0",
+  "mne[hdf]==1.1.0"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/MRIresearch/PANpipelines"
 "Bug Tracker" = "https://github.com/MRIresearch/PANpipelines/issues"
```

### Comparing `panpipelines-0.9.6/PKG-INFO` & `panpipelines-0.9.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: panpipelines
-Version: 0.9.6
+Version: 0.9.7
 Summary: MRI Processing Pipelines for PAN Healthy Minds for Life Study
 Project-URL: Homepage, https://github.com/MRIresearch/PANpipelines
 Project-URL: Bug Tracker, https://github.com/MRIresearch/PANpipelines/issues
 Author-email: Chidi Ugonna <chidiugonna@arizona.edu>
 License: MIT License
         
         Copyright (c) 2023 MRIresearch
@@ -27,14 +27,15 @@
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
+Requires-Dist: mne[hdf]==1.1.0
 Requires-Dist: nibabel==5.2.0
 Requires-Dist: nilearn==0.10.2
 Requires-Dist: nipype==1.8.6
 Requires-Dist: nitransforms==23.0.1
 Requires-Dist: numpy==1.26.3
 Requires-Dist: pandas==2.1.4
 Requires-Dist: pybids==0.16.4
```

