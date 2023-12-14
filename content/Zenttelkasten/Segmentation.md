2023-12-14 09:59
Tags : [[Computer Vision]]

# Segmentation
---
#### What is Segmentation?

Image segmentation is the process of dividing an image into different regions or pixels based on certain criteria or characteristics. It aims to group pixels with similar properties together to extract meaningful information from the image. There are two main types of image segmentation.

#### Semantic Segmentation

Semantic Segmentation involves **assigning a semantic label to each pixel in the image**.
The <b>goal</b> is to understand the scene at a pixel level by categorizing each pixel into predefined classes or categories. 

![[Pasted image 20231214101103.png]]

>[!example] Algorithm
><b>Here's is some algorithm that can perform Semantic Segmentation</b>
>#### Conventional Algorithm
>1. [[Thresholding]]
>2. [[Region-Based]]
>3. [[Boundary-Based]]
>4. [[K-means]]
>#### Deep Learning Algorithm
>1. [[Fully Convolutional Network]]
>2. [[SegNet]]
>3. [[U-Net]]
>4. [[Transformer]]


#### Instance Segmentation

Instance segmentation goes beyond semantic segmentation by not only assigning a label to each pixel but also **distinguishing individual instances of objects within the same class.** 

It aims to identify and **differentiate each object instance separately**, regardless of their class or category.

![[Pasted image 20231214101148.png]]

>[!example] Algorithms
><b>Here's is some algorithm that can perform Instance Segmentation</b>
>1. [[R-CNN Family]]
---
# References
