cmake_minimum_required(VERSION 2.8.12.2)

set(CMAKE_INCLUDE_CURRENT_DIR ON)

set(SOURCES
  mapviewoffile.cpp
)

add_executable(paltest_mapviewoffile_test6
  ${SOURCES}
)

add_dependencies(paltest_mapviewoffile_test6 coreclrpal)

target_link_libraries(paltest_mapviewoffile_test6
  pthread
  m
  coreclrpal
)
