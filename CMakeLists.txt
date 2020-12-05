cmake_minimum_required(VERSION 3.17)
project(HelloWorld)

set(CMAKE_CXX_STANDARD 20)
set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -Wall -Werror")

set(CMAKE_SOURCE_DIR "${PROJECT_SOURCE_DIR}/src/")
set(CMAKE_BINARY_DIR "${PROJECT_SOURCE_DIR}/bin/")
set(CMAKE_RUNTIME_OUTPUT_DIRECTORY "${PROJECT_SOURCE_DIR}/bin/")
file(GLOB source_files "${CMAKE_SOURCE_DIR}/*.cpp")

add_executable(${PROJECT_NAME} ${source_files})
