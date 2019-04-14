cmake_minimum_required(VERSION 3.11)

project("sodium")

add_library(${PROJECT_NAME}
    libsodium/src/libsodium/sodium/codecs.c
    libsodium/src/libsodium/sodium/core.c
    libsodium/src/libsodium/sodium/runtime.c
    libsodium/src/libsodium/sodium/utils.c
    libsodium/src/libsodium/sodium/version.c
)

target_include_directories(${PROJECT_NAME}
    PUBLIC
        libsodium/src/libsodium/include
    PRIVATE
        libsodium/src/libsodium/include/sodium
)

set(VERSION 1.0.17)
set(SODIUM_LIBRARY_VERSION_MAJOR 10)
set(SODIUM_LIBRARY_VERSION_MINOR 2)

configure_file(
    libsodium/src/libsodium/include/sodium/version.h.in
    ${CMAKE_CURRENT_SOURCE_DIR}/libsodium/src/libsodium/include/sodium/version.h
)
