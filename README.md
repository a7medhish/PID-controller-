# PID-controller-
Implanting PID controller for autonomous driving 

## Overview
The scope of the project is to implement a PID controller by taking a factor of CTE (i.e., cross track error), speed and angle of the vehicle and it outputs the steering angle with a fixed speed. 

## Compilation 
The program compiles using ‘Cmake’, and it compiles successfully without any errors or problems. 

## implementation 
The core of the PID controller runs on the PID.cpp using functions PID::UpdateError and PID::TotalError that calculates the  proportional, integral and derivative errors with respects to the CTE . 

## Reflection 
### The probational part (P)
The proportional controller tries to steer the car toward the centre line (against the cross-track error). When utilized along, the car readily overshoots the centre line and swiftly exits the road.
### The Integral part (I)
The integral element attempts to eliminate any potential bias in the controlled system that would prevent the error from being eliminated. When used together, it causes the car to spin in circles. When it comes to the simulator.

### The derivative part (D)
By smoothing the approach to the centre line, the differential portion serves to overcome the proportionate tendency to overshoot. 

## Conclusion 
The PID controller is a well-known controller that have been used in many industries and fields and by this project we can effectively see the impact of this spectacular controller. However, in real industry of self-driving cars it cant used alone as it is utilized beside the deep learning to get a smother driving experience 
