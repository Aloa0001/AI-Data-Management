# Cognitive Load and Wearable Integration Analysis 

## Project Proposal

### What is the problem that you will be investigating?
During the course of this project, the team will explore the correlation between physiological signals captured by wearable devices and cognitive load. 
The cognitive state of a user varies measurably between “resting” and “solving complex tasks”. While it is possible to detect and determine the cognitive state of a person via EEG sensors, it remains to be seen if other physiological data can provide the same results. 
The research question guiding the present study is: 
- ***Are there differences between physiological signals and their correlation with cognitive load based on the wearables used?***

### What is the motivation for this project?
By understanding how wearable data aligns with cognitive states, we aim to investigate real-time cognitive load estimation and evaluate the effectiveness of different wearable devices in capturing cognitive states.

### What data will you use? What preprocessing is required?
The chosen dataset is hosted by physionet.org under open-access. The data was recorded at AGH University of Science and Technology in 2022 [1]. The dataset is composed of two subsets of EEG and biodata: one collected during resting and one collected during a Stroop test. Physiological data from 11 participants was gathered in both sessions via wearables (Empatica E4 watch, Samsung Galaxy Watch4) and an EEG device (Muse) simultaneously. The data are now split in multiple subfolders (550 csv files), which will require merging; afterwards, data cleaning will be performed based on the project's scope. This project originates from a precursor study aimed at assessing the relationship between cognitive load and physiological signals, employing various EEG sensors and wearable devices [2].

### Methods for analyzing the data and come up with insights
Firstly, dimensionality reduction techniques will be applied to select the most meaningful features within the data. Secondly, supervised ML techniques (specifically, classification) will be employed. The cognitive state EEG data will be used as discriminant for predicting cognitive state from physiological signals recorded by the wearable devices. Some of the steps considered at this point are:
1. **Physiological Signal Analysis** - exploring physiological signals captured by wearables ( e.g., BVP, EDA, TEMP, PPG, and EEG signals).
2. **Cognitive Load Signal Analysis** - using machine learning model(s) to estimate cognitive load based on physiological signals.
3. **Comparative Analysis** - conduct a comparative analysis of the cognitive load estimation sourced from different wearables.

### How will you present the results?
Plots of the data will be produced during the process to create visualisations representing the relationships between cognitive load and physiological signals. 
Bar charts could be used for a comparative analysis visualisation, comparing the performance metrics (e.g., F-Score, Accuracy, Precision, Recall).

### How will you evaluate your results?
The team plans to evaluate results via F-score, an established method to assess the precision and recall of a classification model.
The model’s accuracy will be also presented and analysed. Correlation analysis will be used to examine the relationship between the physiological signals and the cognitive load levels.

## Project Implementation

### Dataset Exploration
#### Files Exploration
#### Attributes Relevance
#### Cognitive Load Approach

### Data Pre-processing
#### Dataset Attribute-based Filtering
#### Incomplete-Data Management

## References
[1] “CogWear: Can we detect cognitive effort with consumer-grade wearables? v1.0.0,” [Online]. Available: https://physionet.org/content/consumer-grade-wearables/1.0.0/ Accessed: Feb.  2024. 

[2] M. Grzeszczyk et al., “Can gamification reduce the burden of self-reporting in mHealth applications? A feasibility study using machine learning from smartwatch data to estimate cognitive load.” [Online]. Available: https://arxiv.org/pdf/2302.03616.pdf Accessed: Feb.  2024.
