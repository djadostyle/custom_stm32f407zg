# Copyright (c) 2023 ARM Limited. All rights reserved.
# SPDX-License-Identifier: Apache-2.0

add_library(mbed-INRUSH_MCU_F407ZG INTERFACE)

target_sources(mbed-INRUSH_MCU_F407ZG
    INTERFACE
        PeripheralPins.c
)

target_include_directories(mbed-INRUSH_MCU_F407ZG
    INTERFACE
        .
)

target_link_libraries(mbed-INRUSH_MCU_F407ZG INTERFACE mbed-stm32f407xg)
