FROM mcr.microsoft.com/devcontainers/base:jammy
# # Install the xz-utils package
# RUN apt-get update && apt-get install -y xz-utils

# # install vim
# RUN sudo apt update
# RUN apt install vim

# # wget
# WORKDIR ./
# RUN wget https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh

# xv6
WORKDIR ./
RUN apt-get update
RUN apt-get install qemu
RUN apt-get install -y qemu-system
RUN apt-get install -y qemu-user
RUN apt-get install git
RUN git clone https://github.com/mit-pdos/xv6-public.git
WORKDIR xv6-public
RUN make
RUN make clean
# RUN make qemu
# RUN make qemu-nox

# [Quit qemu]
# ctrl+a c
# quit
