CMAKE_MINIMUM_REQUIRED(VERSION 2.8.12)

project(distance C)

set(HEADERS 
	test.c
	transform.c)

set(SOURCES 
	test.c
	transform.c)

ADD_EXECUTABLE(distance ${SOURCES} ${HEADERS}) 


target_link_libraries(distance
	LINK_PRIVATE m
	)
