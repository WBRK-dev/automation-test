# We'll just use the official Rust image rather than build our own from scratch
FROM docker.io/library/rust:1.54.0-slim-bullseye

ENV KEYRINGS /usr/local/share/keyrings

ENV CARGO_BIN /usr/local/cargo/bin

COPY build_env /usr/local/bin/build_env

# RUN chmod -R 777 /usr/local/bin/build_env

# ENTRYPOINT [ "/usr/local/bin/build_env" ]

RUN set -eux; \
    chmod -R 777 /usr/local/bin/build_env; \
    /usr/local/bin/build_env; 
