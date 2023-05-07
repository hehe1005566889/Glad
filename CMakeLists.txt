project(glad)

add_library(glad STATIC

    ${CMAKE_SOURCE_DIR}/libs/glad/include/glad/glad.h
    ${CMAKE_SOURCE_DIR}/libs/glad/include/KHR/khrplatform.h
    ${CMAKE_SOURCE_DIR}/libs/glad/src/glad.c
)

target_include_directories(glad PRIVATE
    ${CMAKE_SOURCE_DIR}/libs/glad/include
)
