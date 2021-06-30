FROM rust:alpine3.13
RUN set -eux;\
	apk add --no-cache musl-dev;\
	cargo install cargo-chef --version 0.1.21;\
	apk del musl-dev;\
	rm -rf $CARGO_HOME/registry/;\
	cargo-chef --version;