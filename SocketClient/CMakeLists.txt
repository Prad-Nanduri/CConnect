cmake_minimum_required(VERSION 3.23)
project(SocketClient C)

set(CMAKE_C_STANDARD 99)



find_path(TheHeaderFile socketutil.h
        PATHS /home/subra/Desktop/SocketCProjects/SocketUtil)

find_library(TheLibrary
        NAMES SocketUtil
        PATHS /home/subra/Desktop/SocketCProjects/SocketUtil/cmake-build-debug)

add_executable(SocketClient main.c)

include_directories(${TheHeaderFile})
target_link_libraries(${PROJECT_NAME} ${TheLibrary})




