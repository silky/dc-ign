# Deep Convolutional Inverse Graphics Network

This repository contains the code for the network described in http://arxiv.org/abs/1503.03167.

<!-- [![A DC-IGN lighting demo](http://i.imgur.com/ukoMSxt.gif)](http://www.youtube.com/watch?v=FpuhUaugAP0) -->

![A DC-IGN lighting demo](http://i.imgur.com/ukoMSxt.gif)

<!-- Click for the full video. -->
Project Website: http://willwhitney.github.io/dc-ign/www/
## Running

### Requirements
#### Torch7

- nn
- cudnn
- cunn

#### Dataset and pre-trained network
The train/test dataset along with a sample pre-trained network can be downloaded here:
http://wednesday.csail.mit.edu/tejask/dcign/

## Paper abstract
This paper presents the Deep Convolution Inverse Graphics Network (DC-IGN) that aims to learn an interpretable representation of images that is disentangled with respect to various transformations such as object out-of-plane rotations, lighting variations, and texture. The DC-IGN model is composed of multiple layers of convolution and de-convolution operators and is trained using the Stochastic Gradient Variational Bayes (SGVB) algorithm [11]. We propose training procedures to encourage neurons in the graphics code layer to have semantic meaning and force each group to distinctly represent a specific transformation (pose, light, texture, shape etc.). Given a static face image, our model can re-generate the input image with different pose, lighting or even texture and shape variations from the base face. We present qualitative and quantitative results of the model’s efficacy to learn a 3D rendering engine. Moreover, we also utilize the learnt representation for two important visual recognition tasks: (1) an invariant face recognition task and (2) using the representation as a summary statistic for generative modeling.

#### Acknowledgements
We thank Thomas Vetter for giving us access to the Basel face model. T. Kulkarni was graciously supported by the Leventhal Fellowship. This research was supported by ONR award N000141310333, ARO MURI W911NF-13-1-2012 and CBMM.
We would also like to thank (y0ast) https://github.com/y0ast for making the variational autoencoder code online.
