# Burst Tiramisu Network
Extension to Tiramisu network for handling bursts of images.

Based mainly on the implementation of the Tiramisu network by: 

https://github.com/npielawski/pytorch_tiramisu.


# Documentation
The extension adds global max pooling layers to the encoder path for handling bursts of images.
All parameters are the same as in https://github.com/npielawski/pytorch_tiramisu but with added

nr_global_pooling_layers: The number of global max pooling layers to use in the encoder and

global_pool_func = The global pooling function to use (default: max pooling)

The input size tot he network needs to be batch_size, n_images, n_channels, height, width, where n_images is the number of images in the burst