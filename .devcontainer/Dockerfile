FROM mcr.microsoft.com/devcontainers/base:alpine-3.19
# Install the elixir package, the Hex package manager, and phoenix framework
RUN apk update \
    && apk add elixir \
    && mix local.hex \
    && echo y | mix archive.install hex phx_new
