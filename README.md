![Curiosity](/images/curiosity_logo.jpg)

# Background

Curiosity is my version of a motorized model of Mars rovers Curiosity (and Perseverance) . It faithfully reproduces
the [Rocker-Bogie suspension kinematics](https://en.wikipedia.org/wiki/Rocker-bogie) of real
rovers and it is intended to be an hardware platform for future software projects in autonomous
operation.

All information for building Curiosity is free and public open source for anyone to build their
own.

The project was inspired by [JPL's Open Source Rover project](https://opensourcerover.jpl.nasa.gov) and from the many resources I could find on the web. My starting point was to review and redesign in [Shapr3D](https://www.shapr3d.com) the stl files by [Roger-random's Sawppy rover](https://github.com/Roger-random/Sawppy_Rover/tree/main/STL). 
Most of the differences were motivated by a desire to improve the design and fit the project to my requirements (mainly research in IA and autonomous navigation). Moreover JPL's rover is designed for education, to be assembled by a school team and give a robust foundation for structured curriculum. Curiosity is more suited for individual hobbyists like myself who are happy to tinker and willing to develop furthermore.

* Motorization: Instead of using gearmotors with encoders managed by RoboClaw motor controllers, moving the wheels is done with serial bus servo motors. I went for Dynamixel AX-18A I took from a previous hexapod project. 
* Construction Method: Instead of using the [Actobotics construction system](https://www.servocity.com/actobotics), Curiosity will be built from aluminum extrusions connected by 3D-printed plastic parts.

# Development Status
<img src="https://github.com/andreagavazzi/Curiosity/blob/main/images/nasa_logo.jpg" alt="ag_logo" width="600"/>

**Curiosity version 1.0** 

This milestone includes a motorized rolling chassis that is mechanically functional.
The remaining areas (electrical, software, etc.) are still very immature, just barely enough to validate mechanical chassis function. 

**Curiosity version 1.1**

Curiosity will receive only minor mechanical changes for this milestone, expecially on the back of the rover

# IA, Sensors and Controllers
<img src="https://github.com/andreagavazzi/Curiosity/blob/main/images/ag_logo.jpg" alt="ag_logo" width="200"/>
  
Curiosity is planned to be a a [ROS](http://ros.org) robotics platform.

**ROS Melodic**: [a ground-up rewrite of a ROS-centric stack](https://github.com/srmainwaring/curio) by Rhys Mainwaring (srmainwaring) is extensive and powerful. Going beyond responding to `/cmd_vel` commands, it also calculates `/odom` by interpolating the AX-18A position encoder ~270 degree feedback into full 360 degrees. Plus visualizing rover state in RViz, and files to put a digital Curiosity in Gazebo robot simulation environment.

# Pictures

| Design  | Build  | Explore |
| ------------- | ------------- | ------------- |
| [<img src="https://github.com/andreagavazzi/Curiosity/blob/main/images/ico_astronomy.png" alt="ag_logo" width="80"/>](https://github.com/andreagavazzi/Curiosity/blob/main/images/design/design.md) | [<img src="https://github.com/andreagavazzi/Curiosity/blob/main/images/ico_mars-rover.png" alt="ag_logo" width="80"/>](https://github.com/andreagavazzi/Curiosity/blob/main/images/build/build.md) | [<img src="https://github.com/andreagavazzi/Curiosity/blob/main/images/ico_extraterrestrial.png" alt="ag_logo" width="80"/>](https://github.com/andreagavazzi/Curiosity/blob/main/images/explore/explore.md)  |



