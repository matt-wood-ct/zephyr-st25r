# SPDX-License-Identifier: Apache-2.0

zephyr_library()
zephyr_library_sources(
        Src/message/ndef_message.c
        Src/message/ndef_record.c
        Src/message/ndef_type_wifi.c
        Src/message/ndef_types.c
        Src/message/ndef_types_mime.c
        Src/message/ndef_types_rtd.c

        Src/poller/ndef_poller.c
        Src/poller/ndef_t2t.c
        Src/poller/ndef_t3t.c
        Src/poller/ndef_t4t.c
        Src/poller/ndef_t5t.c
)
zephyr_include_directories(Inc/message)
zephyr_include_directories(Inc/poller)
