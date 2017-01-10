cmake_minimum_required (VERSION 2.6)
project (dtmerge)

set(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${CMAKE_BINARY_DIR}/bin)

include_directories(dtc/libfdt)

add_library(
 fdt

 dtc/libfdt/fdt_addresses.c
 dtc/libfdt/fdt.c
 dtc/libfdt/fdt_empty_tree.c
 dtc/libfdt/fdt_ro.c
 dtc/libfdt/fdt_rw.c
 dtc/libfdt/fdt_strerror.c
 dtc/libfdt/fdt_sw.c
 dtc/libfdt/fdt_wip.c)

add_subdirectory(src)
