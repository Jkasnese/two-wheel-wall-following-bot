# Two wheeled wall following robot

This is a two-wheeled wall-following robot that uses ROS and Gazebo as its platform. It assumes the wall is on the right-hand side of the robot
# TO RUN

exec command catkin_make in the catkin_ws/ and simulation_ws/ folders
Add catkin_ws/src and simulation_ws/src to ROS_PACKAGE_PATH
	On Linux you can add by this command: export ROS_PACKAGE_PATH=$ROS_PACKAGE_PATH:<path_to_catkin_src>:<path_to_simulation_src>


open 4 terminals:
0- roscore
1- roslaunch my_worlds world2.launch
2- roslaunch m2wr_description spawn.launch
3- (navigate to catkin_ws/src/motion_plan/scripts and run:) rosrun motion_plan follow_wall.py
