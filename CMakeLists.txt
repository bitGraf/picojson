cmake_minimum_required(VERSION 3.6)
set(LIB_NAME "picojson")

file(GLOB_RECURSE  lib_files "*.h")
set_source_files_properties(${engine_SOURCES} PROPERTIES LANGUAGE CXX)

add_library(picojson ${lib_files})

set_target_properties(picojson PROPERTIES
   OUTPUT_NAME ${LIB_NAME}
   VERSION 1.0.0
   SOVERSION 0
   POSITION_INDEPENDENT_CODE OFF)

target_compile_definitions(picojson PRIVATE _CRT_SECURE_NO_WARNINGS)