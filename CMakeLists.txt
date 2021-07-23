cmake_minimum_required(VERSION 3.2)
#for visual studio
if(MSVC) 
    add_compile_options(/W4) #set warning level to 4
else()
    add_compile_options(-Wall -Wextra -Wpedantic)
endif()
add_executable(intro main.cpp)
target_compile_features(intro PRIVATE cxx_lambda_init_captures)


