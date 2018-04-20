# Camera2Vision

# Documentation

This app aims at developing a non intrusive technique at imaging based automatic analysis to
extract and deliver relevant information to a blind person in a social setting.

The entire process can be divided into 3 stages
1. Using a pi-camera as a camera source
2. Face Detection
3. Extracting relevant features such as landmarks
4. Computing a rough estimate of the distance from the camera
5. Using the Head Pose, give a rough estimate whether the person in front is Looking or not

# Face Detection

The face detection algorithm used is the standard Google vision API. The link for the standard implementation
of the Face Tracker is https://github.com/googlesamples/android-vision

**Note**:
Face tracking extends face detection to video sequences. Any face appearing in a video for any length of time can be tracked.
That is, faces that are detected in consecutive video frames can be identified as being the same person. Note that this is not
a form of face recognition; this mechanism just makes inferences based on the position and motion of the face(s) in a video
sequence.

A feature class has been implemented that helps us in extracting relevant information such as the No of faces, distance from each face, 
mid-point between the eyes etc. successfully. We were inspired by @betri28/FaceDetectCamera.

# Basic UI of the App
![ss](https://user-images.githubusercontent.com/28651490/38755155-4f845f08-3f82-11e8-8396-b5595f1b3c90.jpeg)



