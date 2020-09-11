# Optical Charachter Recognition using Tesseract
[![Watch the video](https://github.com/sakethbachu/ocr_using_tesseract/blob/master/Img/gif%20of%20visionapi.gif)](https://github.com/sakethbachu/ocr_using_tesseract/blob/master/Img/visionraw.mp4)

# Description
Optical charachter recognition is one of the most important tasks in today's automated world. In this repository we have used both Tesseract and Vision-api by Google. We did not benchmark the results obtained by the methods. In this, we will perform both (1) text detection and (2) text recognition using OpenCV, Python, and Tesseract. To perform text detection we use OpenCV’s EAST deep learning model. Using this model we were able to detect and localize the bounding box coordinates of text contained in an image. The next step is to take each of these areas containing text and actually recognize and OCR the text using OpenCV and Tesseract.

# Methods
* In order to perform OpenCV OCR text recognition, we’ll use Tesseract v4 which includes a highly accurate deep learning-based model for text recognition.
* Once we have detected the text regions with OpenCV, we’ll then extract each of the text ROIs and pass them into Tesseract, enabling us to build an entire OpenCV OCR pipeline.

# Features
Tesseract api is an LSTM network used for text recognition. The overall pipeline is given below.
![alt text](https://github.com/sakethbachu/ocr_using_tesseract/blob/master/Img/opencv_ocr_pipeline.png "Logo Title Text 1")

# Contents of this repository
* OCR_source file.py : This is the main python source file to do ocr using tesseract.
* Img : Contains the descriptive images and the omr-sheet.

# Requirements
* Python
* OpenCV
* Tesseract v4
* Google Vision API

# Usage
Use this in command line where python is installed  `python text_recognition.py --east frozen_east_text_detection.pb \ --image images/example_01.jpg`

# Demo
![alt text](https://github.com/sakethbachu/ocr_using_tesseract/blob/master/Img/address.png "Logo Title Text 1")
