---

# A Pendulum based Spherical Robot

## Project Description

Nowadays, robot has a very big role in human life such as industrial robot and medical robot,and also there are many design of the robot. Concerning on the work area such as uneven surface or high friction areas, some design might not be able to work magnificently to achieve objectives and tasks of robot purpose. In that case, the spherical robot is introduced to solve the problem. The spherical robot is a novel mechanism design to move the robot in multiconditioned surfaces. Unlike other kind of legged or wheeled robots, the main feature that make a spherical different from other is a ground contact point which is very small as compared to other designs. In principles, the spherical robot comprises of two DC motor to move forward and backward direction while robot’s heading is altered by the pendulum, which is actuated by another DC motor.

## Acknowledgement

I extend my sincere appreciation to the Integral University Robotics Lab ([https://www.robotics.iul.ac.in/](https://www.robotics.iul.ac.in/)) for their invaluable support throughout the development of the Spherical Robot. Their generous provision of funds, tools, and a conducive environment for research and innovation has been instrumental in bringing this project to fruition. I am deeply grateful for their guidance and expertise, which have played a pivotal role in the successful design and implementation of this robot using Arduino. This project would not have been possible without their unwavering support and mentorship.

## Prerequisite

### Hardware
- **Spherical ball**
- **Node MCU**
- **ESP32 CAM1**
- **Servo motor MG995**
- **DC motors**
- **Brass Metal**

### Software
- **Arduino IDE**
- **Any OS with clients to access the Internet**
- **Coding Lnaguage: C++**
- **Tinkercad**

### Mathematical Analysis

- **Weights required to counter balance the torque of motor:**
  
  **Torque (in Nm)=Power (in watts)/Angular velocity (in radians per second)**
  
  **Angular velocity (in radians per second) =2π×RPM/60 = 10.46 rad/s**

  **Torque =Force (N)×Lever Arm (m) = 0.8Kg.m**

- **Forward Kinematics (Differential Drive):**
  
   **V=(𝑣𝑟+𝑣𝑙)/2 = 1 m/s**
  
   **𝜔=(𝑣𝑟−𝑣𝑙)/L = 10.44 rad/s**

- **Inverse Kinematics (Differential Drive):**
  
    **𝑣𝑟=V+𝜔*𝐿/2 = 1.732m/s**
  
     **𝑣𝑙=V−𝜔*𝐿/2 =0.27m/s**
  
- **Wheel Speed to Linear and Angular Velocity Conversion (Omni Wheels):**
  
  **𝑣𝑥=∑𝑣𝑖cos⁡(𝜃𝑖)**
  **𝑣𝑦=∑𝑣𝑖sin⁡(𝜃𝑖)**
  
- **Dynamic Model (Forces and Torques):**
  
     **𝐹=𝑚𝑎**
  
     **𝜏=𝐼𝛼**

- **Energy Consumption:**
  
    **𝐸=𝑃⋅𝑡 = 10.05 Wh**

- **Euclidean Distance Formula:**
  
   **Distance=sqrt{(xweight−xsphere)^2+(yweight−ysphere)^2+(zweight−zsphere)^2}**
 
     **= 5.93cm**

## Author

SAMEERA HASHMI

sameerahashmi565@gmail.com


---
![internal assembly](https://github.com/Integral-Robotics-Lab/Spherical-Robot/assets/140057631/28ecbd56-0773-49d0-89a9-42b77b628dab)

![Outer view](https://github.com/Integral-Robotics-Lab/Spherical-Robot/assets/140057631/d686b1bd-27be-43ae-b3a6-fc0d39da17a4)

![WiFi controlled](https://github.com/Integral-Robotics-Lab/Spherical-Robot/assets/140057631/a35c33f2-f7e4-4d99-ac8a-2fa15f41d4bf)
