cmake_minimum_required(VERSION 2.8.3)

include(cmake/HunterGate.cmake)
HunterGate(
    URL "https://github.com/ruslo/hunter/archive/v0.23.186.tar.gz"
    SHA1 "b215dc4d88cbe6cc74b5cc9fa9cdd7058775c26b"
)

project(common_msgs)
hunter_add_package(catkin)
hunter_add_package(ros_message_generation)
hunter_add_package(ros_message_runtime)
hunter_add_package(ros_std_msgs)

add_subdirectory(actionlib_msgs)
add_subdirectory(common_msgs)
add_subdirectory(geometry_msgs)
add_subdirectory(diagnostic_msgs)
add_subdirectory(nav_msgs)
add_subdirectory(sensor_msgs)
add_subdirectory(shape_msgs)
add_subdirectory(stereo_msgs)
add_subdirectory(trajectory_msgs)
add_subdirectory(visualization_msgs)
