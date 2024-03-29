# RedPajama model inference with Huggingface API2

## Overview

[RedPajama-INCITE-Instruct-3B-v1](https://huggingface.co/togethercomputer/RedPajama-INCITE-Instruct-3B-v1) was developed by Together and leaders from the open-source AI community.

## Model inference

### Create and run a Notebook server

The dependencies have integrated into the below docker image, you can directly use an image published on VMware harbor repo:

```bash
projects.registry.vmware.com/models/notebook/hf-inference-deploy:v1
```

Start the Notebook server with GPU:

```bash
docker run --gpus all -it -v `pwd`:/mnt projects.registry.vmware.com/models/notebook/hf-inference-deploy:v1
```

### GPU Inference

This requires a GPU with 8GB memory.

```bash
python3 redpajama-inference.py
```
