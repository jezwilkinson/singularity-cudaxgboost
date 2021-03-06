# singularity-cudaxgboost
Singularity container definition for XGBoost/hipe4ml environment

This is a minimal container for running Hipe4ML (https://github.com/hipe4ml/hipe4ml) with XGBoost, including NVidia GPU support with CUDA 11.0. Based on the official CUDA image from NVidia, https://hub.docker.com/r/nvidia/cuda. 

NOTE: If using a GPU method in XGBoost such as "gpu_tree", the container must be run with the --nv switch (e.g. "singularity exec --nv [COMMAND]") in order to access the driver binaries on the host machine.

This environment is also compatible with CPU-only running of Hipe4ML on any host machine, without any additional setup.
