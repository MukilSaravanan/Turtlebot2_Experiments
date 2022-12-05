# Moving Forward
Here the turtlebot 2 moves ahead with a constant velocity fed to it as an input. In this case the robot moves ahead with a velocity of 0.2m/s. 

<p align="center"><img width="500" src="https://user-images.githubusercontent.com/44544565/205492189-238595c8-9f4b-48d9-9597-963dd0b68ed6.png">
</p>
This graph explains the linear velocity vs time. A noticeable period of time lag is observed before the robot reaches its constant linear velocity (cmd_vel_mux) here. The robot takes about 10 seconds before it attains its constant velocity of 0.2m/s. On ending the movement of the robot we see that a constant horizontal line at 0m/s is observed clearly.

<p align="center"><img width="500" src="https://user-images.githubusercontent.com/44544565/205493656-7be0663f-7190-402d-a893-0160de2d90ad.PNG"</p>

A noticeable angular velocity spike is observed over time indicating the presence of an angular velocity component involved in the robot's motion while moving forward with a constant velocity.


<p align="center"><img width="500" src="https://user-images.githubusercontent.com/44544565/205493661-4ec01163-fd5f-4911-b329-67c956b41eee.PNG"</p>

This plot clearly indicates the deviation of the robot from a straight line . A cause for this is the angular velocity component of the robot present during its motion . The presence of specified control strategy (position control) done by wheel encoder accompanied with the algorithm helps solve this issue.

<p align="center"><img width="500" src="https://user-images.githubusercontent.com/44544565/205493665-3640c1e1-7782-4779-95c4-4b0a4a1aa406.PNG"</p>

Figure above indicates the change of yaw rate over time. This is a crucial factor in assessing why the deviation occurs when a robot is moving in a straight path with a constant velocity. This factor contributes to the robot deviation in the xy path from its prescribed initial path.

<p align="center"><img width="500" src="https://user-images.githubusercontent.com/44544565/205493621-3c3489d1-2fcf-4962-aa76-72143494bae8.PNG"</p>


## [Experimentation video]()
-----------------------------------------------------------------------

<div align="center">
  <a href="https://youtu.be/qO01RvUsOIg"> <img width="550" src="https://user-images.githubusercontent.com/44544565/205532435-c13a20d1-0f8c-4af3-a369-5089b18bb3bd.png" alt="Experimentation video"></a>
</div>

