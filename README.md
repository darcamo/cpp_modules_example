# C++ Modules Example


A minimal project that works with C++ modules, including importing
`std`.

This was tested in Linux with clang-18. You need to install `libc++`.
You also need a recent cmake version, such as cmake 3.30.



Note: Creating and using modules is available since C++20, but `import
std;` is only included in C++23. Furthermore, currently only `libc++`
(from `clang`) supports it (search for "P2465R3" in [compiler
support](https://en.cppreference.com/w/cpp/compiler_support)).
