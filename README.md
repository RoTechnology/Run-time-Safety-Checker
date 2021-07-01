# Run-time-Safety-Checker
## Overview
The RSC (Run-Time Safety Checker) is a software module proposed to be used for control and management of the parameters that could be critical for the flight of the drone. The implementation is based on the predefined Safety Rules which define the functioning of the component. The module will be activated whenever one of the safety rules fails and thus it will implement a resolution procedure. The module requires the management of several parameters and their combination as the conditions that may occur are various. 

The RSC tool actually is built for a specific [Comp4Drones](https://www.comp4drones.eu) Runtime Safety, Alarms Systems case study.
## How it works
The module monitors, at runtime, the parameters value acquired by the on-board sensors. 
Sensor parameter values are the input of the Runtime Monitoring, which controls the range at which these values belong to. The ranges define three different state: Safe, Warning and Critical. 
The module activates a safety procedure whenever one or more thresholds are exceeded, in other words, every time a safety rule is broken. When this occurs, the module changes its state to Warning or Critical state, depending on the values of the parameters.
When the measured values identify a Warning or Critical state, the RSC activates a risky situation implementing the operations defined for specific status.							


