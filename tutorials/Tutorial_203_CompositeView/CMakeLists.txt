cmake_minimum_required(VERSION 3.12)

get_filename_component(PROJECT_NAME ${CMAKE_CURRENT_SOURCE_DIR} NAME)
project(${PROJECT_NAME})


add_executable(${PROJECT_NAME}
        main.cpp
        )

set_target_properties(${PROJECT_NAME} PROPERTIES FOLDER "tutorials")

target_link_libraries(${PROJECT_NAME} easy3d::viewer)

