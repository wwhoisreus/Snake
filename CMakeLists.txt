cmake_minimum_required(VERSION 3.26)
project(untitled)

include(FetchContent)
set(BUILD_SHARED_LIBS OFF)
FetchContent_Declare(SFML GIT_REPOSITORY https://github.com/SFML/SFML.git GIT_TAG 2.5.1)
fetchcontent_makeavailable(SFML)

set(CMAKE_CXX_STANDARD 17)

add_executable(untitled main.cpp)

target_link_libraries(untitled sfml-graphics)
