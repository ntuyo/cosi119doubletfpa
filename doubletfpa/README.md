# Nazari's Double TF PA

The doubletf pa demonstrates a quick understanding on how to create new frames, as well as utilizing tf, broadcasters, and listerners in ROS.

## How to run it:

Navigate to the doubletfpa folder, and run 

```bash
roslaunch doubletfpa tf2_pa.launch
```

## What is TF? How is it used in this PA?

TF has static broadcasters, broadcasters, listeners and frames. In this project, listeners, broadcasters, and frames are used. Broadcasters publish transforms similarly to static broadcasters - they publish the changing coordinates of the robot. Listeners are what actually allow tf to be used, and in this PA it accesses the frame transformations published by the broadcasters. 

The turtle_tf2_listener listens for transformations from 'turtle'. The broadcaster publishes information 'turtles' current pose, which is controlled by the keyboard and can change rapidly. This is then recieved and interpreted by the listener, which controls the second, third, and fourth turtle.

## Youtube Video: 
https://youtu.be/9SpmwAsJagM