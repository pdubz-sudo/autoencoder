# 3-layer-AutoEncoder
3-layer AutoEncoder with TensorFlow and Keras

AutoEncoders are neural networks that take an input, reduce the input through a linear to non-linear function, and reconstruct the
data so the output layer is a reflection of the input layer; or at least as close as it can be.
The latent vector, reduced feature, can be retained and used pusposes such as dimensionality reduction. 

I implemented a 3-layer autoencoder in both TensorFlow and Keras. The input data was carbon nanotubes data set from
https://archive.ics.uci.edu/ml/datasets/Carbon+Nanotubes. It has only 6 features. It is just used to run the models.
The Keras notebook also has the MNIST set at the end which can be used to visualize what a latent vector from that dataset 
looks like.

I used the sigmoid activation for the output layer because the dataset had values between 0,1. If I had a input 
data that was in ranges outside of 0,1 and -1,1 I would have just dropped the non-linear activation function
and used the linear output for the cost function.
