FROM $BASE_IMAGE

LABEL org.opencontainers.image.authors="https://github.com/pnatel"

EXPOSE 80:80/tcp

# Extra packages for apps
RUN apt-get update \
    # Memories and Recognize
    && apt-get -y install imagemagick ffmpeg \
    # Extract
    && apt-get -y install unrar-free p7zip p7zip-full
