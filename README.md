# Dexter
Code repository for Project Dexter , an  AGV with 5 DoF Robotic Arm

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
* A complete GUI on RViz to for waypoint navigation and teleoperation,with windows for camera feed,2D map 
* GPS integration for outdoor navigation

###Robotic Manipulator

* 5 DoF SCARA type arm
* 0.5 Kg payload capacity
* Teleoperation and Autonomous modes for object picking and placing
* Moviet to be used for Motion Planning .Complete URDF files
* Simple object picking and placing on Gazebo Sim.
* 
