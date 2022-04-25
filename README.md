# Face-Recognition-Project

Face recognition is the task of identifying an already detected object as a known or unknown face.
Here I have implemented a face recognition system using CNN model for face recognition and a
prebuilt caffemodel for extracting faces from images.

# Dataset Details
The dataset consists of two folders namely 'Final Training Images' and 'Final Testing Images'.
'Final Training Images' further contains two subfolders named 'face0' and 'face1'. 'face0' contains
the images that are false labels and face1 contains the training images for the image that is to be
correctly identified. There are a total of ### images in 'Final Training Images' folder and a total
of # images in 'Final Testing Images' folder.

# Implementation Details
There are 3 modules in the project, one for extracting faces from photos (named as 
Face_extractor.ipynb), second for learning the facial features (Model.ipynb) and final one for 
testing the images (Tester.ipynb).

  # Face_extractor.ipynb
  -Reads the raw images from a folder.
  -Extracts all the faces present in an image and stores them as a different file in a different 
   folder according to need.
  -The images in dataset was generated by running this module
  
  # Model.ipynb
  -It loads the training data from the Final Training Images folder in the dataset
  -Using CNN, it learns the image features and the model is saved in the main folder
  
  # Tester.ipynb
  -It loads the saved model from the main folder and the images to test from the folder 'Final 
   Testing Images' in the dataset
  -It iterates through all the images in the folder and outputs ‘Yes’ if the image is correct face and 
   ‘No’ otherwise.
   
# Design

![image](https://user-images.githubusercontent.com/69210229/165162191-732a2f87-b2e9-4d37-a0e1-7df76c8bdfe3.png)

  # CNN Design
  
![image](https://user-images.githubusercontent.com/69210229/165162311-ad79e596-505b-474e-91b9-dfd4b9f767cb.png)

# Implementation Details

The program is run on Google Colab and the file paths are given as google drive locations. 
There are already eight test images in the testing folder. To test additional images, the images
can be dropped inside ‘Testing Images Raw’ folder in the main folder and Face_extractor.ipynb 
should be run. This would store the face images inside ‘Final Testing Images’ folder inside 
Dataset. Then the Tester.ipynb can be run to output the result.


# References

- https://thinkingneuron.com/face-recognition-using-deep-learning-cnn-in-python/
- https://towardsdatascience.com/extracting-faces-using-opencv-face-detection-neural-network-475c5cd0c260
- https://towardsdatascience.com/real-time-face-recognition-an-end-to-end-project-b738bb0f7348
