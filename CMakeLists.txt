cmake_minimum_required(VERSION 4.1.2)

# We need to enable module support before setting the language to CXX
# (before a project call)
# set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -stdlib=libc++")
set(CMAKE_EXPERIMENTAL_CXX_IMPORT_STD "d0edc3af-4c50-42ea-a356-e2862fe7a444") # See https://gitlab.kitware.com/cmake/cmake/-/issues/25965
set(CMAKE_CXX_MODULE_STD ON)

project(MyProject)

set(CMAKE_RUNTIME_OUTPUT_DIRECTORY "${CMAKE_BINARY_DIR}/bin")

add_subdirectory(src)
