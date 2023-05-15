# Signal Processing Techniques to Improve Feature Space for EEG-based Epileptic Seizure Detection

<p align="justify"> 
Bio-signal processing is an evolving field of science that is critical in the diagnosis, and prognosis of diseases 
and timely intervention to reduce the impact of the disease on the patients. In recent years, the research 
interests have been largely shifted to analyze the functionality of the brain to identify the structural and 
functional changes and characteristics that correspond to different types of neurological disorders including
epileptic seizures, and Alzheimer’s. In this project, the broad objective is oriented toward detecting epileptic 
seizures by analyzing Electroencephalography (EEG) signals recorded in-vivo from the patients diagnosed 
with the disease. 
</p>

![Overall Project Idea](Figures/Picture1.png)

## Dataset

<p align='justify'>
For this project, a publicly available Epileptogie dataset [1] is used which consists of 5 subsets, each containing 
100 EEG segments. The data is sampled at a sampling rate of 173.61 Hz which is recorded using a 128-channel 
amplifier system with an average common reference. The recorded signals have a spectral bandwidth of 0.5 
Hz to 85 Hz. These continuous multichannel EEG recordings from multi-spatial locations are segmented into 
23.6s long epochs after visually inspecting the presence of any artifacts [1]. For this project, I selected 
Intracranial EEG signals that are captured within hippocampus formation.
</p>

|                       Summary of Dataset                    ||
|------------------------------------|:-----------------------:|
|Sampling Frequency                  |173.63Hz                 |
|Inter-Ictal EEG Signal Dataset (D)  |100 segments             | 
|Ictal EEG Signal Dataset (E)        |100 segments             |
|Recording Site                      |Hippocampus Formation    |
|Type of Data                        |Intracranial EEG (iEEG)  |
|Segment Length                      |23.6s (4097 samples)     |
