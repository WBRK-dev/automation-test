# We'll just use the official Rust image rather than build our own from scratch
FROM docker.io/library/rust:1.54.0-slim-bullseye

ENV KEYRINGS /usr/local/share/keyrings

ENV CARGO_BIN /usr/local/cargo/bin

COPY build /usr/local/bin/build
COPY upload /usr/local/bin/upload

# RUN chmod -R 777 /usr/local/bin/build_env

# ENTRYPOINT [ "/usr/local/bin/build_env" ]

RUN set -eux; \
    chmod -R 777 /usr/local/bin/build; \
    chmod -R 777 /usr/local/bin/upload; \
    /usr/local/bin/build; \
    /usr/local/bin/upload;