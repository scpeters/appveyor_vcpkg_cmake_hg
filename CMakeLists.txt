cmake_minimum_required(VERSION 3.5.1 FATAL_ERROR)
cmake_policy(GET CMP0048 policy)
message(STATUS "CMP0048 before: ${policy}")
cmake_policy(SET CMP0048 NEW)
cmake_policy(GET CMP0048 policy)
message(STATUS "CMP0048 after: ${policy}")

#============================================================================
# Find ignition-cmake
#============================================================================
# If you get an error at this line, you need to install ignition-cmake
find_package(ignition-cmake0 REQUIRED)

#============================================================================
# Set up the project
#============================================================================
project(ignition-math4 VERSION 4.0.0)

