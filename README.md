# posedetectionmediapipe1
This code can detect different poses like Namaste Pose, Standing, etc. in real time through video. 

Sample Python program conducting real time pose detection using MediaPipe (to obtain features/landmarks through video), Machine Learning (taking sample poses for training coordinates to make predictions), OpenCV (rendering). 

Renders probability of the user doing the expert move. Tested 4-5 moves, 3 Yoga poses (Tree, Warrior, Namaste), Sitting, Standing. Logistic Regression and Ridge Classifier yield ~70% accuracy.  
Currently only running on Mac webcam (future would like to deploy to phone)
Difficulty in obtaining the most accurate training "expert" poses due to webcam footage and limited space filming 

Converted NN model yielding ~66% accuracy to ONNX to deploy to Unity. 

In Process/Goals:
Connecting the above program to Unity to outsource to ios/phone development
Python with Unity only supports Version 2, but Python with Media Pipe is best w/ P3) 
Solutions: 
MediaPipe Unity Plug-In (Requires C#, not Python code) 
Rewriting program to fit C# MediaPipe Unity using same steps as before 
Holistic Barricuda → was not able to configure  
- Train more Yoga poses (add series to monitor step by step) 
- Overall accuracy rendered to user of how well they did throughout, not just by pose 
