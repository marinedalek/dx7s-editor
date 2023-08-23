# CMakeList.txt : CMake project for dx7s-editor, include source and define
# project specific logic here.
#	
find_package(glfw3 CONFIG REQUIRED)
find_package(imgui CONFIG REQUIRED)
find_package(OpenGL REQUIRED)

# Add source to this project's executable.
add_executable (dx7s-editor "dx7s-editor.cpp" "glad.c")
target_include_directories(dx7s-editor PRIVATE "../include")
target_compile_features(dx7s-editor PRIVATE cxx_std_23)
target_link_libraries(dx7s-editor PRIVATE glfw imgui::imgui OpenGL::GL)

# TODO: Add tests and install targets if needed.
