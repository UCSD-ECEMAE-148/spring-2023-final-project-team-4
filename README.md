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


## **Live Demonstration of Autonomous Trash Collection:**
&ensp; - Our car has the ability to detect trash of different colors in different environments and also distinguish between trash and non-trash. <br />

| Car head                                   | Elephant                                  |
|--------------------------------------------|--------------------------------------------|
| [![Video Title](https://img.youtube.com/vi/3PPiyPLOKiE/0.jpg)](https://youtu.be/3PPiyPLOKiE)| [![Video Title](https://img.youtube.com/vi/kySv7iY4cWU/0.jpg)](https://youtu.be/kySv7iY4cWU) |


[![Video Title](https://img.youtube.com/vi/kySv7iY4cWU/0.jpg)](https://youtu.be/kySv7iY4cWU)

## Code Repository
[Link to Ece-148-team04 repository](https://github.com/AmaanSingh/Ece-148-team04.git)

## Robocar Vacuum System Design 

### Preliminary Design 

**Advantages:**  <br />
&ensp; - The robotic autonomous car has the ability to accommodate and utilize two fans and two cameras, allowing for effective trash detection and collection. <br />
&ensp; - The presence of a hinged door for the garbage disposal unit provides a convenient and efficient means of emptying collected trash.  <br />
    
**Disadvantages:** <br />
&ensp; - One of the disadvantages is that the nozzle of the vacuum mechanism is unchangeable, limiting its adaptability to different types of trash or cleaning scenarios. <br />
&ensp; - The complex geometry of the 3D-printed vacuum mechanism makes it more challenging to manufacture, potentially increasing production difficulties and costs. <br />
  
<p float="left">
  <img src="/images/Sucker v1_1.png" width="300" />
  <img src="/images/Sucker v1_2.png" width="300" /> 
  <img src="/images/Sucker v1_3.png" width="300" />
</p>

### Final Design
**Advantages:**  <br />
&ensp; - Modular design, the parts are interchangeable for different scenarios. <br />
&ensp; - Transform one complex-shaped object into several simple-shaped objects, making it easier and faster to print. <br />
&ensp; - Added two more mounting points to improve stability. <br />
&ensp; - Better aerodynamic efficiency, reducing intake and suction losses. <br />
&ensp; - Stronger fan and optimized nozzle improved sucking force and range of collection. <br />
    
**Disadvantages:** <br />
&ensp; - Airtightness reduced due to seams, needs sealing ring or glue to further improve efficiency. <br />

<p float="left">
  <img src="/images/tube_1.png" height="500" />
  <img src="/images/tube_2.png" height="500" /> 
</p>

![sucker_v2_1](https://github.com/UCSD-ECEMAE-148/spring-2023-final-project-team-4/blob/main/images/Sucker%20v2_1.png)

![sucker_v2_2](https://github.com/UCSD-ECEMAE-148/spring-2023-final-project-team-4/blob/main/images/Sucker%20v2_2.png)


#### Fan Installation
The fan is placed right behind the mesh, intaking air from the nozzle and exhaust backwards, trash will be sucked in together but blocked by the mesh and then falls naturally into the collection box.
<p float="left">
<img src="https://github.com/UCSD-ECEMAE-148/spring-2023-final-project-team-4/blob/main/images/fan%20installation.png" alt="Alt text" width="600" align="mid"/>
</p>

#### Other mechanical parts
A high and curved OAKD camera mount guarantees a great view for the camera.
<p float="left">
  <img src="https://github.com/UCSD-ECEMAE-148/spring-2023-final-project-team-4/blob/main/images/camera%20mount.png" height="400" />
</p>


## Electric Circuit Diagram
We used two cameras as sensor in this project, in which the OAKD camera has a wider field of view, detecting the positition of the trash and naviagtes the car to the trash. When the car is close to the trash and the trash enters the view of the ordinary USB camera, it will run the fan and suck in the trash. The trigger mechanism is that when the USB camera detects the trash, it will send a signal to Jetson nano and Jetson will output 5V high level to the relay, then the relay will connect the circuit of fan and 12V battery.

![Electric Circuit](https://github.com/UCSD-ECEMAE-148/spring-2023-final-project-team-4/blob/main/images/electric_circuit_1.png)


## Color Detection Program

### Functionalities
- Tracking the colored object
- Adjust to any color
- Change the minimum area threshold to avoid noise
### Live Presentation: Color Detection 
[![Video Title](https://img.youtube.com/vi/FbhEe8014F8/0.jpg)](https://youtu.be/FbhEe8014F8)


## Opencv Detection Software
- API Roboflow
- DepthAI
- PyVESC
- Jetson GPIO Board Pins Library
  
 ![model](https://github.com/UCSD-ECEMAE-148/spring-2023-final-project-team-4/blob/main/images/model.png)

