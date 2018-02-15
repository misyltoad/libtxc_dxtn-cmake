cmake_minimum_required(VERSION 3.9)

add_library (libtxc_dxtn STATIC txc_compress_dxtn.c txc_dxtn.h txc_fetch_dxtn.c)

if(CMAKE_COMPILER_IS_GNUCC)
	set(CMAKE_C_FLAGS "-static -static-libgcc -static-libstdc++")
endif(CMAKE_COMPILER_IS_GNUCC)