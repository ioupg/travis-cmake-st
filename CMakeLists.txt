cmake_minimum_required (VERSION 3.1 FATAL_ERROR)
project (SLib)

# The version number.
set (SLIB_VERSION 1)

# add the binary tree to the search path for include files
# so that we will find TutorialConfig.h
include_directories("${PROJECT_BINARY_DIR}")

add_library(SLb slib.cpp)

# c++11 compat

set_property(TARGET ${prj} PROPERTY CXX_STANDARD 11)
set_property(TARGET ${prj} PROPERTY CXX_STANDARD_REQUIRED ON)
