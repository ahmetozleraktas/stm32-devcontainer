cmake_minimum_required(VERSION 3.10)
project(STM32F0_Template C CXX)

set(CMAKE_C_STANDARD 11)
set(CMAKE_CXX_STANDARD 14)

# Include paths
include_directories(inc)

# Add source files
file(GLOB SOURCES "src/*.c")

# Create an executable
add_executable(${PROJECT_NAME} ${SOURCES})
