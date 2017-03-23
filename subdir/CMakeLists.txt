# first definition of "MyTest"
add_test(NAME MyTest COMMAND ${CMAKE_COMMAND} -E echo "MyTest in subdir directory")

add_test(NAME MyTest2 COMMAND ${CMAKE_COMMAND} -E echo "MyTest2 in subdir directory")
