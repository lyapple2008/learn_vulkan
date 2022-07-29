set(THIRD_PARTY_DIR "${ROOT_DIR}/3rdparty")

set(vulkan_include ${THIRD_PARTY_DIR}/vulkansdk/include)
set(vulkan_lib ${THIRD_PARTY_DIR}/vulkansdk/lib/vulkan-1.lib)

add_subdirectory(01_test_glfw)