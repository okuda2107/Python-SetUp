FROM mcr.microsoft.com/vscode/devcontainers/base:ubuntu-20.04

RUN apt-get update && apt-get install -y \
    python3 \
    python3-pip \
    libgl1-mesa-dev xorg-dev \
    python3-tk

RUN pip install numpy matplotlib

ENV DISPLAY host.docker.internal:0.0
