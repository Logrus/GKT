FROM ubuntu:jammy

# Install python and all standard stuff

RUN apt-get update && apt-get install -y \
    ffmpeg \
    libsm6 \
    libxext6 \
    python3 \
    python3-pip \
    git \
    curl \
    wget \
    unzip \
    vim \
    && rm -rf /var/lib/apt/lists/*

COPY segmentation/requirements.txt /tmp/
RUN pip install -r /tmp/requirements.txt
