cmake_minimum_required(VERSION 3.18)
project(ZLIB)
set(BUILD_SHARED_LIBS OFF)
include_directories(${CMAKE_CURRENT_SOURCE_DIR}/include)

set(SOURCE_FILES 
    src/adler32.c
    src/compress.c
    src/crc32.c
    src/deflate.c
    # src/example.c
    src/gzio.c
    src/infblock.c
    src/infcodes.c
    src/inffast.c
    src/inflate.c
    src/inftrees.c
    src/infutil.c
    src/maketree.c
    src/minigzip.c
    src/trees.c
    src/uncompr.c
    src/zutil.c
)

if (BUILD_SHARED_LIBS)
add_library(ZLIB SHARED ${SOURCE_FILES})
else()
add_library(ZLIB STATIC ${SOURCE_FILES})
endif()