# Numberplate_detection


## License Plate Recognition and Extraction Using OpenCV
Automatic number plate recognition (ANPR) is a prevalent computer vision task with various applications.

Common Use Cases:

Toll booth operations
Detection of stolen vehicles
Traffic management systems
Smart parking solutions
In this tutorial, we will build a fundamental automatic number plate recognizer using OpenCV and Python. Once the number plate is recognized, we will employ EasyOCR to extract the vehicle's number from it.

What is OpenCV? OpenCV is a powerful Computer Vision library originally developed in C/C++. It is also available for Python and is extensively used for image processing and real-time vision applications. With over 2500 built-in image processing algorithms, OpenCV is capable of performing a wide range of image processing tasks.

What is EasyOCR? EasyOCR is a Python package designed for Optical Character Recognition (OCR). OCR is a method for extracting and recognizing text from various sources, such as images and PDFs. EasyOCR simplifies text extraction, making it easy to implement OCR capabilities in Python applications.


For our project, we'll utilize EasyOCR to extract the vehicle number from the detected number plate.

How Will We Detect the Number Plate?

We'll employ a Haar Cascade classifier for number plate detection. Haar Cascade is a feature-based object detection method that identifies objects by matching approximately 16,000 features in an image.

What is Object Detection?

Object detection involves identifying and locating specific objects within an image. In our case, we’ll use this technique to find and isolate the number plate from the vehicle’s image.

Haar Features and Training
To train a Haar Cascade classifier, a large set of images is required. This includes:

Positive Images: These images contain the object we want to detect (e.g., number plates).
Negative Images: These images do not contain the object we want to detect.
The Haar Cascade classifier uses these images to learn and identify patterns specific to the object of interest—in this case, number plates.

For our project, we'll use a pre-trained Haar Cascade classifier designed specifically for number plate recognition to detect number plates in images.

Prerequisites
Before starting the project, ensure you have the following software and libraries installed:

Python 3.x (We used Python 3.7.10 for this project)
EasyOCR 1.4
OpenCV 4.5
You can install the required packages using pip:


    pip install easyocr==1.4 opencv-python==4.5

Download the Project Code
You can download the source code for the License Plate Recognition project using OpenCV from the following link: License Number Plate Recognition Project Code

Steps to Implement the Number Plate Recognition Project
Import Necessary Packages and Initialize the Classifier: Set up the environment by importing the required libraries and loading the Haar Cascade classifier.

Detect Number Plate from an Image: Use the Haar Cascade classifier to locate and extract the number plate from the given image.

Extract Text from the Detected Number Plate: Apply EasyOCR to extract the text (vehicle number) from the identified number plate.
