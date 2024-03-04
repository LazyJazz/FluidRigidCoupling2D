
file(GLOB_RECURSE SOURCES *.h *.cpp)

add_executable(fluid-rigid-coupling ${SOURCES})

target_include_directories(fluid-rigid-coupling PRIVATE ${CMAKE_CURRENT_SOURCE_DIR})

find_package(Eigen3 CONFIG REQUIRED)
target_link_libraries(fluid-rigid-coupling PRIVATE Eigen3::Eigen)

find_package(GLUT REQUIRED)
target_link_libraries(fluid-rigid-coupling PRIVATE GLUT::GLUT)
