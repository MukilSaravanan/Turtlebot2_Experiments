{\rtf1\ansi\ansicpg1252\cocoartf2706
\cocoatextscaling0\cocoaplatform0{\fonttbl\f0\fswiss\fcharset0 Helvetica;}
{\colortbl;\red255\green255\blue255;}
{\*\expandedcolortbl;;}
\paperw11900\paperh16840\margl1440\margr1440\vieww11520\viewh8400\viewkind0
\pard\tx566\tx1133\tx1700\tx2267\tx2834\tx3401\tx3968\tx4535\tx5102\tx5669\tx6236\tx6803\pardirnatural\partightenfactor0

\f0\fs24 \cf0 -# Astra Installation\
\
Astra is a powerful and reliable stand-alone 3D camera featuring Orbbec's proprietary 3D microchip and VGA color. It has been developed to be highly compatible with existing OpenNI applications. Astra has a range of 0.4 to 8 meters. In addition to its cliff sensors and bumpers, Astra is one of the ways TurtleBot _sees_ its environment. \
\
## Drivers Installation\
\
This package supports ROS Kinetic and Melodic.\
\
### Install ROS\
refer to [ROS wiki][]\
Install dependencies \
\
```\
sudo apt install ros-**-rgbd-launch ros-**-libuvc ros-*-libuvc-camera ros-*-libuvc-ros\
```\
** - defines ROS distribution\
\
### Create a ROS Workspace(if you don't have one)\
```\
mkdir -p /catkin_ws/src\
```\
### Pull the repository into your ROS workspace\
```\
git clone https://github.com/orbbec/ros_astra_camera\
```\
### Create astra udev ruleroscd astra_camera\
```\
./scripts/create_udev_rules\
```\
Go to catkin workspace and compile astra_camera/catkin_ws\
```\
catkin_make --pkg astra_camera\
```}