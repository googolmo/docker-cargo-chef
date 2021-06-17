FROM rust:alpine3.12 as builder
RUN set -eux;\
	apk add --no-cache musl-dev;\
	cargo install cargo-chef --version 0.1.21;\
	apk del musl-dev;\
	cargo-chef --version;