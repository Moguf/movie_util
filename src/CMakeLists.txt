set(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${CMAKE_SOURCE_DIR}/bin/)
add_definitions(-Wall -O3)
include_directories(${OpenCV_INCLUDE_DIRS})

add_executable(mu main.cpp)

target_link_libraries(mu -l${OpenCV_LIBS})