set(THIRD_PARTY_DIR "${ROOT_DIR}/3rdparty")

set(vulkan_include ${THIRD_PARTY_DIR}/vulkansdk/include)
set(vulkan_lib ${THIRD_PARTY_DIR}/vulkansdk/lib/vulkan-1.lib)
set(glslangValidator_executable ${THIRD_PARTY_DIR}/vulkansdk/bin/glslangValidator.exe)

set(SHADER_COMPILE_TARGET "ShaderCompile")

add_subdirectory(01_test_glfw)
add_subdirectory(02_draw_a_triangle)