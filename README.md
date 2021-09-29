# Gesture Based - Touchless ATM

Gesture Based - Touchless ATM demonstrates a novel way of interacting with ATM machines without the user having to physically touch any part of it. It aims to eliminate the risk of transmission of infectious diseases - such as COVID-19 - that spread through touch.<br><br>


## Installation and Setup:

1. Please get following python libraries:<br>
    - ```pip install opencv-python```<br>
    - ```pip install mediapipe```<br>
    - ```pip install face_recognition```<br>
2. Please create a directory/folder named as “Faces” (case sensitive and without quotes) to store the images of human faces to be matched with faces in video frame.
3. Have a look at the file ```config.py``` in which various configuration parameters are mentioned with their usage. Modify these as per your needs or preferences. Elements such as buttons and text shown on all the pages will be adjusted as per these parameters.<br>

**Note:** While making changes to ```screen_x``` and ```screen_y``` variables in config file, remember that resolution of your webcam should be the maximum resolution you set and not your screen resolution.


## Usage:

You just need two things - your face and one hand. Begin by placing your face in the video frame and with your finger, select the Match button shown on first screen as follows:<br><br>
![Blurred face](https://user-images.githubusercontent.com/25917944/135302560-1f9d16c3-d7b9-4270-933a-6eaa9ffaae76.png)<br><br>

If your face matches with faces from at least one image in the Faces folder, you should be able to go ahead and do the following:<br><br>
![Demo Part 1](https://user-images.githubusercontent.com/25917944/135302527-e3ca914b-c2b9-4657-bc34-49fc2af62f05.gif)<br><br>
![Demo Part 2](https://user-images.githubusercontent.com/25917944/135302516-9c730ff5-d5dc-4d24-bb27-addb50c8bc84.gif)<br><br>


## Technologies Used:

In this project I’ve used open source technologies such as OpenCV, MediaPipe, and Face Recognition python libraries. These technologies/libraries provide abilities to perform various tasks with webcam and its content, tracking of hand(s), and recognising a person’s face respectively. The particular libraries used for this project are standard for the tasks they perform from the collection of publicly available libraries. They also provided all the necessary functions required to achieve the objective. Hence, they were the options chosen by me.


## Challenges Faced:

* Coming up with a way for handling various camera resolutions while processing the video frame.
* Simulating page navigation with changing the content being drawn over the frame.
* Coming up with an interface intuitive and simple enough to be used.
* Using position of fingertip to simulate a “virtual” button click.
* Making the experience identical to real life ATMs.


## References:

* [OpenCV](https://github.com/opencv/opencv)
* [MediaPipe](https://github.com/google/mediapipe)
* [MediaPipe Hand Detection](https://google.github.io/mediapipe/solutions/face_detection)
* [Face Recognition Python Library](https://github.com/ageitgey/face_recognition)
