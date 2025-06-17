# FUZZY-LOGIC-BASED-SELF-BALANCING-ROBOT

This repo presents a MATLAB simulation of a fuzzy logic controller for a self-balancing two-wheeled robot.

## Inverted Pendulum Concept
![image](https://github.com/user-attachments/assets/039c3562-c1b3-4e57-a360-c6deacccfbfa)

- The robot is modeled as an inverted pendulum, a classic unstable system.
- The controller’s goal is to keep the robot upright by adjusting motor torque.

## Block Diagram

![image](https://github.com/user-attachments/assets/cb9c060e-f8c6-4b03-b45c-ff7b1a228e76)

## Key Linguistic Variables
### Input 
- **Cart Angular Velocity**: Rate of change of angle (“Negative”, “Positive”).
  
 ![image](https://github.com/user-attachments/assets/3497c622-4c2f-4e74-84d5-9b2a6501450c)

- **Cart Angle**: Tilt with respect to vertical (“Negative”, “Positive”).
  
![image](https://github.com/user-attachments/assets/008084ec-c12b-4898-8b16-1210e9cf88bf)

- **Cart Velocity**: Speed along the track (“Negative”, “Positive”).
  
![image](https://github.com/user-attachments/assets/2c607538-ac40-4789-9c51-8b50bc8ca1f9)

- **Cart Position**: Displacement from a reference point (“Negative”, “Positive”).
  
 ![image](https://github.com/user-attachments/assets/b70bb8c7-74c0-4e03-90e1-c47b5a9b328b)

### Output
- **TORQUE**: Represents the control action of the fuzzy logic controller, which is 
the torque applied to the system.

![image](https://github.com/user-attachments/assets/95586718-47cf-4c53-9707-81bc10f325a6)


## Fuzzy Rule Base

- The controller applies if-then rules, e.g.:
  - If cart angle is negative, apply medium negative torque.
  - If angular velocity is positive, apply large positive torque.
  - If position is negative, apply small positive torque, etc.

![image](https://github.com/user-attachments/assets/14eced08-1df5-4b23-aca0-b4336c4131cb)

### Fuzzy inference system Interface
![image](https://github.com/user-attachments/assets/5ee10248-09c1-4e61-9a4c-d88d78dd7ea2)


# Simulink model of Self-Balancing Robot

![control_loop_diagram](https://github.com/user-attachments/assets/5ab34912-7350-4cf4-841d-615a6ca36a1a)


