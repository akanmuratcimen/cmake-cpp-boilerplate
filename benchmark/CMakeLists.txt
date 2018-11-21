cmake_minimum_required (VERSION 3.10.3)

find_package(Threads REQUIRED)

set(BENCHMARK_ENABLE_TESTING 
    OFF 
    CACHE BOOL "Suppressing benchmark's tests" FORCE
)

set(SOURCE_FILES 
    main_benchmarks.cpp
)

add_executable(
    benchmarks 
    ${SOURCE_FILES}
)

target_include_directories(benchmarks 
    PUBLIC 
        ../src
)

target_link_libraries(benchmarks 
    benchmark
    ${CMAKE_THREAD_LIBS_INIT}
)
