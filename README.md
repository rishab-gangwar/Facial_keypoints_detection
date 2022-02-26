[//]: # (Image References)

[image1]: ./images/obamas.jpg "Facial Keypoint Detection"
[image2]: ./images/obamakeypoints.jpg "Facial Keypoint Detection"
[image3]: ./images/miche.png "Facial Keypoint Detection"
[image4]: ./images/haar_cascade_micheobama.png "Facial Keypoint Detection"

# Facial Keypoint Detection

## Project Overview

This project uses computer vision techniques and deep learning architectures to build a facial keypoint detection system. Facial keypoints include points around the eyes, nose, and mouth on a face and are used in many applications. These applications include: facial tracking, facial pose recognition, facial filters, and emotion recognition. Task was that our model should be able to look at any image, detect faces, and predict the locations of facial keypoints on each face; examples of the one such sample image and its detection is shown below.
<br>
## `Sample Input`
![obamamiche][image1]
<br>
## `haar cascade classifier's output`
![face detected][image4]
## `Model Output`:
![obama][image2]
![miche][image3]


The project is broken up into in four Python notebooks

__Notebook 1__ : Loading and Visualizing the Facial Keypoint Data

__Notebook 2__ : Defining and Training a Convolutional Neural Network (CNN) to Predict Facial Keypoints.Please note that the main aim of project was to build the end to end pipeline and not just training model for better results, Although one must do it.The model uses sufficient regularization techniques.So,if you want better results train the model for few more epochs and don't forget to change your latest saved model's path in the inference(Notebook 3) notebook.

__Notebook 3__ : Facial Keypoint Detection Using Haar Cascades and your Trained CNN

__Notebook 4__ : Fun Filters and Keypoint Uses

__Model.py__: building the model




### Local Environment Instructions

1. Clone the repository, and navigate to the downloaded folder. This may take a minute or two to clone due to the included image data.
```
git clone https://github.com/rishab-gangwar/Facial_keypoints_detection.git
cd Facial_keypoints_detection
```

2. Create (and activate) a new environment, named `cv-nd` with Python 3.6. If prompted to proceed with the install `(Proceed [y]/n)` type y.

	- __Linux__ or __Mac__: 
	```
	conda create -n cv-nd python=3.6
	source activate cv-nd
	```
	- __Windows__: 
	```
	conda create --name cv-nd python=3.6
	activate cv-nd
	```
	
	At this point your command line should look something like: `(cv-nd) <User>:Facial_keypoints_detection <user>$`. The `(cv-nd)` indicates that your environment has been activated, and you can proceed with further package installations.

3. Install PyTorch and torchvision; this should install the latest version of PyTorch.
	
	- __Linux__ or __Mac__: 
	```
	conda install pytorch torchvision -c pytorch 
	```
	- __Windows__: 
	```
	conda install pytorch-cpu -c pytorch
	pip install torchvision
	```
