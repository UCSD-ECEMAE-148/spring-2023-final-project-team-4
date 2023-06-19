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
Biomimicry was pivotal in designing the 3D-printed vacuum mechanism for trash collection. Inspired by an elephant's nose and mouth, the team replicated their efficiency and adaptability. Through detailed study of muscular tissues and trunk shape, they mimicked its functionality. The mechanism's flexible and elongated components adjust to various trash sizes, akin to the precision of an elephant's trunk. Additionally, interior channels imitated the convoluted nasal passages, optimizing suction for effective collection. This biomimetic approach enhanced functionality, fostering sustainable and nature-inspired waste management innovation.

| Car head                                   | Elephant                                  |
|--------------------------------------------|--------------------------------------------|
| ![side3](https://github.com/UCSD-ECEMAE-148/spring-2023-final-project-team-4/blob/main/images/car_side_3.jpg) | ![elephant](https://github.com/UCSD-ECEMAE-148/spring-2023-final-project-team-4/blob/main/images/elephant.jpg) |

## Code Repository
[Link to Ece-148-team04 repository](https://github.com/AmaanSingh/Ece-148-team04.git)

## Robocar Vacuum System Design 

### Preliminary Design

Advantages:  <br />
-The robotic autonomous car has the ability to accommodate and utilize two fans and two cameras, allowing for effective trash detection and collection. <br />
-The presence of a hinged door for the garbage disposal unit provides a convenient and efficient means of emptying collected trash.  <br />
    
Disadvantages: <br />
-One of the disadvantages is that the nozzle of the vacuum mechanism is unchangeable, limiting its adaptability to different types of trash or cleaning scenarios. <br />
-The complex geometry of the 3D-printed vacuum mechanism makes it more challenging to manufacture, potentially increasing production difficulties and costs. <br />
  
<p float="left">
  <img src="/images/Sucker v1_1.png" width="300" />
  <img src="/images/Sucker v1_2.png" width="300" /> 
  <img src="/images/Sucker v1_3.png" width="300" />
</p>



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

![Electric Circuit](https://github.com/UCSD-ECEMAE-148/spring-2023-final-project-team-4/blob/main/images/electric_circuit.png)



## Color Detection Program

### Functionalities
- Tracking the colored object
- Adjust to any color
- Change the minimum area threshold to avoid noise
### Live Presentation: Color Detection 
[![Video Title](https://img.youtube.com/vi/FbhEe8014F8/0.jpg)](https://youtu.be/FbhEe8014F8)


## Opencv Detection Software

