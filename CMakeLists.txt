cmake_minimum_required(VERSION 3.0)
project(TestsProperties)
include(CTest)
add_subdirectory(subdir)

# second definition of "MyTest"
add_test(NAME MyTest COMMAND ${CMAKE_COMMAND} -E echo "MyTest2 in main directory")

## Comment out to be able to configure project
set_tests_properties(MyTest2 PROPERTIES DEPENDS MyTest)
