# Velocity scaling

Here the turtlebot 2 moves ahead with a constant velocity fed to it as an input. In this case the robot moves ahead with a velocity of 0.2m/s. 

Graphs
<p align="center">
<img width="500" src="https://user-images.githubusercontent.com/44544565/205487707-396a08c3-90b0-4aa0-b440-abaf8bf7aa19.png"></p>


This graph explains the linear velocity vs time. A noticeable period of time lag is observed before the robot reaches its constant linear velocity (cmd_vel_mux) here. The robot takes about 10 seconds before it attains its constant velocity of 0.2m/s. On ending the movement of the robot we see that a constant horizontal line at 0m/s is observed clearly.

<p align="center"><img width="500" src="https://user-images.githubusercontent.com/44544565/205487722-2e43765f-7797-402e-af61-5d7d12618ff9.png"></p>


A noticeable angular velocity spike is observed over time indicating the presence of an angular velocity component involved in the robot's motion while moving forward with a constant velocity.

<p align="center"><img width="500" src="https://user-images.githubusercontent.com/44544565/205487785-47a34c7a-1d93-4af8-bc5d-9c64c2f9d625.png"></p>



This plot clearly indicates the deviation of the robot from a straight line . A cause for this is the angular velocity component of the robot present during its motion . The presence of specified control strategy (position control) done by wheel encoder accompanied with the algorithm helps solve this issue.

<p align="center"><img width="500" src="https://user-images.githubusercontent.com/44544565/205487788-fc03c438-07e9-454d-87b6-b1b70302c751.png"></p>


Figure above indicates the change of yaw rate over time. This is a crucial factor in assessing why the deviation occurs when a robot is moving in a straight path with a constant velocity. This factor contributes to the robot deviation in the xy path from its prescribed initial path.


<p align="center"><img width="500" src="https://user-images.githubusercontent.com/44544565/205487410-2eb74600-ce49-4717-801a-dbbd4cfa3ffd.png"></p>

<p align="center">command line interface of velocity scaling</p>
