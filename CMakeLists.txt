cmake_minimum_required (VERSION 2.8)

project (ShmDB)

add_library(LibShmDb SHARED
        source/shmdb.h
        source/shm.h
        source/shm.c)

add_executable(Test test.c)
TARGET_LINK_LIBRARIES(Test LibShmDb)