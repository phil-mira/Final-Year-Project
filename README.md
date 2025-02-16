# Final-Year-Project: Machine Learning for a Wearable Network of Inerital Sensors

This repository contains samples of results and evidence of data collection from my final year project completed in Machine Learning for a Wearable Network of Inerital Sensors at the University of Bath under the supervision of Dr Alan Hunter. Due to the code being in partnership with a small startup the code developed is not avaliable along with the full results or methodoolgy section. I have included snippets from the abstract, aims and results sections. 

## Abstract:
>Several models were developed to attempt to classify barbell exercises, segment individual reps and recognize the quality of the reps from data collected using bespoke wireless inertial measurement units measuring accelerometer and gyroscopic data attached to various locations on the body. These sensors were provided by  an external company who commissioned this project. Data was collected from participants wearing the sensors in set configurations on the body performing squats, cleans, or deadlifts all using a barbell. An app on a smartphone was used to record the data and upload it to a Google Firebase server. The collected data was then pre-processed, labelled with the start of each rep and fed into an ML model for segmentation and classification using the sliding window technique across the each of the recordings in the dataset. Initially a squat classifier using a specific configuration of sensors was developed with a binary output achieving a balanced accuracy of 79% but was trained and tested on a small dataset with missing data, using leave-one-out cross validation. This was extended to two CNNs of different architectures developed to classify and segment all the exercises for a specific sensor configuration. These performed poorly achieving 69% and 62% balanced accuracy but were trained and tested on a small dataset with missing data, using leave-one-out cross validation. An investigation of the effect of sensor placement was carried out. This investigation varied the inputs to the multi exercise CNNs by using data from combination of sensors located at different parts of the body. This produced better results as more data was available for each model then for the specific sensor configuration and did not contain data with missing sensors. The investigation achieved a balanced accuracy of 77% on the best performing sensor combination of the upper arm, chest, and upper leg; these locations were noted as the best for sensor placement. It was found that the models struggled with classification due to varying techniques. Issues with the methods and models used were highlighted as well as differences between results of the project and that of the literature. Improvements to the models and methods as well as avenues for future work were suggested.


## Aims: 

>1) Can [ML models] be used to segment and classify squat reps for a fixed sensor configuration?
>2) Can [ML models] be used to segment and classify reps of squats, deadlifts, and cleans? Is it better to train a single multi-output network or multiple binary output ones?
>3) What are the best possible sensor locations for classifying exercises and segmenting reps for squats, deadlifts, and cleans from the data collected?
>4) Can [ML models] be used to recognize the quality of technique for squats, deadlifts, and cleans and what is the best sensor locations for this task?



## Methods:
Please see snipptet of the png for the sliding window method for classifying rep locations,


## Results
Please see snippet of the confusion matrix showing the results for one of the sensor configurations. 
