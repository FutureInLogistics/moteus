# Copyright 2023 mjbots Robotic Systems, LLC.  info@mjbots.com

# moteus does not use cmake to build, but does expose some client
# libraries for use in cmake projects.

cmake_minimum_required(VERSION 3.10)
project(moteus VERSION 0.1.20230821)

add_subdirectory(lib/cpp)


# A client project can use this as follows:
#
# include(FetchContent)
# FetchContent_Declare(
#   moteus
#   GIT_REPOSITORY https://github.com/mjbots/moteus.git
#   GIT_TAG        00112233445566778899aabbccddeeff00112233
# )
#
# FetchContent_MakeAvailable(moteus)
#
# add_executable(myproject myproject.cc)
# target_link_libraries(myproject moteus::cpp)
