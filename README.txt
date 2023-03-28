segwayrmp version 1.0 27/03/2023

Description:
segwayrmp provides a ROS interface (Noetic) to Segway Robotics Mobility Platforms. 
It consists of different packages whose purpose is described below:
  - rmp_base: controls the base and publishes sensor data and status related information 
  - rmp_teleop: provides a joystick interface to control the base
  - rmp_description: provides a URDF (http://wiki.ros.org/urdf) description of the platform(s) 
  - rmp_msgs: defines RMP sepecific messages

Requirements:
  - ROS  Noetic musts be installed 

Installation:
  - cd to the segwayrmp directory
  - update your shell with your ros environment configuration: source /path/to/ros/install/setup.bash (typically /opt/ros/hydro/setup.bash)
  - catkin_make --source segwayrmp

Usage:
  - check that everything is properly connected :-)
  - edit the launch files according to your rmp/joystick setup
  - source the setup file from the devel directory, for example source devel/setup.bash
  - start the base node: roslaunch rmp_base rmp440le.launch
  - start the joystick: roslaunch rmp_teleop joystick.launch
