cmake_minimum_required(VERSION 3.14 FATAL_ERROR)

project(UTemplate VERSION 0.4.7)
message(STATUS "[Project] ${PROJECT_NAME}")

include(cmake/InitUCMake.cmake)
Ubpa_InitUCMake()

Ubpa_InitProject()

Ubpa_AddSubDirsRec(include)
Ubpa_AddSubDirsRec(src)

Ubpa_Export(DIRECTORIES "include")
