cmake_minimum_required(VERSION 3.10)

if(NOT TARGET lasticotlib)
	project(LasticotCMake VERSION 1.0)
	find_package(LasticotCMake REQUIRED CONFIG)
	enable_testing()
endif()

add_executable(test_worm test_worm.cpp)
target_link_libraries(test_worm PUBLIC lasticotlib)
add_test(NAME test_worm COMMAND test_worm)