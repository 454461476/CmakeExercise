cmake_minimum_required(VERSION 3.5)

project(cmakeTest LANGUAGES CXX)

set(projectname cmakeTest..CACHE)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

add_executable(cmakeTest main.cpp)

include(GNUInstallDirs)
install(TARGETS cmakeTest
    LIBRARY DESTINATION ${CMAKE_INSTALL_LIBDIR}
    RUNTIME DESTINATION ${CMAKE_INSTALL_BINDIR}
)
