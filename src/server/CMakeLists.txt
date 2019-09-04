cmake_minimum_required(VERSION 2.8)

include(CodeGenerator)
generate_code(
  MODELS ${CMAKE_CURRENT_SOURCE_DIR}/interface
  SERVER_IMPL_LIB_EXTRA_HEADERS ${KMS_FILTERS_IMPL_HEADERS}
  SERVER_STUB_DESTINATION ${CMAKE_CURRENT_SOURCE_DIR}/implementation/objects
)
