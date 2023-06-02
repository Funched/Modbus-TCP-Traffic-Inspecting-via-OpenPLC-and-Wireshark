# Modbus/TCP-Sniff
Modbus/TCP sniffing Lab via Factory IO and OpenPLC
I have created a Lab environment for sniff and analyze Modbus/TCP traffic in this repo.

For this:

OpenPLC Editor: Used for creating and compiling PLC program.

OpenPLC Service: Works as PLC and HMI. 

Factory IO: Contains 3D models of actuators and sensors that can interact with OpenPLC Server. 

# Lab Environment

![resim](https://github.com/don-talcapone/Modbus-Sniff/assets/135317904/7c5b1170-5c45-4001-83b9-dd96f8aa51a5)

It has a conveyor actuator as output and a sensor as input. In this scenario, the conveyor runs until the box reaches the sensor. The conveyor will stop when the box arrives.

# Programming

PLC is programmed so that the conveyor can be controlled with. The program has basic contactor and actuator and is created with ladder diagram.
