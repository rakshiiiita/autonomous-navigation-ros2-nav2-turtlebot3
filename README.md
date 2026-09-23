# Autonomous Navigation using ROS 2 Nav2 and TurtleBot3

## 📌 Overview

This project demonstrates autonomous point-to-point navigation of a TurtleBot3 Burger using the ROS 2 Navigation (Nav2) stack in a simulated environment.

The work was completed as an academic practical for the Robot System Design and SLAM course. The experiment focuses on robot localization, path planning, obstacle avoidance, costmaps, and autonomous navigation using RViz2 and Gazebo.

---

## 🎯 Objectives

- Perform autonomous navigation of a TurtleBot3 Burger.
- Load and use an occupancy-grid map.
- Localize the robot using AMCL.
- Generate a global navigation path.
- Execute the path using a local controller.
- Send navigation goals through RViz2.
- Understand costmaps and obstacle inflation.
- Observe the robot navigating toward a specified goal.
- Verify successful goal achievement.

---

## 🛠️ Technologies Used

- ROS 2
- Nav2
- TurtleBot3 Burger
- RViz2
- Gazebo
- AMCL
- A* Global Planner
- DWB Local Controller
- Costmaps
- Occupancy Grid Map

---

## 🤖 Navigation Pipeline

```text
        Map
         ↓
   AMCL Localization
         ↓
 Global Path Planning
         ↓
   Local Controller
         ↓
 Obstacle Avoidance
         ↓
    Navigation Goal
