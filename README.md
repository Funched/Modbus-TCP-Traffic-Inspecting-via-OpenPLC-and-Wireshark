# Modbus/TCP-Sniff
Modbus/TCP sniffing Lab via Factory IO and OpenPLC
I have created a Lab environment for sniff and analyze Modbus/TCP traffic in this repo.

For this:

OpenPLC Editor: Used for creating and compiling PLC program.

OpenPLC Service: Works as PLC and HMI. 

Factory IO: Contains 3D models of actuators and sensors that can interact with OpenPLC Server. 

# Lab Environment

![resim](https://github.com/don-talcapone/Modbus-Sniff/assets/135317904/01f53904-8245-4d88-a5fe-0e9c75f1ce96)

It has a conveyor actuator as output and a sensor as input. In this scenario, the conveyor runs until the box reaches the sensor. The conveyor will stop when the box arrives.

# Programming

PLC is programmed so that the conveyor can be controlled with. The program has basic contactor and actuator and is created with ladder diagram. I used OpenPLC Editor for this.

![resim](https://github.com/don-talcapone/Modbus-Sniff/assets/135317904/37a90e02-8d18-4f3b-82b2-1c9f8aafa7a5)

# OpenPLC configuration and service start


