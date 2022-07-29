cmake_minimum_required(VERSION 3.23 FATAL_ERROR)

project(LearnVulkan)

SET(CMAKE_CXX_STANDARD 17)
SET(CMAKE_CXX_STANDARD_REQUIRED ON)

if(PROJECT_SOURCE_DIR STREQUAL PROJECT_BINARY_DIR)
  message(
    FATAL_ERROR
      "In-source builds not allowed. Please make a new directory (called a build directory) and run CMake from there."
  )
endif()

set(ROOT_DIR "${CMAKE_CURRENT_SOURCE_DIR}")

add_subdirectory(3rdparty)
add_subdirectory(src)
