cmake_minimum_required(VERSION 3.10)
set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
set(CMAKE_CXX_EXTENSIONS OFF)

project("UsbDeviceNotification")

set(TARGET "UsbDeviceNotificationLibrary")

add_library(${TARGET}
  src/device_notification.cpp
  include/usb_device_notification/device_notification.h)

target_include_directories(${TARGET} PUBLIC include)

set(TARGET "UsbDeviceNotificationExampleApp")
add_executable(${TARGET} main.cpp)
target_link_libraries(${TARGET} PRIVATE UsbDeviceNotificationLibrary)
