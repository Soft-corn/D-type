cmake_minimum_required(VERSION 3.16)

project(D-type)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

add_executable(D-type
    "EntryPoint.cpp"
 "Core/Application.h" "Core/Application.cpp")


set(SPDLOG_INCLUDE_DIR ${CMAKE_SOURCE_DIR}/vendor/spdlog/include)

target_include_directories(D-type PRIVATE ${SPDLOG_INCLUDE_DIR})

