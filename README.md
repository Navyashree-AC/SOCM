# SOCM - Smart Oxygen Cylinger Monitoring

Project vision:
The amount of oxygen present inside an oxygen cylinder is a very vital piece information when such cylinders are in use for supply of oxygen in the current COVID scenario. Since the number of patients infected by COVID are very large, it becomes difficult to monitor all the isolation wards in the hospital simultaneously. Therefore, we aim to design a smart oxygen cylinder to automate this monitoring process by using a pressure sensor at the nozzle of the oxygen cylinder and using a precision barometric pressure and altimeter sensor to isolate the location of the cylinder that requires a refill. 

Description and realization:
Components:
•	Arduino development board – ATMEGA 32U4
•	Node MCU – ESP-8266
•	Precision Barometric Pressure and Altimeter - Adafruit BMP390L
•	Pressure transducer – M3031
•	Amplifier circuit 
The amount of oxygen present inside the cylinder is measured by the pressure at the outlet nozzle. The pressure is measured using a high precision Pressure Sensor. The output of the pressure sensor is cascaded with a microcontroller to process the signal and display the pressure of oxygen cylinder. Whenever the level of oxygen is below a pre-decided value, a signal is further transmitted to the monitoring station through wireless communication module which in turn uses indoor localization which further conveys the exact location of the cylinder to give more accurate location of the oxygen cylinder in a populated hospital room and alerts the nearest attendant of the patient, so that the patient can be attended at the quickest. Graphical display is used at monitoring station to indicate the pressure in the oxygen cylinders to initiate actions like replacement of empty cylinders with filled ones.
References: 
1) https://ieeexplore.ieee.org/document/621606
2) https://ieeexplore.ieee.org/abstract/document/8821209 

![image](https://user-images.githubusercontent.com/83449084/118696139-431da000-b80e-11eb-89e9-264a2cf28c09.png)


Time plan:
Week 21-2021	Acquiring pressure transducer values and sending it to Arduino
Week 22-2021	Acquiring location details of the cylinder
Week 23-2021	Sending values to the cloud
Week 24-2021	Getting alerts to mobile
Week 25-2021	Integration
Week 26-2021	Pre-final presentation and improvement
Week-27-2021	Pre-final presentation and improvement
Week-28-2021	Final presentation
Week-29-2021	Final presentation

BOM link: 		https://octopart.com/bom-tool/JY80t9N7 

Evaluation plan:
•	Correctness of the pressure values from the pressure transducer
•	Extracting accurate location details
•	Receiving alerts immediately as soon as the pressure decreases beyond the threshold value. 




