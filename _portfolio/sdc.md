---
title: "Self Driving Car Specialization, Coursera"
permalink: "/portfolio/sdc"
layout: "single"
date: 2020-03-11
toc: true
toc_label: "Contents"
---

This Specialization gives you a comprehensive understanding of state-of-the-art engineering practices used in the self-driving car industry. By interacting with real data sets from an autonomous vehicle (AV), you’ll implement methods for static and dynamic object detection, localization and mapping, behaviour and maneuver planning, and vehicle control ― all through hands-on projects using the open source simulator CARLA. You’ll learn from a highly realistic driving environment that features 3D pedestrian modeling and environmental conditions. When you complete the Specialization successfully, you’ll be able to build your own self-driving software stack and be ready to apply for jobs in the autonomous vehicle industry.


# Introduction to Self-Driving Cars
This course will introduce you to the terminology, design considerations and safety assessment of self-driving cars. By the end of this course, you will be able to:

- Understand commonly used hardware used for self-driving cars
- Identify the main components of the self-driving software stack
- Program vehicle modelling and control
- Analyze the safety frameworks and current industry practices for vehicle development

For the final project in this course, you will develop control code to navigate a self-driving car around a racetrack in the CARLA simulation environment. You will construct longitudinal and lateral dynamic models for a vehicle and create controllers that regulate speed and path tracking performance using Python. You’ll test the limits of your control design and learn the challenges inherent in driving at the limit of vehicle performance.

## Final Project

![](/images/projects/sdc/intro.png)
![](/images/projects/sdc/intro2.png)
<iframe src="https://drive.google.com/file/d/1_8cezxhPAS0KNAQ62mf8u1xVuv92Oafo/preview" width="768" height="432" allowfullscreen></iframe>

# State Estimation and Localization for Self-Driving Cars
This course will introduce you to the different sensors and how we can use them for state estimation and localization in a self-driving car. By the end of this course, you will be able to:

- Understand the key methods for parameter and state estimation used for autonomous driving, such as the method of least-squares
- Develop a model for typical vehicle localization sensors, including GPS and IMUs
- Apply extended and unscented Kalman Filters to a vehicle state estimation problem
- Understand LIDAR scan matching and the Iterative Closest Point algorithm
- Apply these tools to fuse multiple sensor streams into a single state estimate for a self-driving car

For the final project in this course, you will implement the Error-State Extended Kalman Filter (ES-EKF) to localize a vehicle using data from the CARLA simulator.

## Final Project

![](/images/projects/sdc/state_estimation.png)
![](/images/projects/sdc/state_estimation2.png)

# Motion Planning for Self-Driving Cars
This course will introduce you to the main planning tasks in autonomous driving, including mission planning, behavior planning and local planning. By the end of this course, you will be able to find the shortest path over a graph or road network using Dijkstra’s and the A* algorithm, use finite state machines to select safe behaviors to execute, and design optimal, smooth paths and velocity profiles to navigate safely around obstacles while obeying traffic laws. You’ll also build occupancy grid maps of static elements in the environment and learn how to use them for efficient collision checking. This course will give you the ability to construct a full self-driving planning solution, to take you from home to work while behaving like a typical driving and keeping the vehicle safe at all times. For the final project in this course, you will implement a hierarchical motion planner to navigate through a sequence of scenarios in the CARLA simulator, including avoiding a vehicle parked in your lane, following a lead vehicle and safely navigating an intersection. You’ll face real-world randomness and need to work to ensure your solution is robust to changes in the environment.

## Final Project
![](/images/projects/sdc/course4.jpg)
<iframe src="https://drive.google.com/file/d/1Xz3LWEFMwP3UAjFFc3YJslhbrrwK_NYb/preview" width="768" height="432" allowfullscreen></iframe>