cmake_minimum_required(VERSION 3.7)
project(zs-apc-spdu-ctl)

set(CMAKE_INSTALL_BINDIR bin CACHE PATH "Installation directory for binaries")
set(CMAKE_MODULE_PATH ${CMAKE_MODULE_PATH} ${PROJECT_SOURCE_DIR}/cmake)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

find_package(Threads REQUIRED)
find_package(NetSNMP REQUIRED)
find_package(LowlevelZS REQUIRED)

add_subdirectory(src)
