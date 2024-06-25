# ROS-noetic-drone
# Prerequisites
Ubuntu 20.04
ROS Noetic installed and configured
Git for cloning repositories
# Steps to Set Up the Project
Clone the Repository:
git clone -b noetic https://github.com/your-repo/sjtu_drone.git
Create a Catkin Workspace:
mkdir -p ~/catkin_ws/src
cd ~/catkin_ws/src
ln -s ~/path_to_sjtu_drone/sjtu_drone .
cd ~/catkin_ws
catkin_make
Source the Setup File:
source ~/catkin_ws/devel/setup.bash
Launch the Drone:
roslaunch sjtu_drone start.launch
# Project Structure
src/: Contains the source code for the drone.
include/: Header files for the project.
launch/: Launch files to start the ROS nodes.
models/: 3D models and URDF files for the drone.
CMakeLists.txt: Build configuration.
package.xml: Package configuration.
