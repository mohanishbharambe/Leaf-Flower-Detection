# Leaf-Flower-Detection

This is a python Project with image identification and classification. The User Interface is made using Python-Flask.

You build an intelligent system that was trained with massive dataset of flower/plant images.
Your system predicts the label/class of the flower/plant using Computer Vision techniques and Machine Learning algorithms.
Your system searches the web for all the flower/plant related data after predicting the label/class of the captured image.
Your system helps gardeners and farmers to increase their productivity and yield with the help of automating tasks in garden/farm.
Your system applies the recent technological advancements such as Internet of Things (IoT) and Machine Learning in the agricultural domain.
You build such a system for your home or your garden to monitor your plants using a Raspberry Pi.

Feature Extraction
Features are the information or list of numbers that are extracted from an image. These are real-valued numbers (integers, float or binary). There are a wider range of feature extraction algorithms in Computer Vision.

When deciding about the features that could quantify plants and flowers, we could possibly think of Color, Texture and Shape as the primary ones. This is an obvious choice to globally quantify and represent the plant or flower image.

But this approach is less likely to produce good results, if we choose only one feature vector, as these species have many attributes in common like sunflower will be similar to daffodil in terms of color and so on. So, we need to quantify the image by combining different feature descriptors so that it describes the image more effectively.


Figure 3. Feature Extraction
Global Feature Descriptors
These are the feature descriptors that quantifies an image globally. These don’t have the concept of interest points and thus, takes in the entire image for processing. Some of the commonly used global feature descriptors are

Color - Color Channel Statistics (Mean, Standard Deviation) and Color Histogram
Shape - Hu Moments, Zernike Moments
Texture - Haralick Texture, Local Binary Patterns (LBP)
Others - Histogram of Oriented Gradients (HOG), Threshold Adjancency Statistics (TAS)
Local Feature Descriptors
These are the feature descriptors that quantifies local regions of an image. Interest points are determined in the entire image and image patches/regions surrounding those interest points are considered for analysis. Some of the commonly used local feature descriptors are

SIFT (Scale Invariant Feature Transform)
SURF (Speeded Up Robust Features)
ORB (Oriented Fast and Rotated BRIEF)
BRIEF (Binary Robust Independed Elementary Features)
Combining Global Features
There are two popular ways to combine these feature vectors.

For global feature vectors, we just concatenate each feature vector to form a single global feature vector. This is the approach we will be using in this tutorial.
For local feature vectors as well as combination of global and local feature vectors, we need something called as Bag of Visual Words (BOVW). This approach is not discussed in this tutorial, but there are lots of resources to learn this technique. Normally, it uses Vocabulory builder, K-Means clustering, Linear SVM, and Td-Idf vectorization.

Figure 4. Global Features to quantify a flower image
This is made for plant leaf identification, the flowers can also be detectedn using this method.
