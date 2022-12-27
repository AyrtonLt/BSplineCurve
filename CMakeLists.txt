cmake_minimum_required(VERSION 3.24)
project(BSplineCurve)

find_package(OpenGL REQUIRED)
find_package(GLUT REQUIRED)

set(CMAKE_CXX_STANDARD 17)

add_executable(BSplineCurve main.cpp)

target_link_libraries(BSplineCurve ${OPENGL_LIBRARIES})
target_link_libraries(BSplineCurve ${GLUT_LIBRARIES})
target_link_libraries(BSplineCurve -lopengl32 -g -lfreeglut)