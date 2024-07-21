ARG BASE_APP_IMAGE

FROM $(BASE_APP_IMAGE)

ARG DEBIAN_FRONTEND=noninteractive

RUN \
  echo "**** Installing Ubuntu Desktop ****" && \
    apt-get update && \
    apt-get install -y ubuntu-desktop

ENV XDG_RUNTIME_DIR=/tmp/.X11-unix

ARG IMAGE_SOURCE
LABEL org.opencontainers.image.source=$IMAGE_SOURCE
