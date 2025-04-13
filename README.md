# libsodium-cmake

## Description

CMakeWrapper for [libsodium](https://github.com/jedisct1/libsodium), the modern, portable, easy to use crypto library.

This wrapper is written with a few goals in mind:
1. It should be easy to build
1. It should be obvious that libsodium's source code hasn't been touched
1. It should be easy to integrate into projects

## Building

Clone!

`git clone --recursive https://github.com/robinlinden/libsodium-cmake.git`

Build!

```sh
mkdir build && cd build
cmake ..
make
make test
```

## Using in your project

```cmake
cmake_minimum_required(VERSION 3.14)
# 3.11 and higher is supported, but this example uses
# `FetchContent_MakeAvailable` which is only available starting with 3.14.

include(FetchContent)

# Update the commit to point to whatever libsodium-cmake-commit you want to target.
FetchContent_Declare(Sodium
    GIT_REPOSITORY https://github.com/robinlinden/libsodium-cmake.git
    GIT_TAG e5b985ad0dd235d8c4307ea3a385b45e76c74c6a # HEAD, last updated at 2025-04-13
)
set(SODIUM_DISABLE_TESTS ON)
FetchContent_MakeAvailable(Sodium)

target_link_libraries(${PROJECT_NAME}
    PRIVATE
        sodium
)
```
