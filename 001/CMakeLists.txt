cmake_minimum_required(VERSION 3.5)
project(HelloWindow)
add_definitions(-W -Wall -std=c++11)
set(sources main.cpp 
	glad.c
	)
add_executable(${PROJECT_NAME} ${sources})
target_link_libraries(${PROJECT_NAME} glfw3 dl pthread )
