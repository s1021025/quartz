14/12/2023 11:01
Tags : [[Segmentation#Semantic Segmentation]]

# Fully Convolutional Network
---
#### What is Fully Convolutional Network ?

A fully convolutional network (FCN) is a type of neural network architecture designed specifically for dense pixel-wise predictions in tasks such as **semantic segmentation**.

#### The Key Idea

Replace the fully connected layers at the end of a CNN with convolutional layers that operate on the entire input image or feature maps. 

This allows the network to **produce a dense output map of predictions**, where each pixel in the input image is associated with a prediction or label.

#### Architecture

![[Pasted image 20231214112831.png]]
#### Encoder

The encoder in an FCN extracts features from the image and maps them to a 1 x 1 x d-dimensional vector, where d represents the number of prediction classes.

![[Pasted image 20231214113425.png]]

#### Decoder

The decoder in a Fully Convolutional Network (FCN) is responsible for upsampling the feature maps from the encoder to the original image resolution and generating dense predictions.

##### Transposed Convolution

Transposed convolution in FCNs, also known as deconvolution or upsampling, applies learned filters to the feature maps from the encoder. 
By utilizing parameters such as padding and stride, it controls the output dimensions during upsampling. 
The filters are learned through backpropagation during training to optimize the network's performance.

![[Pasted image 20231214114336.png]]

#### Skip Connection
Skip connections are designed to address the loss of information during the upsampling process in the decoder. As the decoder upsamples the feature maps, spatial dimensions are increased but some details may be lost. Skip connections tackle this issue by **directly connecting the feature maps from the encoder to the corresponding layers in the decoder.**

![[Pasted image 20231214121007.png]]


>[!summary] Result
><b>The result of using different skip connection : </b>
>
>![[Pasted image 20231214121136.png]]

---
# References
<iframe width="560" height="315" src="https://www.youtube.com/embed/Ahge3GzQ3Kg?si=5UAQOVQvjh9sZfjY" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

[arxiv.org/pdf/1411.4038.pdf](https://arxiv.org/pdf/1411.4038.pdf)