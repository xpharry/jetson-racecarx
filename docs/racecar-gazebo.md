# Run racecar simulator in Gazebo

## Packages

- racecar: git clone https://github.com/mit-racecar/racecar.git
- racecar-gazebo: git clone https://github.com/mit-racecar/racecar_gazebo.git

## Dependencies

- tf2_geometry_msgs
- ackermann_msgs
- joy
- map_server

Install by running

```
sudo apt-get install ros-kinetic-tf2-geometry-msgs ros-kinetic-ackermann-msgs ros-kinetic-joy ros-kinetic-map-server
```

## Installation

To install the packages, clone them into your catkin workspace:

```
cd ~/catkin_ws/src
git clone https://github.com/mit-racecar/racecar.git
git clone https://github.com/mit-racecar/racecar_gazebo.git
```

Then run catkin_make to build them:

```
cd ~/catkin_ws
catkin_make
source devel/setup.bash
```

## Quick Start

Simulates an RC car in the MIT tunnel.

Run

```
roslaunch racecar_gazebo racecar.launch
```

or

```
roslaunch racecar_gazebo racecar_tunnel.launch
```
