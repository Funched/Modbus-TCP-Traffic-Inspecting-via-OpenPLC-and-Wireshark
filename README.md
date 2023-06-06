# Modbus/TCP Inspecting

I have created a Lab environment for inspect Modbus/TCP traffic in this repo via Factory IO and OpenPLC.

For this:

OpenPLC Editor: Used for creating and compiling PLC program.

OpenPLC Service: Works as PLC and HMI. 

Factory IO: Contains 3D models of actuators and sensors that can interact with OpenPLC Server. 

# Lab Environment

<img src="https://github.com/don-talcapone/Modbus-Sniff/assets/135317904/01f53904-8245-4d88-a5fe-0e9c75f1ce96.png" width="60%">

It has a conveyor actuator as output and a sensor as input. In this scenario, the conveyor runs until the box reaches the sensor. The conveyor will stop when the box arrives.

<img src="https://github.com/don-talcapone/Modbus-Sniff/assets/135317904/9ba6c776-5183-4a1a-a6f2-76a0fc8f470f.png" width="60%">

Driver configured as Modbus TCP/IP server. 
# Programming

PLC is programmed so that the conveyor can be controlled with. The program has basic contactor and actuator and is created with ladder diagram. Used OpenPLC Editor for this.

<img src="https://github.com/don-talcapone/Modbus-Sniff/assets/135317904/49673d1a-0fc3-4992-bcf1-9543627f8777" width="60%">

# OpenPLC configuration and service start

OpenPLC installed and configured on Ubuntu.

It is important to make sure that the OpenPLC service is enabled and running correctly. 

<img src="https://github.com/don-talcapone/Modbus-Sniff/assets/135317904/017636b2-0664-405f-b9ac-8015fe077a13.png" width="60%">

Now we can configurate OpenPLC from web interface.

<img src="https://github.com/don-talcapone/Modbus-Sniff/assets/135317904/2c9fa4ac-63c7-40f0-a7f0-128ede766002.png" width="60%">

After the device configuration completed, the [program.st](https://github.com/don-talcapone/Modbus-Sniff/edit/main/program.st) file can be uploaded from the program tab.

When the operations are done correctly, we are completely ready to run OpenPLC.

<img src="https://github.com/don-talcapone/Modbus-Sniff/assets/135317904/00b03387-92b9-43da-8d7a-a670ab025a95.png" width="60%">

# Monitoring

The status of the sensor and actuator can be followed from the Openplc monitoring tab. 

<p float="left">
  <img src="https://github.com/don-talcapone/Modbus-Sniff/assets/135317904/a7336d2b-60d6-442b-9c1e-70cdf0a29182.png" width="45%" />
  <img src="https://github.com/don-talcapone/Modbus-Sniff/assets/135317904/6b463ac2-9d24-4686-8734-2e6e748a7d57.png" width="50%" />
</p>

<p float="left">
  <img src="https://github.com/don-talcapone/Modbus-Sniff/assets/135317904/3af88448-0dec-4136-9a40-eaf841a62ae2.png" width="45%" />
  <img src="https://github.com/don-talcapone/Modbus-Sniff/assets/135317904/6bded30f-3462-47c8-b295-f55ad91e3810.png" width="50%" />
</p>

# Inspecting Traffic

Finally the Modbus traffic can be inspected via Wireshark. 

<img src="https://github.com/don-talcapone/Modbus-Sniff/assets/135317904/d7859686-20ce-4969-ae58-a3adb4193916.png" width="70%" />
