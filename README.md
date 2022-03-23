# Assignment

1. End-To-End Computer Vision Pipeline
	##IMAGE##
  
2. Approch for this Assignment project

In this project I had trained my model in my own machine without using GPU, another way was to to train model on Google Colab but in real world colab-notebook 
is not going to work we are virtual machines with high GPU’s for training models so I did.

--> I tried to detect 4 classes i.e Car, Bus, Train, Auto-riksha
--> I used Fine-Tuning approch with pre-trained SSD_Resnet_152 model

Note: Fine-Tuning: It means we have weights (trained weights) on top of that we are trying to send labled or unlabled data to predect Y value. 
      I had used supervised fine-tuning in which we use pre-trained weights and retrain on supervised dataset.

**Data Selection**

   The first step towards having a high-quality training set is understanding the collected data.It is very important process while creating CV model. The data should not be biases as I had collected images from day time as well as in night time. Also there are many other points to be remember while collecting dataset.
Now a days there are many sites where we can get annotated dataset, some sites that I had used:
Google- Open image Dataset
Google Search dataset
Kaggle
Google Image search
Also I had used images from the given video to give model some real life stuff and such strategy will definitely increase the accuracy of the model.

**Data Augmentation**

I had not done much augmentation in this project on images, as it was not required. Generally with color contrast, image sharpning, gray scale images, rotating, zooming etc we can increase the dataset artificially.

**Data Annotation**

For annotating images I had used labeimg tool.

**Model Selection**

Selection of pre-trained model depents on project to project like if we are deploying the model on iot divices we can use SSD lite, SSD mobilenet, Yolo tiny(small)ets. 
Here I had used  SSD ResNet152 V1 FPN 640x640 (RetinaNet152)  model because  in such problem speed maters a loot it is having good mAp = 35.4 and speed = 80 , also as problem statement this model may be deployed on IOT devices for solving traffic problems.

**Model Trainning**

As you said You will be marked on your approach to the problem not on the accuracy  I didn't trained my model on much epoch also I was not having GPU so I trained using CPU power. Set training step= 25000

**Validating and Comparing models**

**Model Tunning**

**Object Tracking**

For object tracking I had used Deep SORT.

**Custom Code**

For using the model I had created my own customized code with TensorFlow 2.X which can Detect object, Track object, Measure distance of object from camera.
For using different model I just need to add that model and need to change some paths that's it.

Model Testing
Video 1
Video 2


1. Testing video (Easy): Cars Moving On Road Stock Footage - Free Download - YouTube
2. Testing video (Hard): Heavy Traffic after rain | Delhi | Rain| - YouTube
