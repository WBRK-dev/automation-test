# We'll just use the official Rust image rather than build our own from scratch
FROM docker.io/library/rust:1.54.0-slim-bullseye

ENV KEYRINGS /usr/local/share/keyrings

COPY build_env /usr/local/bin/build_env

ENTRYPOINT [ "/usr/local/bin/build_env" ]
