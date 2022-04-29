
aux_swift_source_directory(${CMAKE_CURRENT_SOURCE_DIR} _sources)
aux_swift_source_directory(${CMAKE_CURRENT_SOURCE_DIR}/Decoder _decoder_sources)
aux_swift_source_directory(${CMAKE_CURRENT_SOURCE_DIR}/Encoder _encoder_sources)
add_library(StructuredFieldValues ${_sources} ${_decoder_sources} ${_encoder_sources})
target_link_libraries(StructuredFieldValues RawStructuredFieldValues)