# Localization Package for ROS 2

The Localization package for ROS 2 provides functionality for localizing a robot within its environment. It includes several scripts for different tasks related to localization:

## Scripts

### controller

This script receives a set point and implements a proportional controller to guide the robot to the desired point published on the `/set_point` topic.

### coordinate_transform

The `coordinate_transform` script transforms positions so that they can be visualized accurately in RViz.

### joint_states

The `joint_states` script simulates the movement of the robot's wheels.

### Kinematic_model

The `Kinematic_model` script publishes the velocities of the robot's wheels and its pose.

### localization

The `localization` script calculates odometry to estimate the robot's position.

## Running the Package

To run the package, follow these steps:

1. Launch the `puzzlebot_rviz.launch.py` launch file.
   ```
   ros2 launch localization puzzlebot_rviz.launch.py
   ```
2. Send a point to /set_point topic of type Pose to specify the desired location for the robot.
## Demostration
[![Demo del Proyecto](http://img.youtube.com/vi/3rQhMq-2rSc/0.jpg)](https://www.youtube.com/watch?v=3rQhMq-2rSc)
