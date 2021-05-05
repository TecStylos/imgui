cmake_minimum_required(VERSION 3.8)

project ("imgui")

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED TRUE)

set(
	IMGUI_LIB_FILES
	"imgui.cpp"
	"imgui_draw.cpp"
	"imgui_widgets.cpp"
	"imgui_tables.cpp"
	"imgui_demo.cpp"
)

set(
	IMGUI_LINK_LIBRARIES
	#GLFW
)

add_library(
	imgui STATIC
	${IMGUI_LIB_FILES}
)

target_link_libraries(
	imgui PUBLIC 
	${IMGUI_LINK_LIBRARIES}
)