# CMakeLists.txt for TestFortran project using ExternalProject
cmake_minimum_required(VERSION 4.0)
project(TestFortranExternal)

include(ExternalProject)

ExternalProject_Add(TestFortran_ext
    SOURCE_DIR ${CMAKE_SOURCE_DIR}/TestFortran
    CMAKE_ARGS -DCMAKE_INSTALL_PREFIX=${CMAKE_BINARY_DIR}/install
    INSTALL_COMMAND ""
)

# Optionally, add a target to depend on the external project
add_custom_target(TestFortran ALL
    DEPENDS TestFortran_ext
)

