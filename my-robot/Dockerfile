FROM ros:noetic

# Install required packages
RUN apt update && apt install -y \
    ros-noetic-joint-state-publisher \
    ros-noetic-robot-state-publisher \
    ros-noetic-rviz \
    ros-noetic-xacro \
    ros-noetic-tf2-ros \
    && rm -rf /var/lib/apt/lists/*

# Copy your robot files
WORKDIR /home/ros/catkin_ws
COPY ./my-robot ./urdf
COPY ./launch ./launch

# Source ROS
CMD ["roslaunch", "launch/robot.launch"]