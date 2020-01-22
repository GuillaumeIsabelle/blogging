---
ID: 1595
post_title: Docker  |  TensorFlow | GPU
author: gicomadmin
post_excerpt: ""
layout: post
permalink: >
  http://guillaumeisabelle.com/blogging/2020/01/22/docker-tensorflow-gpu/
published: true
post_date: 2020-01-22 13:58:35
---
> GPU support Docker is the easiest way to run TensorFlow on a GPU since the host machine only requires the NVIDIA® driver (the NVIDIA® CUDA® Toolkit is not required). Install the Nvidia Container Toolkit to add NVIDIA® GPU support to Docker. nvidia-container-runtime is only available for Linux. See the nvidia-container-runtime platform support FAQ for details. Check if a GPU is available: lspci | grep -i nvidia Verify your nvidia-docker installation: docker run --gpus all --rm nvidia/cuda nvidia-smi No Source: *[Docker  |  TensorFlow][1]*

 [1]: https://www.tensorflow.org/install/docker#gpu_support