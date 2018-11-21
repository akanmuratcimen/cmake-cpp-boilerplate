cmake_minimum_required (VERSION 3.10.3)

set(SOURCE_FILES 
    main.cpp
)

add_executable(main 
    ${SOURCE_FILES}
)

set_target_properties(main
    PROPERTIES
    RUNTIME_OUTPUT_DIRECTORY "${CMAKE_BINARY_DIR}/bin"
)
