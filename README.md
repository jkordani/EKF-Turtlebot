Since rosdep didn't work, I had to install these packages manually

on Ubuntu 16.04

apt install -y gazebo7 python-catkin-tools ros-kinetic-robot-pose-ekf build-essential ros-kinetic-joy* ros-kinetic-turtlebot-*

then roslaunch main main.launch

You'll have to edit the launch files for the paths to the rviz config files.

There is a Dockerfile to get this all set up for you. But I've found that the gazebo ros plugin crashes on my machine.  Anyways...

alias udacity='docker run -e DISPLAY -e QT_X11_NO_MITSHM=1 -v ~/.Xauthority:/home/user/.Xauthority --net host -v /path/to/workspace:/local -u user -it --rm udacity:latest /bin/bash'

