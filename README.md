# libsodium-cmake

[![Travis build status](https://travis-ci.org/robinlinden/libsodium-cmake.svg?branch=master)](https://travis-ci.org/robinlinden/libsodium-cmake)
[![Appveyor build status](https://ci.appveyor.com/api/projects/status/ra7l1pmh1viiss6k/branch/master?svg=true)](https://ci.appveyor.com/project/robinlinden/libsodium-cmake/branch/master)

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
FetchContent_Declare(
    Sodium
    GIT_REPOSITORY https://github.com/robinlinden/libsodium-cmake.git
)

FetchContent_GetProperties(Sodium)
if(NOT sodium_POPULATED)
    set(SODIUM_DISABLE_TESTS ON)

    FetchContent_Populate(Sodium)
    add_subdirectory(
        ${sodium_SOURCE_DIR}
        ${sodium_BINARY_DIR}
    )
endif()

target_link_libraries(${PROJECT_NAME}
    PRIVATE
        sodium
)
```
