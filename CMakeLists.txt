cmake_minimum_required(VERSION 2.8.3)
project(husky_teleop)

## Find catkin macros and libraries
## if COMPONENTS list like find_package(catkin REQUIRED COMPONENTS xyz)
## is used, also find other catkin packages
find_package(catkin REQUIRED)

catkin_package()

install(
  DIRECTORY launch 
  DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}
)

install(
  PROGRAMS scripts/joystick_teleop
  DESTINATION ${CATKIN_PACKAGE_BIN_DESTINATION}
)
