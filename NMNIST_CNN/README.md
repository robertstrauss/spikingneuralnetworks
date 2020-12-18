# a spiking convolutional neural network applied to NMNIST data.
NMNIST (neuromorphic MNIST) are MNIST data converted to spike input by being recorded with a DVS sensor on a pan-tilt unit. Dataset by Garrick Orchard. [Link](https://www.garrickorchard.com/datasets/n-mnist)

Code is based off that from [slayerPytorch](https://github.com/bamsumit/slayerPytorch).


 - nmnistCNN_architectures: testing different network architectures to find the best depth and size of the network.
 - nmnistCNN_noise: adding random noise into data to test effect on performance.
 - nmnistCNN_moredata: trained network with full size NMNIST dataset, whereas previously it only used a small subsection of the data.
 - nmnistCNN_speed: testing notebook to find the source of slowdowns and speed things up.
 - nmnist_spike_to_image: using NMNIST in combination with standard MNIST dataset, training a network to reconstruct the MNIST image from spike data.
 - nmnist_spike_to_image_to_spike: network trained to reconstruct MNIST image in a middle layer from spikes, like above, but then also go from that back to spikes.
