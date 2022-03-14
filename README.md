# Neural-Cellular-Automata-Image-Manipulation

This is the repository for both style transfer and CLIP text based image modification using deep neural cellular automata, NCA. NCAs were pioneered by Alexander Mordvintsev et. al.[1] as an extension to conventional cellular automata by making the update rule learnable via backpropagation. This class of deep learning method has been applied for image recreation [1], texture synthesis [1] and for reinforcement learning applications [2] among others. Furthermore NCAs have been generalized to work on all graphs rather than just grids [3].

This repo contains code to use NCAs to transform images. One notebook contains the code for a Gatys et. al. type style transfer and the other a OpenAI CLIP based version where a prompt can be given to train NCAs to perform that transformation. 

The state space is given by a grid with the width and height of the image that is to be edited with 18 channels, 3 rgb of the stating image that cant be overwritten by the NCAs, 3 rgb channels of the image that is being iterated on and 12 hidden channels. The three channels that correspond to the original unedited image so that the NCA have access to the unaltered image as reference.

In the CLIP notebook there is a additional loss function for "aesthetics" which is something Katherine Crowson [4] came up with. The target rating goes from 0 to 10 where the later corresponds to the most aesthetic. 


CLIP:\
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1ieXiaoXfrcTt6f2vIGx3Fw1Oz3hyZm-Y?usp=sharing)

StyleTransfer:\
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1c7S7R52KjgNM3XrmADIRNKEFpEmgQONX?usp=sharing)

CLIP Example:\
Prompt: "A pencil sketch"\
<img src="./media/CLIP_sketch.gif" height="300">

CLIP Example:\
Prompt: "A painting made with multi-colored airport carpet fabric"\
<img src="./media/CLIP_carpet.gif" height="300">

Style Transfer Example:
Style Image: A picture of cooked pasta\
<img src="./media/vgg_pasta.gif" height="300">

Acknowledgements: 

I would like to thank the following people for their ideas and code that has been instrumental in making this work!

I would like to thank Alexander Mordvintsev, Ettore Randazzo, Eyvind Niklasson, Michael Levin (hopefully I did not miss anyone) for coming up with NCAs and for providing the code that forms the backbone of this notebook. If you see messy code, it is likely something I added. Since most of the code stems from them, I added their license. For more on NCAs check out their wonderful distill publications on the topic. https://distill.pub/2020/selforg/

I would also like to thank Katherine Crowson since the CLIP guidance code as well as the content loss code stems from her implementation of "A Neural Algorithm of Artistic Style" Gatys et al. (2015)

Lastly, I would like to thank John Whitaker (https://twitter.com/JohnowhitakerA) whom I saw use CLIP to guide texture synthesis in NCAs and therefore inspired this work.

Sources:

[1] "Differentiable Self-organizing Systems" Alexander Mordvintsev, Ettore Randazzo, Eyvind Niklasson, Michael Levin, Sam Greydanus. Distill.pub 2020

[2] "Using neural cellular automata to robustly control a cart-pole agent" Alexandre Variengien, Sidney Pontes-Filho, Tom Glover1, Stefano Nichele. IMI 2021

[3] "Learning Graph Cellular Automata" Daniele Grattarola, Lorenzo Livi, Cesare Alippi. NeurIPS 2021

[4] https://twitter.com/RiversHaveWings/status/1472334873096376320

For more updates follow me on twitter [![Twitter Follow](https://img.shields.io/twitter/follow/AntonObukhov1?style=social&label=Subscribe!)](https://twitter.com/Omorfiamorphism)
