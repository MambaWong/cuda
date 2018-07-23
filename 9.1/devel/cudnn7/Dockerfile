ARG repository
FROM ${repository}:9.1-devel-ubuntu16.04
LABEL maintainer "NVIDIA CORPORATION <cudatools@nvidia.com>"

ENV CUDNN_VERSION 7.1.2.21
LABEL com.nvidia.cudnn.version="${CUDNN_VERSION}"

RUN apt-get update && apt-get install -y --allow-downgrades --no-install-recommends \ 
    libcudnn7=7.0.5.15-1+cuda9.1 \
    libcudnn7-dev=7.0.5.15-1+cuda9.1 && \
    rm -rf /var/lib/apt/lists/*
