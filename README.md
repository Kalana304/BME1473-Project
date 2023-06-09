# Signal Processing Techniques to Improve Feature Space for EEG-based Epileptic Seizure Detection

<p align="justify"> 
Bio-signal processing is an evolving field of science that is critical in the diagnosis, and prognosis of diseases and timely intervention to reduce the impact of the disease on the patients. In recent years, the research interests have been largely shifted to analyze the functionality of the brain to identify the structural and functional changes and characteristics that correspond to different types of neurological disorders including epileptic seizures, and Alzheimer’s. In this project, the broad objective is oriented toward detecting epileptic seizures by analyzing Electroencephalography (EEG) signals recorded in-vivo from the patients diagnosed with the disease. 
</p>

![Overall Project Idea](Figures/Picture1.png)

## Dataset

<p align='justify'>
For this project, a publicly available Epileptogie dataset [1] is used which consists of 5 subsets, each containing 100 EEG segments. The data is sampled at a sampling rate of 173.61 Hz which is recorded using a 128-channel amplifier system with an average common reference. The recorded signals have a spectral bandwidth of 0.5 Hz to 85 Hz. These continuous multichannel EEG recordings from multi-spatial locations are segmented into 
23.6s long epochs after visually inspecting the presence of any artifacts [1]. For this project, I selected Intracranial EEG signals that are captured within hippocampus formation.
</p>

|Properties of Dataset               |Values                   |
|------------------------------------|:-----------------------:|
|Sampling Frequency                  |173.63Hz                 |
|Inter-Ictal EEG Signal Dataset (D)  |100 segments             | 
|Ictal EEG Signal Dataset (E)        |100 segments             |
|Recording Site                      |Hippocampus Formation    |
|Type of Data                        |Intracranial EEG (iEEG)  |
|Segment Length                      |23.6s (4097 samples)     |


## Methodology and Results
For the details on the methodologies used to analyze EEG signal in the project and the results obtained for Epileptic Seizure Detection, please refer to Section 2 and Section 3 respectively of the [Report](https://github.com/Kalana304/BME1473-Project/blob/main/Docs/Kalana%20Abeywardena%20-%20BME%201473%20-%20Project%20Report%20Final.pdf).

## Run the code
The codes are provided in [Scipts](https://github.com/Kalana304/BME1473-Project/tree/main/Scripts) as Jupyter Notebooks. The notebooks were designed and executed in Google Colab.
- ***01_DatasetAnalysis.ipynb*** : Use to visualize and analyse the Dataset used. If you are uisng a different dataset, the codes may need to change.
- ***02_Denoising.ipynb*** : Use to run the preprocessing pipeline of the dataset -- including detrending and sphering and denoising. 
- ***03_FeatureExtraction.ipynb*** : Uses to extract the features from the saved preprocessed data files from earlier step. For this FeatureExtraction.py is used as a Util file which is based on these [tutorials](https://github.com/Eldave93/Seizure-Detection-Tutorials).
- ***04_Classification.ipynb*** : Performs Epilepsy detection and evaluates the performance. 
## References
```
[1] I. Ullah, M. Hussain, E. ul H. Qazi, and H. Aboalsamh, “An automated system for epilepsy detection using EEG brain signals based on deep learning approach,” Expert Syst Appl, vol. 107, pp. 61–71, Oct. 2018.
[2] J. L. Semmlow and B. Griffel, “BIOSIGNAL and MEDICAL IMAGE PROCESSING Third Edition.”
```
