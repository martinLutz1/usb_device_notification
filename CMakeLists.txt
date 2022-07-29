cmake_minimum_required(VERSION 3.10)
set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
set(CMAKE_CXX_EXTENSIONS OFF)

project("usb_device_notification")
set(TARGET "UsbDeviceNotification")

add_executable(${TARGET} 
  main.cpp 
  device_notification.cpp 
  device_notification.h)

target_include_directories(${TARGET} PRIVATE ${CMAKE_CURRENT_SOURCE_DIR})

