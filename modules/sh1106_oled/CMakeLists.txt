zephyr_include_directories(${CMAKE_CURRENT_SOURCE_DIR}/include)

zephyr_library()

zephyr_library_sources(
    src/sh1106.c
)

zephyr_library_include_directories(include)
