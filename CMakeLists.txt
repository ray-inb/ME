cmake_minimum_required(VERSION 3.20 FATAL_ERROR)
project(surface-control-maintenance)

set(CMAKE_AUTOMOC ON)
set(CMAKE_AUTORCC ON)
set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_EXTENSIONS OFF)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
set(CMAKE_INSTALL_PREFIX ${CMAKE_SOURCE_DIR}/install)

string(TOLOWER ${CMAKE_SYSTEM_NAME} PLATFORM)

find_package(Conan)
find_package(Qt6 REQUIRED COMPONENTS Core Gui Qml Quick Network)

find_program(7ZIP_EXECUTABLE "7z")

enable_testing()
add_subdirectory(source)
