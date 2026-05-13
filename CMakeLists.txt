cmake_minimum_required(VERSION 3.10)
project(fit4012_lab4_aes LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
set(CMAKE_CXX_EXTENSIONS OFF)

add_executable(encrypt encrypt.cpp
        cbc_decrypt.cpp
        cbc_encrypt.cpp)
add_executable(decrypt decrypt.cpp
        cbc_decrypt.cpp
        cbc_encrypt.cpp)

target_compile_options(encrypt PRIVATE -Wall -Wextra -pedantic)
target_compile_options(decrypt PRIVATE -Wall -Wextra -pedantic)
