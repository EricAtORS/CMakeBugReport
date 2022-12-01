Project(HelloWorld CXX)

add_executable(hello_world src/main.cpp)
set(OUTPUT_FOLDER "${CMAKE_CURRENT_SOURCE_DIR}/output/bin")
set_target_properties(hello_world
        PROPERTIES
        PREFIX ""
        ARCHIVE_OUTPUT_DIRECTORY    "${OUTPUT_FOLDER}" 
        COMPILE_PDB_OUTPUT_DIRECTORY "${OUTPUT_FOLDER}" 
        PDB_OUTPUT_DIRECTORY        "${OUTPUT_FOLDER}" 
        EXECUTABLE_OUTPUT_DIRECTORY "${OUTPUT_FOLDER}" 
        RUNTIME_OUTPUT_DIRECTORY    "${OUTPUT_FOLDER}" 
        LIBRARY_OUTPUT_DIRECTORY    "${OUTPUT_FOLDER}"
)
