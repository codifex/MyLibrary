cmake_minimum_required(VERSION 3.28.0)

project(mylibrary LANGUAGES C VERSION 1.0.0 DESCRIPTION "MyLibrary description")

add_library(
    mylibrary SHARED # creates .so, STATIC creates .a 
    mylib.h mylib.c
)

set_property(TARGET mylibrary PROPERTY C_STANDARD 23)
set_property(TARGET mylibrary PROPERTY C_STANDARD_REQUIRED ON)
set_property(TARGET mylibrary PROPERTY C_EXTENSIONS OFF)
