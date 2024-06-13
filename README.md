# Enhancing Indoor Navigation During Emergency Situations with Mobile AR Technology utilizing on-device machine learning and device built-in sensors.

## CS291I Spring 24 - Final Project
Liyanamahadura Ravindu De Silva, Suraj Kattimuttathu Suresh, Chieh-Ying (Jamie) Lai

## Overview
![overview](/pics/fig2.png)

*This repo contains two parts, one is the AR indoor navigation and the other is object detection.*

Modern evacuation plans during emergencies rely on outdated methods, such as neon exit signs, which can be ineffective during natural disasters, power outages, and for visually impaired individuals in unfamiliar settings.

To address these challenges, we introduce a mobile augmented reality (AR) application designed for indoor navigation during emergencies. 

## System Flow
![system_flow](/pics/fig1.png)


The workflow of our application is as shown of above fugure. This system begins by downloading the latest building LiDAR maps from firebase when the user enters a new place. It uses GPS and beacons to find the user's exact location and shows a safe way out on the screen using augmented reality. It detects obstacles using a modified YOLOv8 model, updating the route dynamically. Voice instructions are also provided to guide users effectively during an evacuation. 
_Note: Text To Speech model are not yet been implemented_

## Technology stack
The application is written in Swift. We utilize ARkit for the AR features, sensors readings found on the iphone(including camera, LiDAR, GPS), Firebase for storage of maps and routes, YOLOv8 as our object detection models, and CoreML for model convertion.

## Some outputs and Demo
Demo video of indoor navigation in HFH 2nd floor:
https://youtube.com/shorts/IKviHSl2N4o

Fine-tuned YOLOv8 model:
https://youtube.com/shorts/l8GHucg6l28?feature=share

This is the dataset we used for fine-tuning (captured in HFH at UCSB):
https://drive.google.com/file/d/1uXyu4xwke3mfsDMjyDG9ZrP2u02e_uaE/view

Visualization of HFH 2nd Floor:
https://youtu.be/ADnK1CSN6fY

MVP:
https://youtu.be/HBIlqxuHLdE

## Links to presentation:
Final: https://docs.google.com/presentation/d/1BA4sMZY5mg3-f2aDVmF_nhdjte1lI4XRwZTCEBge00k/edit?usp=sharing

