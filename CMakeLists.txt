cmake_minimum_required(VERSION 3.28.0)
    
project(mylibrary LANGUAGES C VERSION 1.0.0 DESCRIPTION "MyLibrary description")

add_library(
    ${PROJECT_NAME} SHARED
    mylib.h mylib.c
)

set_property(TARGET ${PROJECT_NAME} PROPERTY C_STANDARD 23)
set_property(TARGET ${PROJECT_NAME} PROPERTY C_STANDARD_REQUIRED ON)
set_property(TARGET ${PROJECT_NAME} PROPERTY C_EXTENSIONS OFF)
