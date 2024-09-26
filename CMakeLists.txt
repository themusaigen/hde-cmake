cmake_minimum_required(VERSION 3.15)

project(hde LANGUAGES C)

add_library(${PROJECT_NAME} STATIC 
	"src/hde/hde32.c"
	"src/hde/hde32.h"
	"src/hde/hde64.c"
	"src/hde/hde64.h"
	"src/hde/table32.h"
	"src/hde/table64.h"
)

target_include_directories(${PROJECT_NAME} PUBLIC "src/hde")