# ati_sensor
Package for publishing ATI Force Torque sensor measurements to ROS.

REQUIREMENTS
CMAKE VERSION > 3.11
Compile and install jsd from https://github.com/nasa-jpl/jsd. Installation will be done at /opt/jsd. Tested with version 2.3.10.

FOR ATI SENSOR
sudo ./devel/lib/ati_sensor/ati_sensor eno1 1 1000 0

FOR ATI ROS
sudo su
source /opt/ros/noetic/setup.bash
rosrun/roslaunch ati_ros

FOR FASTER SOEM operation
sudo ethtool -C eno1 rx-usecs 0 rx-frames 1 tx-usecs 0 tx-frames 1


