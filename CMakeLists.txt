cmake_minimum_required(VERSION 2.8.3)
project(restorable_core)

add_compile_options(-std=c++11)

find_package(catkin REQUIRED COMPONENTS
  roscpp
  rospy
)

catkin_package(
  INCLUDE_DIRS include
#  LIBRARIES restorable_core
  CATKIN_DEPENDS roscpp rospy
#  DEPENDS system_lib
)

include_directories(
  include
  ${catkin_INCLUDE_DIRS}
)
