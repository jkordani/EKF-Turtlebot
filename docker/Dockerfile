FROM ros:kinetic
ENV export DEBIAN_FRONTEND=noninteractive
RUN apt update &&  apt install -y \
    ros-kinetic-desktop-full gazebo7 \
    && rm -rf /var/lib/apt/lists/*

RUN apt update && apt install -y \
    python-catkin-tools \
    build-essential \
    ros-kinetic-robot-pose-ekf \
    && rm -rf /var/lib/apt/lists/*

RUN adduser --gecos "" --disabled-password user && echo "user:user" | chpasswd
RUN usermod -aG sudo user
