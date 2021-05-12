![Curiosity](/images/perseverance_logo.jpg)

# Background

Perseverance is my version of a motorized model of Mars rovers Perseverance. It faithfully reproduces
the [Rocker-Bogie suspension kinematics](https://en.wikipedia.org/wiki/Rocker-bogie) of real
rovers and it is intended to be an hardware platform for future software projects in autonomous
operations and IA development.

All information for building Perseverance is free and public open source for anyone to build their
own.

The project was somehow inspired by [JPL's Open Source Rover project](https://opensourcerover.jpl.nasa.gov) and from the many resources I could find on the web. Unfortunately I did not fully like the design, too far from the original, so I decided to model one by myself. I used [Shapr3D](https://www.shapr3d.com) on my iPad pro, great piece of software still growing.
Most of the differences were motivated by a desire to fit the project to my requirements (mainly research in IA and autonomous navigation). Fitting Dynamixel servos was quite a challange and there is still room for improvements.

* Motorization: Moving the wheels is done with serial bus servo motors. I went for Dynamixel AX-18A I took from a previous hexapod project. 
* Construction Method: Instead of using the [Actobotics construction system](https://www.servocity.com/actobotics), Perseverance will be built from aluminum extrusions connected by 3D-printed plastic parts.

# Development Status and Milestones
<img src="https://github.com/andreagavazzi/Curiosity/blob/main/images/nasa_logo.jpg" alt="ag_logo" width="600"/>
 
**Perseverance version 1.0** 

- [ ] This milestone includes a basic rolling chassis that is mechanically functional
- [ ] Aestetic add-ons on the chassis (reactor, attachments and linkages, ...)
- [ ] Camera turret (webcamto be defined)
- [ ] Dynamixel + OpenCR controller
 
**Perseverance version 1.1**  
- [ ] Complete redesign of the differential
 
**Perseverance version 1.2**  
- [x] Redesign of wheels

  
# IA, Sensors and Controllers
<img src="https://github.com/andreagavazzi/Curiosity/blob/main/images/ag_logo.jpg" alt="ag_logo" width="200"/>
  
Perseverance is planned to be a a [ROS](http://ros.org) robotics platform running on Linux Ubuntu.

**ROS Melodic**: [a ground-up rewrite of a ROS-centric stack](https://github.com/srmainwaring/curio) by Rhys Mainwaring (srmainwaring) is extensive and powerful. Going beyond responding to `/cmd_vel` commands, it also calculates `/odom` by interpolating the AX-18A position encoder ~270 degree feedback into full 360 degrees. Plus visualizing rover state in RViz, and files to put a digital Perseverance in Gazebo robot simulation environment.

**NVIDIA Jetson AGX Xavier**: The latest addition to the Jetson platform. It’s an AI computer for autonomous machines, delivering the performance of a GPU workstation in an embedded module under 30W. Jetson AGX Xavier is designed for robots, drones and other autonomous machines.

Additional material can be found in my [Onedrive shared folder](https://1drv.ms/f/s!AkUtNLbG6ptfpiPbJ0WKSoO58hIA).

# Pictures

| Design  | Build  | Explore |
| ------------- | ------------- | ------------- |
| [<img src="https://github.com/andreagavazzi/Curiosity/blob/main/images/ico_astronomy.png" alt="ag_logo" width="80"/>](https://github.com/andreagavazzi/Curiosity/blob/main/images/design/design.md) | [<img src="https://github.com/andreagavazzi/Curiosity/blob/main/images/ico_mars-rover.png" alt="ag_logo" width="80"/>](https://github.com/andreagavazzi/Curiosity/blob/main/images/build/build.md) | [<img src="https://github.com/andreagavazzi/Curiosity/blob/main/images/ico_extraterrestrial.png" alt="ag_logo" width="80"/>](https://github.com/andreagavazzi/Curiosity/blob/main/images/explore/explore.md)  |



