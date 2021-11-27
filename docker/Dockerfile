FROM ros:kinetic
ENV export DEBIAN_FRONTEND=noninteractive
RUN apt update && apt upgrade -y && \
    apt install -y ros-kinetic-desktop-full gazebo7 python-catkin-tools && \
    rm -rf /var/lib/apt/lists/*
