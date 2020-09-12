cmake_minimum_required(VERSION 3.6)

add_library(picojson INTERFACE)
target_sources(picojson picojson.h)
target_include_directories(picojson INTERFACE ${CMAKE_CURRENT_SOURCE_DIR})

set_target_properties(picojson PROPERTIES LINKER_LANGUAGE CXX)