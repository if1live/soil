project(SOIL C)
cmake_minimum_required(VERSION 2.8)

add_definitions(-Wall)

add_library(SOIL
    src/image_helper.c
    src/stb_image_aug.c
    src/image_DXT.c
    src/SOIL.c
)

target_link_libraries(SOIL)

install(FILES src/SOIL.h DESTINATION include)
install(TARGETS SOIL DESTINATION lib)
