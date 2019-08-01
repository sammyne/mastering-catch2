cmake_minimum_required(VERSION 3.14)

include_directories(
    ${CMAKE_CURRENT_SOURCE_DIR}
    ${vendorDir}/Catch2/single_include
)

set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++11")

aux_source_directory(${CMAKE_CURRENT_SOURCE_DIR} srcs)

add_executable(main ${srcs})