# program-robots-with-ros

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
the try to install the module:
```
(_venv_py2.7) $ pip install pyside2
```
