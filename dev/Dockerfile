# ARG BASE_IMAGE

# FROM $BASE_IMAGE

# LABEL org.opencontainers.image.authors="https://github.com/pnatel"

# EXPOSE 80/tcp

# # Extra packages for apps
# RUN apt-get update \
#     # Memories and Recognize
#     && apt-get -y install imagemagick ffmpeg \
#     # Extract
#     && apt-get -y install unrar-free p7zip p7zip-full


ARG BASE_IMAGE=nextcloud:apache
FROM ${BASE_IMAGE}

# Optimize apt behaviour for low-memory / CI emulation environments
ENV DEBIAN_FRONTEND=noninteractive \
    APT_LISTBUGS_DISABLE=true \
    APT_LISTCHANGES_DISABLE=true

RUN apt-get update && \
    # 1. Force apt to use minimal memory by disabling index and package caching
    apt-get install -y -q --no-install-recommends \
        -o APT::Keep-Downloaded-Packages="false" \
        -o Dir::Cache::Archives="none" \
        -o Dir::Cache="none" \
        # 2. Target specific multimedia packages explicitly 
        ffmpeg \
        imagemagick \
        libmagickwand-dev && \
    # 3. Aggressively purge APT listings immediately in the same layer
    rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
