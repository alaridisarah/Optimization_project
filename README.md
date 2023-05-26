# Optimization and Metaheuristics project

[Original Code](https://github.com/soumitri2001/Wrapper-Filter-Speech-Emotion-Recognition)

Speech Emotion Recognition is the process of detecting the emotional state of a speaker by analyzing their speech signal. It involves extracting relevant features from the speech signal and using machine learning algorithms to classify the emotion expressed in the speech. SER has applications in psychology, healthcare, and human-computer interaction.

Feature selection is a process in machine learning where a subset of the original features or variables in a dataset is selected for use in a model. The goal of feature selection is to identify the most relevant features that have the strongest predictive power and remove or ignore the less important ones. In this repository will using an optimization algorithm to u important features.

## Overall process 
![1](https://b.top4top.io/p_2702bzsgh1.png)
## Requirements
To install all requirments run this code:
```bash
pip install -r requirements.txt
```
## Dataset
The dataset that used is The EMODB database which is German emotional database. EMODB has seven classes Boredom, Fear, Disgust, Happiness, Sadness, Anger, and Neutral. In order to spilt this dataset into train and val we're use splitfolders library, first must install: 
```bash
 pip install split-folders
 ```
Next run this code, we spilt this dataset into 80% train 20% val.
```bash
import splitfolders
splitfolders.ratio("/EMO-DB_dataset", # The location of dataset
                   output="/data_audio", # The output location
                   seed=42, # The number of seed
                   ratio=(.8, .2, 0), # The ratio of splited dataset
                   group_prefix=None, # If your dataset contains more than one file like ".jpg", ".pdf", etc
                   move=False # If you choose to move, turn this into True
                   )
```
Required directory structure: ("data_audio" directory contains class-wise the raw audio ).
```bash
+-- data_audio
|   +-- .
|   +-- train
|   +-- val
+-- PasiLuukka.py
+-- WOA_FS.py
+-- __init__.py
+-- audio2spectrogram.py
+-- main.py
+-- model.py
```
## Running the code 
In the uploaded files there is a notebook you just need to run all cell.

## Done by
- [Sarah Alaridi](https://github.com/alaridisarah)
- [Reem Alqahtani](https://github.com/reemabdulmohsen)
- [Shoug Alsuhaibani](https://github.com/alsuhaibanishoug)
- [Reema Aloqayli](https://github.com/Roqayli)
- [Norah Alsharhan](https://github.com/Noraty)



