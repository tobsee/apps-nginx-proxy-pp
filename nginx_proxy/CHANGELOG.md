# Changelog

## 0.1.0

- Renamed from "add-on" to "app" and moved repository to `tobsee/apps-nginx-proxy-pp`
- Updated to Alpine 3.23 base image (build config moved from `build.yaml` into the Dockerfile)
- Dropped deprecated `armhf`, `armv7` and `i386` architectures

## 0.0.3

- Add mutual TLS (mTLS) support for client certificate verification
- Add `mtls` and `client_certfile` configuration options
- Add startup validation for mTLS configuration

## 0.0.2

- Add port validation and fix documentation for split proxy protocol

## 0.01

- Add possibility to split https and tcp traffic
