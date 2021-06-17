FROM rust:1.52.1-alpine3.13 as builder
RUN set -eux;\
	apk add --no-cache musl-dev;\
	cargo install cargo-chef --version 0.1.21;\
	apk del musl-dev;\
	cargo-chef --version;