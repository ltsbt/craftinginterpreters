cmake_minimum_required(VERSION 3.10)
project(lox)

set(CMAKE_C_STANDARD 11)
set(CMAKE_C_STANDARD_REQUIRED True)

set(CMAKE_C_FLAGS "${CMAKE_C_FLAGS} -Wall -Wextra -g")

include_directories(include)

file(GLOB SOURCE_FILES "src/*.c")
set(CMAKE_EXPORT_COMPILE_COMMANDS ON)

add_executable(lox ${SOURCE_FILES})

