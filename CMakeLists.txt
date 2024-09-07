cmake_minimum_required(VERSION 3.30)

# We need to enable module support before setting the language to CXX
# (before a project call)
set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -stdlib=libc++")
set(CMAKE_EXPERIMENTAL_CXX_IMPORT_STD "0e5b6991-d74f-4b3d-a41c-cf096e0b2508") # See https://gitlab.kitware.com/cmake/cmake/-/issues/25965
set(CMAKE_CXX_MODULE_STD ON)

project(MyProject)

set(CMAKE_RUNTIME_OUTPUT_DIRECTORY "${CMAKE_BINARY_DIR}/bin")

add_subdirectory(src)
