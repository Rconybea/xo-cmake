cmake_minimum_required(VERSION 3.10)

project(xo_macros VERSION 1.0)

# if any are useful for this project..
#include (cmake/foo.cmake)

# ----------------------------------------------------------------
# cmake export

set(XO_PROJECT_NAME xo_macros)

install(
    FILES
    "cmake/xo_macros/xo-project-macros.cmake"
    "cmake/xo_macros/xo_cxx.cmake"
    "cmake/xo_macros/code-coverage.cmake"
    PERMISSIONS OWNER_READ GROUP_READ WORLD_READ
    DESTINATION share/cmake/xo_macros
)
