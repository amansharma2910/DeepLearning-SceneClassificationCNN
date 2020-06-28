<h1 align = 'center'>Scene Classification Using CNN</h1>
 
In this project, originally hosted on Kaggle, I have worked on a Deep Learning model based on the powerful CNN algorithm, capable of detecting the scene in an input image. 

\***[Link to Kaggle Notebook](https://www.kaggle.com/bravehart101/sceneclassification-cnn-pytorch)**

<h2>Understanding the Problem Statement</h2>

The dataset that I have used for this project is the Intel Image Classification dataset. 

This is a multi-class classification problem where, given a picture, our model processes the image then classifies it as one of the six possible classes- 
 * buildings: 0
 * mountain: 1 
 * street: 2
 * forest: 3 
 * sea: 4 
 * glacier: 5

As per the data source, each image is a 150 × 150 pixel, 3-channeled (RGB) image, with around 14k images in the training set and 3k images in the testing set.

<h2>Key Highlights</h2>

 This is a complete, end-to-end project, where, in order to achieve the optimum performance I have implemented different Deep Learning techniques, namely-
 
 * **data normalization** 
 * **data augmentation**
 * **batch normalization**
 * **weight-decay-prevention** 
 * **learning rate scheduling**  
 
 Along with above mentioned techniques, I have also tried using different CNN architectures, comparing the model performance for each architecture.
 
 \*Note- *Each separate jupyter notebooks contains a different model architecture along with different transformation and optimization techniques. This is an ongoing project so I'll keep adding more notebooks with different custom CNN architectures in the future.* 
 
 
