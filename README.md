# Two wheeled wall following robot

This is a two-wheeled wall-following robot that uses ROS and Gazebo as its platform. It assumes the wall is on the right-hand side of the robot



## Setup 

- exec command catkin_make in the catkin_ws/ and simulation_ws/ folders
- Add catkin_ws/src and simulation_ws/src to ROS_PACKAGE_PATH
  - On Linux you can add by this command: export ROS_PACKAGE_PATH=$ROS_PACKAGE_PATH:<path_to_catkin_src>:<path_to_simulation_src> to each command shell



## Running 

Open 3 terminals and type those commands in each of them:

- 0- roscore
- 1- roslaunch my_worlds world2.launch
- 2- rosrun motion_plan follow_wall.py