# BrainTumorDetection
## Introduction
Brain tumor occurs owing to uncontrolled and rapid growth of cells. If not treated at an initial phase, it may lead to death. Despite many significant efforts and promising outcomes in this domain, accurate segmentation and classification remain a challenging task. A major challenge for brain tumor detection arises from the variations in tumor location, shape, and size. The objective of this project is to deliver a a machine learning based algorithm on brain tumor detection using magnetic resonance imaging to help/aid the doctors. We proposes a deep learning based model which predicts and classifies brain tumor MRI Images into four respective classes, i.e, glioma tumor, meningioma tumor, pituitary tumor, no tumor
## Dataset Used
### Abstract:
A Brain tumor is considered as one of the aggressive diseases, among children and adults. Brain tumors account for 85 to 90 percent of all primary Central Nervous System(CNS) tumors. Every year, around 11,700 people are diagnosed with a brain tumor. The 5-year survival rate for people with a cancerous brain or CNS tumor is approximately 34 percent for men and 36 percent for women. Brain Tumors are classified as: Benign Tumor, Malignant Tumor, Pituitary Tumor, etc. Proper treatment, planning, and accurate diagnostics should be implemented to improve the life expectancy of the patients. The best technique to detect brain tumors is Magnetic Resonance Imaging (MRI). A huge amount of image data is generated through the scans. These images are examined by the radiologist. A manual examination can be error-prone due to the level of complexities involved in brain tumors and their properties.
Application of automated classification techniques using Machine Learning(ML) and Artificial Intelligence(AI)has consistently shown higher accuracy than manual classification. Hence, proposing a system performing detection and classification by using Deep Learning Algorithms using Convolution Neural Network (CNN), Artificial Neural Network (ANN), and Transfer Learning (TL) would be helpful to doctors all around the world.
### Dataset Description
The dataset contains MRI image data. The images are already split into Training and Testing folders. Each folder has more four subfolders. These folders have MRIs of respective tumor classes.
Dataset Classes:
a) glioma tumor
b) meningioma tumor
c) pituitary tumor
d) no tumor
## Base Model From Scratch
### What are Convolutions ?
The convolution layer is the core building block of the CNN. It carries the main portion of the network’s computational load.
This layer performs a dot product between two matrices, where one matrix is the set of learnable parameters otherwise known as a kernel, and the other matrix is the restricted portion of the receptive field. 
The kernel is spatially smaller than an image but is more in-depth. This means that, if the image is composed of three (RGB) channels, the kernel height and width will be spatially small, but the depth extends up to all three channels.
### Padding and Striding
Before we go further, it’s also useful to talk about padding and striding. These techniques are often used in CNNs:
1) Padding. Padding expands the input matrix by adding fake pixels to the borders of the matrix. This is done because convolution reduces the size of the matrix. For example, a 5x5 matrix turns into a 3x3 matrix when a filter goes over it.
2) Striding. It often happens that when working with a convolutional layer, you need to get an output that is smaller than the input. One way to achieve this is to use a pooling layer. Another way to achieve this is to use striding. The idea behind stride is to skip some areas when the kernel slides over: for example, skipping every 2 or 3 pixels. It reduces spatial resolution and makes the network more computationally efficient.


