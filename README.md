# JARP - Just Another Rover Project

Just Another Rover Project, or **JARP**, is a personal project I started to start putting my 3D printer to use and to learn more about ROS and autonomous vehicles in general. 
This repository will contain the code to run JARP in ROS as well as the Solidworks/STL files for the rover itself. It will also contain some of the documentation related to this project.

## Hardware required

Here is the list of hardware used for this project.
Quantity |Item name
----------|----------
1|Jetson Nano V1
1|WiFi/BT Module
1|Arduino Nano
1|RP-Lidar A1
4|6v 230rpm Motors <br>with built-in encoders
2|L298N Motor Drivers
1|5v Step-Down Converter
1|PCA9685 PWM Driver
1|2200mah LiPo Battery

## Xbox One Controller Setup

An Xbox One Controller was to to initially test out the functions of the rover before going more into autonomous functions. Mainly to set up the motor functions / odometery.

Step 1: Install sysfsutils
> sudo apt install sysfsutils

Step 2: Edit the conf file
> sudo nano /etc/sysfs.conf

Step 3: Copy the line before to sysfs.conf
>module/bluetooth/parameters/disable_ertm = 1

Step 4: Restart and connect to BT.

Ensure that your Xbox One controller is one of the newer ones that has bluetooth, don't make the mistake I did and spend hours troubleshooting only to realise that you have an older controller.
