## Navigating TurtleBot 2
For any mobile device, the ability to navigate in its environment is important. Avoiding dangerous situations such as collisions and
unsafe conditions comes in line of priority. This experiment will present an overview of the skill of navigation.

In order to navigate in its environment, the robot or any other mobility device requires representation, i.e. a map of the environment and the ability  to interpret that representation.

```
$ roslaunch turtlebot_gazebo turtlebot_world.launch
```
If this command gives you an error, add the following line to your .bashrc file:
```
export TURTLEBOT_3D_SENSOR=astra
```
```
$ roslaunch turtlebot_rviz_launchers view_navigation.launch
```
The rviz window should appear.


Click the 2DPose Nav button on the top toolbar of rviz and then click on the location on the map where TurtleBot should be located. Orient the large green arrow by dragging the cursor in the direction TurtleBot is facing.

![Screenshot from 2022-12-04 23-05-34](https://user-images.githubusercontent.com/44544565/205489845-12a868e8-5e4f-4a38-b96b-7002bc293a0b.png)


To get TurtleBot to navigate autonomously across the map, click on the 2D Nav Goal button and click on the map location where you want TurtleBot to go and drag the green arrow in the direction TurtleBot should be facing when he reaches that location.

![Screenshot from 2022-12-04 23-05-25](https://user-images.githubusercontent.com/44544565/205489857-34b92296-cd54-4dad-a263-0ecd7ce7c2b8.png)

## Graphical Representation

<p align="center"><img width="600" src="https://user-images.githubusercontent.com/44544565/205494869-7b33c090-4af5-462d-8129-80406a178353.PNG"></p>
<h3 align="center">Angular vel. vs. Time</h3> 

<p align="center"><img width="600" src="https://user-images.githubusercontent.com/44544565/205494872-019316d9-02e5-4258-be11-f93798e7af7a.PNG"></p>
<h3 align="center">Linear vel. vs. Time</h3> 

<p align="center"><img width="600" src="https://user-images.githubusercontent.com/44544565/205494875-9bc37076-dfb1-406d-aa84-2386d820b6ce.PNG"></p>
<h3 align="center">X - Y position</h3> 

<p align="center"><img width="600" src="https://user-images.githubusercontent.com/44544565/205494878-aa08cc62-cbf1-4936-9807-19ef614d1af0.PNG"></p>
<h3 align="center">Yaw vs. Time</h3> 
