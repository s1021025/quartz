14/12/2023 12:22
Tags :[[Segmentation#Semantic Segmentation]] [[Fully Convolutional Network]]

# SegNet
---
#### What is SegNet ?
SegNet is a variant of a [[Fully Convolutional Network]]
One of the key differences between SegNet and the original FCN is the utilization of pooling indices in the skip connections.
#### Architecture

![[Pasted image 20231214122451.png]]

#### Pooling Indices

In SegNet, instead of directly adding the entire output from the encoder's pooling layer, only the pooling indices are copied and used in the decoder.

![[Pasted image 20231214124259.png]]

These pooling indices help guide the upsampling process, allowing SegNet to retain important spatial information and improve its performance.

#### Sample Result Output

![[Pasted image 20231214124601.png]]
---
# References
[Understanding of Semantic Segmentation & How Segnet Model work to perform Semantic Segmentation | by Fezan | Medium](https://medium.com/@fezancs/understanding-of-semantic-segmentation-how-segnet-model-work-to-perform-semantic-segmentation-5c426112e499)

[arxiv.org/pdf/1511.00561.pdf](https://arxiv.org/pdf/1511.00561.pdf)