# Copyright (c) 2023, CATIE
# SPDX-License-Identifier: Apache-2.0

add_library(mbed-swo INTERFACE)

target_include_directories(mbed-swo
    INTERFACE
        .
        ./swo
)

target_sources(mbed-swo
    INTERFACE
        src/swo.cpp
)