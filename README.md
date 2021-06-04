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

![SubjectWalkingWithkeypoints](https://user-images.githubusercontent.com/61535921/120775133-8178c600-c555-11eb-84be-7bf6b2a63727.png)

![OpenPose_keypoints](https://user-images.githubusercontent.com/61535921/120775746-18458280-c556-11eb-9e94-be72ee757ab0.png)

![NumberOfFramesWithKeypointsDetcted](https://user-images.githubusercontent.com/61535921/120775752-1976af80-c556-11eb-861f-1f34b5d91bc3.png)

![KeypointsMovementOverFrame](https://user-images.githubusercontent.com/61535921/120776096-6e1a2a80-c556-11eb-9308-29696f0ca6a5.png)
![FramesInSequentialOrder](https://user-images.githubusercontent.com/61535921/120776100-6f4b5780-c556-11eb-85bd-62c92cd8a505.png)


### Video Of Keypoint Extraction Using Openpose :
[![Watch the video](https://github.com/kenaimachine/HumanIdentification_Openpose/blob/f4219e5de2572359a6408186e83bca5f91a272ff/videos/KeypointExtraction.png)](https://github.com/kenaimachine/HumanIdentification_Openpose/blob/1fdf43519c84521c87a7868fe91abb40c0334ba0/videos/KeypointExtraction.mov)

### Video Of Onboarding New Personnel And Model Inference :
[![Watch the video](https://github.com/kenaimachine/HumanIdentification_Openpose/blob/f4219e5de2572359a6408186e83bca5f91a272ff/videos/OnboardingAndInference.png)](https://github.com/kenaimachine/HumanIdentification_Openpose/blob/f4219e5de2572359a6408186e83bca5f91a272ff/videos/OnboardingAndInference.mov)




https://github.com/kenaimachine/HumanIdentification_Openpose/blob/main/videos/OnboardingAndInference.mov
