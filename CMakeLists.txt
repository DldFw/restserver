cmake_minimum_required(VERSION 3.6)
project("rest_server")
set(CMAKE_CXX_STANDARD 17)

#find_package(PkgConfig)
#pkg_check_modules(Pistache REQUIRED IMPORTED_TARGET libpistache)

add_executable(${PROJECT_NAME} rest_server.cc)
target_link_libraries(${PROJECT_NAME} pistache pthread)
