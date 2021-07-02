# SOCM - Smart Oxygen Cylinder Monitoring

# Project vision:

The amount of oxygen present inside an oxygen cylinder is a vital piece of information as such cylinders are in use for supply of oxygen in the current COVID scenario. Since the number of patients infected by COVID are very large, it becomes difficult to monitor all the isolation wards in the hospital simultaneously. Therefore, we aim to design a smart oxygen cylinder to automate this monitoring process by using a pressure transducer [M3031] at the nozzle of the oxygen cylinder and using indoor localisation to isolate the location of the cylinder that requires a refill. 

# Description and realization:

 Components:

•	Arduino development board – ATMEGA 32U4

•	ESP32 pico kit

•	Pressure transducer – M3031

•	Amplifier circuit 

The amount of oxygen present inside the cylinder is measured by measuring the pressureb at the outlet nozzle using a high precision Pressure transducer [M3031] which gives an output of range from 0.5-5v for a pressure range of 0-2500psi. The output of the pressure sensor is cascaded with a microcontroller to process the signal and display the pressure of oxygen cylinder. Whenever the level of oxygen is below a pre-decided value, a signal is further transmitted to the monitoring station through wireless communication module which in turn uses indoor localization [ Google's geo location API ] which further conveys the location of the cylinder alerts the nearest attendant of the patient, so that the patient can be attended at the quickest. Graphical display is used at monitoring station to indicate the pressure in the oxygen cylinders to initiate actions like replacement of empty cylinders with filled ones.

# References: 
1) https://ieeexplore.ieee.org/document/621606
2) https://ieeexplore.ieee.org/abstract/document/8821209 

![image](https://user-images.githubusercontent.com/83449084/118696139-431da000-b80e-11eb-89e9-264a2cf28c09.png)


# Time plan:

Week 21-2021 Acquiring pressure transducer values and sending it to Arduino

Week 22-2021	Sending values to the cloud - check MQTT connection using ESP32 pico kit

Week 23-2021	Acquiring location details of the cylinder using GOOGLE LOCATION API

Week 24-2021	Calibration and evaluvation of real-time results

Week 25-2021	Integration

Week 26-2021	Flutter Mobile APP to connect to mqtt cloud

Week-27-2021 Alerts using Flutter app

Week-28-2021	Pre-final presentation and improvement

Week-29-2021	Final presentation

BOM link: 		https://octopart.com/bom-tool/JY80t9N7 

# Evaluation plan:

•	Correctness of the pressure values from the pressure transducer

•	Extracting location details using geo-location api succesfully

•	Receiving alerts immediately as soon as the pressure decreases beyond the threshold value. 




