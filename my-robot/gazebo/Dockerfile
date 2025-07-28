FROM osrf/ros:noetic-desktop-full

# Install Ignition Fortress + Web
RUN apt update && apt install -y \
    ignition-fortress \
    ignition-fortress-web \
    && rm -rf /var/lib/apt/lists/*

# Run gzserver and web bridge
CMD ["bash", "-c", "ign gazebo -v 4 --gui-server & ign gazebo-web"]FROM osrf/ros:noetic-desktop-full

# Install Ignition Fortress + Web
RUN apt update && apt install -y \
    ignition-fortress \
    ignition-fortress-web \
    && rm -rf /var/lib/apt/lists/*

# Run gzserver and web bridge
CMD ["bash", "-c", "ign gazebo -v 4 --gui-server & ign gazebo-web"]