# Neural-Cellular-Automata-Image-Manipulation

This is the repository for both style transfer and CLIP text based image modification using deep neural cellular automata, NCA. NCAs were pioneered by Alexander Mordvintsev et. al.[1] as an extension to conventional cellular automata by making the update rule learnable via backpropagation. This class of deep learning method has been applied for image recreation [1], texture synthesis [1] and for reinforcement learning applications [2] among others. Furthermore NCAs have been generalized to work on all graphs rather than just grids [3].

This repo contains code to use NCAs to transform images. One notebook contains the code for a Gatys et. al. type style transfer and the other a OpenAI CLIP based version where a prompt can be given to train NCAs to perform that transformation. 

The state space is given by a grid with the width and height of the image that is to be edited with 18 channels, 3 rgb of the stating image that cant be overwritten by the NCAs, 3 rgb channels of the image that is being iterated on and 12 hidden channels. The three channels that correspond to the original unedited image so that the NCA have access to the unaltered image as reference. 

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

[1] "Differentiable Self-organizing Systems" Alexander Mordvintsev, Ettore Randazzo, Eyvind Niklasson, Michael Levin, Sam Greydanus. Distill.pub 2020

[2] "Using neural cellular automata to robustly control a cart-pole agent" Alexandre Variengien, Sidney Pontes-Filho, Tom Glover1, Stefano Nichele. IMI 2021

[3] "Learning Graph Cellular Automata" aniele Grattarola, Lorenzo Livi, Cesare Alippi. NeurIPS 2021

For more updates follow me on twitter [![Twitter Follow](https://img.shields.io/twitter/follow/AntonObukhov1?style=social&label=Subscribe!)](https://twitter.com/Omorfiamorphism)
