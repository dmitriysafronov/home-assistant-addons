ARG BUILD_FROM
FROM $BUILD_FROM

WORKDIR /data

# Install requirements for add-on
RUN \
  apk add --no-cache \
    rsync

# Copy root filesystem
COPY rootfs/ /

# Change access rights
RUN \
  chmod -c a+x \
    /usr/bin/ssl-refresher \
    /etc/services.d/rsync-ssl/finish \
    /etc/services.d/rsync-ssl/run
