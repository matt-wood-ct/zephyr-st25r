# SPDX-License-Identifier: Apache-2.0

if(CONFIG_ST25R3911)
    zephyr_compile_definitions("-DST25R3911")
endif()

if(CONFIG_ST25R3911B)
    zephyr_compile_definitions("-DST25R3911B")
endif()

zephyr_library()
zephyr_library_sources(
        rfal_rfst25r3911.c
        st25r3911.c
        st25r3911_com.c
        st25r3911_interrupt.c
        timer.c
)
zephyr_include_directories(.)
