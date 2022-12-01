Project(CmakeBugReport CXX)

include(${CMAKE_CURRENT_SOURCE_DIR}/output/conan/conanbuildinfo.cmake)
conan_basic_setup(TARGETS )


set(OUTPUT_FOLDER "${CMAKE_CURRENT_SOURCE_DIR}/output/bin")

set(CMAKE_LIBRARY_OUTPUT_DIRECTORY  ${OUTPUT_FOLDER} )
set(CMAKE_ARCHIVE_OUTPUT_DIRECTORY  ${OUTPUT_FOLDER} )
set(CMAKE_RUNTIME_OUTPUT_DIRECTORY  ${OUTPUT_FOLDER} )

add_subdirectory(plugins)