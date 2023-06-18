ARG BUILD_FROM
FROM $BUILD_FROM

WORKDIR /data

# Install requirements for add-on
RUN \
  apk add --no-cache \
    rsync

# Copy root filesystem
COPY rootfs /
