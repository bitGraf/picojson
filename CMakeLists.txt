cmake_minimum_required(VERSION 3.6)

add_library(picojson picojson.h)

target_include_directories(picojson PUBLIC ${CMAKE_CURRENT_SOURCE_DIR})
set_target_properties(picojson PROPERTIES LINKER_LANGUAGE CXX)