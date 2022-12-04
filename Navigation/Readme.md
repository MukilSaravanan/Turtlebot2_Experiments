For any mobile device, the ability to navigate in its environment is important. Avoiding dangerous situations such as collisions and 
unsafe conditions comes in line of priority. This experiment will present an overview of the skill of navigation and try to identify the basic blocks of a robot navigation system, types of navigation systems, and closer look at its related building components.

In order to navigate in its environment, the robot or any other mobility device requires representation, i.e. a map of the environment and the ability  to interpret that representation.

## Navigating TurtleBot 2

$ roslaunch turtlebot_gazebo turtlebot_world.launch

If this command gives you an error, add the following line to your .bashrc file:
```
export TURTLEBOT_3D_SENSOR=astra
```

In a second terminal window, start the amcl operation:
```
$ roslaunch turtlebot_gazebo amcl_demo.launch
map_file:=/<pwd_path_to_files>/simulation_map.yaml
```
Look for the following text on your window: _odom received!_

Open another terminal window and view navigation on rviz:
```
$ roslaunch turtlebot_rviz_launchers view_navigation.launch
The rviz window should appear.
```

Orient the rviz map to align with the Gazebo World!
TurtleBot should be told its current location on the map as it corresponds to the Gazebo environment. 

Click the 2DPose Estimate button on the top toolbar of rviz and then click on the location on the map where TurtleBot should be located. Orient the large green arrow by dragging the cursor in the direction TurtleBot is facing.

To get TurtleBot to navigate autonomously across the map, click on the 2D Nav Goal button and click on the map location where you want TurtleBot to go and drag the green arrow in the direction TurtleBot should be facing when he reaches that location.

In the first terminal window, type the command:
```
$ roslaunch turtlebot_gazebo turtlebot_world.launch
```
Open another terminal window, check the initial pose of TurtleBot:
```
$ rostopic echo /odom/pose/pose -n1
```
