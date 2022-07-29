set(TARGET_NAME "01_test_glfw")
set(SOURCE main.cpp)
add_executable(${TARGET_NAME} ${SOURCE})
target_link_libraries(${TARGET_NAME} PUBLIC glfw opengl32)