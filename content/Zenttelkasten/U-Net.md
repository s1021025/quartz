14/12/2023 12:46
Tags : [[Fully Convolutional Network]] [[Segmentation#Semantic Segmentation]]

# U-Net
---
#### What is U-Net?

SegNet is a variant of a [[Fully Convolutional Network]]
U-Net is first proposed to tackle the Medical image segmentation problem and lately discovered that U-Net does incredible performance in image generation e.g. DALL-E 2

#### Architecture

U-Net is a symmetric Encoder and Decoder Architecture which the dimension of the encoder and decoder is the same and connected together.

![[Pasted image 20231214125932.png]]

#### Skip Connections
U-Net simply concatenate the symmetrical stages of the encoder  / decoder. 

![[Pasted image 20231214132228.png]]

The combination of the encoder & decoder features can leverage the spatial information of the encoder features and the semantic information of the decoder features.

![[Pasted image 20231214132154.png]]

---
# References
<iframe width="560" height="315" src="https://www.youtube.com/embed/NhdzGfB1q74?si=zkto9BSF7c1L7hYA" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>