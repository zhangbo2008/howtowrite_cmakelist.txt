# howtowrite_cmakelist.txt




2021-01-25,11点06


cmaklist文件的写法:


cmake_minimum_required(VERSION 2.8.4)
project(untitled3 C)
# https://blog.csdn.net/yyyerica/article/details/70169102
set(CMAKE_C_STANDARD 99)
set(CMAKE_CXX_STANDARD 11)
set(CMAKE_C_FLAGS -pthread)
set(CMAKE_C_FLAGS -lpthread)

LINK_LIBRARIES(m)    # 添加math.h头文件.   //在add_executable之前.



add_executable(untitled3 main.c)
#include_directories( "/usr/include/eigen3" )
#add_executable(untitled3 ${SOURCE_FILES})
#find_package(untitled3 REQUIRED)
#target_link_libraries(untitled3 Threads::Threads)

