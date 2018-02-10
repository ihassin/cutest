cmake_minimum_required (VERSION 2.6)

add_definitions(-DDEBUG)

set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++11 -fexceptions -Wall -fpermissive -ggdb")

set(LIBRARY_OUTPUT_PATH ../link)

file(GLOB SRC_FILES *.cpp *.h)
add_library(cutestLib ${SRC_FILES})
