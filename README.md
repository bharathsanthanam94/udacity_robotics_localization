**Monte Carlo Localization with ROS**


**Introduction**


A robot is designed using URDF format and it is equipped with Hokuyo laser sensor. Monte carlo lozalization is implemented to localize the robot in a simulated environment.

**Concepts explored in this Project:**

1. Monte Carlo Localization
2. ROS AMCL package

**Launching the project**

Clone the repository and execute,

$ catkin_make

$ source devel/setup.launch

$ roslaunch my_robot world.launch

All nodes will be initialized. In Rviz, there will a robot surrounded with red arrows representing the particles associated with the AMCL filter.

Using "2D Nav goal" in Rviz, move the robot . The robot will move and the red arrows will condense around the robot showing the best guess for the position of robot.


To move the robot via keyboard, open a new-terminal and use teleop package.

Execute,

$ source devel/setup.bash

$ rosrun teleop_twist_keyboard teleop_twist_keyboard.py

The terminal displays the keys to operate the robot.
