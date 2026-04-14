# Automatic Wet Grinder Smart Control System

## Overview
This project focuses on automating the water dispensing process in a wet grinder by analyzing batter consistency using real-time sensor feedback. The system reduces manual effort and improves consistency by dynamically adjusting water addition during grinding.

## Objective
To develop an intelligent control system that monitors grinder load conditions and automatically dispenses water based on batter consistency.

## Key Features
- Real-time RPM monitoring using Hall Effect sensor  
- Load detection using current sensing  
- Automatic water dispensing using relay control  
- Reduced manual intervention  
- Improved consistency of batter  

## Hardware Components
- Microcontroller (Arduino)
- Hall Effect Sensor (for RPM measurement)
- Current Sensor Module (for load/current detection)
- Relay Module (to control water valve/pump)
- Wet Grinder setup

## Working Principle
The Hall Effect sensor measures the rotational speed (RPM) of the grinder motor, while the current sensor monitors the current drawn by the motor, which varies based on batter consistency.

- When the batter is thick → motor load increases → current increases → RPM may drop  
- When the batter is thin → motor load decreases → current decreases → RPM stabilizes  

The system continuously analyzes these parameters and determines whether water needs to be added.

If the batter is detected to be too thick:
→ The controller activates the relay  
→ Water is dispensed into the grinder  

Once optimal consistency is reached:
→ The relay is turned OFF  
→ Water flow stops automatically  

## Results
- Achieved automated control of water dispensing  
- Improved batter consistency across multiple trials  
- Reduced need for manual monitoring  

## Challenges Faced
- Sensor calibration for accurate load detection  
- Noise in sensor readings  
- Setting appropriate threshold conditions  

## Future Improvements
- IoT-based monitoring and control  
- Adaptive algorithms for better consistency detection  
- Mobile app integration for user control  
