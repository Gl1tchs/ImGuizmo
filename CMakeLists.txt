cmake_minimum_required(VERSION 3.25)

project(ImGuizmo)

add_library(ImGuizmo
    GraphEditor.cpp
    GraphEditor.h
    ImCurveEdit.cpp
    ImCurveEdit.h
    ImGradient.cpp
    ImGradient.h
    ImGuizmo.cpp
    ImGuizmo.h
    ImSequencer.cpp
    ImSequencer.h
    ImZoomSlider.h
)

target_include_directories(ImGuizmo PUBLIC
    ${VENDOR_DIR}/ImGuizmo
    ${VENDOR_DIR}/ImGui
)

target_link_libraries(ImGuizmo PUBLIC ImGui)
