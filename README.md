# Human Detector

tech: OpenCV
version: 1.0.1

![output_pharcyde_sm](https://user-images.githubusercontent.com/84317349/140078298-80a49eac-d547-4e7c-9b0e-174d8d0bc9d8.gif)

## Overview
This application detects and boxes humans in a video feed using MobileNet-SSD pre-trained model.<br>
The model was obtained from this repo : https://github.com/chuanqi305/MobileNet-SSD

Inference time (how quick the network processes the feed) is displayed at the bottom left corner of the video.

## Dependencies

1. Create a virtual environment :

        python -m venv virtual
        
2. Activate the virtual environment :

    on Linux:

        source virtual/Scripts/activate
        
    on Windows:
        
        .\virtual\Scripts\activate
        
3. Install the necessary librairies :

        pip install opencv-python
        pip install pyzbar

## Improvements

The current version of the application requires one video input and outputs the corresponding human-detected video.<br>
Following improvements are planned in the future :

v1.2:
+ allowing use of webcam feed

v2: 
+ deploying web application on Flask
+ allowing user to upload video or paste video url

v3: 
+ allowing triming of uploaded video
+ implementing output format options (for e.g. gif)