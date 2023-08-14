Drowsiness Detection System using Python and Computer Vision
Drowsiness Detection

This repository contains a Python script for a Drowsiness Detection System using computer vision techniques and deep learning. The system monitors a person's eyes in real-time using a webcam feed and alerts them if their eyes are closed for an extended period, indicating drowsiness. It employs the popular Pygame library for audio alerts and OpenCV for image processing.

Features
Detects closed and open eyes using Haar Cascade classifiers.
Utilizes a pre-trained convolutional neural network (CNN) model to classify eye states.
Provides real-time feedback on eye status and a drowsiness "score."
Raises an audio alarm when the drowsiness score surpasses a certain threshold.


Prerequisites
Python 3.10 or later
OpenCV (cv2)
Pygame
Keras (with TensorFlow backend)

Installation
Clone this repository to your local machine:
git clone https://github.com/AnuragNagare/drowsiness-detection.git
cd drowsiness-detection

Install the required dependencies:
pip install opencv-python pygame keras

1]Download the Haar Cascade XML files for face and eye detection and place them in the appropriate directory (haar cascade files).

2]Download the pre-trained CNN model for eye state classification (e.g., cnncat2.h5) and place it in the models directory.

Usage
1]Run the drowsiness_detection.py script:
python drowsiness_detection.py

1]The script will launch the webcam feed, and you'll see real-time video with rectangles around detected faces and eyes. The drowsiness score and status (open/closed eyes) will be displayed on the frame.

2]If the drowsiness score exceeds a threshold, an audio alarm will sound, and a red rectangle will be drawn around the video frame.

Customization
1]Adjust the drowsiness threshold (score > 15) in the script to set when the alarm should trigger.
2]Customize the audio alarm by replacing alarm.wav with your preferred sound file.

Contributions
Contributions to this project are welcome! If you find any issues or have enhancements to propose, feel free to submit a pull request.

Credits
Original author: Anurag Nagare
This project is inspired by various drowsiness detection systems and open-source computer vision projects.
