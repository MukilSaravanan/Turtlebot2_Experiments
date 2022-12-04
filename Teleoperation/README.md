# Teleoperation
- Teleoperation allows you to manually control TurtleBot. Keyboard and joystick are the two primary ways to do this. Before we experiment with these two methods, we need to set up TurtleBot to receive our commands.
- Make sure TurtleBot’s Kobuki base is turned on (on/off switch is on the side).

<p align="center">
<img width ="450" alt="screenshot" src="https://user-images.githubusercontent.com/44544565/201526105-3ec7328c-13ba-4760-bb2e-efb7b5981ae9.jpeg">
</p>


- The Kobuki base status light will turn green if you have sufficient battery power.
<p align="center">
<img width ="450" alt="screenshot1" src="https://user-images.githubusercontent.com/44544565/201526522-5030b9e2-36bd-430e-8337-7d6602c49a0a.JPG">
</p>

- On starting the turtlebot 2 a chime would be heard. This indicates that the Kobuki base of the turtlebot2 is booting up. Once booting is completed , Open another terminal tab and run:

```
roslaunch turtlebot_teleop keyboard_teleop.launch
```

------------------------
## Implementation
![Video](https://youtu.be/9U_yMXyyd2g)
