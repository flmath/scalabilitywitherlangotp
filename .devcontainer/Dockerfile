# Base image for development containers
FROM mcr.microsoft.com/devcontainers/base:ubuntu

# Update and install Erlang
RUN apt-get update \
    && apt-get install -y --no-install-recommends \
       erlang \
       build-essential \
       libssl-dev \
       libncurses5-dev \
       unixodbc-dev \
    && apt-get clean \
    && rm -rf /var/lib/apt/lists/*

# Set the default shell to bash (optional)
SHELL ["/bin/bash", "-c"]
