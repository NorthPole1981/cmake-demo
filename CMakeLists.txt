cmake_minimum_required(VERSION 3.25 FATAL_ERROR)
project(cmake-demo
    VERSION 0.0.1
)

list(APPEND CMAKE_MODULE_PATH "${CMAKE_SOURCE_DIR}/cmake")
include(BuildInfo)
add_subdirectory(src)
add_subdirectory(external)
add_subdirectory(docs)
add_subdirectory(test)
add_subdirectory(packaging)