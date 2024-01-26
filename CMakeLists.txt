cmake_minimum_required(VERSION 3.5.0)
project(Raylib-Boilder VERSION 0.1.0 LANGUAGES C)

include(CTest)
enable_testing()

add_executable(Raylib-Boilder main.c)
target_link_libraries(Raylib-Boilder raylib)

set(CPACK_PROJECT_NAME ${PROJECT_NAME})
set(CPACK_PROJECT_VERSION ${PROJECT_VERSION})
include(CPack)
