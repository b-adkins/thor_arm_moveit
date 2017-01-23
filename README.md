# thor_arm_moveit
ROS MoveIt configuration for Thor open source robot arm

# Required packages
- [Robot Operating System](http://www.ros.org/)
- [MoveIt](http://moveit.ros.org/)
- [thor_arm_description](https://github.com/b-adkins/thor_arm_description)

(Developed on Ubuntu 14.04, ROS Indigo, and MoveIt 0.7.5. Will probably work with newer versions.)

# Installation instructions
- Install ROS packages
```sh
 apt-get install ros-indigo-desktop ros-indigo-moveit-ros
```
- [Create a catkin workspace](http://wiki.ros.org/catkin/Tutorials/create_a_workspace)
- Git clone this repository into the "src" directory. Repeat for thor_arm_description
- Build
```sh
cd [catkin_workspace_root]
catkin_make
```
Set up environment
```sh
# Add this line $HOME/.bashrc to add this to all your environments
source [catkin_workspace_root]/devel/setup.sh
```
# Demo instructions
   
- Launch the MoveIt demo:
```sh
roslaunch thor_arm_moveit demo.launch
```
- Drag the end-effector position and orientation sliders. Have fun!
