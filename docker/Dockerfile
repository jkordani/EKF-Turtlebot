FROM ubuntu:16.04
ENV export DEBIAN_FRONTEND=noninteractive
RUN sh -c 'echo "deb http://packages.ros.org/ros/ubuntu $(lsb_release -sc) main" > /etc/apt/sources.list.d/ros-latest.list'; apt update && apt install -y curl && curl -s https://raw.githubusercontent.com/ros/rosdistro/master/ros.asc | apt-key add - && apt update && apt install -y ros-kinetic-desktop-full && rm -rf /var/lib/apt/lists/*

RUN apt update && apt install gazebo7 && rm -rf /var/lib/apt/lists/*
