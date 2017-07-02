cmake_minimum_required(VERSION 3.7)
project(readwritequeue)

set(CMAKE_CXX_STANDARD 11)
SET(CMAKE_CXX_FLAGS ${CMAKE_CXX_FLAGS} " -pthread")
#readerwriterqueue.h ../../atomicops.h ../common/simplethread.h ../common/simplethread.cpp
set(SOURCE_FILES main.cpp simplethread.cpp)
add_executable(readwritequeue ${SOURCE_FILES})