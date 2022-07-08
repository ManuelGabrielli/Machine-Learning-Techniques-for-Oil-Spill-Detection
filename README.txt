+ ----------------------------------------------------- +
|						        |
|     MACHINE LEARNING TECHNIQUES FOR OIL DETECTION     |
|						        |
+ ----------------------------------------------------- +

1 - PROJECT GOALS
In this project I experiment two different techinques, 
Convolutional Neural Networks and Transfer Learning, for oil spill detection. 
I also consider techniques for data augmentation and artificial noise 
generation, to provide a wider spectrum of experiments. 

2 - PROJECT DESCRIPTION
The project is divided into three macro sections.
In the first, data are loaded and analyzed, and
all the structures necessary for the data augmentation are prepared.
In the second macro-section a model that exploits the Convolutional Neural Networks, is created.
This is trained on the training images created by the data augmentation and then its performances 
are analyzed both on the simple testing images provided, and on the same testing images to which 
noise with increasing frequency is applied.
In the third macro-section a new model is created, using the Transfer Learning technique, in which
an existing model is extended, obtained at the link 
'https://tfhub.dev/google/imagenet/mobilenet_v2_100_224/feature_vector/5'.
Also, on this model the previous procedure is conducted, in which the model is trained on the images
created with data augmentation and in which it is evaluated on both the original testing images and
on those affected by noise with increasing frequency.

3 - RESULTS
The two models give extremely different results.
The newly created model, which uses Convolutional Neural Networks, does not perform well on the 
original testing images.
The predictions do not have very high Precision and Recall values, and this is also given 
by the fact that it is trained on a set of images very small and very unbalanced in the distribution 
of classes.
However, it is robust to noise, as its performance does not decrease much when evaluated on images
suffering from this.
The model obtained by the Transfer Learning Technique, on the other hand, has excellent performances, 
obtaining extremely high Precision and Recall values for all classes, especially for the 'Oil Spill' class, 
target of the project.
This model is also very robust to noise, even in cases where it is very pronounced.
This means that the second model provides an excellent solution to the central problem of the project.
 




