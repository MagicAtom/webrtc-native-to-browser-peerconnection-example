cmake_minimum_required(VERSION 3.10)

project(rtc_server)

set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED True)

include_directories(${PROJECT_SOURCE_DIR}/include)
link_directories(${PROJECT_SOURCE_DIR}/lib)

add_executable(
    rtc_server
    main.cc
    peer_channel.cc
    data_socket.cc
    utils.cc
)

target_link_libraries(rtc_server libwebrtc.a)