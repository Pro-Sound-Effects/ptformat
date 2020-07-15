CMAKE_MINIMUM_REQUIRED(VERSION 2.8)
PROJECT(ptformat)

ADD_EXECUTABLE(ptftool ptftool.cc ptformat.cc)
TARGET_INCLUDE_DIRECTORIES(ptftool PUBLIC 
	${CMAKE_CURRENT_SOURCE_DIR}/ptformat)

ADD_EXECUTABLE(ptunxor ptunxor.cc ptformat.cc)
TARGET_INCLUDE_DIRECTORIES(ptunxor PUBLIC 
	${CMAKE_CURRENT_SOURCE_DIR}/ptformat)

ADD_EXECUTABLE(ptgenmissing ptgenmissing.cc ptformat.cc)
TARGET_INCLUDE_DIRECTORIES(ptunxor PUBLIC 
	${CMAKE_CURRENT_SOURCE_DIR}/ptformat)