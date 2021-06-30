FROM rust:buster
RUN apt update;\
	apt install -y musl-dev;\
	cargo install cargo-chef --version 0.1.21;\
	apt remove -y musl-dev;\
	apt -y clean;\
	rm -rf $CARGO_HOME/registry/;\
	cargo-chef --version;