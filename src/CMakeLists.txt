add_executable(test_vec4 test_vec4.c)
target_link_libraries(test_vec4 m)

add_executable(test_mat4 test_mat4.c)
target_link_libraries(test_mat4 m)

add_executable(test_gl test_gl.c)
target_link_libraries(test_gl m ${SDL2_LIBRARY} ${OPENGL_LIBRARIES} ${GLEW_LIBRARY})

install(TARGETS test_vec4 test_mat4 test_gl DESTINATION "${SSE_Stuff_SOURCE_DIR}/bin")

