Face Liveness Detection (CRMNet)
alt text

Description
CRMNet: A deep-learning pipeline capable of spotting fake vs legitimate faces and performing anti-face spoofing in face recognition systems. It is built with the help of Keras, Tensorflow, and OpenCV. A sample dataset is uploaded in the sample_dataset_folder.

Method
The problem of detecting fake faces vs real/legitimate faces is treated as a binary classification task. Basically, given an input image, we’ll train a Convolutional Neural Network capable of distinguishing real faces from fake/spoofed faces. There are 4 main steps involved in the task:

Build the image dataset itself.
Implement a CNN capable of performing liveness detector(Livenessnet).
Train the liveness detector network.
Create a Python + OpenCV script capable of taking our trained liveness detector model and apply it to real-time video.
Create a webplatform to access the liveness detection algorithm in an interactive manner.
Contents of this repository
sample_liveness_data : contains the sample dataset.
Face Liveness Detection -Saketh.pptx : A couple of slides that will give you information on th project and our motivation.
demo.py : Our demonstration script will fire up your webcam to grab frames to conduct face liveness detection in real-time.
deploy.prototxt : Support file for pretrained face detector.
le.pickle : Our class label encoder.
liveness.model : The liveness model file.
livenessnet.py : The python file containing the model.
res10_300x300_ssd_iter_140000.caffemodel: Pretrained face detector.
train_liveness.py: The python script to train the model.
Working flow
alt text

Further work
Gathering data having a larger set of ethnicity and different types of fake/spoofed photos.
Adding more heuristics to team up with deep-learning.
Disclaimer
This work was done during my internship at SimpleCRM, Nagpur.
