# TurtleBot3 ROS2 Simulation Setup

## System Information
- **OS:** Ubuntu 22.04 LTS
- **ROS2 Version:** Humble

## Team Members
- LUQMAN HAKIM BIN ZULKIFLI

## Installation Commands
sudo apt update && sudo apt upgrade -y
sudo apt install ros-humble-desktop -y
echo "source /opt/ros/humble/setup.bash" >> ~/.bashrc
source ~/.bashrc
sudo apt install -y ros-humble-gazebo-ros-pkgs ros-humble-gazebo-ros
sudo apt install -y ros-humble-turtlebot3* ros-humble-turtlebot3-simulations
echo "export TURTLEBOT3_MODEL=burger" >> ~/.bashrc
source ~/.bashrc
ros2 launch turtlebot3_gazebo turtlebot3_world.launch.py
rviz2
ros2 run turtlebot3_teleop teleop_keyboard
ros2 topic list

### 1. Issues
1. old laptop cannot run gazebo on ros humble.
2. currently using personal laptop that has GPU driver. Storing Ubuntu in external hard drive
