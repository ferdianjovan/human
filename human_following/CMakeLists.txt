cmake_minimum_required(VERSION 2.8.3)
project(human_following)

find_package(catkin REQUIRED COMPONENTS
  rospy
  std_msgs
  actionlib_msgs
)

generate_messages(
   DEPENDENCIES
   std_msgs
   actionlib_msgs
 )

catkin_package(
#  INCLUDE_DIRS include
#  LIBRARIES human_following
#  CATKIN_DEPENDS rospy std_msgs
#  DEPENDS system_lib
   CATKIN_DEPENDS actionlib_msgs
)

include_directories(
  ${catkin_INCLUDE_DIRS}
)
