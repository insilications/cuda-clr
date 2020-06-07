message(STATUS "cmake version ${CMAKE_VERSION}")
project (cuda)
cmake_minimum_required (VERSION 2.8.8) # OBJECT libraries require 2.8.8

set(CUDA_INSTALL_DIR /usr/cuda CACHE STRING "CUDA install location")

install(DIRECTORY ${PROJECT_SOURCE_DIR}/opt/cuda/ DESTINATION ${CUDA_INSTALL_DIR} USE_SOURCE_PERMISSIONS)