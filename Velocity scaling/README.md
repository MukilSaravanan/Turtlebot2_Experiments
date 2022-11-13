# Moving Forward with a Specific Velocity

Here the turtlebot 2 moves ahead with a constant velocity fed to it as an input. In this case the robot moves ahead with a velocity of 0.2m/s. 

Graphs

This graph explains the linear velocity vs time. A noticeable period of time lag is observed before the robot reaches its constant linear velocity (cmd_vel_mux) here. The robot takes about 10 seconds before it attains its constant velocity of 0.2m/s. On ending the movement of the robot we see that a constant horizontal line at 0m/s is observed clearly.


A noticeable angular velocity spike is observed over time indicating the presence of an angular velocity component involved in the robot's motion while moving forward with a constant velocity.



This plot clearly indicates the deviation of the robot from a straight line . A cause for this is the angular velocity component of the robot present during its motion . The presence of specified control strategy (position control) done by wheel encoder accompanied with the algorithm helps solve this issue.



Figure above indicates the change of yaw rate over time. This is a crucial factor in assessing why the deviation occurs when a robot is moving in a straight path with a constant velocity. This factor contributes to the robot deviation in the xy path from its prescribed initial path.
