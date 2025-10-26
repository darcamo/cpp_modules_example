# C++ Modules Example


A minimal project that works with C++ modules, including importing
`std`.

This was tested in Linux with clang-18. You need to install `libc++`.
You also need a recent cmake version, such as cmake 3.30.

**Update**: Tested on 2025-06-16 seg with clang-20 and cmake 4.0. The
value of `CMAKE_EXPERIMENTAL_CXX_IMPORT_STD` was updated to the one
used in CMake 4.0.

**Update**: Tested on 2025-10-26 with clang-21, gcc-15 and cmake
4.1.2. The value of `CMAKE_EXPERIMENTAL_CXX_IMPORT_STD` did not need
to be updated. `import std` now works with gcc, but completions still
do not work reliably with either gcc or clang.


Note: Creating and using modules is available since C++20, but `import
std;` is only included in C++23. ~~Furthermore, currently only
`libc++` (from `clang`) supports it (search for "P2465R3" in [compiler
support](https://en.cppreference.com/w/cpp/compiler_support)).~~
