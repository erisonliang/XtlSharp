cmake_minimum_required(VERSION 3.15)
project(libxtl)

set(CMAKE_CXX_STANDARD 17)
include_directories(.)
add_compile_options(-bigobj)
add_library(libxtl SHARED general.h TensorRef.h fillcopy.h fillcopy.cpp general.cpp elementwise.h elementwise.cpp ClipClosePow.h ClipClosePow.cpp reducing.h reducing.cpp slicing.h slicing.cpp)
