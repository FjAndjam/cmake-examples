cmake_minimum_required(VERSION 3.5)

project (hello_headers)

set(SOURCES
	src/main.cpp
	src/Hello.cpp
)

add_executable(${PROJECT_NAME} ${SOURCES})

target_include_directories(hello_headers
	PRIVATE
		${PROJECT_SOURCE_DIR}/include
)
