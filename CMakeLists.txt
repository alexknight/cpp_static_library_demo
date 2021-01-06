cmake_minimum_required(VERSION 3.17)
project(demo)

set(CMAKE_CXX_STANDARD 14)

link_directories(third_party)

aux_source_directory(. DIR_SRCS)
#add_subdirectory(third_party)
add_executable(demo ${DIR_SRCS})

target_link_libraries(demo libMathFunctions.a)

cmake_minimum_required (VERSION 2.8)
