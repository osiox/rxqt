cmake_minimum_required(VERSION 3.2 FATAL_ERROR)

project(rxqt VERSION 0.0.1 LANGUAGES CXX)

add_library(rxqt INTERFACE)

target_include_directories(rxqt INTERFACE
    $<BUILD_INTERFACE:${CMAKE_CURRENT_SOURCE_DIR}/include/>
    $<INSTALL_INTERFACE:include/rxqt>
)
