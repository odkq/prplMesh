###############################################################
# SPDX-License-Identifier: BSD-2-Clause-Patent
# SPDX-FileCopyrightText: 2019-2020 the prplMesh contributors (see AUTHORS.md)
# This code is subject to the terms of the BSD+Patent license.
# See LICENSE file for more details.
###############################################################

ARG image=ubuntu:18.04
FROM $image

# Update Software repository
RUN apt-get update && apt-get install -y \
    autoconf \
    autogen \
    binutils \
    clang-format \
    cmake \
    curl \
    gcc \
    gcovr \
    git \
    libjson-c-dev \
    libncurses-dev \
    libnl-genl-3-dev \
    libreadline-dev \
    libssl-dev \
    libssl-dev \
    libtool \
    libzmq3-dev \
    ninja-build \
    pkg-config \
    python \
    python-yaml \
    python3 \
    python3-yaml \
    uuid-runtime \
    valgrind \
    vim \
    && rm -rf /var/lib/apt/lists/*

ENTRYPOINT ["./tools/maptools.py", "build"]
