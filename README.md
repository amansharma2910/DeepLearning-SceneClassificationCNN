<h1 align = 'center'>Scene Classification Using CNN</h1>
 
In this project, originally hosted on Kaggle, I have worked on a Deep Learning model based on the powerful CNN algorithm, capable of detecting the scene in an input image. 

\***[Link to Kaggle Notebook](https://www.kaggle.com/bravehart101/sceneclassification-cnn-pytorch)**

<h2>Project Objectives</h2>

The following are the project objectives-
* Creating a Google Images-like multi-class scene classifier using the CNN algorithm.
* Working on different CNN architectures and comparing their performance.
* Comparing performance gain (or loss) while working with different deep learning techniques.  

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

<h2>Observations</h2>
For the scene classifier, I worked with two CNN architectures— A custom ResNet9 model, and a ResNeXt9 model based on the ResNet9 model where I replaced the residual blocks with ResNeXt blocks of cardinality 4.

The ResNet9 model had around 7 million learnable parameters, while on the other hand, the ResNeXt9 model had around 22 million learnable parameters (around 3 times more). Here are the observations after training and testing the model-

* After training with 10 epochs, the ResNet9 model an accuracy of somewhere about 83% on the test dataset. At the same time, it took around 15 epochs for the ResNeXt9 model to achieve 81% accuracy on the test set.
* Increasing the architectural complexity reduces the speed of training. Also, more learnable parameters doesn't guarantee a performance boost. Rather, making the architecture more complex can result in overfitting, thus causing the classifier system to lose generalization capabilities which might cause it to perform poorly on test/real-world data.
* Normalizing the data can significantly reduce learning time while also showing a boost in accuracy. This observation was derived with the ResNet9 model which showed around 5% accuracy after normalizing both the training and testing dataset.

<h2>Key Highlights</h2>

 This is a complete, end-to-end project, where, in order to achieve the optimum performance I have implemented different Deep Learning techniques, namely-
 
 * **data normalization** 
 * **data augmentation**
 * **batch normalization**
 * **weight-decay-prevention** 
 * **learning rate scheduling**  
 
 Along with above mentioned techniques, I have also tried using different CNN architectures, comparing the model performance for each architecture.
 
 \*Note- *Each separate jupyter notebooks contains a different model architecture along with different transformation and optimization techniques. This is an ongoing project so I'll keep adding more notebooks with different custom CNN architectures in the future.* 
 
 
