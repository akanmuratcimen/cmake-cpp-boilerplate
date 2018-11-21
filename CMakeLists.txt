cmake_minimum_required (VERSION 3.10.3)

project (boilerplate LANGUAGES CXX C)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
set(CMAKE_CXX_EXTENSIONS OFF)

include(CTest)

enable_testing()

add_subdirectory(src)
add_subdirectory(benchmark)
add_subdirectory(test)

add_subdirectory(lib/benchmark)
add_subdirectory(lib/benchmark/googletest)
