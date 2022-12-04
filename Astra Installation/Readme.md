# Astra Installation

Astra is a powerful and reliable stand-alone 3D camera featuring Orbbec's proprietary 3D microchip and VGA color. It has been developed to be highly compatible with existing OpenNI applications. Astra has a range of 0.4 to 8 meters. In addition to its cliff sensors and bumpers, Astra is one of the ways TurtleBot _sees_ its environment.

<p align="center">
  <img width="500" src="https://user-images.githubusercontent.com/44544565/205486652-a231efbc-cf9e-468b-9248-e0d3b9ddf388.jpeg" title="Orbnec Astra camera module"</p>

## Drivers Installation

This package supports ROS Kinetic and Melodic.\

### Install ROS
refer to [ROS wiki][]
Install dependencies

```
sudo apt install ros-**-rgbd-launch ros-**-libuvc ros-*-libuvc-camera ros-*-libuvc-ros\
```
** - defines ROS distribution

### Create a ROS Workspace(if you don't have one)\
```
mkdir -p /catkin_ws/src\
```
### Pull the repository into your ROS workspace\
```
git clone https://github.com/orbbec/ros_astra_camera\
```
### Create astra udev ruleroscd astra_camera\
```
./scripts/create_udev_rules\
```
Go to catkin workspace and compile astra_camera/catkin_ws\
```
catkin_make --pkg astra_camera\
```
