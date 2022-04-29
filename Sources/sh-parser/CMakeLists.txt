
aux_swift_source_directory(${CMAKE_CURRENT_SOURCE_DIR} _sources)
add_executable(sh-parser ${_sources})
target_link_libraries(sh-parser StructuredFieldValues)
