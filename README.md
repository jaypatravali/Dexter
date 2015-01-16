# Dexter
Code repository for Project Dexter , an AGV with a5 DoF Robotic Arm
Dexter is mobile manipulation platform which has applications in Warehouse and Office Inventory Management. In the first protoype we aim to demonstrate autonomous navigation in unknown environment with obstacle avoidance. It will then pick a target object and transport it to the goal point.
We are also looking for field applications of Dexter with GPS integration and teleoperation.

##First Prototype

Software
-----------------
###Autonomous Navigation

* We use Navigation stack on ROS for autonomous Navigation
* Onboard Kinect provides 3D maps and RGB feed.
* Tweaked parameters in RTABMAP to obtain faster mapping and robot localization
* RPLidar( a 2D laser scanner) provides range data upto 6m 
* Wheel encoders, visual Odometry, IMU sensor data are published to robot_localization which fuses sensor data using Extended Kalman Filters
* Ultrasonic sensor placed at bottom for obstacle avoidance in blind spots of the Camera
* A complete GUI on RViz to for waypoint navigation and teleoperation,with windows for camera feed, 2D map 
* GPS integration for outdoor navigation.
* Laptop with 4th gen Intel i7 processor 

###Robotic Manipulator

* 5 DoF SCARA type arm
* 0.5 Kg payload capacity
* Teleoperation and Autonomous modes for object picking and placing
* Moviet to be used for Motion Planning .Complete URDF files
* Simulation of object picking and placing on Gazebo Sim.

