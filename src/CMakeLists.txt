

add_library(mymodule)
target_compile_features(mymodule PUBLIC cxx_std_23)
target_sources(mymodule
  PUBLIC
  FILE_SET CXX_MODULES
  FILES
  mymodule.cppm
)

add_executable(main main.cpp)
target_link_libraries(main mymodule)
