cmake_minimum_required(VERSION 3.8)

project ("imgui")

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED TRUE)

add_library(
    imgui STATIC
	"imgui.cpp"
	"imgui_draw.cpp"
	"imgui_widgets.cpp"
    "imgui_tables.cpp"
	"imgui_demo.cpp"
)
