cmake_minimum_required(VERSION 4.0)
project(test CXX C)

message(STATUS "Fortran Link Libs: ${CMAKE_Fortran_IMPLICIT_LINK_LIBRARIES}") # return empty

enable_language(Fortran)
message(STATUS "Fortran Link Libs: ${CMAKE_Fortran_IMPLICIT_LINK_LIBRARIES}") # return empty 
message(STATUS "Fortran Compiler: ${CMAKE_Fortran_COMPILER}") # -> gfortran
