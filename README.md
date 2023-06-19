# TEAM 4: SMART ELEPHANT - Autonomous Vacuum Cleaner

## Team Members
![team photo](https://github.com/UCSD-ECEMAE-148/spring-2023-final-project-team-4/blob/main/images/team_photo.jpg)
From left to right: Amaan, Fengrui, Shuyan, Hector

## Car Images
![side1](https://github.com/UCSD-ECEMAE-148/spring-2023-final-project-team-4/blob/main/images/car_side_1.jpg)
![front](https://github.com/UCSD-ECEMAE-148/spring-2023-final-project-team-4/blob/main/images/car_front.jpg)
![above](https://github.com/UCSD-ECEMAE-148/spring-2023-final-project-team-4/blob/main/images/car_above.jpg)
![side2](https://github.com/UCSD-ECEMAE-148/spring-2023-final-project-team-4/blob/main/images/car_side_2.jpg)

## Abstract:
This project presents the development of a robotic autonomous car equipped with a Jetson Nano, VESC controller, two cameras, and two fans to detect and collect trash from the ground. The system employs a custom Detection Software written in Python, which utilizes the camera feed to identify trash objects. By controlling a relay switch based on the software's analysis, the fans are activated or deactivated depending on the presence of trash in front of the car. In addition to the detection mechanism, a 3D printed and designed vacuum mechanism is incorporated to effectively collect the identified trash. This project aims to create an efficient and automated solution for trash detection and collection, contributing to a cleaner and more sustainable environment.

## Why Elephant?
| Car head                                   | Elephant                                  |
|--------------------------------------------|--------------------------------------------|
| ![side3](https://github.com/UCSD-ECEMAE-148/spring-2023-final-project-team-4/blob/main/images/car_side_3.jpg) | ![elephant](https://github.com/UCSD-ECEMAE-148/spring-2023-final-project-team-4/blob/main/images/elephant.jpg) |

## Code Repository
[Link to Ece-148-team04 repository](https://github.com/AmaanSingh/Ece-148-team04.git)

## Robocar Vacuum System Design 

### Preliminary Design
At first we designed a one-piece structure and mounted the vacuum cleaner to the front bumper of the car.
<p float="left">
  <img src="/images/Sucker v1_1.png" width="300" />
  <img src="/images/Sucker v1_2.png" width="300" /> 
  <img src="/images/Sucker v1_3.png" width="300" />
</p>

pros:
cons:

### Final Design
After evaluating the performance of the preliminary design, we made significant improvements, using modular design and added two more mounting points.
<p float="left">
  <img src="/images/tube_1.png" height="500" />
  <img src="/images/tube_2.png" height="500" /> 
</p>


![sucker_v2_1](images/Sucker v2_1jpg)

![sucker_v2_2](images/Sucker v2_2.jpg)


### Fan Installation
The fan is placed right behind the mesh.
![fan installation](images/fan installation.jpg)


## Electric Circuit Diagram



## Color Detection Program

### Functionalities
- Tracking the colored object
- Adjust to any color
- Change the minimum area threshold to avoid noise
### Live Presentation: Color Detection 
[![Video Title](https://img.youtube.com/vi/FbhEe8014F8/0.jpg)](https://youtu.be/FbhEe8014F8)


## Opencv Detection Software

