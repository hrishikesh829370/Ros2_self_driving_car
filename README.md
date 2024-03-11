# Ros2_self_driving_car


Ros2_Self-Driving_Car

This project implements a Level 3 self-driving car using OSRF packages within the ROS2 framework. A Level 3 self-driving car can operate conditionally under specific environmental conditions and may require human intervention in some situations.

Functionalities:

    Designed a city environment in Blender and simulated it in Gazebo.
    Developed a perception pipeline for lane detection and traffic signal recognition.
    Implemented an advanced control algorithm for navigating T-junctions, intersections, and cruise control.
    Utilized a custom CNN for object classification.
    Implemented Dijkstra's and A* algorithms for path planning.

The World:
![world](https://github.com/hrishikesh829370/Ros2_self_driving_car/assets/131910887/af6f7590-821c-4449-9545-6287c3107b12)


A realistic city environment created in Blender and simulated in Gazebo.

Traffic Signal Recognition:
![traffic_signal](https://github.com/hrishikesh829370/Ros2_self_driving_car/assets/131910887/fb6eeadc-ab3d-422c-94b8-7b6844594673)

The car identifies the traffic signal (red light) and comes to a stop.
