FROM mcr.microsoft.com/vscode/devcontainers/base:ubuntu-20.04

RUN apt-get update && apt-get install -y \
    python3 \
    python3-pip \
    libgl1-mesa-dev xorg-dev \
    python3-tk \
    && mkdir -p /home/vscode/.local/lib/python3.8/site-packages /home/vscode/.local-insiders \
    && chown -R vscode:vscode /home/vscode/.local /home/vscode/.local-insiders \
    && ln -s /home/vscode/.local/lib/python3.8/site-packages /home/vscode/.local/lib/python3.8/site-packages

ENV DISPLAY host.docker.internal:0.0
