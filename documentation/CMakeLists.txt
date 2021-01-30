#
# @file      CMakeLists.txt
# @copyright 2021 Andrew MacIsaac
#
# @remarks
#   SPDX-License-Identifier: MPL-2.0
#
# @brief      Generate documentation for S-Pool.
#
project(s-pool-docs)

find_package(Sphinx REQUIRED)

# Configured documentation tools and intermediate build results.
set(BINARY_BUILD_DIR "${CMAKE_CURRENT_BINARY_DIR}/_docbuild")

# Sphinx cache with pickled ReST documents.
set(SPHINX_CACHE_DIR "${CMAKE_CURRENT_BINARY_DIR}/_doctrees")

# HTML output directory.
set(SPHINX_HTML_DIR "${CMAKE_CURRENT_BINARY_DIR}/html")

add_custom_target(s-pool-docs ALL
    ${SPHINX_EXECUTABLE}
        -q -b html
        -d "${SPHINX_CACHE_DIR}"
        "${CMAKE_CURRENT_SOURCE_DIR}"
        "${SPHINX_HTML_DIR}"
    COMMENT "Building HTML documentation with Sphinx"
)
