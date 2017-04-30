cmake_minimum_required(VERSION 2.8.3)
project(ardrone_joystick)

find_package(catkin REQUIRED COMPONENTS
  geometry_msgs
  roscpp
  sensor_msgs
  std_srvs
)


catkin_package(
#  INCLUDE_DIRS include
#  LIBRARIES ardrone_joystick
#  CATKIN_DEPENDS geometry_msgs roscpp sensor_msgs std_srvs
#  DEPENDS system_lib
)

include_directories(
  ${catkin_INCLUDE_DIRS}
)

# Create visualizer library
#ADD_LIBRARY(ardrone_joystick src/main.cpp)
#TARGET_LINK_LIBRARIES(ardrone_joystick ${catkin_LIBRARIES})
# create library
#ADD_LIBRARY(ardrone_joystick SHARED src/main.cpp)

add_executable(ardrone_teleop src/main.cpp)
target_link_libraries(ardrone_teleop ${catkin_LIBRARIES})
