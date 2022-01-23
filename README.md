# Neural-Cellular-Automata-Image-Manipulation

This is the repository for both style transfer and CLIP text based image modification using deep neural cellular automata, NCA. NCAs were pioneered by A.M.[1] as an extension to conventional cellular automata by making the update rule learnable via backpropagation. This class of deep learning method has been applied for image recreation [1], texture synthesis [2] and for reinforcement learning applications [3] among others. Furthermore NCAs have been generalized to work on all graphs rather than just grids [4].

This repo contains code to use NCAs to transform images. One notebook contains the code for a Gatys et. al. type style transfer and the other a OpenAI CLIP based version where a prompt can be given to train NCAs to perform that transformation. 

CLIP:\
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1ieXiaoXfrcTt6f2vIGx3Fw1Oz3hyZm-Y?usp=sharing)

StyleTransfer:\
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1c7S7R52KjgNM3XrmADIRNKEFpEmgQONX?usp=sharing)

CLIP Example:\
Prompt: "A pencil sketch"\
<img src="./media/CLIP_sketch.gif" height="300">

Style Transfer Example:
Style Image: A picture of cooked pasta\
<img src="./media/vgg_pasta.gif" height="300">

Sources:
[1]

[2]

[3]

[5]

[6]

[7]

For more updates follow me on twitter [![Twitter Follow](https://img.shields.io/twitter/follow/AntonObukhov1?style=social&label=Subscribe!)](https://twitter.com/Omorfiamorphism)
