cmake_minimum_required(VERSION 3.1)
project(nbnet_examples)

add_subdirectory(echo)
add_subdirectory(echo_bytes)
add_subdirectory(/home/randy/work/game/game4/3ps/libdatachannel libdatachannel-build)

if (NOT DEFINED CPP_COMPILE)
    # not supported in CPP
    add_subdirectory(rpc)
endif (NOT DEFINED CPP_COMPILE)
