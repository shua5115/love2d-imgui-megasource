cmake_minimum_required(VERSION 3.1)

project(imgui)

set(IMGUI_SRC
imgui.cpp
imgui_demo.cpp
imgui_draw.cpp
imgui_tables.cpp
imgui_widgets.cpp
)

add_library(imgui-static STATIC ${IMGUI_SRC})
target_include_directories(imgui-static PUBLIC ".")