if(NOT CLANG_BUILD_EXAMPLES)
  set_property(DIRECTORY PROPERTY EXCLUDE_FROM_ALL ON)
endif()

if(CLANG_ENABLE_STATIC_ANALYZER)
add_subdirectory(analyzer-plugin)
endif()
add_subdirectory(clang-interpreter)
add_subdirectory(PrintFunctionNames)
