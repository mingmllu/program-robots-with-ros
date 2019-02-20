# program-robots-with-ros

## Installations
```
$ sudo apt-get install ros-kinetic-turtlebot-gazebo
```
```
$ pip install defusedxml
```
```
export TURTLEBOT_GAZEBO_WORLD_FILE=/opt/ros/kinetic/share/turtlebot_gazebo/worlds/playground.world

roslaunch turtlebot_gazebo turtlebot_world.launch
```

```
sudo apt-get install ros-kinetic-turtlebot*
```
```
source ~/.bashrc
```
If you got errors about PyQt5 module:
```
ImportError: Could not find Qt binding (looked for: 'pyqt', 'pyside'):
  ImportError for 'pyqt': No module named PyQt5.QtCore
```
then try to install the module:
```
(_venv_py2.7) $ pip install pyside2
```

## [Visulization of Velodyne bag data](http://wiki.ros.org/velodyne/Tutorials/Getting%20Started%20with%20the%20Velodyne%20VLP16)

Steps:
* Start up ROS Master: ```$ roscore```
* Play back ros bag data: ```$ rosbag play -l PATH/TO/BAG_DATA``` where the loop playback option -l used in case the duration of bag data is too short
* In a new terminal, run ```$ rosrun rviz rviz -f velodyne```. It is critical to set fixed frame to ```velodyne```
[Screenshot](fixed_frame_velodyne.png)
