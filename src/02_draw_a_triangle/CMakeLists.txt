set(TARGET_NAME "02_draw_a_triangle")
set(SOURCE "main.cpp")

add_subdirectory(shaders)

add_executable(${TARGET_NAME} ${SOURCE})
target_link_libraries(${TARGET_NAME} PUBLIC ${vulkan_lib})
target_link_libraries(${TARGET_NAME} PUBLIC glfw)

target_include_directories(
  ${TARGET_NAME}
  PUBLIC $<BUILD_INTERFACE:${vulkan_include}>)

add_dependencies(${TARGET_NAME} ${SHADER_COMPILE_TARGET})