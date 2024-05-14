# We'll just use the official Rust image rather than build our own from scratch
FROM docker.io/library/rust:1.54.0-slim-bullseye

ENV KEYRINGS /usr/local/share/keyrings

ENV CARGO_BIN /usr/local/cargo/bin

COPY create_env /usr/local/bin/create_env
COPY build /usr/local/bin/build
COPY upload /usr/local/bin/upload

RUN /usr/local/bin/create_env; \
    /usr/local/bin/build; \
    /usr/local/bin/upload;