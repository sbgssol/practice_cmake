project(header_only_lib_2)

add_library(${PROJECT_NAME} INTERFACE)
add_library(lib_2 ALIAS ${PROJECT_NAME})
target_include_directories(${PROJECT_NAME} INTERFACE ${PROJECT_SOURCE_DIR})