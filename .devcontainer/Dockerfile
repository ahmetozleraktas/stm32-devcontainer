# Use an official Ubuntu image as a base
FROM ubuntu:20.04

# Install required packages
RUN apt-get update && apt-get install -y \
    build-essential \
    cmake \
    openocd \
    gcc-arm-none-eabi \
    stlink-tools \
    gdb-multiarch \
    git \
    python3 \
    python3-pip \
    && rm -rf /var/lib/apt/lists/*

# Create a user for development
RUN useradd -ms /bin/bash vscode
USER vscode
WORKDIR /workspace
