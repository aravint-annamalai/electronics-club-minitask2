# MINI TASK 2

## PROJECT 1: AUTOMATIC WATER LEVEL CONTROLLER

Link: https://www.electronicshub.org/water-level-controller-using-8051-microcontroller/

### Problem Statement:
To implement an automatic control of a motor which pumps water into a tank such that it automatically stops when the motor is full and automatically starts when the motor is empty. 

### Ideate solution:

#### 1. Choice of microcontroller:
In the link given, the 8051 microcontroller is used. I suggest using an Arduino MEGA (MEGA because we will be using a lot of pins). We can use smaller Arduinos as well if we choose to do away with the extra feature of displaying the level of water as well as the status of motor(whether running or off) on LED.

Advantage: The largest Arduino available, Arduino MEGA, costs less than half of an 8051 microcontroller. Also, Arduino can be coded easily and we can focus on the electronics part of the project rather than coding.

Disadvantage: We miss out on working with a new kind of a microcontroller, so the learning outcome of the project will be slightly reduced if we use an Arduino.

#### 2. Water Level Measurement:
This circuit is based on the fact that water conducts electricity. The way in which the water level is measured is depicted in the circuit below:

![](


