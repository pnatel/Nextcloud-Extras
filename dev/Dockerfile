ARG BASE_IMAGE

FROM $BASE_IMAGE

LABEL org.opencontainers.image.authors="https://github.com/pnatel"

EXPOSE 80:80/tcp

# Extra packages for apps
RUN apt-get update \
    # Memories and Recognize
    && apt-get -y install imagemagick ffmpeg \
    # Extract
    && apt-get -y install unrar-free p7zip p7zip-full

# Support for Storj External Storage (https://apps.nextcloud.com/apps/storj)
RUN apt install -y libffi-dev && docker-php-ext-install ffi
RUN echo ffi.enable=true > /usr/local/etc/php/conf.d/ffi.ini