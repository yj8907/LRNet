# LRNet in TensorFlow

Implementation of Long-Range connections in convolutional neural network. Adapted from Deep Residual Network.

Still in Progress.

## GOAL
Being able to improve on convolutional neural network by borrowing concepts from neuroscience research, including anatomical and functional understanding of nervous system.

## Model description
Standard deep convnets only contains local convolution, pooling or averaging. Full-connected layer is usually implemented at much deeper layers, where long-range interaction between local information could have been lost. However, in visual system, long-range interaction emerge as early as V1 layers, suggesting the importance of long range interaction at early layers. Therefore, to preserve long-range interaction, a layer with broader recpetive field is implemented by tensorflow function, tf.nn.atrous_conv2d, immediately after the first two layers of convolution and pooling.(atrous algorithm)


