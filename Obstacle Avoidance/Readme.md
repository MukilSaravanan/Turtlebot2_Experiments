# Obstacle avoidance

Obstacle avoidance is an intelligent machanism that can automatically senses the obstacle in front of it's view psotion and avoid them by traversing in another direction. This mechanism allows the robot to navigate in an unknown environment by avoiding collisions, which is a primary requirement for any autonomous mobile robot.

Obstacle avoidance is also the task of satisfying some control objective subject to non-intersection or non-collision position constraints. 

## Obstacle avoidance with Obstacles
The obstacle avoidance is executed using a structure of path finding, local planner and localization algorithms. Here the robot uses A-star algorithm for for local planner and Dynamic window(DW) planning for executing **cmd_vel** (Command velocity) messages for communication. Initially the robot detect the obstacles on the path and plans accordingly.

<p align="center"><img width="600" src="https://user-images.githubusercontent.com/44544565/205494844-1e727b21-786a-4549-9981-c585f9bbee06.PNG"></p>
<h3 align="center">Angular vel. vs. Time</h3> 

<p align="center"><img width="600" src="https://user-images.githubusercontent.com/44544565/205494847-2036e886-f7f7-4dfd-be13-08ea11b699db.PNG"></p>
<h3 align="center">Linear vel. vs. Time</h3> 

<p align="center"><img width="600" src="https://user-images.githubusercontent.com/44544565/205494850-c278ee33-06fe-4aa8-aca1-874e776188f5.PNG"></p>
<h3 align="center">X - Y position</h3> 

<p align="center"><img width="600" src="https://user-images.githubusercontent.com/44544565/205494853-919a6bbe-2af6-4a88-a974-afa517e83b9b.PNG"></p>
<h3 align="center">Yaw vs. Time</h3> 

## Obstacle avoidance without Obstacles
The obstacle avoidance is executed using a structure of path finding, local planner and localization algorithms. Here the robot uses A-star algorithm for for local planner and Dynamic window(DW) planning for executing **cmd_vel** (Command velocity) messages for communication.

<p align="center"><img width="600" src="https://user-images.githubusercontent.com/44544565/205494869-7b33c090-4af5-462d-8129-80406a178353.PNG"></p>
<h3 align="center">Angular vel. vs. Time</h3> 

<p align="center"><img width="600" src="https://user-images.githubusercontent.com/44544565/205494872-019316d9-02e5-4258-be11-f93798e7af7a.PNG"></p>
<h3 align="center">Linear vel. vs. Time</h3> 

<p align="center"><img width="600" src="https://user-images.githubusercontent.com/44544565/205494875-9bc37076-dfb1-406d-aa84-2386d820b6ce.PNG"></p>
<h3 align="center">X - Y position</h3> 

<p align="center"><img width="600" src="https://user-images.githubusercontent.com/44544565/205494878-aa08cc62-cbf1-4936-9807-19ef614d1af0.PNG"></p>
<h3 align="center">Yaw vs. Time</h3> 
