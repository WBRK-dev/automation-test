# We'll just use the official Rust image rather than build our own from scratch
FROM docker.io/library/rust:1.54.0-slim-bullseye

ENV KEYRINGS /usr/local/share/keyrings

COPY install /usr/local/bin/install_rust

RUN set -eux; \
    chmod -R 777 /usr/local/bin/install_rust; \
    /usr/local/bin/install_rust; 