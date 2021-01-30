#
# @file      CMakeLists.txt
# @copyright 2021 Andrew MacIsaac
#
# @remarks
#   SPDX-License-Identifier: MPL-2.0
#
# @brief     Entry point for S-Pool build process.
#
cmake_minimum_required(VERSION 3.19)
project(s-pool)
enable_testing()

set(CMAKE_MODULE_PATH "${CMAKE_SOURCE_DIR}/cmake")

add_subdirectory(documentation)
