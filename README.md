# The repository of data collected during the IoCT-Care project  
  
This repository is the public description of the data collected for evaluation and experiments during the research on the IoCT-CARE project, a joint project between the Academy of Finland and the National Science Foundation (NSF) of the United States. The data files are available in University of Turku projects repository (https://gitlab.utu.fi/) and can be accessed upon request.
  
## Shimmer data  
The data is collected with a Shimmer ExG device. The ExG module provides a configurable digital front-end, optimized for the measurement of physiological signals for example 5-lead ECG (Electrocardiography) or 2-channel EMG (Electromyography).  
These files contain continuous ECG and IMU data collected from 3 subjects during their daily activities.  
The first subject monitored for 12 hours and 38 minutes. The file size is 3.24GB.  
The second subject monitored for 16 hours and 2 minutes. The file size is 4.12GB.  
The third subject monitored for 26 hours and 14 minutes. The file size is 6.69GB.  
The purpose was to study the effect of the intensity of daily activities on vital signs. The data are stored in CSV format and contains:  
  
- Timestamp, (ms)  
- Acceleration Linear X, m/(s^2)  
- Acceleration Linear Y, m/(s^2)  
- Acceleration Linear Z, m/(s^2)  
- Acceleration Wide-range X, m/(s^2)  
- Acceleration Wide-range Y, m/(s^2)  
- Acceleration Wide-range Z, m/(s^2)  
- Battery, mV  
- ECG_EMG_Status1  
- ECG_EMG_Status2  
- ECG LA-RA, mV  
- ECG LL-LA, mV  
- ECG LL-RA, mV  
- ECG_Vx-RL, mV  
- Gyroscope X, deg/s  
- Gyroscope Y, deg/s  
- Gyroscope Z, deg/s  
- Magnetometer X, local_flux  
- Magnetometer Y, local_flux  
- Magnetometer Z, local_flux  
- Air Pressure, kPa  
- Temperature, Degrees Celsius  
  
## BioHarness data  
The data is collected with a BioHarness 3 chest strap. It stores and transmits vital sign data including ECG, heart rate, respiration rate, body orientation, and activity.   
Data is collected from 5 subjects, each subject 10 minutes. The file format is CSV, the sampling rate is 1Hz, and the file size is around 10MB.  
The structure of the CSV file is as follow:  
  
- Time  
- Heart Rate  
- Respiration Rate  
- Skin Temperature  
- Posture  
- Activity  
- Peak Acceleration  
- Battery Voltage  
- Battery Level  
- Breathing Wave Amplitude  
- Breathing Wave Noise  
- Respiration Rate Confidence  
- ECG Amplitude  
- ECG Noise  
- Heart Rate Confidence  
- HRV  
- System Confidence  
- GSR  
- ROGState (Color indication of subject physiological status in BioGauge)  
- ROG Time  
- Vertical Posture Wave Minimum  
- Vertical Posture Wave Peak  
- Lateral Posture Wave Minimum  
- Lateral Posture Wave Peak  
- Sagittal Posture Wave Minimum  
- Sagittal Posture Wave Peak  
- Device Temperature  
- Status Info  
- Link Quality  
- RSSI  
- Tx Power  
- Core Temperature  
- Aux ADC1 (not used)  
- Aux ADC2 (not used)  
- Aux ADC3 (not used)  
  
  
## PPG data including accurate baselines  
<b>First set:</b> Data collected from 8 subjects, each subject 15 minutes.  
The file format is CSV, the sampling rate is 50Hz, and the file size is around 3.2MB.  
  
The structure of the CSV file is as follow:  
  
- Timestamp, microsecond  
- PPG LED current, micro Amper  
- Tested IR LED reflection intensity   
- Tested red LED reflection intensity  
- Baseline ECG-based heart rate  
- Baseline respiration, Airflow sensor  
- Body temperature  
- Baseline IR LED reflection intensity   
- Baseline red LED reflection intensity  
- Acceleration X  
- Acceleration Y  
- Acceleration Z  
- Baseline body temperature  
  
  
<b>Second set:</b> 12.5 hours of data is collected from 6 subjects, in 25 different conditions in including 5 types of activities (Sleeping, Sitting, Walking, Jogging, and Running) and 5 different levels of PPG sensor current consumption (0.8mA, 3.5mA, 6.3mA, 9.2mA, and 12mA). There are 150 files, each file contains 5 minutes of recorded data, the average file size is 3.7MB, and the sampling rate is 50Hz.  
  
- The structure of the CSV file is as follow:  
- Timestamp, millisecond  
- Baseline IR LED reflection intensity   
- Baseline red LED reflection intensity  
- Tested IR LED reflection intensity   
- Tested red LED reflection intensity  
- Baseline respiration, Airflow sensor  
- Acceleration X  
- Acceleration Y  
- Acceleration Z  
- Body temperature  
- Baseline ECG-based heart rate  

If you used this data repository in your research please reference the data source by citing the following paper:  
- Arman Anzanpour, Delaram Amiri, Iman Azimi, Marco Levorato, Nikil Dutt, Pasi Liljeberg, and Amir M. Rahmani. 2020. Edge-Assisted Control for Healthcare Internet of Things: A Case Study on PPG-Based Early Warning Score. ACM Trans. Internet Things 2, 1, Article 1 (October 2020), 21 pages. DOI:https://doi.org/10.1145/3407091  
  
```

@article{10.1145/3407091,  
author = {Anzanpour, Arman and Amiri, Delaram and Azimi, Iman and Levorato, Marco and Dutt, Nikil and Liljeberg, Pasi and Rahmani, Amir M.},  
title = {Edge-Assisted Control for Healthcare Internet of Things: A Case Study on PPG-Based Early Warning Score},  
year = {2020},  
issue_date = {October 2020},  
publisher = {Association for Computing Machinery},  
address = {New York, NY, USA},  
volume = {2},  
number = {1},  
issn = {2691-1914},  
url = {https://doi.org/10.1145/3407091},  
doi = {10.1145/3407091},  
journal = {ACM Trans. Internet Things},  
month = oct,  
articleno = {1},  
numpages = {21},  
keywords = {Internet of Things, edge computing, Health monitoring, wearable electronics, early warning score, edge-assisted control}  
}  
 
```

