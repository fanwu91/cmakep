CMAKE_MINIMUM_REQUIRED (VERSION 3.22.1)
PROJECT (Hello)
ADD_SUBDIRECTORY (Adder/)
ADD_EXECUTABLE (${PROJECT_NAME} main.cpp) # generate executable 
TARGET_INCLUDE_DIRECTORIES (${PROJECT_NAME} PUBLIC Adder/) # assign include path of the executable, in this case the "./Adder" folder
TARGET_LINK_LIBRARIES (${PROJECT_NAME} Adder) # link the libAdder with the executable
