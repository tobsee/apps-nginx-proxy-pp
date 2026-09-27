# https://developers.home-assistant.io/docs/apps/configuration#app-dockerfile
ARG BUILD_FROM=ghcr.io/home-assistant/base:3.23
FROM ${BUILD_FROM}

# Setup base
RUN apk add --no-cache nginx openssl

# Copy data
COPY rootfs /

WORKDIR /

LABEL \
    org.opencontainers.image.title="Home Assistant App: NGINX SSL Proxy (Proxy Protocol)" \
    org.opencontainers.image.description="An SSL/TLS proxy with optional separate proxy protocol port" \
    org.opencontainers.image.source="https://github.com/tobsee/apps-nginx-proxy-pp" \
    org.opencontainers.image.licenses="Apache License 2.0"
