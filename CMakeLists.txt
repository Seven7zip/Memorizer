cmake_minimum_required(VERSION 3.0.0)
project(Onecard VERSION 0.1.0)
set(CMAKE_CXX_FLAGS_DEBUG "-g")
set(CMAKE_CXX_FLAGS_RELEASE "-O3")
set(CMAKE_CXX_STANDARD 20)
include(CTest)
enable_testing()
add_subdirectory(src)
add_subdirectory(tests)
add_subdirectory(random)
include(CPack)
#install(TARGETS Onecard RUNTIME DESTINATION bin)
