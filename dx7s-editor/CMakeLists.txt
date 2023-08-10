# CMakeList.txt : CMake project for dx7s-editor, include source and define
# project specific logic here.
#

# Add source to this project's executable.
add_executable (dx7s-editor "dx7s-editor.cpp" "dx7s-editor.h")

if (CMAKE_VERSION VERSION_GREATER 3.12)
  set_property(TARGET dx7s-editor PROPERTY CXX_STANDARD 20)
endif()

# TODO: Add tests and install targets if needed.
