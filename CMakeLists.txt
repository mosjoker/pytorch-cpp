cmake_minimum_required(VERSION 3.0 FATAL_ERROR)
project(custom_ops)

find_package(Torch REQUIRED)

# OpenCV
set(OpenCV_DIR "/home/yuyong/soft/opencv-3.4.0/build/install/share/OpenCV")
find_package(OpenCV REQUIRED)

add_executable(example-app example-app.cpp)
target_link_libraries(example-app "${TORCH_LIBRARIES}" ${OpenCV_LIBS})
set_property(TARGET example-app PROPERTY CXX_STANDARD 11)


