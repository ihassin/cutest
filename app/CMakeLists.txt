cmake_minimum_required (VERSION 3.7.2)

add_definitions(-DDEBUG)
set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++11 -fexceptions -Wall -fpermissive -ggdb")

add_executable (cutest AllTests.c CuTest.c CuTestTest.c)

set(EXECUTABLE_OUTPUT_PATH ../bin)
