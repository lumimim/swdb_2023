# hash:sha256:2a6f0afb03189c44f91a2265dad3c300692c854c5961aa678c5864a5e798cb49
FROM registry.codeocean.allenneuraldynamics.org/codeocean/miniconda3:4.9.2-cuda11.7.0-cudnn8-ubuntu20.04

ARG DEBIAN_FRONTEND=noninteractive

ARG GIT_ASKPASS
ARG GIT_ACCESS_TOKEN
COPY git-askpass /

RUN conda install -y \
        jupyterlab==3.5.3 \
        matplotlib==3.7.1 \
        numpy==1.24.3 \
        scikit-learn==1.2.2 \
    && conda clean -ya
