
# Human Identification Using Openpose

## Project Title: 
#### Human Identification Via Walking Posture

Due to the Covid-19 situation, people are made to wear masks. This will make facial recognition difficult. 
Therefore, other human identification methods will be required. 

Gait recognition may be a feasible method for human identification. 

Human gait or walking manner is a potential biometric feature that provide unique identification of a person when other biometric featues such as face is not visible. Gait recognition also has the added advantage that it can be performed at a long distance, and requires no physical contact with surfaces or close proximity to another human.    

## Objective:
#### Develope a Neural Network based algorithm to recognize a person from video footage of walking posture.

#### Reference Paper : 
Human Identification From Freestyle Walks Using Posture Based Gait Feature

https://ieeexplore.ieee.org/document/8007293

### Training Dataset:

Training dataset consist of video footage of walking postures. 

**Download Dataset :**. https://data.mendeley.com/datasets/gprg4s73v4/2 

This video dataset comprises (44) recordings of the human gait with (396) edited videos, with stable background.

Pose estimation is used to generate keypoint data from video frames. The keypoint data will then be input to a neural network as training data. Below are screenshots of a video of a subject walking and the keypoints are identified using pose estimation.

**This Project Uses OPENPOSE as a real time multi-person system to detect human body keypoints on single images**

https://github.com/CMU-Perceptual-Computing-Lab/openpose

![SubjectWalkingWithkeypoints](https://user-images.githubusercontent.com/61535921/120775133-8178c600-c555-11eb-84be-7bf6b2a63727.png)


The output of the JSON files consist of a set of keypoints, whose ordering is realted with the outputformat shown:

**Pose Output Format (COCO) - total of 18 keypoints**

![OpenPose_keypoints](https://user-images.githubusercontent.com/61535921/120775746-18458280-c556-11eb-9e94-be72ee757ab0.png)


**Running OPENPOSE throught our training dataset, the number of video frames with keypoints detected are:**

![NumberOfFramesWithKeypointsDetcted](https://user-images.githubusercontent.com/61535921/120775752-1976af80-c556-11eb-861f-1f34b5d91bc3.png)

**Using a sample training data, I illustrate how the keypoints coordinates changes over time across the image frame:** 

![KeypointsMovementOverFrame](https://user-images.githubusercontent.com/61535921/120776096-6e1a2a80-c556-11eb-9308-29696f0ca6a5.png)


![FramesInSequentialOrder](https://user-images.githubusercontent.com/61535921/120776100-6f4b5780-c556-11eb-85bd-62c92cd8a505.png)

### Gait Recognition Model And Results

#### Gait Recognition Model
![GaitRecognitionModel](https://user-images.githubusercontent.com/61535921/120878533-b6d1f200-c5ef-11eb-9ab8-4bc91da6497f.png)

#### Gait Recognition Accuracy, Loss Curve
![GaitRecognitionAccuracyLossCurve](https://user-images.githubusercontent.com/61535921/120878539-c3564a80-c5ef-11eb-87e5-0226176333ce.png)

#### Gait Recognition Confusion Matrix
![GaitRecognitionConfusionMatrix](https://user-images.githubusercontent.com/61535921/120878541-c7826800-c5ef-11eb-857d-66ad7b9ebf37.png)



### Gait Verification Model And Results

![DataAugmentation](https://user-images.githubusercontent.com/61535921/120878633-5d1df780-c5f0-11eb-93a6-d9ec38e904b3.png)
![SiameseModel](https://user-images.githubusercontent.com/61535921/120878639-6313d880-c5f0-11eb-95e5-549d165eb140.png)
![SiameseModelDiagram](https://user-images.githubusercontent.com/61535921/120878641-66a75f80-c5f0-11eb-86c8-888e368b9a6d.png)
![SiameseModelResult](https://user-images.githubusercontent.com/61535921/120878643-69a25000-c5f0-11eb-9999-876ef2608324.png)
![NumberOfFramesAndResults](https://user-images.githubusercontent.com/61535921/120878645-6c04aa00-c5f0-11eb-8911-3f347895ba4c.png)



### Video Of Keypoint Extraction Using Openpose :

[![Watch the video](https://user-images.githubusercontent.com/61535921/120838500-74ca9100-c59a-11eb-9891-b6683f98a94b.png)](https://drive.google.com/file/d/1TGUPnTu4VeK-PUUsh7wZn62VIQfJMnoR/view?usp=sharing)

### Video Of Onboarding New Personnel:

[![Watch the video](https://user-images.githubusercontent.com/61535921/120838512-785e1800-c59a-11eb-9adb-5ce94af596c6.png)](https://drive.google.com/file/d/1FOGhffbtyeaY5Dpzb8qx7bUl-oeTIM4A/view?usp=sharing)

### Video Of Model Inference On Onboarded New Personnel: 

[![Watch the video](https://user-images.githubusercontent.com/61535921/120878275-dbc56580-c5ed-11eb-8c7e-d860913daa72.png)](https://drive.google.com/file/d/12-17gPIUk96K-SZwv5hrG5sYQl88JvTK/view?usp=sharing)





