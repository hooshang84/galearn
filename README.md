# Galaxy Classification with Artificial Neural Networks
The aim of this work (in prep) is to use multi-band high-resolution space-based observation of galaxies to construct an automatic classification algorithm for separating different populations based on their observed images. Here we take advantage of GANs to generate a complete library of high resolution data from existing space images. We then use a pre-trained NN architecture (ResNet) to construct feature vector for each object and then use dimensionality reduction and visualization tools to explore the existing trends in our generated sample.

### Data
The data for this study is from deep Hubble Space Telescope (HST) observation in the optical and near-infrared bands. In particular, we use the F435W (Blue), F850LP (Red) and F160w (infrared) as our main three color channels for our final classification scheme.

### GANs
We use the high-resolution HST data to generate a comprehensive library of different galaxy populations using Generative Adversarial Network (GAN) compared to our previous attempts of using just observed data to extract features. GANs provide us a better library that captures the full feature complexity existing in galaxy imaging while balancing our data-set by providing a complete sample for different data types.  

### Classification
We take advantage of a trained ResNet (He et al. 2015) to construct feature vectors for our sample and used t-distributed stochastic neighbor embedding (TSNE) to reduce the multi-dimensional space of feature vectors and to visualize the output classified sample.

Below we show our classification scheme on the high-resolution data resembling that of space-based observations as discussed above. We see that the algorithm is successful in separating the spiral disk-like systems from that of classical early types and the labeling very much agrees with that of traditional classifications using color-color space. This provides an excellent toolkit for classification of sources on large data-sets without resorting to limited features used by traditional techniques.

![ResNet Galaxy Image](https://github.com/hooshang84/galearn/blob/master/galaxy_features.jpg)
