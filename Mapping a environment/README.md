# Mapping the environment

This experiment shows how to build a map which lets the robot remember the environment. TurtleBot can autonomously navigate around using the map.

### 1. Creating a Map
Create a folder for maps
```
mkdir ~/turtlebot_custom_maps 
```
### 2. Launch Gazebo world
```
roslaunch turtlebot_gazebo turtlebot_world.launch
```

### 3. Start map building
```
roslaunch turtlebot_gazebo gmapping_demo.launch
```

### 4. Use Rviz to visualize the map building process.
```
roslaunch turtlebot_rviz_launchers view_navigation.launch
```

### 5. Change the option.
Local map->Costmap->Topic (choose /map from drop-down list).

### 6. Change the option.

Global map->Costmap->Topic (choose /map from drop-down list)

### 7. Launch teleop.
```
roslaunch turtlebot_teleop keyboard_teleop.launch
```

### 8. Drive the TurtleBot around.
NOTE: The terminal with teleop launching has to be active all the time otherwise you won’t be able to operate the TurtleBot.

<<<<<<< Updated upstream
<p align="center">
<img width="750" alt="mapping1" src="https://user-images.githubusercontent.com/44544565/201525126-76d40dc1-cdc7-4d6e-9f57-a8943de7d14c.png">
</p>

=======
<p align ="center">
  <img width="600" height="400" src="resources/mapping_env/mapping1.png">
</p>

![Resource](resources/img/turtlebot_resized.png)

>>>>>>> Stashed changes
### 9. Save a map when the picture is good enough.

```
rosrun map_server map_saver -f /home/<user_name>/turtlebot_custom_maps/tutorial
```

## Testing the Newly Created Map
We can test the result of our work.
### 1. Launch Gazebo
```
roslaunch turtlebot_gazebo turtlebot_world.launch
```

### 2. Launch navigation demo
```
roslaunch turtlebot_gazebo amcl_demo.launch map_file:=/home/<user_name>/turtlebot_custom_maps/tutorial.yaml
```
You can launch the default map for playground world if you have not your own map
Run this command:
```
roslaunch turtlebot_gazebo amcl_demo.launch
```

### 3. Launch Rviz
```
roslaunch turtlebot_rviz_launchers view_navigation.launch
```

### 4. If you see a picture like this then creating the map has been realized successfully
<p align="center">
<img width="750" alt="Screenshot 2022-11-13 at 7 25 19 PM" src="https://user-images.githubusercontent.com/44544565/201525520-9e927a50-103f-4e0f-a3a0-ed26137f13d1.png">
</p>

### 5. Interrupt processes and close the terminals
-------------
## Implementation
[![Implementation](https://i9.ytimg.com/vi_webp/Z2DBJi2g5F4/mq1.webp?sqp=CJCvw5sG-oaymwEmCMACELQB8quKqQMa8AEB-AH-CYAC0AWKAgwIABABGFQgZShiMA8=&rs=AOn4CLD9oYh0rdEixRnDkWPinEnblsRZSw)](https://youtu.be/Z2DBJi2g5F4)
<<<<<<< Updated upstream
=======

>>>>>>> Stashed changes
