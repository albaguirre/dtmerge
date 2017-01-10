cmake_minimum_required (VERSION 2.6)
project (dtmerge)

set(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${CMAKE_BINARY_DIR}/bin)

include_directories(libfdt)

add_subdirectory(libfdt)
add_subdirectory(src)
