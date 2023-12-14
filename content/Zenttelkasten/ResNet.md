14/12/2023 13:25
Tags : [[Convolutional Neural Network]] 

# ResNet
---
#### What is ResNet ?

ResNet is a deep convolutional neural network architecture that addresses the problem of vanishing gradients and **enables the training of very deep neural networks**. 

![[Pasted image 20231214143831.png]]
#### Residual Block

A residual block consists of two or three convolutional layers with a shortcut connection that bypasses one or two convolutional layers. 

![[Pasted image 20231214143059.png]]

This enables the network to **learn both identity mappings and residual mappings**, depending on what is more suitable for the given task.

With the identity residual connection, the gradients are very easy to back-propagated back to bottom network layers, which solves the Optimization difficulties

#### Dimension Matching
ResNet will decrease the dimensionality few residual block, the original paper will change the stride to 2 to divide the height and with by 2 but double the number of features to main the same amount of computation requirement

![[Pasted image 20231214144758.png]]

---
# References
<iframe width="560" height="315" src="https://www.youtube.com/embed/o_3mboe1jYI?si=4Zz4F4A3KZG0BfDA" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
[arxiv.org/pdf/1512.03385.pdf](https://arxiv.org/pdf/1512.03385.pdf)