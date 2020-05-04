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

![](Mini-Task%202%20Images/1.png)

There will be two wires at each level. One set of wires will be connected to ground. The other set of wires are connected to different pins of the Arduino. Since water conducts electricity, when the water reaches that level, the two wires will be shorted and the voltage at the pin of the Arduino will be 0 as it is shorted to the wire which is connected to the ground. We can check the topmost level which has zero potential and report that as the level of water.

This is a simple way to measure the water. The only possible disadvantage/implementation issue is how effective water is as an electrical conductor. But in day-to-day life, we experience shock when we try to operate any electrical equipment with our hands wet. So this won't be that much of an issue I guess. 

#### 3. LCD display (Optional feature):
It is very convenient to have an LCD display which displays the level of water in the tank, as well as whether the motor is running or not. This enables the user to have a sense of what is happening as far as the motor controller is concerned. 

Advantage: The main advantage of the LCD display is that we can actually check whether the automatic motor controller is working or not. If the level of water is empty but if the motor is not running yet, then there is seriously some problem over there. And if we have a manual controller(switch) for the motor as well, and if we want the tank to be full at a particular point of time (for example, if there are a lot of guests at your home, and if they have to freshen up to go to a function, then we don't want the tank to be empty suddenly), then we can check the display and take actions accordingly. So, LCD display is a must if we want to use it in real life.

But if it is a project at the college level, then we don't have much time to work on the LCD display, since the rest of the electronics will take a considerable amount of time and most of the college projects are either one semester or one year projects. If we have time, then surely we can work on the LCD display.
