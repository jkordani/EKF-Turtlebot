Since rosdep didn't work, I had to install these packages manually

on Ubuntu 16.04

apt install -y gazebo7 python-catkin-tools ros-kinetic-robot-pose-ekf build-essential ros-kinetic-joy* ros-kinetic-turtlebot-*

then roslaunch main main.launch

You'll have to edit the launch files for the paths to the rviz config files.
