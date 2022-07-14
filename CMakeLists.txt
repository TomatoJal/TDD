cmake_minimum_required(VERSION 3.22)
project(OpenSSLTest)

set(GOOGLE_TEST_ROOT_DIR  ${PROJECT_SOURCE_DIR}/googletest)

link_directories(${GOOGLE_TEST_ROOT_DIR}/build/lib)
link_libraries(libgtest.a)
link_libraries(libgmock.a)
link_libraries(libgtest_main.a)
link_libraries(libgmock_main.a)

include_directories(${GOOGLE_TEST_ROOT_DIR}/googletest/include)
include_directories(${GOOGLE_TEST_ROOT_DIR}/googlemock/include)

add_subdirectory(template)

