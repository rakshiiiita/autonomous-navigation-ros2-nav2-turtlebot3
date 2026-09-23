# Autonomous Navigation using ROS 2 Nav2 and TurtleBot3

## Overview

This is an academic robotics project completed as part of the Robot System Design and SLAM practical course.

The project demonstrates autonomous point-to-point navigation of a TurtleBot3 Burger in a simulated environment using the ROS 2 Navigation (Nav2) stack.

## Objectives

- Load and use a saved occupancy-grid map.
- Localize the robot using AMCL.
- Plan a collision-free global path.
- Send navigation goals through RViz2.
- Understand global and local path planning.
- Observe obstacle inflation using the costmap.
- Test navigation recovery behavior.
- Verify navigation using action feedback.

## Technologies Used

- ROS 2
- Nav2
- TurtleBot3 Burger
- RViz2
- AMCL
- A* Global Planner
- DWB Local Controller
- Costmap
- Gazebo / Simulation

## Navigation Workflow

The navigation process follows:

Map → Localization → Global Planning → Local Control → Goal

The robot uses the saved occupancy-grid map to understand the environment, AMCL for localization, a global planner for generating a path, and a local controller for executing the path while considering obstacles.

## Key Concepts

### AMCL
Adaptive Monte Carlo Localization is used to estimate the robot's position on the known map.

### Global Planning
A global planner generates a collision-free path from the robot's current position to the target position.

### Local Control
The local controller generates velocity commands that allow the robot to follow the planned path while responding to nearby obstacles.

### Costmap
The costmap represents obstacles and their surrounding regions. Obstacle inflation helps maintain a safe distance from obstacles.

## Result

The TurtleBot3 was configured for autonomous point-to-point navigation in the simulated environment. Navigation goals were provided through RViz2 and the robot's navigation behavior was observed and verified.

## Academic Context

Course: Robot System Design and SLAM

Experiment: 7

Project Type: Academic Practical

## Author

Rakshita Dhaketa

B.Tech Robotics and Automation  
Medi-Caps University
