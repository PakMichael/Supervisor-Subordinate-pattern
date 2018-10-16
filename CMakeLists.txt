cmake_minimum_required (VERSION 2.6)
project (Supervisor-Subordinate)

set(SOURCES 
	test.cpp
	Src/subordinate.cpp
	Src/supervisor.cpp
	Headers/subordinate.h
	Headers/supervisor.h
	)

 add_executable(${PROJECT_NAME} ${SOURCES})
 
target_include_directories(${PROJECT_NAME}
    PRIVATE
        ${PROJECT_SOURCE_DIR}/Headers
)


