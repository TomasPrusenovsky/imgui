cmake_minimum_required(VERSION 3.10)
project(ImGui)

set(headers
        imconfig.h
        imgui.h
        imgui_internal.h
        imstb_rectpack.h
        imstb_textedit.h
        imstb_truetype.h
)

set(sources
        imgui.cpp
        imgui_demo.cpp
        imgui_draw.cpp
        imgui_tables.cpp
        imgui_widgets.cpp
)

add_library(ImGui STATIC ${headers} ${sources})
target_include_directories(ImGui PUBLIC ${CMAKE_CURRENT_SOURCE_DIR})