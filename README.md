# Fire and Flood Fighter Octocopter

It's a Pixhawk & Raspberry Pi based remote controlled or autonomous 8-armed UAV which will fight as firefighter & work as flood relief distributor.

The project was featured at IEEE Maker Fair Website: https://transmitter.ieee.org/makerproject/view/cabcb

# Table of Contents
- [Introduction](https://github.com/ArghyaChatterjee/fire-and-flood-fighter-octocopter/tree/master?tab=readme-ov-file#introduction)
  - [Hardware](https://github.com/ArghyaChatterjee/fire-and-flood-fighter-octocopter/tree/master?tab=readme-ov-file#hardware)
  - [Project Contributors](https://github.com/ArghyaChatterjee/fire-and-flood-fighter-octocopter/tree/master?tab=readme-ov-file#project-contributors)
  - [Live Demo](https://github.com/ArghyaChatterjee/fire-and-flood-fighter-octocopter/tree/master?tab=readme-ov-file#live-demo)
- [Fire Fighter Octocopter](https://github.com/ArghyaChatterjee/fire-and-flood-fighter-octocopter/tree/master?tab=readme-ov-file#fire-fighter-octocopter)
  - [Mission Planner for Ground Station](https://github.com/ArghyaChatterjee/fire-and-flood-fighter-octocopter/tree/master?tab=readme-ov-file#mission-planner-for-ground-station)
  - [Mission Planner Overview](https://github.com/ArghyaChatterjee/fire-and-flood-fighter-octocopter/tree/master?tab=readme-ov-file#mission-planner-overview)
  - [Launch on Windows](https://github.com/ArghyaChatterjee/fire-and-flood-fighter-octocopter/tree/master?tab=readme-ov-file#launch-on-windows)
- [Flood Relief Distributor Octocopter](https://github.com/ArghyaChatterjee/fire-and-flood-fighter-octocopter/tree/master?tab=readme-ov-file#flood-relief-distributor-octocopter)
  - [Compile on Linux](https://github.com/ArghyaChatterjee/fire-and-flood-fighter-octocopter/tree/master?tab=readme-ov-file#compile-on-linux)
  - [Face Recognition During Delivery Mission](https://github.com/ArghyaChatterjee/fire-and-flood-fighter-octocopter/tree/master?tab=readme-ov-file#face-recognition-during-delivery-mission)

# Introduction
## Hardware
<p float="left">
  <img src="assets/3D_view.png", width="370">
  <img src="assets/Solid_Design.jpg", width="450">
</p>

## Project Contributors
- Arghya Chatterjee
- Rumayel Hasan Pallock 
- Boshra Aziz Roshni
- Al Mamun

## Live Demo
For watching the copter in action, please visit [here](https://www.youtube.com/watch?v=dqQoOxy7XEo&list=PLVy6YSUUzzp0ME0aE1SHiJquqTTtoAA5Z).

# Fire Fighter Octocopter
<p float="left">
  <img src="assets/Fire_Fighter.png", width="400">
  <img src="assets/F2_Fightocopter.png", width="420">
</p>

## Mission Planner for Ground Station

- Website : http://ardupilot.org/planner/  
- Forum : http://discuss.ardupilot.org/c/ground-control-software/mission-planner
- Download latest stable version : http://firmware.ardupilot.org/Tools/MissionPlanner/MissionPlanner-latest.msi
- Changelog : https://github.com/ArduPilot/MissionPlanner/blob/master/ChangeLog.txt  
- License : https://github.com/ArduPilot/MissionPlanner/blob/master/COPYING.txt  

## Mission Planner Overview
<p align="center">
  <img src="assets/Mission_planner.png", width="600">
</p>

## Launch on Windows

- Get the lastest zipped version of Mission Planner here : https://firmware.ardupilot.org/Tools/MissionPlanner/MissionPlanner-latest.zip
- Unzip in the directory you want
- Go into the directory
- run with: 
```
mono MissionPlanner.exe
```

You can debug Mission Planner on Mono with:
```
MONO_LOG_LEVEL=debug mono MissionPlanner.exe
```
# Flood Relief Distributor Octocopter
<p float="left">
  <img src="assets/Octocopter.jpg", width="400">
  <img src="assets/Front_octocopter.jpg", width="400">
</p>

## Compile On Linux

Those instructions were tested on Ubuntu 16.04.
Please install Mono, either :
```
sudo apt install mono-runtime libmono-system-windows-forms4.0-cil libmono-system-core4.0-cil libmono-winforms2.0-cil libmono-corlib2.0-cil libmono-system-management4.0-cil libmono-system-xml-linq4.0-cil
```

or full Mono :
```
sudo apt install mono-complete
```

## Face Recognition During Delivery Mission
<p align="center">
  <img src="assets/delivery detection.gif", width="600">
</p>

1. Update libraries: 
```
sudo apt-get update
sudo apt-get upgrade
```
2. Installing Face Recognition Module: 
```
sudo apt-get install build-essential cmake
sudo apt-get install python3-setuptools
sudo apt-get -y install python3-pip
sudo pip3 install dlib
sudo pip3 install face_recognition
```
3. Running the Delivery Recognition model:
```
cd ~/UAV Delivery Recognition 
python3 drone_delivery.py
```

# Project Goal

<div align="center">
  <a href="https://www.youtube.com/watch?v=WFqThcMIN7A" target="_blank">
    <img src="assets/fire_drone.gif" width="400">
  </a>
  <a href="https://www.youtube.com/watch?v=Bm2BVTTir4c" target="_blank">
    <img src="assets/fire_drone_2.gif" width="400">
  </a>
</div>
