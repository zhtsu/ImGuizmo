cmake_minimum_required(VERSION 3.16)
project(ImGuizmo)

aux_source_directory(. SRC_LIST)
add_library(ImGuizmo SHARED ${SRC_LIST})
target_include_directories(ImGuizmo PUBLIC .)
target_link_libraries(ImGuizmo imgui)
