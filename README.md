# RoboND-Term2-P2-WhereAmI
Udacity Robotics ND - Term 2 - Project 2: Localization, URDF &amp; ROS Package Creation

Utilize ROS packages to accurately localize a mobile robot inside a provided map in the Gazebo and RViz simulation environments.
Several aspects of robotics with a focus on ROS have been explored, including -
* Building a mobile robot for simulated tasks.
* Creating a ROS package that launches a custom robot model in a Gazebo world and utilizes packages like AMCL and the Navigation Stack.
* Exploring, adding, and tuning specific parameters corresponding to each package to achieve the best possible localization results.

## Installation, Build & Running Scripts ##

* Following package installation might be required (Assumed that Linux 16.04 and ROS Kinetic installation is already there)
```
$ sudo apt-get install ros-kinetic-navigation
$ sudo apt-get install ros-kinetic-map-server
$ sudo apt-get install ros-kinetic-move-base
$ rospack profile
$ sudo apt-get install ros-kinetic-amcl
```

* Download the repository folder 'sg_bot' to catkin workspace folder
Use following command to clone entire repository, and copy 'sg_bot' folder to your catkin_ws/src folder.
```
$ git clone https://github.com/gorsnehal/RoboND-Term2-P2-WhereAmI.git
```
* Compile & Build the sg_bot package
```
catkin_make; 
source devel/setup.bash
```
* After the above steps, you should be able to run the commands below in separate terminals
```
roslaunch sg_bot sg_world.launch
roslaunch sg_bot amcl.launch
rosrun sg_bot navigation_goal
```

## Refer project Report 'Where_Am_I - SG Ver 1.0.pdf' for technical details ##