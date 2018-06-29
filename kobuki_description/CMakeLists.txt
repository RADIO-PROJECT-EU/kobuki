cmake_minimum_required(VERSION 2.8.3)
project(kobuki_description)
find_package(catkin REQUIRED COMPONENTS urdf xacro kobuki_gazebo_plugins)

catkin_package(
   CATKIN_DEPENDS urdf xacro kobuki_gazebo_plugins
)

install(DIRECTORY launch
        DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}
)
install(DIRECTORY meshes
        DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}
)
install(DIRECTORY rviz
        DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}
)
install(DIRECTORY urdf
        DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}
)
